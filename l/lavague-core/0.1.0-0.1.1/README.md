# Comparing `tmp/lavague_core-0.1.0.tar.gz` & `tmp/lavague_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.1.0.tar", max compression
+gzip compressed data, was "lavague_core-0.1.1.tar", max compression
```

## Comparing `lavague_core-0.1.0.tar` & `lavague_core-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-29 20:11:19.282709 lavague_core-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-29 20:11:19.282709 lavague_core-0.1.0/README.md
--rw-r--r--   0        0        0      370 2024-05-07 21:38:42.293576 lavague_core-0.1.0/lavague/core/__init__.py
--rw-r--r--   0        0        0      809 2024-05-07 16:08:17.886783 lavague_core-0.1.0/lavague/core/action_context.py
--rw-r--r--   0        0        0     3978 2024-05-07 15:42:37.222732 lavague_core-0.1.0/lavague/core/action_engine.py
--rw-r--r--   0        0        0     2595 2024-05-07 23:55:05.291906 lavague_core-0.1.0/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1294 2024-04-29 20:11:19.282709 lavague_core-0.1.0/lavague/core/extractors.py
--rw-r--r--   0        0        0      572 2024-05-07 21:41:12.520599 lavague_core-0.1.0/lavague/core/prompt_templates.py
--rw-r--r--   0        0        0    11518 2024-05-14 15:43:48.460467 lavague_core-0.1.0/lavague/core/retrievers.py
--rw-r--r--   0        0        0     2101 2024-04-29 20:11:19.282709 lavague_core-0.1.0/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     2055 2024-04-29 20:11:19.282709 lavague_core-0.1.0/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1330 2024-04-29 20:11:19.282709 lavague_core-0.1.0/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0      962 2024-05-07 22:11:53.320222 lavague_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 lavague_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 19:17:05.210186 lavague_core-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-15 19:17:05.210186 lavague_core-0.1.1/README.md
+-rw-r--r--   0        0        0      993 2024-05-15 19:20:55.646558 lavague_core-0.1.1/lavague/core/__init__.py
+-rw-r--r--   0        0        0     4084 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/action_engine.py
+-rw-r--r--   0        0        0     5556 2024-05-15 20:57:47.605949 lavague_core-0.1.1/lavague/core/agents.py
+-rw-r--r--   0        0        0     2778 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/base_driver.py
+-rw-r--r--   0        0        0     1896 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/extractors.py
+-rw-r--r--   0        0        0      613 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/prompt_templates.py
+-rw-r--r--   0        0        0    12118 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     3793 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     3561 2024-05-15 20:58:35.889500 lavague_core-0.1.1/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1361 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0      491 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1080 2024-05-15 19:17:05.210186 lavague_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.1/PKG-INFO
```

### Comparing `lavague_core-0.1.0/LICENSE` & `lavague_core-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.0/lavague/core/action_engine.py` & `lavague_core-0.1.1/lavague/core/action_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,45 @@
 from __future__ import annotations
-from typing import Optional, Generator
+from typing import Optional, Generator, List
 from llama_index.core.query_engine import RetrieverQueryEngine
-from llama_index.core import get_response_synthesizer
-from llama_index.core import PromptTemplate
+from llama_index.core import get_response_synthesizer, PromptTemplate, QueryBundle
 from llama_index.core.base.llms.base import BaseLLM
 from llama_index.core.base.embeddings.base import BaseEmbedding
 from lavague.core.extractors import BaseExtractor
 from lavague.core.retrievers import BaseHtmlRetriever
 from lavague.core.base_driver import BaseDriver
-from lavague.core.action_context import ActionContext
+from lavague.core.context import Context, get_default_context
+
 
 class ActionEngine:
     """
     ActionEngine leverages the llm model and the embedding model to output code from the prompt and the html page.
 
     Args:
         driver (`BaseDriver`):
             The Web driver used to interact with the headless browser
-        llm (`BaseLLM`):
-            The llm that will be used the generate the python code
-        embedding: (`BaseEmbedding`)
-            The embedder used by the retriever
-        retriever (`BaseHtmlRetriever`)
-            The retriever used to extract context from the html page
-        prompt_template (`str`):
-            The prompt_template given to the llm, later completed by chunks of the html page and the query
-        cleaning_function (`Callable[[str], Optional[str]]`):
-            Function to extract the python code from the llm output
     """
 
     def __init__(
         self,
         driver: BaseDriver,
-        llm: BaseLLM,
-        embedding: BaseEmbedding,
-        retriever: BaseHtmlRetriever,
-        prompt_template: PromptTemplate,
-        extractor: BaseExtractor,
+        context: Optional[Context] = None,
     ):
-        self.driver = driver
-        self.llm = llm
-        self.embedding = embedding
-        self.retriever = retriever
-        self.prompt_template = prompt_template.partial_format(driver_capability=driver.get_capability())
-        self.extractor = extractor
-
-    def from_context(driver: BaseDriver, context: ActionContext) -> ActionEngine:
-        return ActionEngine(driver, context.llm, context.embedding, context.retriever, context.prompt_template, context.extractor)
-
-    def _get_query_engine(
-        self, streaming: bool = True
-    ) -> RetrieverQueryEngine:
+        if context is None:
+            context = get_default_context()
+        self.driver: BaseDriver = driver
+        self.llm: BaseLLM = context.llm
+        self.embedding: BaseEmbedding = context.embedding
+        self.retriever: BaseHtmlRetriever = context.retriever
+        self.prompt_template: PromptTemplate = context.prompt_template.partial_format(
+            driver_capability=driver.get_capability()
+        )
+        self.extractor: BaseExtractor = context.extractor
+
+    def _get_query_engine(self, streaming: bool = True) -> RetrieverQueryEngine:
         """
         Get the llama-index query engine
 
         Args:
             html: (`str`)
             streaming (`bool`)
 
@@ -74,14 +59,39 @@
 
         query_engine.update_prompts(
             {"response_synthesizer:text_qa_template": self.prompt_template}
         )
 
         return query_engine
 
+    def get_nodes(self, query: str) -> List[str]:
+        """
+        Get the nodes from the html page
+
+        Args:
+            html (`str`): The html page
+
+        Return:
+            `List[str]`: The nodes
+        """
+        source_nodes = self.retriever.retrieve_html(
+            self.driver, self.embedding, QueryBundle(query_str=query)
+        )
+        source_nodes = [node.text for node in source_nodes]
+        return source_nodes
+
+    def get_action_from_context(self, context: str, query: str) -> str:
+        """
+        Generate the code from a query and a context
+        """
+        prompt = self.prompt_template.format(context_str=context, query_str=query)
+        response = self.llm.complete(prompt).text
+        code = self.extractor.extract(response)
+        return code
+
     def get_action(self, query: str) -> Optional[str]:
         """
         Generate the code from a query
 
         Args:
             query (`str`): Instructions given at the end of the prompt to tell the model what to do on the html page
```

### Comparing `lavague_core-0.1.0/lavague/core/base_driver.py` & `lavague_core-0.1.1/lavague/core/base_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from typing import Tuple, Any, Callable, Optional
 from abc import ABC, abstractmethod
-from lavague.core.utilities.format_utils import extract_code_from_funct, extract_imports_from_lines
+from lavague.core.utilities.format_utils import (
+    extract_code_from_funct,
+    extract_imports_from_lines,
+)
 
-class BaseDriver(ABC):
 
+class BaseDriver(ABC):
     def __init__(self, url: Optional[str], init_function: Optional[Callable[[], Any]]):
         """Init the driver with the init funtion, and then go to the desired url"""
-        self.init_function = init_function if init_function is not None else self.default_init_code
+        self.init_function = (
+            init_function if init_function is not None else self.default_init_code
+        )
         self.driver = self.init_function()
 
         # extract import lines for later exec of generated code
         init_lines = extract_code_from_funct(self.init_function)
         self.import_lines = extract_imports_from_lines(init_lines)
 
         if url is not None:
@@ -28,14 +33,20 @@
 
     @abstractmethod
     def get_driver(self) -> Any:
         """Return the expected variable name and the driver object"""
         pass
 
     @abstractmethod
+    def resize_driver(driver, width, height):
+        """
+        Resize the driver to a targeted height and width.
+        """
+
+    @abstractmethod
     def get_url(self) -> Optional[str]:
         """Get the url of the current page"""
         pass
 
     @abstractmethod
     def go_to_url_code(self, url: str) -> str:
         """Return the code to navigate to the url"""
@@ -52,28 +63,28 @@
         Returns the HTML of the current page.
         If clean is True, We remove unnecessary tags and attributes from the HTML.
         Clean HTMLs are easier to process for the LLM.
         """
         pass
 
     @abstractmethod
-    def get_screenshot(self, filename: str) -> None:
+    def save_screenshot(self, filename: str) -> None:
         """Save a screenshot to the file filename"""
         pass
 
     @abstractmethod
     def get_dummy_code(self) -> str:
         """Return testing code relevant for the current driver"""
         pass
 
     @abstractmethod
     def check_visibility(self, xpath: str) -> bool:
         """Check an element visibility by its xpath"""
         pass
-    
+
     @abstractmethod
     def exec_code(self, code: str):
         """Exec generated code"""
         pass
 
     @abstractmethod
     def get_capability(self) -> str:
```

### Comparing `lavague_core-0.1.0/lavague/core/extractors.py` & `lavague_core-0.1.1/lavague/core/extractors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from abc import ABC, abstractmethod
 import re
 
+
 class BaseExtractor(ABC):
     @abstractmethod
     def extract(self, text: str) -> str:
         pass
 
+
 class PythonFromMarkdownExtractor(BaseExtractor):
     """
     Extractor for the prompts that end with (or similar to) the following:
 
     --------------------------------------------
     Completion:
     --------------------------------------------
     """
+
     def extract(self, markdown_text: str) -> str:
         # Pattern to match the first ```python ``` code block
         pattern = r"```python(.*?)```"
 
         # Using re.DOTALL to make '.' match also newlines
         match = re.search(pattern, markdown_text, re.DOTALL)
         if match:
             # Return the first matched group, which is the code inside the ```python ```
             return match.group(1).strip()
         else:
             # Return None if no match is found
             return None
 
+
 class UntilEndOfMarkdownExtractor(BaseExtractor):
     """
     Extractor for the prompts that end with (or similar to) the following:
-    
+
     --------------------------------------------
     Completion:
     ```python
     # Let's proceed step by step.
     --------------------------------------------
     """
+
     def extract(self, text: str) -> str:
-        return text.split("```")[0]
+        return text.split("```")[0]
```

### Comparing `lavague_core-0.1.0/lavague/core/retrievers.py` & `lavague_core-0.1.1/lavague/core/retrievers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,54 +8,66 @@
 from llama_index.core.base.base_retriever import BaseRetriever
 from llama_index.core import Document
 from llama_index.core.node_parser import CodeSplitter
 from llama_index.core import VectorStoreIndex
 from llama_index.core import QueryBundle
 from llama_index.core.schema import NodeWithScore
 from llama_index.core.schema import TextNode
-from langchain_text_splitters import RecursiveCharacterTextSplitter
+from langchain.text_splitter import RecursiveCharacterTextSplitter
 from llama_index.core.node_parser import LangchainNodeParser
 from lavague.core.base_driver import BaseDriver
 from lavague.core.utilities.format_utils import clean_html
 
 
 class _LlamaIndexAdapter(BaseRetriever):
     """Adapter for HtmlRetriever to be compatible with the llama index BaseRetriever"""
 
-    def __init__(self, html_retriever: BaseHtmlRetriever, driver: BaseDriver, embedding: BaseEmbedding):
+    def __init__(
+        self,
+        html_retriever: BaseHtmlRetriever,
+        driver: BaseDriver,
+        embedding: BaseEmbedding,
+    ):
         self.html_retriever = html_retriever
         self.driver = driver
-        self.embedding = embedding 
+        self.embedding = embedding
         super().__init__()
 
     def _retrieve(self, query_bundle: QueryBundle) -> List[NodeWithScore]:
-        return self.html_retriever._retrieve_html(self.driver, self.embedding, query_bundle)
+        return self.html_retriever._retrieve_html(
+            self.driver, self.embedding, query_bundle
+        )
 
 
 class BaseHtmlRetriever(ABC):
-
     @abstractmethod
-    def _retrieve_html(self, driver: BaseDriver, embedding: BaseEmbedding, query: QueryBundle) -> List[NodeWithScore]:
+    def retrieve_html(
+        self, driver: BaseDriver, embedding: BaseEmbedding, query: QueryBundle
+    ) -> List[NodeWithScore]:
         """
         This method should be implemented by the user
         """
         pass
 
-    def to_llama_index(self, driver: BaseDriver, embedding: BaseEmbedding) -> BaseRetriever:
+    def to_llama_index(
+        self, driver: BaseDriver, embedding: BaseEmbedding
+    ) -> BaseRetriever:
         """Convert to a llama-index compatible retriever"""
         return _LlamaIndexAdapter(self, driver, embedding)
 
 
-class LegacyRetriever(BaseHtmlRetriever):
+class BM25HtmlRetriever(BaseHtmlRetriever):
     """Mainly for benchmarks, do not use it as the performances are not up to par with the other retrievers"""
 
     def __init__(self, top_k: int = 3):
         self.top_k = top_k
 
-    def _retrieve_html(self, driver: BaseDriver, embedding: BaseEmbedding, query: QueryBundle) -> List[NodeWithScore]:
+    def retrieve_html(
+        self, driver: BaseDriver, embedding: BaseEmbedding, query: QueryBundle
+    ) -> List[NodeWithScore]:
         text_list = [clean_html(driver.get_html())]
         documents = [Document(text=t) for t in text_list]
 
         splitter = CodeSplitter(
             language="html",
             chunk_lines=50,  # lines per chunk
             chunk_lines_overlap=15,  # lines overlap between chunks
@@ -78,180 +90,217 @@
         group_by: int = 10,
         rank_fields: List[str] = ["element", "placeholder", "text", "name"],
     ):
         self.top_k = top_k
         self.group_by = group_by
         self.rank_fields = rank_fields
 
-    def _generate_xpath(self, element, path=""): # used to generate dict nodes
-        """ Recursive function to generate the xpath of an element """
+    def _generate_xpath(self, element, path=""):  # used to generate dict nodes
+        """Recursive function to generate the xpath of an element"""
         if element.parent is None:
             return path
         else:
-            siblings = [sib for sib in element.parent.children if sib.name == element.name]
+            siblings = [
+                sib for sib in element.parent.children if sib.name == element.name
+            ]
             if len(siblings) > 1:
                 count = siblings.index(element) + 1
                 path = f"/{element.name}[{count}]{path}"
             else:
                 path = f"/{element.name}{path}"
             return self._generate_xpath(element.parent, path)
-        
+
     def _add_xpath_attributes(self, html_content):
         """
         Add an 'xpath' attribute to each element in the HTML content with its computed XPath.
         """
-        soup = BeautifulSoup(html_content, 'lxml')
+        soup = BeautifulSoup(html_content, "lxml")
         for element in soup.find_all(True):
             xpath = self._generate_xpath(element)
-            element['xpath'] = xpath
+            element["xpath"] = xpath
         return str(soup)
 
-    def _create_nodes_dict(self, html, only_body=True, max_length=200): # used to generate dict nodes
-        ''' Create a list of xpaths and a list of dict of attributes of all elements in the html'''
-        soup = BeautifulSoup(html, 'html.parser')
+    def _create_nodes_dict(
+        self, html, only_body=True, max_length=200
+    ):  # used to generate dict nodes
+        """Create a list of xpaths and a list of dict of attributes of all elements in the html"""
+        soup = BeautifulSoup(html, "html.parser")
         if only_body:
             root = soup.body
         else:
             root = soup.html
         element_attributes_list = []
         stack = [root]  # stack to keep track of elements and their paths
         while stack:
             element = stack.pop()
             if element.name is not None:
                 element_attrs = dict(element.attrs)
-                direct_text_content = ''.join([str(content).strip() for content in element.contents if isinstance(content, NavigableString) and content.strip()])
+                direct_text_content = "".join(
+                    [
+                        str(content).strip()
+                        for content in element.contents
+                        if isinstance(content, NavigableString) and content.strip()
+                    ]
+                )
                 if direct_text_content:
-                    element_attrs['text'] = direct_text_content
-                    element_attrs['element'] = element.name
+                    element_attrs["text"] = direct_text_content
+                    element_attrs["element"] = element.name
                     for key in element_attrs:
                         if len(element_attrs[key]) > max_length:
                             element_attrs[key] = element_attrs[key][:max_length]
                     element_attributes_list.append(element_attrs)
                 elif element_attrs != {}:
-                    element_attrs['element'] = element.name
+                    element_attrs["element"] = element.name
                     for key in element_attrs:
                         if len(element_attrs[key]) > max_length:
                             element_attrs[key] = element_attrs[key][:max_length]
                     element_attributes_list.append(element_attrs)
                 for child in element.children:
                     if child.name is not None:
                         stack.append(child)
         return element_attributes_list
 
     def _chunk_dicts(self, dicts, chunk_size=10):
         def chunks(lst, n):
             for i in range(0, len(lst), n):
-                yield lst[i:i + n]
+                yield lst[i : i + n]
+
         grouped_chunks = []
         for chunk in chunks(dicts, chunk_size):
-            all_keys = set(key for d in chunk for key in d.keys()) 
+            all_keys = set(key for d in chunk for key in d.keys())
             grouped = {key: [] for key in all_keys}
             for d in chunk:
                 for key in all_keys:
-                    grouped[key].append(d.get(key, ''))  
-            grouped_chunks.append(grouped)   
+                    grouped[key].append(d.get(key, ""))
+            grouped_chunks.append(grouped)
         return grouped_chunks
 
     def _unchunk_dicts(self, grouped_chunks):
         flat_list = []
         for group in grouped_chunks:
             max_length = max(len(v) for v in group.values())
             for i in range(max_length):
                 new_dict = {}
                 for key, values in group.items():
                     if i < len(values):
-                        if values[i] != '':
+                        if values[i] != "":
                             new_dict[key] = values[i]
                 if new_dict:
                     flat_list.append(new_dict)
         return flat_list
 
-    def _clean_attributes(self, attributes_list): # used to generate dict nodes
+    def _clean_attributes(self, attributes_list):  # used to generate dict nodes
         if self.rank_fields:
-            self.rank_fields.append('xpath')
-            attributes_list = [{k: v for k, v in d.items() if k in self.rank_fields} for d in attributes_list]
-        attributes_list = [d for d in attributes_list if (not((len(list(d.keys()))==2) and (('element' in list(d.keys())) and 'xpath' in list(d.keys())))) or d=={}]
+            self.rank_fields.append("xpath")
+            attributes_list = [
+                {k: v for k, v in d.items() if k in self.rank_fields}
+                for d in attributes_list
+            ]
+        attributes_list = [
+            d
+            for d in attributes_list
+            if (
+                not (
+                    (len(list(d.keys())) == 2)
+                    and (("element" in list(d.keys())) and "xpath" in list(d.keys()))
+                )
+            )
+            or d == {}
+        ]
         return attributes_list
 
-    def _get_results(self, embedding, query, html): # used to generate and retrieve dict nodes
-        ''' Return the top_k elements of the html that are the most relevant to the query as Node objects with xpath in their metadata'''
+    def _get_results(
+        self, embedding, query, html
+    ):  # used to generate and retrieve dict nodes
+        """Return the top_k elements of the html that are the most relevant to the query as Node objects with xpath in their metadata"""
         attributes_list = self._create_nodes_dict(html)
-        #cleaning the attributes_list
+        # cleaning the attributes_list
         attributes_list = self._clean_attributes(attributes_list)
-        #retrieving the top_k results
-        
+        # retrieving the top_k results
+
         list_of_results = []
         attributes_list = self._chunk_dicts(attributes_list, self.group_by)
         l = len(attributes_list)
-        #grouping the attributes_list in groups of 1000 to avoid memory errors
+        # grouping the attributes_list in groups of 1000 to avoid memory errors
         list_of_grouped_results = []
         for j in range(0, l, 1000):
             nodes = []
-            attr = attributes_list[j:j+1000]
+            attr = attributes_list[j : j + 1000]
             for d in attr:
-                xpath = d.pop('xpath')
-                nodes.append(TextNode(text=str(d), metadata={'xpath': xpath}))
+                xpath = d.pop("xpath")
+                nodes.append(TextNode(text=str(d), metadata={"xpath": xpath}))
             index = VectorStoreIndex(nodes, embed_model=embedding)
-            retriever = BM25Retriever.from_defaults(index = index, similarity_top_k=self.top_k)
+            retriever = BM25Retriever.from_defaults(
+                index=index, similarity_top_k=self.top_k
+            )
             results = retriever.retrieve(query)
             list_of_grouped_results += results
         nodes = []
         for grouped_results in list_of_grouped_results:
-            xpaths = grouped_results.metadata['xpath']
+            xpaths = grouped_results.metadata["xpath"]
             ds = self._unchunk_dicts([ast.literal_eval(grouped_results.text)])
             assert len(xpaths) == len(ds)
             for xpath, d in zip(xpaths, ds):
-                nodes.append(TextNode(text=str(d), metadata={'xpath': xpath}))
+                nodes.append(TextNode(text=str(d), metadata={"xpath": xpath}))
         l2 = len(nodes)
         for j in range(0, l2, 1000):
-            index = VectorStoreIndex(nodes[j:j+1000], embed_model=embedding)
-            retriever = BM25Retriever.from_defaults(index = index, similarity_top_k=self.top_k)
+            index = VectorStoreIndex(nodes[j : j + 1000], embed_model=embedding)
+            retriever = BM25Retriever.from_defaults(
+                index=index, similarity_top_k=self.top_k
+            )
             results = retriever.retrieve(query)
             list_of_results += results
         list_of_results = sorted(list_of_results, key=lambda x: x.score, reverse=True)
-        results = list_of_results[:self.top_k]
+        results = list_of_results[: self.top_k]
         results_dict = [ast.literal_eval(r.text) for r in results]
         for i in range(len(results_dict)):
-            results_dict[i]['xpath'] = results[i].metadata['xpath']
+            results_dict[i]["xpath"] = results[i].metadata["xpath"]
         scores = [r.score for r in results]
         return results_dict, scores
 
     def _match_element(self, attributes, element_specs):
-        i=0
+        i = 0
         for spec in element_specs:
-            if attributes['xpath'] == spec['xpath']:
-                return i       
-            i+=1
+            if attributes["xpath"] == spec["xpath"]:
+                return i
+            i += 1
         return None
 
     def _return_nodes_with_xpath(self, nodes, results_dict, score):
         returned_nodes = []
         for node in nodes:
             split_html = node.text
-            soup = BeautifulSoup(split_html, 'html.parser')
-            for element  in soup.descendants:
+            soup = BeautifulSoup(split_html, "html.parser")
+            for element in soup.descendants:
                 try:
                     indice = self._match_element(element.attrs, results_dict)
                     if indice is not None:
-                        node.metadata['score'] = score[indice]
+                        node.metadata["score"] = score[indice]
                         returned_nodes.append(node)
                 except:
                     pass
         return returned_nodes
 
-    def _retrieve_html(self, driver: BaseDriver, embedding: BaseEmbedding, query: QueryBundle) -> List[NodeWithScore]:
+    def retrieve_html(
+        self, driver: BaseDriver, embedding: BaseEmbedding, query: QueryBundle
+    ) -> List[NodeWithScore]:
         html = self._add_xpath_attributes(driver.get_html())
         text_list = [html]
         documents = [Document(text=t) for t in text_list]
-        splitter = LangchainNodeParser(lc_splitter=RecursiveCharacterTextSplitter.from_language(
+        splitter = LangchainNodeParser(
+            lc_splitter=RecursiveCharacterTextSplitter.from_language(
                 language="html",
-            ))
+            )
+        )
         nodes = splitter.get_nodes_from_documents(documents)
         results_dict, score = self._get_results(embedding, query.query_str, html)
         for r in results_dict:
-            if not driver.check_visibility(r['xpath']):
+            if not driver.check_visibility(r["xpath"]):
                 i = results_dict.index(r)
                 results_dict.remove(r)
                 score.pop(i)
         results_nodes = self._return_nodes_with_xpath(nodes, results_dict, score)
-        results = [NodeWithScore(node=node, score=node.metadata['score']) for node in results_nodes] 
+        results = [
+            NodeWithScore(node=node, score=node.metadata["score"])
+            for node in results_nodes
+        ]
         return results
```

### Comparing `lavague_core-0.1.0/lavague/core/utilities/version_checker.py` & `lavague_core-0.1.1/lavague/core/utilities/version_checker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import requests
 import pkg_resources
 
-YELLOW = '\033[93m'
-RESET = '\033[0m'
+YELLOW = "\033[93m"
+RESET = "\033[0m"
+
 
 def compare_versions(version1, version2):
-    v1 = list(map(int, version1.split('.')))
-    v2 = list(map(int, version2.split('.')))
-    
+    v1 = list(map(int, version1.split(".")))
+    v2 = list(map(int, version2.split(".")))
+
     while len(v1) < len(v2):
         v1.append(0)
     while len(v2) < len(v1):
         v2.append(0)
-    
+
     for i in range(len(v1)):
         if v1[i] > v2[i]:
             return 1
         elif v1[i] < v2[i]:
             return -1
-    
+
     return 0
 
+
 def get_installed_version(dist_name, lookup_dirs=None):
     req = pkg_resources.Requirement.parse(dist_name)
 
     if lookup_dirs is None:
         working_set = pkg_resources.WorkingSet()
     else:
         working_set = pkg_resources.WorkingSet(lookup_dirs)
 
     dist = working_set.find(req)
     return dist.version if dist else None
 
+
 def check_latest_version():
     package_version = get_installed_version("lavague")
     url = "https://pypi.org/pypi/lavague/json"
     response = requests.get(url)
     data = response.json()
     latest_version = data["info"]["version"]
-    if (compare_versions(package_version, latest_version) < 0):
-        print(YELLOW + f"You are using lavague version {package_version}, however version {latest_version} is "
-        "available.\nYou should consider upgrading via the "
-        "'pip install --upgrade lavague' command." + RESET)
+    if compare_versions(package_version, latest_version) < 0:
+        print(
+            YELLOW
+            + f"You are using lavague version {package_version}, however version {latest_version} is "
+            "available.\nYou should consider upgrading via the "
+            "'pip install --upgrade lavague' command." + RESET
+        )
```

### Comparing `lavague_core-0.1.0/pyproject.toml` & `lavague_core-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.1.0"
+version = "0.1.1"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -20,9 +20,15 @@
 keywords = ["LAM", "action", "automation", "LLM", "NLP", "RAG", "selenium", "playwright"]
 homepage = "https://lavague.ai"
 repository = "https://github.com/lavague-ai/LaVague/"
 documentation = "https://docs.lavague.ai/en/latest/"
 packages = [{include = "lavague/"}]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = "^3.10.0"
 llama-index = "^0.10.19"
+llama-index-retrievers-bm25 = "^0.1.3"
+lxml = "^5.2.2"
+langchain = "^0.1.20"
+ipython = "^8.24.0"
+msgpack = "^1.0.8"
+
```

### Comparing `lavague_core-0.1.0/PKG-INFO` & `lavague_core-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: ipython (>=8.24.0,<9.0.0)
+Requires-Dist: langchain (>=0.1.20,<0.2.0)
 Requires-Dist: llama-index (>=0.10.19,<0.11.0)
+Requires-Dist: llama-index-retrievers-bm25 (>=0.1.3,<0.2.0)
+Requires-Dist: lxml (>=5.2.2,<6.0.0)
+Requires-Dist: msgpack (>=1.0.8,<2.0.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
```

