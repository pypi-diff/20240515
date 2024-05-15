# Comparing `tmp/gpt-command-line-0.1.5.tar.gz` & `tmp/gpt_command_line-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-command-line-0.1.5.tar", last modified: Mon Mar  4 17:05:17 2024, max compression
+gzip compressed data, was "gpt_command_line-0.1.6.tar", last modified: Wed May 15 01:44:09 2024, max compression
```

## Comparing `gpt-command-line-0.1.5.tar` & `gpt_command_line-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:05:17.669823 gpt-command-line-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-03-04 17:05:17.669823 gpt-command-line-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:05:17.669823 gpt-command-line-0.1.5/gpt_command_line.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-03-04 17:05:17.000000 gpt-command-line-0.1.5/gpt_command_line.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-04 17:05:17.000000 gpt-command-line-0.1.5/gpt_command_line.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 17:05:17.000000 gpt-command-line-0.1.5/gpt_command_line.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-04 17:05:17.000000 gpt-command-line-0.1.5/gpt_command_line.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-04 17:05:17.000000 gpt-command-line-0.1.5/gpt_command_line.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-04 17:05:17.000000 gpt-command-line-0.1.5/gpt_command_line.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:05:17.669823 gpt-command-line-0.1.5/gptcli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/google.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7996 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/gptcli/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 17:05:17.669823 gpt-command-line-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:05:17.669823 gpt-command-line-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/tests/test_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-04 17:05:08.000000 gpt-command-line-0.1.5/tests/test_term_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:44:09.245084 gpt_command_line-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-15 01:44:09.245084 gpt_command_line-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:44:09.241084 gpt_command_line-0.1.6/gpt_command_line.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-15 01:44:09.000000 gpt_command_line-0.1.6/gpt_command_line.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 01:44:09.000000 gpt_command_line-0.1.6/gpt_command_line.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 01:44:09.000000 gpt_command_line-0.1.6/gpt_command_line.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 01:44:09.000000 gpt_command_line-0.1.6/gpt_command_line.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 01:44:09.000000 gpt_command_line-0.1.6/gpt_command_line.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 01:44:09.000000 gpt_command_line-0.1.6/gpt_command_line.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:44:09.241084 gpt_command_line-0.1.6/gptcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/google.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7884 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/gptcli/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 01:44:09.245084 gpt_command_line-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:44:09.241084 gpt_command_line-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/tests/test_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-15 01:44:00.000000 gpt_command_line-0.1.6/tests/test_term_utils.py
```

### Comparing `gpt-command-line-0.1.5/LICENSE` & `gpt_command_line-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/PKG-INFO` & `gpt_command_line-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.5
+Version: 0.1.6
 Summary: Command-line interface for ChatGPT, Claude and Bard
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -19,27 +19,27 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: anthropic==0.17.0
+Requires-Dist: anthropic==0.25.9
 Requires-Dist: attrs==23.2.0
-Requires-Dist: black==24.2.0
-Requires-Dist: mistralai==0.1.3
+Requires-Dist: black==24.4.2
+Requires-Dist: mistralai==0.1.8
 Requires-Dist: google-generativeai==0.1.0
-Requires-Dist: openai==1.13.3
+Requires-Dist: openai==1.30.1
 Requires-Dist: prompt-toolkit==3.0.43
 Requires-Dist: pytest==7.3.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: rich==13.7.1
-Requires-Dist: tiktoken==0.6.0
-Requires-Dist: tokenizers==0.15.2
-Requires-Dist: typing_extensions==4.10.0
+Requires-Dist: tiktoken==0.7.0
+Requires-Dist: tokenizers==0.19.1
+Requires-Dist: typing_extensions==4.11.0
 Provides-Extra: llama
 Requires-Dist: llama-cpp-python==0.2.55; extra == "llama"
 
 # gpt-cli
 
 Command-line interface for ChatGPT Claude and Bard.
 
@@ -209,14 +209,22 @@
 ```
 $ gpt pirate
 
 > Arrrr
 Ahoy, matey! What be bringing ye to these here waters? Be it treasure or adventure ye seek, we be sailing the high seas together. Ready yer map and compass, for we have a long voyage ahead!
 ```
 
+### Customize OpenAI API URL
+If you are using other models compatible with the OpenAI Python SDK, you can configure them by modifying the `openai_base_url` setting in the config file or using the `OPENAI_BASE_URL` environment variable .  
+
+Example:
+```
+openai_base_url: https://your-custom-api-url.com/v1
+```
+
 ## Other chat bots
 
 ### Anthropic Claude
 
 To use Claude, you should have an API key from [Anthropic](https://console.anthropic.com/) (currently there is a waitlist for API access). After getting the API key, you can add an environment variable
 
 ```bash
```

### Comparing `gpt-command-line-0.1.5/README.md` & `gpt_command_line-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -168,14 +168,22 @@
 ```
 $ gpt pirate
 
 > Arrrr
 Ahoy, matey! What be bringing ye to these here waters? Be it treasure or adventure ye seek, we be sailing the high seas together. Ready yer map and compass, for we have a long voyage ahead!
 ```
 
+### Customize OpenAI API URL
+If you are using other models compatible with the OpenAI Python SDK, you can configure them by modifying the `openai_base_url` setting in the config file or using the `OPENAI_BASE_URL` environment variable .  
+
+Example:
+```
+openai_base_url: https://your-custom-api-url.com/v1
+```
+
 ## Other chat bots
 
 ### Anthropic Claude
 
 To use Claude, you should have an API key from [Anthropic](https://console.anthropic.com/) (currently there is a waitlist for API access). After getting the API key, you can add an environment variable
 
 ```bash
```

### Comparing `gpt-command-line-0.1.5/gpt_command_line.egg-info/PKG-INFO` & `gpt_command_line-0.1.6/gpt_command_line.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.5
+Version: 0.1.6
 Summary: Command-line interface for ChatGPT, Claude and Bard
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -19,27 +19,27 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: anthropic==0.17.0
+Requires-Dist: anthropic==0.25.9
 Requires-Dist: attrs==23.2.0
-Requires-Dist: black==24.2.0
-Requires-Dist: mistralai==0.1.3
+Requires-Dist: black==24.4.2
+Requires-Dist: mistralai==0.1.8
 Requires-Dist: google-generativeai==0.1.0
-Requires-Dist: openai==1.13.3
+Requires-Dist: openai==1.30.1
 Requires-Dist: prompt-toolkit==3.0.43
 Requires-Dist: pytest==7.3.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: rich==13.7.1
-Requires-Dist: tiktoken==0.6.0
-Requires-Dist: tokenizers==0.15.2
-Requires-Dist: typing_extensions==4.10.0
+Requires-Dist: tiktoken==0.7.0
+Requires-Dist: tokenizers==0.19.1
+Requires-Dist: typing_extensions==4.11.0
 Provides-Extra: llama
 Requires-Dist: llama-cpp-python==0.2.55; extra == "llama"
 
 # gpt-cli
 
 Command-line interface for ChatGPT Claude and Bard.
 
@@ -209,14 +209,22 @@
 ```
 $ gpt pirate
 
 > Arrrr
 Ahoy, matey! What be bringing ye to these here waters? Be it treasure or adventure ye seek, we be sailing the high seas together. Ready yer map and compass, for we have a long voyage ahead!
 ```
 
+### Customize OpenAI API URL
+If you are using other models compatible with the OpenAI Python SDK, you can configure them by modifying the `openai_base_url` setting in the config file or using the `OPENAI_BASE_URL` environment variable .  
+
+Example:
+```
+openai_base_url: https://your-custom-api-url.com/v1
+```
+
 ## Other chat bots
 
 ### Anthropic Claude
 
 To use Claude, you should have an API key from [Anthropic](https://console.anthropic.com/) (currently there is a waitlist for API access). After getting the API key, you can add an environment variable
 
 ```bash
```

### Comparing `gpt-command-line-0.1.5/gpt_command_line.egg-info/SOURCES.txt` & `gpt_command_line-0.1.6/gpt_command_line.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/gptcli/anthropic.py` & `gpt_command_line-0.1.6/gptcli/anthropic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import os
 from typing import Iterator, List
 import anthropic
 
-from gptcli.completion import CompletionProvider, Message
+from gptcli.completion import (
+    CompletionProvider,
+    Message,
+    CompletionError,
+    BadRequestError,
+)
 
 api_key = os.environ.get("ANTHROPIC_API_KEY")
 
 
 def get_client():
     if not api_key:
         raise ValueError("ANTHROPIC_API_KEY environment variable not set")
@@ -49,21 +54,26 @@
         if len(messages) > 0 and messages[0]["role"] == "system":
             kwargs["system"] = messages[0]["content"]
             messages = messages[1:]
 
         kwargs["messages"] = messages
 
         client = get_client()
-        if stream:
-            with client.messages.stream(**kwargs) as stream:
-                for text in stream.text_stream:
-                    yield text
-        else:
-            response = client.messages.create(**kwargs, stream=False)
-            yield "".join(c.text for c in response.content)
+        try:
+            if stream:
+                with client.messages.stream(**kwargs) as completion:
+                    for text in completion.text_stream:
+                        yield text
+            else:
+                response = client.messages.create(**kwargs, stream=False)
+                yield "".join(c.text for c in response.content)
+        except anthropic.BadRequestError as e:
+            raise BadRequestError(e.message) from e
+        except anthropic.APIError as e:
+            raise CompletionError(e.message) from e
 
 
 def num_tokens_from_messages_anthropic(messages: List[Message], model: str) -> int:
     prompt = make_prompt(messages)
     client = get_client()
     return client.count_tokens(prompt)
```

### Comparing `gpt-command-line-0.1.5/gptcli/assistant.py` & `gpt_command_line-0.1.6/gptcli/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/gptcli/cli.py` & `gpt_command_line-0.1.6/gptcli/cli.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/gptcli/composite.py` & `gpt_command_line-0.1.6/gptcli/composite.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/gptcli/config.py` & `gpt_command_line-0.1.6/gptcli/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @dataclass
 class GptCliConfig:
     default_assistant: str = "general"
     markdown: bool = True
     show_price: bool = True
     api_key: Optional[str] = os.environ.get("OPENAI_API_KEY")
     openai_api_key: Optional[str] = os.environ.get("OPENAI_API_KEY")
+    openai_base_url: Optional[str] = os.environ.get("OPENAI_BASE_URL")
     anthropic_api_key: Optional[str] = os.environ.get("ANTHROPIC_API_KEY")
     google_api_key: Optional[str] = os.environ.get("GOOGLE_API_KEY")
     log_file: Optional[str] = None
     log_level: str = "INFO"
     assistants: Dict[str, AssistantConfig] = {}
     interactive: Optional[bool] = None
     llama_models: Optional[Dict[str, LLaMAModelConfig]] = None
```

### Comparing `gpt-command-line-0.1.5/gptcli/cost.py` & `gpt_command_line-0.1.6/gptcli/cost.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,30 @@
 }
 
 GPT_4_32K_PRICE_PER_TOKEN = {
     "prompt": 60.0 / 1_000_000,
     "response": 120.0 / 1_000_000,
 }
 
+GPT_4_O_PRICE_PER_TOKEN = {
+    "prompt": 5.0 / 1_000_000,
+    "response": 15.0 / 1_000_000,
+}
+
 
 def gpt_pricing(model: str, prompt: bool) -> Optional[float]:
     if model.startswith("gpt-3.5-turbo-16k"):
         pricing = GPT_3_5_TURBO_16K_PRICE_PER_TOKEN
     elif model.startswith("gpt-3.5-turbo"):
         pricing = GPT_3_5_TURBO_PRICE_PER_TOKEN
     elif model.startswith("gpt-4-32k"):
         pricing = GPT_4_32K_PRICE_PER_TOKEN
-    elif re.match(r"gpt-4-\d\d\d\d-preview", model):
+    elif model.startswith("gpt-4o"):
+        pricing = GPT_4_O_PRICE_PER_TOKEN
+    elif model.startswith("gpt-4-turbo") or re.match(r"gpt-4-\d\d\d\d-preview", model):
         pricing = GPT_4_TURBO_PRICE_PER_TOKEN
     elif model.startswith("gpt-4"):
         pricing = GPT_4_PRICE_PER_TOKEN
     else:
         return None
     return pricing["prompt" if prompt else "response"]
```

### Comparing `gpt-command-line-0.1.5/gptcli/google.py` & `gpt_command_line-0.1.6/gptcli/google.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/gptcli/gpt.py` & `gpt_command_line-0.1.6/gptcli/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,23 +164,21 @@
             filename=filename,
             level=args.log_level,
             format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
         )
         # Disable overly verbose logging for markdown_it
         logging.getLogger("markdown_it").setLevel(logging.INFO)
 
+    if config.openai_base_url:
+        openai.base_url = config.openai_base_url
+
     if config.api_key:
         openai.api_key = config.api_key
     elif config.openai_api_key:
         openai.api_key = config.openai_api_key
-    else:
-        print(
-            "No API key found. Please set the OPENAI_API_KEY environment variable or `api_key: <key>` value in ~/.config/gpt-cli/gpt.yml"
-        )
-        sys.exit(1)
 
     if config.anthropic_api_key:
         gptcli.anthropic.api_key = config.anthropic_api_key
 
     if config.google_api_key:
         genai.configure(api_key=config.google_api_key)
```

### Comparing `gpt-command-line-0.1.5/gptcli/llama.py` & `gpt_command_line-0.1.6/gptcli/llama.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/gptcli/logging.py` & `gpt_command_line-0.1.6/gptcli/logging.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/gptcli/openai.py` & `gpt_command_line-0.1.6/gptcli/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 from typing import Iterator, List, cast
 import openai
 from openai import OpenAI
 from openai.types.chat import ChatCompletionMessageParam
 
 import tiktoken
 
-from gptcli.completion import CompletionProvider, Message
+from gptcli.completion import (
+    CompletionProvider,
+    Message,
+    CompletionError,
+    BadRequestError,
+)
 
 
 class OpenAICompletionProvider(CompletionProvider):
     def __init__(self):
-        self.client = OpenAI(api_key=openai.api_key)
+        self.client = OpenAI(api_key=openai.api_key, base_url=openai.base_url)
 
     def complete(
         self, messages: List[Message], args: dict, stream: bool = False
     ) -> Iterator[str]:
         kwargs = {}
         if "temperature" in args:
             kwargs["temperature"] = args["temperature"]
         if "top_p" in args:
             kwargs["top_p"] = args["top_p"]
 
-        if stream:
-            response_iter = self.client.chat.completions.create(
-                messages=cast(List[ChatCompletionMessageParam], messages),
-                stream=True,
-                model=args["model"],
-                **kwargs,
-            )
-
-            for response in response_iter:
+        try:
+            if stream:
+                response_iter = self.client.chat.completions.create(
+                    messages=cast(List[ChatCompletionMessageParam], messages),
+                    stream=True,
+                    model=args["model"],
+                    **kwargs,
+                )
+
+                for response in response_iter:
+                    next_choice = response.choices[0]
+                    if next_choice.finish_reason is None and next_choice.delta.content:
+                        yield next_choice.delta.content
+            else:
+                response = self.client.chat.completions.create(
+                    messages=cast(List[ChatCompletionMessageParam], messages),
+                    model=args["model"],
+                    stream=False,
+                    **kwargs,
+                )
                 next_choice = response.choices[0]
-                if next_choice.finish_reason is None and next_choice.delta.content:
-                    yield next_choice.delta.content
-        else:
-            response = self.client.chat.completions.create(
-                messages=cast(List[ChatCompletionMessageParam], messages),
-                model=args["model"],
-                stream=False,
-                **kwargs,
-            )
-            next_choice = response.choices[0]
-            if next_choice.message.content:
-                yield next_choice.message.content
+                if next_choice.message.content:
+                    yield next_choice.message.content
+        except openai.BadRequestError as e:
+            raise BadRequestError(e.message) from e
+        except openai.APIError as e:
+            raise CompletionError(e.message) from e
 
 
 def num_tokens_from_messages_openai(messages: List[Message], model: str) -> int:
     encoding = tiktoken.encoding_for_model(model)
     num_tokens = 0
     for message in messages:
         # every message follows <im_start>{role/name}\n{content}<im_end>\n
```

### Comparing `gpt-command-line-0.1.5/gptcli/session.py` & `gpt_command_line-0.1.6/gptcli/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import abstractmethod
 from typing_extensions import TypeGuard
 from gptcli.assistant import Assistant
-from gptcli.completion import Message, ModelOverrides
-from openai import BadRequestError, OpenAIError
+from gptcli.completion import Message, ModelOverrides, CompletionError, BadRequestError
 from typing import Any, Dict, List, Tuple
 
 
 class ResponseStreamer:
     def __enter__(self) -> "ResponseStreamer":
         return self
 
@@ -111,15 +110,15 @@
                     stream.on_next_token(response)
         except KeyboardInterrupt:
             # If the user interrupts the chat completion, we'll just return what we have so far
             pass
         except BadRequestError as e:
             self.listener.on_error(e)
             return False
-        except OpenAIError as e:
+        except CompletionError as e:
             self.listener.on_error(e)
             return True
 
         next_message: Message = {"role": "assistant", "content": next_response}
         self.listener.on_chat_message(next_message)
         self.listener.on_chat_response(self.messages, next_message, args)
```

### Comparing `gpt-command-line-0.1.5/gptcli/shell.py` & `gpt_command_line-0.1.6/gptcli/shell.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/pyproject.toml` & `gpt_command_line-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gpt-command-line"
-version = "0.1.5"
+version = "0.1.6"
 description = "Command-line interface for ChatGPT, Claude and Bard"
 authors = [{name = "Val Kharitonov", email = "val@kharvd.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 keywords = ["cli", "command-line", "assistant", "openai", "claude", "bard", "gpt-3", "gpt-4", "llm", "chatgpt", "gpt-cli", "google-bard", "anthropic", "gpt-client", "anthropic-claude", "palm2"]
 classifiers = [
@@ -13,27 +13,27 @@
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
-    "anthropic==0.17.0",
+    "anthropic==0.25.9",
     "attrs==23.2.0",
-    "black==24.2.0",
-    "mistralai==0.1.3",
+    "black==24.4.2",
+    "mistralai==0.1.8",
     "google-generativeai==0.1.0",
-    "openai==1.13.3",
+    "openai==1.30.1",
     "prompt-toolkit==3.0.43",
     "pytest==7.3.1",
     "PyYAML==6.0.1",
     "rich==13.7.1",
-    "tiktoken==0.6.0",
-    "tokenizers==0.15.2",
-    "typing_extensions==4.10.0",
+    "tiktoken==0.7.0",
+    "tokenizers==0.19.1",
+    "typing_extensions==4.11.0",
 ]
 
 [project.optional-dependencies]
 llama = [
     "llama-cpp-python==0.2.55",
 ]
```

### Comparing `gpt-command-line-0.1.5/tests/test_assistant.py` & `gpt_command_line-0.1.6/tests/test_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.5/tests/test_session.py` & `gpt_command_line-0.1.6/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import mock
 import httpx
 
-from openai import BadRequestError, OpenAIError
+from gptcli.completion import CompletionError, BadRequestError
 
 from gptcli.session import ChatSession
 
 system_message = {"role": "system", "content": "system message"}
 
 
 def setup_assistant_mock():
@@ -194,21 +194,15 @@
     )
     listener_mock.on_chat_message.assert_has_calls([mock.call(assistant_message)])
 
 
 def test_invalid_request_error():
     assistant_mock, listener_mock, session = setup_session()
 
-    error = BadRequestError(
-        "error message",
-        response=httpx.Response(
-            401, request=httpx.Request("POST", "http://localhost/")
-        ),
-        body=None,
-    )
+    error = BadRequestError("error message")
     assistant_mock.complete_chat.side_effect = error
 
     user_input = "user message"
     should_continue = session.process_input(user_input, {})
     assert should_continue
 
     user_message = {"role": "user", "content": user_input}
@@ -225,22 +219,18 @@
 
     assistant_mock.complete_chat.assert_not_called()
     listener_mock.on_chat_message.assert_not_called()
     listener_mock.on_error.assert_not_called()
     listener_mock.on_chat_rerun.assert_called_once_with(False)
 
 
-class OpenAITestError(OpenAIError):
-    pass
-
-
 def test_openai_error():
     assistant_mock, listener_mock, session = setup_session()
 
-    error = OpenAITestError()
+    error = CompletionError("error message")
     assistant_mock.complete_chat.side_effect = error
 
     user_input = "user message"
     should_continue = session.process_input(user_input, {})
     assert should_continue
 
     user_message = {"role": "user", "content": user_input}
```

### Comparing `gpt-command-line-0.1.5/tests/test_term_utils.py` & `gpt_command_line-0.1.6/tests/test_term_utils.py`

 * *Files identical despite different names*

