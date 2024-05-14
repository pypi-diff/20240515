# Comparing `tmp/arize_phoenix_evals-0.8.1.tar.gz` & `tmp/arize_phoenix_evals-0.8.2.tar.gz`

## Comparing `arize_phoenix_evals-0.8.1.tar` & `arize_phoenix_evals-0.8.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/__init__.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/classify.py
--rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/default_templates.py
--rw-r--r--   0        0        0    15930 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/evaluators.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/exceptions.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/executors.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/generate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/py.typed
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/retrievals.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/templates.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/utils.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/anthropic.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/base.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/bedrock.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/litellm.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/mistralai.py
--rw-r--r--   0        0        0    15069 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/openai.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/rate_limiters.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/vertex.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/vertexai.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/.gitignore
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/IP_NOTICE
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/LICENSE
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/README.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/__init__.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/classify.py
+-rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/default_templates.py
+-rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/evaluators.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/exceptions.py
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/executors.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/generate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/py.typed
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/retrievals.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/templates.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/utils.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/anthropic.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/base.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/bedrock.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/litellm.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/mistralai.py
+-rw-r--r--   0        0        0    15069 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/openai.py
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/rate_limiters.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/vertex.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/vertexai.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/.gitignore
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/IP_NOTICE
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/LICENSE
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/README.md
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/PKG-INFO
```

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/__init__.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/classify.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/classify.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/default_templates.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/default_templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/evaluators.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/evaluators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from textwrap import indent
-from typing import List, Mapping, Optional, Tuple, Type
+from typing import List, Mapping, Optional, Tuple
 
 from phoenix.evals.default_templates import EvalCriteria
 from phoenix.evals.models import BaseModel, OpenAIModel, set_verbosity
 from phoenix.evals.templates import (
     ClassificationTemplate,
     PromptOptions,
     PromptTemplate,
@@ -160,84 +159,103 @@
             use_openai_function_call=use_openai_function_call,
             verbose=verbose,
         )
         score = self._template.score(label)
         return label, score, explanation
 
 
-def _create_llm_evaluator_subclass(
-    class_name: str, template: ClassificationTemplate, docstring: str
-) -> Type[LLMEvaluator]:
-    """A factory method that dynamically creates subclasses of LLMEvaluator.
-
-    Args:
-        class_name (str): Name of the class to be created (should match the name
-        of the assignment variable).
-
-        template (ClassificationTemplate): The classification template to use
-        for evaluation.
-
-        docstring (str): The docstring that will be attached to the subclass.
-
-    Returns:
-        Type[LLMEvaluator]: The dynamically created subclass.
-    """
-
-    def __init__(self: LLMEvaluator, model: BaseModel) -> None:
-        LLMEvaluator.__init__(self, model, template)
-
-    __init__.__doc__ = f"""
-        Initializer for {class_name}.
-
-        Args:
-            model (BaseEvalModel): The LLM model to use for evaluation."""
-
-    docstring += f" Outputs railed classes {', '.join(template.rails)}."
-    docstring += "\n\nThe template used for evaluation (without explanation) is:\n\n"
-    docstring += indent(template.template, 2 * _TAB)
-
-    return type(class_name, (LLMEvaluator,), {"__init__": __init__, "__doc__": docstring})
-
-
-(
-    HallucinationEvaluator,
-    RelevanceEvaluator,
-    ToxicityEvaluator,
-    QAEvaluator,
-    SummarizationEvaluator,
-) = map(
-    lambda args: _create_llm_evaluator_subclass(*args),
-    (
-        (
-            "HallucinationEvaluator",
-            EvalCriteria.HALLUCINATION.value,
-            'Leverages an LLM to evaluate whether a response (stored under an "output" column) is a hallucination given a query (stored under an "input" column) and one or more retrieved documents (stored under a "reference" column).',  # noqa: E501
-        ),
-        (
-            "RelevanceEvaluator",
-            EvalCriteria.RELEVANCE.value,
-            'Leverages an LLM to evaluate whether a retrieved document (stored under a "reference" column) is relevant or irrelevant to the corresponding query (stored under the "input" column).',  # noqa: E501
-        ),
-        (
-            "ToxicityEvaluator",
-            EvalCriteria.TOXICITY.value,
-            'Leverages an LLM to evaluate whether the string stored under the "input" column contains racist, sexist, chauvinistic, biased, or otherwise toxic content.',  # noqa: E501
-        ),
-        (
-            "QAEvaluator",
-            EvalCriteria.QA.value,
-            'Leverages an LLM to evaluate whether a response (stored under an "output" column) is correct or incorrect given a query (stored under an "input" column) and one or more retrieved documents (stored under a "reference" column).',  # noqa: E501
-        ),
-        (
-            "SummarizationEvaluator",
-            EvalCriteria.SUMMARIZATION.value,
-            'Leverages an LLM to evaluate whether a summary (stored under an "output" column) provides an accurate synopsis of an input document (stored under a "input" column).',  # noqa: E501
-        ),
-    ),
-)
+class HallucinationEvaluator(LLMEvaluator):
+    """
+    Leverages an LLM to evaluate whether a response (stored under an "output"
+    column) is a hallucination given a query (stored under an "input" column)
+    and one or more retrieved documents (stored under a "reference" column).
+    """
+
+    def __init__(self, model: BaseModel) -> None:
+        """
+        Initializer for HallucinationEvaluator.
+
+        Args:
+            model (BaseEvalModel): The LLM model to use for evaluation.
+        """
+
+        super().__init__(model=model, template=EvalCriteria.HALLUCINATION.value)
+
+
+class RelevanceEvaluator(LLMEvaluator):
+    """
+    Leverages an LLM to evaluate whether a retrieved document (stored under a
+    "reference" column) is relevant or irrelevant to the corresponding query
+    (stored under the "input" column).
+    """
+
+    def __init__(self, model: BaseModel) -> None:
+        """
+        Initializer for RelevanceEvaluator.
+
+        Args:
+            model (BaseEvalModel): The LLM model to use for evaluation.
+        """
+
+        super().__init__(model=model, template=EvalCriteria.RELEVANCE.value)
+
+
+class QAEvaluator(LLMEvaluator):
+    """
+    Leverages an LLM to evaluate whether a response (stored under an "output"
+    column) is correct or incorrect given a query (stored under an "input"
+    column) and one or more retrieved documents (stored under a "reference"
+    column).
+    """
+
+    def __init__(self, model: BaseModel) -> None:
+        """
+        Initializer for QAEvaluator.
+
+        Args:
+            model (BaseEvalModel): The LLM model to use for evaluation.
+        """
+
+        super().__init__(model=model, template=EvalCriteria.QA.value)
+
+
+class ToxicityEvaluator(LLMEvaluator):
+    """
+    Leverages an LLM to evaluate whether the string stored under the "input"
+    column contains racist, sexist, chauvinistic, biased, or otherwise toxic
+    content.
+    """
+
+    def __init__(self, model: BaseModel) -> None:
+        """
+        Initializer for ToxicityEvaluator.
+
+        Args:
+            model (BaseEvalModel): The LLM model to use for evaluation.
+        """
+
+        super().__init__(model=model, template=EvalCriteria.TOXICITY.value)
+
+
+class SummarizationEvaluator(LLMEvaluator):
+    """
+    Leverages an LLM to evaluate whether a summary (stored under an
+    "output" column) provides an accurate synopsis of an input document
+    (stored under a "input" column).
+    """
+
+    def __init__(self, model: BaseModel) -> None:
+        """
+        Initializer for SummarizationEvaluator.
+
+        Args:
+            model (BaseEvalModel): The LLM model to use for evaluation.
+        """
+
+        super().__init__(model=model, template=EvalCriteria.SUMMARIZATION.value)
 
 
 class MapReducer:
     """
     Evaluates data that is too large to fit into a single context window using a
     map-reduce strategy. The data must first be divided into "chunks" that
     individually fit into an LLM's context window. Each chunk of data is
```

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/executors.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/executors.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/generate.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/generate.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/retrievals.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/retrievals.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/templates.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/utils.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/anthropic.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/base.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/base.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/bedrock.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/litellm.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/litellm.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/mistralai.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/mistralai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/openai.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/openai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/rate_limiters.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/rate_limiters.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/vertex.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/vertex.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/vertexai.py` & `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/vertexai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/LICENSE` & `arize_phoenix_evals-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/README.md` & `arize_phoenix_evals-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.1/pyproject.toml` & `arize_phoenix_evals-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-version = "0.8.1"
+version = "0.8.2"
 dependencies = [
   "pandas",
   "tqdm",
   "typing-extensions>=4.5, <5",
 ]
 
 [project.optional-dependencies]
```

### Comparing `arize_phoenix_evals-0.8.1/PKG-INFO` & `arize_phoenix_evals-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arize-phoenix-evals
-Version: 0.8.1
+Version: 0.8.2
 Summary: LLM Evaluations
 Project-URL: Documentation, https://docs.arize.com/phoenix/
 Project-URL: Issues, https://github.com/Arize-ai/phoenix/issues
 Project-URL: Source, https://github.com/Arize-ai/phoenix
 Author-email: Arize AI <phoenix-devs@arize.com>
 License: Elastic-2.0
 License-File: IP_NOTICE
```

