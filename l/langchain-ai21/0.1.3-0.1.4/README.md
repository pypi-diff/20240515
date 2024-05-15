# Comparing `tmp/langchain_ai21-0.1.3.tar.gz` & `tmp/langchain_ai21-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ai21-0.1.3.tar", max compression
+gzip compressed data, was "langchain_ai21-0.1.4.tar", max compression
```

## Comparing `langchain_ai21-0.1.3.tar` & `langchain_ai21-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1072 2024-04-01 17:48:43.198428 langchain_ai21-0.1.3/LICENSE
--rw-r--r--   0        0        0     3146 2024-04-01 17:48:43.198428 langchain_ai21-0.1.3/README.md
--rw-r--r--   0        0        0      413 2024-04-01 17:48:43.198428 langchain_ai21-0.1.3/langchain_ai21/__init__.py
--rw-r--r--   0        0        0     1475 2024-04-01 17:48:43.198428 langchain_ai21-0.1.3/langchain_ai21/ai21_base.py
--rw-r--r--   0        0        0     6208 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/chat_models.py
--rw-r--r--   0        0        0     3067 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/contextual_answers.py
--rw-r--r--   0        0        0     2255 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/embeddings.py
--rw-r--r--   0        0        0     5238 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/llms.py
--rw-r--r--   0        0        0        0 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/py.typed
--rw-r--r--   0        0        0     5121 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/semantic_text_splitter.py
--rw-r--r--   0        0        0     2367 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 langchain_ai21-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3146 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/README.md
+-rw-r--r--   0        0        0      413 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/langchain_ai21/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/langchain_ai21/ai21_base.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/langchain_ai21/chat/__init__.py
+-rw-r--r--   0        0        0     4114 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/langchain_ai21/chat/chat_adapter.py
+-rw-r--r--   0        0        0      351 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/langchain_ai21/chat/chat_factory.py
+-rw-r--r--   0        0        0     5161 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/langchain_ai21/chat_models.py
+-rw-r--r--   0        0        0     3067 2024-05-01 20:10:52.661656 langchain_ai21-0.1.4/langchain_ai21/contextual_answers.py
+-rw-r--r--   0        0        0     2255 2024-05-01 20:10:52.665656 langchain_ai21-0.1.4/langchain_ai21/embeddings.py
+-rw-r--r--   0        0        0     5238 2024-05-01 20:10:52.665656 langchain_ai21-0.1.4/langchain_ai21/llms.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:10:52.665656 langchain_ai21-0.1.4/langchain_ai21/py.typed
+-rw-r--r--   0        0        0     5121 2024-05-01 20:10:52.665656 langchain_ai21-0.1.4/langchain_ai21/semantic_text_splitter.py
+-rw-r--r--   0        0        0     2449 2024-05-01 20:10:52.665656 langchain_ai21-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 langchain_ai21-0.1.4/PKG-INFO
```

### Comparing `langchain_ai21-0.1.3/LICENSE` & `langchain_ai21-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.3/README.md` & `langchain_ai21-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.3/langchain_ai21/ai21_base.py` & `langchain_ai21-0.1.4/langchain_ai21/ai21_base.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.3/langchain_ai21/chat_models.py` & `langchain_ai21-0.1.4/langchain_ai21/chat_models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,25 @@
 import asyncio
 from functools import partial
-from typing import Any, List, Mapping, Optional, Tuple, cast
+from typing import Any, Dict, List, Mapping, Optional
 
-from ai21.models import ChatMessage, RoleType
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.messages import (
-    AIMessage,
     BaseMessage,
-    HumanMessage,
-    SystemMessage,
 )
 from langchain_core.outputs import ChatGeneration, ChatResult
+from langchain_core.pydantic_v1 import root_validator
 
 from langchain_ai21.ai21_base import AI21Base
-
-
-def _get_system_message_from_message(message: BaseMessage) -> str:
-    if not isinstance(message.content, str):
-        raise ValueError(
-            f"System Message must be of type str. Got {type(message.content)}"
-        )
-
-    return message.content
-
-
-def _convert_messages_to_ai21_messages(
-    messages: List[BaseMessage],
-) -> Tuple[Optional[str], List[ChatMessage]]:
-    system_message = None
-    converted_messages: List[ChatMessage] = []
-
-    for i, message in enumerate(messages):
-        if message.type == "system":
-            if i != 0:
-                raise ValueError("System message must be at beginning of message list.")
-            else:
-                system_message = _get_system_message_from_message(message)
-        else:
-            converted_message = _convert_message_to_ai21_message(message)
-            converted_messages.append(converted_message)
-
-    return system_message, converted_messages
-
-
-def _convert_message_to_ai21_message(
-    message: BaseMessage,
-) -> ChatMessage:
-    content = cast(str, message.content)
-
-    role = None
-
-    if isinstance(message, HumanMessage):
-        role = RoleType.USER
-    elif isinstance(message, AIMessage):
-        role = RoleType.ASSISTANT
-
-    if not role:
-        raise ValueError(
-            f"Could not resolve role type from message {message}. "
-            f"Only support {HumanMessage.__name__} and {AIMessage.__name__}."
-        )
-
-    return ChatMessage(role=role, text=content)
-
-
-def _pop_system_messages(messages: List[BaseMessage]) -> List[SystemMessage]:
-    system_message_indexes = [
-        i for i, message in enumerate(messages) if isinstance(message, SystemMessage)
-    ]
-
-    return [cast(SystemMessage, messages.pop(i)) for i in system_message_indexes]
+from langchain_ai21.chat.chat_adapter import ChatAdapter
+from langchain_ai21.chat.chat_factory import create_chat_adapter
 
 
 class ChatAI21(BaseChatModel, AI21Base):
     """ChatAI21 chat model.
 
     Example:
         .. code-block:: python
@@ -115,14 +57,28 @@
     presence_penalty: Optional[Any] = None
     """ A penalty applied to tokens that are already present in the prompt."""
 
     count_penalty: Optional[Any] = None
     """A penalty applied to tokens based on their frequency 
     in the generated responses."""
 
+    n: int = 1
+    """Number of chat completions to generate for each prompt."""
+
+    _chat_adapter: ChatAdapter
+
+    @root_validator()
+    def validate_environment(cls, values: Dict) -> Dict:
+        values = super().validate_environment(values)
+        model = values.get("model")
+
+        values["_chat_adapter"] = create_chat_adapter(model)  # type: ignore
+
+        return values
+
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
 
     @property
     def _llm_type(self) -> str:
@@ -135,14 +91,15 @@
             "model": self.model,
             "num_results": self.num_results,
             "max_tokens": self.max_tokens,
             "min_tokens": self.min_tokens,
             "temperature": self.temperature,
             "top_p": self.top_p,
             "top_k_return": self.top_k_return,
+            "n": self.n,
         }
 
         if self.count_penalty is not None:
             base_params["count_penalty"] = self.count_penalty.to_dict()
 
         if self.frequency_penalty is not None:
             base_params["frequency_penalty"] = self.frequency_penalty.to_dict()
@@ -155,47 +112,52 @@
     def _build_params_for_request(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> Mapping[str, Any]:
         params = {}
-        system, ai21_messages = _convert_messages_to_ai21_messages(messages)
+        converted_messages = self._chat_adapter.convert_messages(messages)
 
         if stop is not None:
             if "stop" in kwargs:
                 raise ValueError("stop is defined in both stop and kwargs")
             params["stop_sequences"] = stop
 
         return {
-            "system": system or "",
-            "messages": ai21_messages,
+            **converted_messages,
             **self._default_params,
             **params,
             **kwargs,
         }
 
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> ChatResult:
         params = self._build_params_for_request(messages=messages, stop=stop, **kwargs)
+        messages = self._chat_adapter.call(self.client, **params)
+        generations = [ChatGeneration(message=message) for message in messages]
 
-        response = self.client.chat.create(**params)
-
-        outputs = response.outputs
-        message = AIMessage(content=outputs[0].text)
-        return ChatResult(generations=[ChatGeneration(message=message)])
+        return ChatResult(generations=generations)
 
     async def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> ChatResult:
         return await asyncio.get_running_loop().run_in_executor(
             None, partial(self._generate, **kwargs), messages, stop, run_manager
         )
+
+    def _get_system_message_from_message(self, message: BaseMessage) -> str:
+        if not isinstance(message.content, str):
+            raise ValueError(
+                f"System Message must be of type str. Got {type(message.content)}"
+            )
+
+        return message.content
```

### Comparing `langchain_ai21-0.1.3/langchain_ai21/contextual_answers.py` & `langchain_ai21-0.1.4/langchain_ai21/contextual_answers.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.3/langchain_ai21/embeddings.py` & `langchain_ai21-0.1.4/langchain_ai21/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.3/langchain_ai21/llms.py` & `langchain_ai21-0.1.4/langchain_ai21/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.3/langchain_ai21/semantic_text_splitter.py` & `langchain_ai21-0.1.4/langchain_ai21/semantic_text_splitter.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.3/pyproject.toml` & `langchain_ai21-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "langchain-ai21"
-version = "0.1.3"
+version = "0.1.4"
 description = "An integration package connecting AI21 and LangChain"
 authors = []
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.28"
+langchain-core = "^0.1.48"
 langchain-text-splitters = "^0.0.1"
-ai21 = "^2.1.2"
+ai21 = "^2.2.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = { path = "../../core", develop = true }
+langchain-standard-tests = { path = "../../standard-tests", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -46,15 +47,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
 
 [tool.mypy]
```

### Comparing `langchain_ai21-0.1.3/PKG-INFO` & `langchain_ai21-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: langchain-ai21
-Version: 0.1.3
+Version: 0.1.4
 Summary: An integration package connecting AI21 and LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ai21 (>=2.1.2,<3.0.0)
-Requires-Dist: langchain-core (>=0.1.28,<0.2.0)
+Requires-Dist: ai21 (>=2.2.1,<3.0.0)
+Requires-Dist: langchain-core (>=0.1.48,<0.2.0)
 Requires-Dist: langchain-text-splitters (>=0.0.1,<0.0.2)
 Description-Content-Type: text/markdown
 
 # langchain-ai21
 
 This package contains the LangChain integrations for [AI21](https://docs.ai21.com/) through their [AI21](https://pypi.org/project/ai21/) SDK.
```

