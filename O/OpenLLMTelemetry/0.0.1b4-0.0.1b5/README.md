# Comparing `tmp/openllmtelemetry-0.0.1b4.tar.gz` & `tmp/openllmtelemetry-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openllmtelemetry-0.0.1b4.tar", max compression
+gzip compressed data, was "openllmtelemetry-0.0.1b5.tar", max compression
```

## Comparing `openllmtelemetry-0.0.1b4.tar` & `openllmtelemetry-0.0.1b5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/LICENSE
--rw-r--r--   0        0        0     4317 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/README.md
--rw-r--r--   0        0        0       75 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/__init__.py
--rw-r--r--   0        0        0     8339 2024-04-25 19:18:19.665151 openllmtelemetry-0.0.1b4/openllmtelemetry/config.py
--rw-r--r--   0        0        0     1933 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrument.py
--rw-r--r--   0        0        0    11339 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/LICENSE
--rw-r--r--   0        0        0        0 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/__init__.py
--rw-r--r--   0        0        0    11395 2024-04-25 19:18:19.665151 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0     1673 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
--rw-r--r--   0        0        0     1044 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     4007 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/__init__.py
--rw-r--r--   0        0        0     7703 2024-04-25 19:18:19.665151 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
--rw-r--r--   0        0        0     4740 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
--rw-r--r--   0        0        0     2838 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
--rw-r--r--   0        0        0      560 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/utils.py
--rw-r--r--   0        0        0     1726 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/v0/__init__.py
--rw-r--r--   0        0        0     2233 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/v1/__init__.py
--rw-r--r--   0        0        0       28 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     1403 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/intrument_openai.py
--rw-r--r--   0        0        0     3150 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/secure.py
--rw-r--r--   0        0        0     1786 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
--rw-r--r--   0        0        0      809 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/span_exporter.py
--rw-r--r--   0        0        0      477 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/version.py
--rw-r--r--   0        0        0     1653 2024-04-25 19:18:19.665151 openllmtelemetry-0.0.1b4/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/LICENSE
+-rw-r--r--   0        0        0     4317 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/README.md
+-rw-r--r--   0        0        0       99 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/__init__.py
+-rw-r--r--   0        0        0     8376 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/config.py
+-rw-r--r--   0        0        0     2629 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrument.py
+-rw-r--r--   0        0        0    11339 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/__init__.py
+-rw-r--r--   0        0        0    12023 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0     2344 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
+-rw-r--r--   0        0        0     1715 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     4678 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0        0        0     8374 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0        0        0     5411 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0        0        0     3509 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0        0        0     1231 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/utils.py
+-rw-r--r--   0        0        0     2397 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/v0/__init__.py
+-rw-r--r--   0        0        0     2904 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     1403 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b5/openllmtelemetry/intrument_openai.py
+-rw-r--r--   0        0        0     3150 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b5/openllmtelemetry/secure.py
+-rw-r--r--   0        0        0     2457 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
+-rw-r--r--   0        0        0      809 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b5/openllmtelemetry/span_exporter.py
+-rw-r--r--   0        0        0      477 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/openllmtelemetry/version.py
+-rw-r--r--   0        0        0     1653 2024-05-15 14:56:39.985842 openllmtelemetry-0.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b5/PKG-INFO
```

### Comparing `openllmtelemetry-0.0.1b4/LICENSE` & `openllmtelemetry-0.0.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b4/README.md` & `openllmtelemetry-0.0.1b5/README.md`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/config.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         )
 
     @property
     def whylabs_traces_endpoint(self) -> str:
         assert self.whylabs_endpoint is not None, "WhyLabs endpoint is not set."
         return f"{self.whylabs_endpoint.rstrip('/')}/v1/traces"
 
-    def guardrail_client(self, default_dataset_id: str) -> Optional[GuardrailsApi]:
+    def guardrail_client(self, default_dataset_id: Optional[str]) -> Optional[GuardrailsApi]:
         if self.guardrails_endpoint and self.guardrails_api_key:
             return GuardrailsApi(
                 guardrails_endpoint=self.guardrails_endpoint,
                 guardrails_api_key=self.guardrails_api_key,
                 dataset_id=default_dataset_id,
             )
         LOGGER.warning("GuardRails endpoint is not set.")
@@ -105,15 +105,17 @@
                 CFG_API_KEY: self.guardrails_api_key,
             }
         with open(config_path, "w") as configfile:
             config.write(configfile)
 
     def __repr__(self):
         # hide the api_key from output
-        field_strs = [f"{field.name}='***key***'" if 'key' in field.name else f"{field.name}={getattr(self, field.name)}" for field in fields(self)]
+        field_strs = [
+            f"{field.name}='***key***'" if 'key' in field.name else f"{field.name}={getattr(self, field.name)}" for field in fields(self)
+        ]
         return f"{self.__class__.__name__}({', '.join(field_strs)})"
 
     @classmethod
     def read(cls, config_path: str) -> "GuardrailConfig":
         config = configparser.ConfigParser()
         ok_files = config.read(config_path)
         if len(ok_files) == 0:
@@ -123,15 +125,15 @@
         whylabs_api_key = config.get(CFG_WHYLABS_SECTION, CFG_API_KEY)
         guardrails_endpoint = config.get(CFG_GUARDRAILS_SECTION, CFG_ENDPOINT_KEY, fallback=None)
         guardrails_api_key = config.get(CFG_GUARDRAILS_SECTION, CFG_API_KEY, fallback=None)
 
         return GuardrailConfig(whylabs_endpoint, whylabs_api_key, guardrails_endpoint, guardrails_api_key)
 
 
-def load_config() -> Optional[GuardrailConfig]:
+def load_config() -> GuardrailConfig:
     config_path = os.environ.get("WHYLABS_GUARDRAILS_CONFIG")
     if config_path is None:
         config_path = _DEFAULT_CONFIG_FILE
     config = GuardrailConfig(None, None, None, None)
     try:
         config = GuardrailConfig.read(config_path)
     except:  # noqa
@@ -140,15 +142,15 @@
         config = _load_config_from_env(config)
     if config.is_partial and _in_ipython_session:
         config = _interactive_config(config)
 
     return config
 
 
-def load_dataset_id(dataset_id: str) -> Optional[str]:
+def load_dataset_id(dataset_id: Optional[str]) -> Optional[str]:
     effective_dataset_id = os.environ.get("WHYLABS_DEFAULT_DATASET_ID", dataset_id)
     if effective_dataset_id is None:
         if _in_ipython_session:
             effective_dataset_id = input("Set the default dataset ID: ").strip()
             if len(effective_dataset_id) > 0:
                 print("Using dataset ID: ", effective_dataset_id)
             else:
@@ -196,13 +198,13 @@
 
     save_config = input("Do you want to save these settings to a configuration file? [y/n]: ").strip().lower()
     if save_config == "y" or save_config == "yes":
         try:
             os.makedirs(_CONFIG_DIR, exist_ok=True)
             guardrail_config.write(_DEFAULT_CONFIG_FILE)
         except Exception as e:  # noqa
-            LOGGER.exception("Failed to write the configuration file.")
+            LOGGER.exception(f"Failed to write the configuration file: {e}")
 
             print("Failed to write the configuration file.")
 
     print(f"Set config: {guardrail_config}")
     return guardrail_config
```

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/instrument.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/instrument.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 import os
 from logging import getLogger
-from typing import Optional
+from typing import Dict, Optional, Tuple
 
 from opentelemetry import trace
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.trace import Tracer
 
 from openllmtelemetry.config import load_config, load_dataset_id
 from openllmtelemetry.intrument_openai import init_instrumentors
 from openllmtelemetry.version import __version__
 
 LOGGER = getLogger(__name__)
 
+_tracer_cache: Dict[str, trace.Tracer] = {}
+_last_added_tracer: Optional[Tuple[str, trace.Tracer]] = None
+
 
 def instrument(
     application_name: Optional[str] = None,
     dataset_id: Optional[str] = None,
     tracer_name: Optional[str] = None,
     service_name: Optional[str] = None,
     disable_batching: bool = False,
 ) -> Tracer:
+    global _tracer_cache, _last_added_tracer
+
     config = load_config()
     dataset_id = load_dataset_id(dataset_id)
+    if dataset_id is None:
+        raise ValueError(
+            "dataset_id must be specified in a parameter or in env var: e.g. "
+            "os.environ[\"WHYLABS_DEFAULT_DATASET_ID\"] = \"model-1\""
+        )
     guardrails_api = config.guardrail_client(default_dataset_id=dataset_id)
 
     if application_name is None:
         otel_service_name = os.environ.get("OTEL_SERVICE_NAME")
         if otel_service_name:
             application_name = otel_service_name
         else:
@@ -45,10 +55,21 @@
     )
 
     tracer_provider = TracerProvider(resource=resource)
     config.config_tracer_provider(tracer_provider, dataset_id=dataset_id, disable_batching=disable_batching)
 
     tracer = trace.get_tracer(tracer_name)
     trace.set_tracer_provider(tracer_provider)
+    _tracer_cache[tracer_name] = tracer
+    _last_added_tracer = (tracer_name, tracer)
 
     init_instrumentors(tracer, guardrails_api)
     return tracer
+
+
+def get_tracer(name: Optional[str] = None) -> Optional[Tracer]:
+    if _last_added_tracer is None:
+        return None
+    elif name is None:
+        return _last_added_tracer[1]
+    else:
+        return _tracer_cache.get(name)
```

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/LICENSE` & `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/bedrock/__init__.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/bedrock/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,27 @@
-"""OpenTelemetry Bedrock instrumentation"""
+
+"""
+Copyright 2024 traceloop
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+Changes made: customization for WhyLabs
+
+Original source: openllmetry: https://github.com/traceloop/openllmetry
+"""
 import json
 import logging
 import os
 from functools import wraps
 from typing import Collection, Optional
 
 from opentelemetry import context as context_api
```

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright 2024 traceloop
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+Changes made: customization for WhyLabs
+
+Original source: openllmetry: https://github.com/traceloop/openllmetry
+"""
 from botocore.exceptions import (
     ReadTimeoutError,
     ResponseStreamingError,
 )
 from botocore.response import StreamingBody
 from urllib3.exceptions import ProtocolError as URLLib3ProtocolError
 from urllib3.exceptions import ReadTimeoutError as URLLib3ReadTimeoutError
```

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/__init__.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright 2024 traceloop
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+Changes made: customization for WhyLabs
+
+Original source: openllmetry: https://github.com/traceloop/openllmetry
+"""
 import json
 import logging
 import os
 import types
 from importlib.metadata import version
 
 import openai
```

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright 2024 traceloop
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+Changes made: customization for WhyLabs
+
+Original source: openllmetry: https://github.com/traceloop/openllmetry
+"""
 import json
 import logging
 
 from opentelemetry import context as context_api
 
 # noinspection PyProtectedMember
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
```

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright 2024 traceloop
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+Changes made: customization for WhyLabs
+
+Original source: openllmetry: https://github.com/traceloop/openllmetry
+"""
 import logging
 from typing import Optional
 
 from opentelemetry import context as context_api
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
```

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright 2024 traceloop
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+Changes made: customization for WhyLabs
+
+Original source: openllmetry: https://github.com/traceloop/openllmetry
+"""
 import logging
 
 from opentelemetry import context as context_api
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.trace import SpanKind
 
 from openllmtelemetry.instrumentation.openai.shared import (
```

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/intrument_openai.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/intrument_openai.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/secure.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/secure.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b4/openllmtelemetry/span_exporter.py` & `openllmtelemetry-0.0.1b5/openllmtelemetry/span_exporter.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b4/pyproject.toml` & `openllmtelemetry-0.0.1b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenLLMTelemetry"
-version = "0.0.1.b4"
+version = "0.0.1.b5"
 description = "End-to-end observability with built-in security guardrails."
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `openllmtelemetry-0.0.1b4/PKG-INFO` & `openllmtelemetry-0.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenLLMTelemetry
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: End-to-end observability with built-in security guardrails.
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

