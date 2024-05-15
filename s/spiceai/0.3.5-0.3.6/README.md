# Comparing `tmp/spiceai-0.3.5.tar.gz` & `tmp/spiceai-0.3.6.tar.gz`

## Comparing `spiceai-0.3.5.tar` & `spiceai-0.3.6.tar`

### file list

```diff
@@ -1,23 +1,20 @@
--rw-r--r--   0        0        0    28879 2020-02-02 00:00:00.000000 spiceai-0.3.5/tags
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.5/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.3.5/.ropeproject/globalnames
--rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.3.5/.ropeproject/history
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.5/scripts/mytoml.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.5/scripts/prompt.txt
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.5/scripts/run.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/errors.py
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/models.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/providers.py
--rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/spice.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/spice_message.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/utils.py
--rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/wrapped_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.5/tests/conftest.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 spiceai-0.3.5/tests/test_spice.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.5/LICENSE
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.5/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.6/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.6/scripts/mytoml.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.6/scripts/prompt.txt
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.6/scripts/run.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/errors.py
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/models.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/providers.py
+-rw-r--r--   0        0        0    35102 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/spice_message.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/utils.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.6/spice/wrapped_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.6/tests/conftest.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 spiceai-0.3.6/tests/test_spice.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.6/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.6/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.6/PKG-INFO
```

### Comparing `spiceai-0.3.5/.github/workflows/ruff.yml` & `spiceai-0.3.6/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/scripts/run.py` & `spiceai-0.3.6/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/spice/errors.py` & `spiceai-0.3.6/spice/errors.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/spice/models.py` & `spiceai-0.3.6/spice/models.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/spice/providers.py` & `spiceai-0.3.6/spice/providers.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/spice/spice.py` & `spiceai-0.3.6/spice/spice.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from jinja2 import DictLoader, Environment
 from openai.types.chat.completion_create_params import ResponseFormat
 
 from spice.errors import InvalidModelError, UnknownModelError
 from spice.models import EmbeddingModel, Model, TextModel, TranscriptionModel, get_model_from_name
 from spice.providers import Provider, get_provider_from_name
 from spice.spice_message import MessagesEncoder, SpiceMessage
-from spice.utils import embeddings_request_cost, print_stream, text_request_cost, transcription_request_cost
+from spice.utils import embeddings_request_cost, text_request_cost, transcription_request_cost
 from spice.wrapped_clients import WrappedClient
 
 
 @dataclass
 class SpiceCallArgs:
     model: str
     messages: Collection[SpiceMessage]
@@ -56,17 +56,14 @@
 
     completed: bool
     """Whether or not this response was fully completed. This will only ever be false for incomplete streamed responses."""
 
     cost: Optional[float]
     """The cost of this request in cents. May be inaccurate for incompleted streamed responses. Will be None if the cost of the model used is not known."""
 
-    retries: int = 0
-    """The number of retries that were made to get this response. Will be 0 if no retries were made."""
-
     @property
     def total_tokens(self) -> int:
         """The total tokens, input and output, in this response."""
         return self.input_tokens + self.output_tokens
 
     @property
     def characters_per_second(self) -> float:
@@ -396,17 +393,17 @@
 
             validator: If given, will be called with the text of the response. If it returns False, the response will be discarded and another attempt will be made.
 
             streaming_callback: If given, will be called with the text of the response as it is received.
 
             retries: The number of times to retry getting a valid response. If 0, will not retry. If after all retries no valid response is received, will raise a ValueError.
         """
-        start_time = timer()
         cost = 0
         for i in range(retries + 1):
+            start_time = timer()
             text_model = self._get_text_model(model)
             client = self._get_client(text_model, provider)
             call_args = self._fix_call_args(
                 messages, text_model, streaming_callback is not None, temperature, max_tokens, response_format
             )
 
             with client.catch_and_convert_errors():
@@ -428,22 +425,25 @@
                     text, input_tokens, output_tokens = client.extract_text_and_tokens(chat_completion)
 
             completion_cost = text_request_cost(text_model, input_tokens, output_tokens)
             if completion_cost is not None:
                 cost += completion_cost
                 self._total_cost += completion_cost
 
-            if validator is not None and not validator(text):
-                continue
             end_time = timer()
-            response = SpiceResponse(
-                call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost, retries=i
-            )
-            self._log_response(response, name)
-            return response
+            response = SpiceResponse(call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost)
+            if validator is not None and not validator(text):
+                if name:
+                    retry_name = f"{name}-retry-{i}-fail"
+                else:
+                    retry_name = f"retry-{i}-fail"
+                self._log_response(response, retry_name)
+            else:
+                self._log_response(response, name)
+                return response
         raise ValueError("Failed to get a valid response after all retries")
 
     async def stream_response(
         self,
         messages: Collection[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
```

### Comparing `spiceai-0.3.5/spice/spice_message.py` & `spiceai-0.3.6/spice/spice_message.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/spice/utils.py` & `spiceai-0.3.6/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/spice/wrapped_clients.py` & `spiceai-0.3.6/spice/wrapped_clients.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/tests/conftest.py` & `spiceai-0.3.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/tests/test_spice.py` & `spiceai-0.3.6/tests/test_spice.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,9 +27,8 @@
         cache += text
 
     response = await spice.get_response(
         messages=[], model=HAIKU, validator=validator, streaming_callback=accumulator, retries=2
     )
 
     assert response.text == "test"
-    assert response.retries == 1
     assert cache == "Hello, world!test"
```

### Comparing `spiceai-0.3.5/LICENSE` & `spiceai-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/README.md` & `spiceai-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.5/pyproject.toml` & `spiceai-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch]
 
 [tool.hatch.build.targets.wheel]
 packages=["spice"]
 
 [project]
 name = "spiceai"
-version = "0.3.5"
+version = "0.3.6"
 license = {text = "Apache-2.0"}
 description = "A Python library for building AI-powered applications."
 readme = "README.md"
 dependencies = [
     "python-dotenv",
     "openai",
     "anthropic",
```

### Comparing `spiceai-0.3.5/PKG-INFO` & `spiceai-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: httpx
 Requires-Dist: jinja2
 Requires-Dist: openai
```

