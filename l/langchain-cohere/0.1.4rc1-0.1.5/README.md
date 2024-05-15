# Comparing `tmp/langchain_cohere-0.1.4rc1.tar.gz` & `tmp/langchain_cohere-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cohere-0.1.4rc1.tar", max compression
+gzip compressed data, was "langchain_cohere-0.1.5.tar", max compression
```

## Comparing `langchain_cohere-0.1.4rc1.tar` & `langchain_cohere-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/LICENSE
--rw-r--r--   0        0        0     5585 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/README.md
--rw-r--r--   0        0        0      608 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/__init__.py
--rw-r--r--   0        0        0    19128 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/chat_models.py
--rw-r--r--   0        0        0     8173 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/cohere_agent.py
--rw-r--r--   0        0        0     1585 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/common.py
--rw-r--r--   0        0        0     5813 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/embeddings.py
--rw-r--r--   0        0        0     8058 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/llms.py
--rw-r--r--   0        0        0        0 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/py.typed
--rw-r--r--   0        0        0     3340 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/rag_retrievers.py
--rw-r--r--   0        0        0        0 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/__init__.py
--rw-r--r--   0        0        0     4913 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/agent.py
--rw-r--r--   0        0        0     4060 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/default_prompt_constants.py
--rw-r--r--   0        0        0    11351 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/parsing.py
--rw-r--r--   0        0        0     9728 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/prompt.py
--rw-r--r--   0        0        0     4134 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/langchain_cohere/rerank.py
--rw-r--r--   0        0        0     1655 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/langchain_cohere/utils.py
--rw-r--r--   0        0        0     2682 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/pyproject.toml
--rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 langchain_cohere-0.1.4rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5585 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/README.md
+-rw-r--r--   0        0        0      608 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/__init__.py
+-rw-r--r--   0        0        0    19079 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/chat_models.py
+-rw-r--r--   0        0        0     8141 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/cohere_agent.py
+-rw-r--r--   0        0        0     1585 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/common.py
+-rw-r--r--   0        0        0     5813 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/embeddings.py
+-rw-r--r--   0        0        0     8058 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/llms.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/py.typed
+-rw-r--r--   0        0        0     3340 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/rag_retrievers.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/__init__.py
+-rw-r--r--   0        0        0     4913 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/agent.py
+-rw-r--r--   0        0        0     4060 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/default_prompt_constants.py
+-rw-r--r--   0        0        0    11351 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/parsing.py
+-rw-r--r--   0        0        0     9728 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/prompt.py
+-rw-r--r--   0        0        0     4134 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/rerank.py
+-rw-r--r--   0        0        0     1655 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/langchain_cohere/utils.py
+-rw-r--r--   0        0        0     2889 2024-05-15 19:11:27.919180 langchain_cohere-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6408 1970-01-01 00:00:00.000000 langchain_cohere-0.1.5/PKG-INFO
```

### Comparing `langchain_cohere-0.1.4rc1/LICENSE` & `langchain_cohere-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/README.md` & `langchain_cohere-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/__init__.py` & `langchain_cohere-0.1.5/langchain_cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/chat_models.py` & `langchain_cohere-0.1.5/langchain_cohere/chat_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     Optional,
     Sequence,
     Type,
     Union,
 )
 
 from cohere.types import NonStreamedChatResponse, ToolCall
-from langchain_core._api import beta
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.documents import Document
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
@@ -240,15 +239,14 @@
         self,
         tools: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool]],
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         formatted_tools = _format_to_cohere_tools(tools)
         return super().bind(tools=formatted_tools, **kwargs)
 
-    @beta()
     def with_structured_output(
         self,
         schema: Union[Dict, Type[BaseModel]],
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, Union[Dict, BaseModel]]:
         """Model wrapper that returns outputs formatted to match the given schema.
```

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/cohere_agent.py` & `langchain_cohere-0.1.5/langchain_cohere/cohere_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from typing import Any, Callable, Dict, List, Sequence, Tuple, Type, Union
 
 from cohere.types import (
-    ChatRequestToolResultsItem,
     Tool,
     ToolCall,
     ToolParameterDefinitionsValue,
+    ToolResult,
 )
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.outputs import Generation
 from langchain_core.outputs.chat_generation import ChatGeneration
 from langchain_core.prompts.chat import ChatPromptTemplate
@@ -81,15 +81,15 @@
                 tool_call_parameters = json.loads(agent_action.tool_input)
                 if not isinstance(tool_call_parameters, dict):
                     raise ValueError()
             except ValueError:
                 # tool_input is a string, last ditch attempt at having something useful.
                 tool_call_parameters = {"input": agent_action.tool_input}
         tool_results.append(
-            ChatRequestToolResultsItem(
+            ToolResult(
                 call=ToolCall(
                     name=agent_action.tool,
                     parameters=tool_call_parameters,
                 ),
                 outputs=[{"answer": observation}],
             ).dict()
         )
```

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/common.py` & `langchain_cohere-0.1.5/langchain_cohere/common.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/embeddings.py` & `langchain_cohere-0.1.5/langchain_cohere/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/llms.py` & `langchain_cohere-0.1.5/langchain_cohere/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/rag_retrievers.py` & `langchain_cohere-0.1.5/langchain_cohere/rag_retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/agent.py` & `langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/default_prompt_constants.py` & `langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/default_prompt_constants.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/parsing.py` & `langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/parsing.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/prompt.py` & `langchain_cohere-0.1.5/langchain_cohere/react_multi_hop/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/rerank.py` & `langchain_cohere-0.1.5/langchain_cohere/rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/langchain_cohere/utils.py` & `langchain_cohere-0.1.5/langchain_cohere/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc1/pyproject.toml` & `langchain_cohere-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-cohere"
-version = "0.1.4rc1"
+version = "0.1.5"
 description = "An integration package connecting Cohere and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-cohere"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-cohere/tree/main/libs/cohere"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.42"
-cohere = ">=5.3,<6.0"
+langchain-core = ">=0.1.42,<0.3"
+cohere = ">=5.5,<6.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
@@ -34,15 +34,16 @@
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
-langchain = "^0.1.14"
+langchain = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/langchain" }
+langchain-text-splitters = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/text-splitters" }
 pytest-vcr = "^1.0.2"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
```

### Comparing `langchain_cohere-0.1.4rc1/PKG-INFO` & `langchain_cohere-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-cohere
-Version: 0.1.4rc1
+Version: 0.1.5
 Summary: An integration package connecting Cohere and LangChain
 Home-page: https://github.com/langchain-ai/langchain-cohere
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cohere (>=5.3,<6.0)
-Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
+Requires-Dist: cohere (>=5.5,<6.0)
+Requires-Dist: langchain-core (>=0.1.42,<0.3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-cohere
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-cohere/tree/main/libs/cohere
 Description-Content-Type: text/markdown
 
 # Langchain-Cohere
 
 This package contains the LangChain integrations for [Cohere](https://cohere.com/).
```

