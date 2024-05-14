# Comparing `tmp/ez_openai-0.0.4.tar.gz` & `tmp/ez_openai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_openai-0.0.4.tar", max compression
+gzip compressed data, was "ez_openai-0.0.5.tar", max compression
```

## Comparing `ez_openai-0.0.4.tar` & `ez_openai-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34523 2023-12-08 01:53:42.705527 ez_openai-0.0.4/LICENSE
--rw-r--r--   0        0        0     2803 2023-12-20 02:38:52.405545 ez_openai-0.0.4/README.md
--rw-r--r--   0        0        0     6080 2023-12-20 02:38:52.405545 ez_openai-0.0.4/ez_openai/__init__.py
--rw-r--r--   0        0        0     2006 2023-12-19 16:52:27.127668 ez_openai-0.0.4/ez_openai/decorator.py
--rw-r--r--   0        0        0      550 2023-12-20 02:39:04.017489 ez_openai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 ez_openai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-14 20:10:15.472466 ez_openai-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2983 2024-05-14 23:08:34.641317 ez_openai-0.0.5/README.md
+-rw-r--r--   0        0        0     7428 2024-05-14 23:39:19.596277 ez_openai-0.0.5/ez_openai/__init__.py
+-rw-r--r--   0        0        0     2006 2024-05-14 20:10:15.473164 ez_openai-0.0.5/ez_openai/decorator.py
+-rw-r--r--   0        0        0      612 2024-05-14 23:43:42.829718 ez_openai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 ez_openai-0.0.5/PKG-INFO
```

### Comparing `ez_openai-0.0.4/LICENSE` & `ez_openai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_openai-0.0.4/README.md` & `ez_openai-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,22 @@
 # The library will handle all the background function calls itself:
 conversation.ask("Hi, what's the weather like in Thessaloniki and Athens right now?")
 > I'm getting the weather for Thessaloniki woooooo
 > I'm getting the weather for Athens woooooo
 > "The weather today in both Thessaloniki and Athens is quite similar, with a
    temperature of 26°C and a humidity level at 60%. Enjoy a pleasant and comfortable
    day!"
+
+It also supports images:
+
+conversation.ask("What's in this image?", image_url="https://www.someimage.com/")
+
+or:
+
+conversation.ask("What's in this image?", image_file="file.jpg")
 ```
 
 Because assistants change (eg if you want to add some more functions), and it's tedious
 to create new ones every time, there's a helper method that will update an assistant
 with new functions/instructions:
 
 ```python
```

### Comparing `ez_openai-0.0.4/ez_openai/__init__.py` & `ez_openai-0.0.5/ez_openai/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 import os
 import time
-from typing import Callable
+from typing import Callable, Any
 
 import openai
 
 from .decorator import openai_function  # noqa
 
+DEFAULT_MODEL = "gpt-4o"
+
 
 class Conversation:
     """
     A conversation, with multiple messages.
 
     This is roughly what OpenAI calls a thread.
     """
@@ -48,16 +50,38 @@
     def create(self) -> "Conversation":
         self._thread = self._assistant._client.beta.threads.create()
         return self
 
     def delete(self) -> None:
         self._assistant._client.beta.threads.delete(self.id)
 
-    def ask(self, message) -> str:
-        self._client.beta.threads.messages.create(self.id, role="user", content=message)
+    def ask(
+        self,
+        message: str | None,
+        image_url: str | None = None,
+        image_file: bytes | None = None,
+    ) -> str:
+        content = []
+        file = None
+        if message is not None:
+            content.append({"type": "text", "text": message})
+        if image_url is not None:
+            content.append({"type": "image_url", "image_url": {"url": image_url}})  # type: ignore
+        if image_file is not None:
+            file = self._client.files.create(
+                file=open(image_file, "rb"), purpose="assistants"
+            )
+            content.append(
+                {
+                    "type": "image_file",
+                    "image_file": {"file_id": file.id},  # type: ignore
+                }
+            )
+
+        self._client.beta.threads.messages.create(self.id, role="user", content=content)
 
         last_run = self._client.beta.threads.runs.create(
             thread_id=self.id, assistant_id=self._assistant.id
         )
 
         while True:
             while last_run.status in ("queued", "in_progress"):
@@ -84,16 +108,18 @@
 
             elif last_run.status == "completed":  # type: ignore[attr-defined]
                 thread_messages = self._client.beta.threads.messages.list(
                     self._thread.id, limit=4
                 )
                 response = thread_messages.data[0].content[0].text.value
                 return response
-            else:
-                raise ValueError("ERROR: Got unknown run status.")
+            elif last_run.status == "failed":
+                raise ValueError(
+                    f"ERROR: Got unknown run status: {last_run.last_error.message}"
+                )
 
 
 class Assistant:
     def __init__(
         self,
         api_key: str = "",
         functions: None | list[Callable] = None,
@@ -149,43 +175,55 @@
 
     @classmethod
     def get_and_modify(
         cls,
         id: str,
         name: str,
         instructions: str = "",
-        model="gpt-4-1106-preview",
+        model=DEFAULT_MODEL,
+        temperature: float | None = None,
+        response_format: Any = None,
         functions: None | list[Callable] = None,
         api_key: str = "",
     ) -> "Assistant":
         """Retrieve a previously-created assistant, and modify it to the parameters."""
         assistant = cls.get(id, functions=functions, api_key=api_key)
-        assistant._client.beta.assistants.update(
-            id,
-            instructions=instructions,
-            name=name,
-            tools=[fn._openai_fn for fn in assistant._functions.values()],  # type: ignore
-            model=model,
-        )
+        params = {
+            "instructions": instructions,
+            "name": name,
+            "tools": [fn._openai_fn for fn in assistant._functions.values()],  # type: ignore
+            "model": model,
+        }
+        if response_format:
+            params["response_format"] = response_format
+        if temperature:
+            params["temperature"] = temperature
+        assistant._client.beta.assistants.update(id, **params)
         return assistant
 
     @classmethod
     def create(
         cls,
         name: str,
         instructions: str = "",
-        model="gpt-4-1106-preview",
+        model=DEFAULT_MODEL,
+        temperature: float = 1.0,
+        response_format: Any = None,
         functions: None | list[Callable] = None,
         api_key: str = "",
     ) -> "Assistant":
         """Create an assistant."""
         assistant = cls(api_key=api_key, functions=functions)
-        assistant._assistant = assistant._client.beta.assistants.create(
-            instructions=instructions,
-            name=name,
-            model=model,
-            tools=[fn._openai_fn for fn in assistant._functions.values()],  # type: ignore
-        )
+        params = {
+            "instructions": instructions,
+            "name": name,
+            "model": model,
+            "temperature": temperature,
+            "tools": [fn._openai_fn for fn in assistant._functions.values()],  # type: ignore
+        }
+        if response_format:
+            params["response_format"] = response_format
+        assistant._assistant = assistant._client.beta.assistants.create(**params)
         return assistant
 
     def delete(self):
         self._client.beta.assistants.delete(self.id)
```

### Comparing `ez_openai-0.0.4/ez_openai/decorator.py` & `ez_openai-0.0.5/ez_openai/decorator.py`

 * *Files identical despite different names*

### Comparing `ez_openai-0.0.4/pyproject.toml` & `ez_openai-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "ez-openai"
-version = "0.0.4"
+version = "0.0.5"
 description = "A more reasonable OpenAI API."
 authors = ["Stavros Korokithakis <hi@stavros.io>"]
 repository = "https://github.com/skorokithakis/ez-openai/"
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1"
+python = ">=3.8,<4"
 openai = ">=1.3.5"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-ignore = ["F403", "E501", "N802", "N803", "N806", "C901", "D100", "D102", "D102", "D10"]
+lint.ignore = ["F403", "E501", "N802", "N803", "N806", "C901", "D100", "D102", "D102", "D10"]
```

### Comparing `ez_openai-0.0.4/PKG-INFO` & `ez_openai-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ez-openai
-Version: 0.0.4
+Version: 0.0.5
 Summary: A more reasonable OpenAI API.
 Home-page: https://github.com/skorokithakis/ez-openai/
 License: AGPL-3.0-or-later
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
-Requires-Python: >=3.7.1
+Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.3.5)
 Project-URL: Repository, https://github.com/skorokithakis/ez-openai/
 Description-Content-Type: text/markdown
 
 # Ez OpenAI
 
 My opinion of the `openai` Python library is best illustrated by the fact that if you
@@ -97,14 +98,22 @@
 # The library will handle all the background function calls itself:
 conversation.ask("Hi, what's the weather like in Thessaloniki and Athens right now?")
 > I'm getting the weather for Thessaloniki woooooo
 > I'm getting the weather for Athens woooooo
 > "The weather today in both Thessaloniki and Athens is quite similar, with a
    temperature of 26°C and a humidity level at 60%. Enjoy a pleasant and comfortable
    day!"
+
+It also supports images:
+
+conversation.ask("What's in this image?", image_url="https://www.someimage.com/")
+
+or:
+
+conversation.ask("What's in this image?", image_file="file.jpg")
 ```
 
 Because assistants change (eg if you want to add some more functions), and it's tedious
 to create new ones every time, there's a helper method that will update an assistant
 with new functions/instructions:
 
 ```python
```

