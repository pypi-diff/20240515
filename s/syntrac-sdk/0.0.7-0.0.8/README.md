# Comparing `tmp/syntrac_sdk-0.0.7.tar.gz` & `tmp/syntrac_sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_sdk-0.0.7.tar", max compression
+gzip compressed data, was "syntrac_sdk-0.0.8.tar", max compression
```

## Comparing `syntrac_sdk-0.0.7.tar` & `syntrac_sdk-0.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      395 2024-05-12 08:53:28.807631 syntrac_sdk-0.0.7/README.md
--rw-r--r--   0        0        0     2072 2024-05-12 08:53:28.826929 syntrac_sdk-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-05-12 08:53:28.809045 syntrac_sdk-0.0.7/syntrac/sdk/.DS_Store
--rw-r--r--   0        0        0     6417 2024-05-12 08:53:28.809158 syntrac_sdk-0.0.7/syntrac/sdk/__init__.py
--rw-r--r--   0        0        0      358 2024-05-12 08:53:28.811132 syntrac_sdk-0.0.7/syntrac/sdk/config/__init__.py
--rw-r--r--   0        0        0     1117 2024-05-12 08:53:28.811456 syntrac_sdk-0.0.7/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2024-05-12 08:53:28.811804 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__init__.py
--rw-r--r--   0        0        0      491 2024-05-12 08:53:28.812218 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3126 2024-05-12 08:53:28.812507 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc
--rw-r--r--   0        0        0    10195 2024-05-12 08:53:28.812742 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     9276 2024-05-12 08:53:28.812912 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1571 2024-05-12 08:53:28.813245 syntrac_sdk-0.0.7/syntrac/sdk/decorators/helper.py
--rw-r--r--   0        0        0     7917 2024-05-12 08:53:28.813556 syntrac_sdk-0.0.7/syntrac/sdk/decorators/task.py
--rw-r--r--   0        0        0     7099 2024-05-12 08:53:28.813851 syntrac_sdk-0.0.7/syntrac/sdk/decorators/workflow.py
--rw-r--r--   0        0        0     2650 2024-05-12 08:53:28.814088 syntrac_sdk-0.0.7/syntrac/sdk/fetcher.py
--rw-r--r--   0        0        0      465 2024-05-12 08:53:28.814201 syntrac_sdk-0.0.7/syntrac/sdk/instruments.py
--rw-r--r--   0        0        0        0 2024-05-12 08:53:28.814430 syntrac_sdk-0.0.7/syntrac/sdk/metrics/__init__.py
--rw-r--r--   0        0        0      202 2024-05-12 08:53:28.814791 syntrac_sdk-0.0.7/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3362 2024-05-12 08:53:28.815016 syntrac_sdk-0.0.7/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
--rw-r--r--   0        0        0     2109 2024-05-12 08:53:28.815255 syntrac_sdk-0.0.7/syntrac/sdk/metrics/metrics.py
--rw-r--r--   0        0        0     2721 2024-05-12 08:53:28.815524 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__init__.py
--rw-r--r--   0        0        0     2638 2024-05-12 08:53:28.815836 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      225 2024-05-12 08:53:28.816064 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     7151 2024-05-12 08:53:28.816261 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/trace_exporter/__init__.py
--rw-r--r--   0        0        0     9686 2024-05-12 08:53:28.816578 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      607 2024-05-12 08:53:28.816734 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/version.py
--rw-r--r--   0        0        0     2424 2024-05-12 08:53:28.816862 syntrac_sdk-0.0.7/syntrac/sdk/telemetry.py
--rw-r--r--   0        0        0     6148 2024-05-12 08:53:28.817160 syntrac_sdk-0.0.7/syntrac/sdk/tracing/.DS_Store
--rw-r--r--   0        0        0      302 2024-05-12 08:53:28.817385 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__init__.py
--rw-r--r--   0        0        0      650 2024-05-12 08:53:28.817703 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1969 2024-05-12 08:53:28.818120 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
--rw-r--r--   0        0        0     4806 2024-05-12 08:53:28.818307 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc
--rw-r--r--   0        0        0      877 2024-05-12 08:53:28.818516 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
--rw-r--r--   0        0        0      818 2024-05-12 08:53:28.818774 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc
--rw-r--r--   0        0        0     2748 2024-05-12 08:53:28.818912 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc
--rw-r--r--   0        0        0    27029 2024-05-12 08:53:28.819384 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
--rw-r--r--   0        0        0      846 2024-05-12 08:53:28.819525 syntrac_sdk-0.0.7/syntrac/sdk/tracing/content_allow_list.py
--rw-r--r--   0        0        0     2509 2024-05-12 08:53:28.819650 syntrac_sdk-0.0.7/syntrac/sdk/tracing/context.py
--rw-r--r--   0        0        0      297 2024-05-12 08:53:28.819915 syntrac_sdk-0.0.7/syntrac/sdk/tracing/context_manager.py
--rw-r--r--   0        0        0      322 2024-05-12 08:53:28.820140 syntrac_sdk-0.0.7/syntrac/sdk/tracing/context_passing.py
--rw-r--r--   0        0        0     1880 2024-05-12 08:53:28.820252 syntrac_sdk-0.0.7/syntrac/sdk/tracing/span_from_context.py
--rw-r--r--   0        0        0    22217 2024-05-12 08:53:28.820606 syntrac_sdk-0.0.7/syntrac/sdk/tracing/tracing.py
--rw-r--r--   0        0        0      878 2024-05-12 08:53:28.820842 syntrac_sdk-0.0.7/syntrac/sdk/utils/__init__.py
--rw-r--r--   0        0        0     2171 2024-05-12 08:53:28.821058 syntrac_sdk-0.0.7/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2112 2024-05-12 08:53:28.821348 syntrac_sdk-0.0.7/syntrac/sdk/utils/in_memory_span_exporter.py
--rw-r--r--   0        0        0       22 2024-05-12 08:53:28.821473 syntrac_sdk-0.0.7/syntrac/sdk/version.py
--rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      395 2024-05-14 12:30:48.102957 syntrac_sdk-0.0.8/README.md
+-rw-r--r--   0        0        0     2072 2024-05-14 12:30:48.124836 syntrac_sdk-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-14 12:30:48.105917 syntrac_sdk-0.0.8/syntrac/sdk/.DS_Store
+-rw-r--r--   0        0        0     6417 2024-05-14 12:30:48.106063 syntrac_sdk-0.0.8/syntrac/sdk/__init__.py
+-rw-r--r--   0        0        0      358 2024-05-14 12:30:48.107769 syntrac_sdk-0.0.8/syntrac/sdk/config/__init__.py
+-rw-r--r--   0        0        0     1117 2024-05-14 12:30:48.108356 syntrac_sdk-0.0.8/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2024-05-14 12:30:48.108821 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-14 12:30:48.109245 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3126 2024-05-14 12:30:48.109542 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc
+-rw-r--r--   0        0        0    10195 2024-05-14 12:30:48.109740 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     9276 2024-05-14 12:30:48.110033 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1571 2024-05-14 12:30:48.110356 syntrac_sdk-0.0.8/syntrac/sdk/decorators/helper.py
+-rw-r--r--   0        0        0     7917 2024-05-14 12:30:48.110510 syntrac_sdk-0.0.8/syntrac/sdk/decorators/task.py
+-rw-r--r--   0        0        0     7099 2024-05-14 12:30:48.110724 syntrac_sdk-0.0.8/syntrac/sdk/decorators/workflow.py
+-rw-r--r--   0        0        0     2650 2024-05-14 12:30:48.110901 syntrac_sdk-0.0.8/syntrac/sdk/fetcher.py
+-rw-r--r--   0        0        0      465 2024-05-14 12:30:48.111145 syntrac_sdk-0.0.8/syntrac/sdk/instruments.py
+-rw-r--r--   0        0        0        0 2024-05-14 12:30:48.111345 syntrac_sdk-0.0.8/syntrac/sdk/metrics/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-14 12:30:48.111991 syntrac_sdk-0.0.8/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3362 2024-05-14 12:30:48.112212 syntrac_sdk-0.0.8/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0        0        0     2109 2024-05-14 12:30:48.112451 syntrac_sdk-0.0.8/syntrac/sdk/metrics/metrics.py
+-rw-r--r--   0        0        0     2721 2024-05-14 12:30:48.112861 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__init__.py
+-rw-r--r--   0        0        0     2638 2024-05-14 12:30:48.113182 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      225 2024-05-14 12:30:48.113319 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     7791 2024-05-14 12:30:48.113644 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/trace_exporter/__init__.py
+-rw-r--r--   0        0        0    10408 2024-05-14 12:30:48.113862 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      607 2024-05-14 12:30:48.114183 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/version.py
+-rw-r--r--   0        0        0     2424 2024-05-14 12:30:48.114441 syntrac_sdk-0.0.8/syntrac/sdk/telemetry.py
+-rw-r--r--   0        0        0     6148 2024-05-14 12:30:48.114817 syntrac_sdk-0.0.8/syntrac/sdk/tracing/.DS_Store
+-rw-r--r--   0        0        0      302 2024-05-14 12:30:48.114945 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__init__.py
+-rw-r--r--   0        0        0      650 2024-05-14 12:30:48.115162 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1969 2024-05-14 12:30:48.115395 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
+-rw-r--r--   0        0        0     4806 2024-05-14 12:30:48.115527 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc
+-rw-r--r--   0        0        0      877 2024-05-14 12:30:48.115774 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
+-rw-r--r--   0        0        0      818 2024-05-14 12:30:48.116022 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc
+-rw-r--r--   0        0        0     2748 2024-05-14 12:30:48.116171 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0    27176 2024-05-14 12:30:48.116356 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
+-rw-r--r--   0        0        0      846 2024-05-14 12:30:48.116607 syntrac_sdk-0.0.8/syntrac/sdk/tracing/content_allow_list.py
+-rw-r--r--   0        0        0     2509 2024-05-14 12:30:48.116737 syntrac_sdk-0.0.8/syntrac/sdk/tracing/context.py
+-rw-r--r--   0        0        0      297 2024-05-14 12:30:48.116963 syntrac_sdk-0.0.8/syntrac/sdk/tracing/context_manager.py
+-rw-r--r--   0        0        0      322 2024-05-14 12:30:48.117283 syntrac_sdk-0.0.8/syntrac/sdk/tracing/context_passing.py
+-rw-r--r--   0        0        0     1880 2024-05-14 12:30:48.117414 syntrac_sdk-0.0.8/syntrac/sdk/tracing/span_from_context.py
+-rw-r--r--   0        0        0    22336 2024-05-14 12:30:48.117769 syntrac_sdk-0.0.8/syntrac/sdk/tracing/tracing.py
+-rw-r--r--   0        0        0      878 2024-05-14 12:30:48.118042 syntrac_sdk-0.0.8/syntrac/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2024-05-14 12:30:48.118253 syntrac_sdk-0.0.8/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2112 2024-05-14 12:30:48.118486 syntrac_sdk-0.0.8/syntrac/sdk/utils/in_memory_span_exporter.py
+-rw-r--r--   0        0        0       22 2024-05-14 12:30:48.118610 syntrac_sdk-0.0.8/syntrac/sdk/version.py
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.8/PKG-INFO
```

### Comparing `syntrac_sdk-0.0.7/pyproject.toml` & `syntrac_sdk-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "syntrac-sdk"
-version = "0.0.7"
+version = "0.0.8"
 description = "Syntrac Software Development Kit (SDK) for Python"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/syntracAI/syntrac"
 documentation = "https://syntrac.com/docs/openllmetry"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/.DS_Store` & `syntrac_sdk-0.0.8/syntrac/sdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/__init__.py` & `syntrac_sdk-0.0.8/syntrac/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9c1a3f66 (Sat May 11 07:13:32 2024 UTC)
+moddate:  0x72174366 (Tue May 14 07:49:06 2024 UTC)
 files sz: 1571
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 14
    flags     : 0
    code
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8c1a3f66 (Sat May 11 07:13:16 2024 UTC)
+moddate:  0x72174366 (Tue May 14 07:49:06 2024 UTC)
 files sz: 7917
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x191a3f66 (Sat May 11 07:11:21 2024 UTC)
+moddate:  0x72174366 (Tue May 14 07:49:06 2024 UTC)
 files sz: 7099
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/decorators/helper.py` & `syntrac_sdk-0.0.8/syntrac/sdk/decorators/helper.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/decorators/task.py` & `syntrac_sdk-0.0.8/syntrac/sdk/decorators/task.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/decorators/workflow.py` & `syntrac_sdk-0.0.8/syntrac/sdk/decorators/workflow.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/fetcher.py` & `syntrac_sdk-0.0.8/syntrac/sdk/fetcher.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/metrics/metrics.py` & `syntrac_sdk-0.0.8/syntrac/sdk/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__init__.py` & `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/trace_exporter/__init__.py` & `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/trace_exporter/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from opentelemetry.sdk.trace import ReadableSpan
 from syntrac.sdk.otlp.json import (
     _OTLP_HTTP_HEADERS,
     DEFAULT_ENDPOINT,
     Compression,
 )
 from opentelemetry.util.re import parse_env_headers
+from syntrac.sdk import Telemetry
 
 _logger = logging.getLogger(__name__)
 
 DEFAULT_COMPRESSION = Compression.NoCompression
 DEFAULT_TRACES_EXPORT_PATH = "v1/traces"
 DEFAULT_TIMEOUT = 10  # in seconds
 REQUESTS_SUCCESS_STATUS_CODES = (200, 202)
@@ -91,16 +92,30 @@
         self._session.headers.update(self._headers)
         self._session.headers.update(_OTLP_HTTP_HEADERS)
         if self._compression is not Compression.NoCompression:
             self._session.headers.update(
                 {"Content-Encoding": self._compression.value}
             )
         self._shutdown = False
+        Telemetry().capture(
+            "span_exporter:init",
+            {
+                "endpoint": self._endpoint,
+                "certificate_file": self._certificate_file,
+                "timeout": self._timeout,
+            },
+        )
 
     def export(self, spans: Sequence[ReadableSpan]) -> SpanExportResult:
+        Telemetry().capture(
+            "span_exporter:export",
+            {
+                "shutdown": self._shutdown,
+            },
+        )
         # After the call to Shutdown subsequent calls to Export are
         # not allowed and should return a Failure result
         if self._shutdown:
             logger.warning("Exporter already shutdown, ignoring batch")
             return SpanExportResult.FAILURE
 
         serialized_data = self._serialize_spans(spans)
@@ -114,14 +129,19 @@
             "Failed to export batch code: %s, reason: %s",
             resp.status_code,
             resp.text,
         )
         return SpanExportResult.FAILURE
 
     def shutdown(self) -> None:
+        Telemetry().capture(
+            "span_exporter:shutdown",
+            {
+            },
+        )
         if self._shutdown:
             logger.warning("Exporter already shutdown, ignoring call")
             return
         self._session.close()
         self._shutdown = True
 
     def force_flush(self, timeout_millis: int = 30000) -> bool:
@@ -133,15 +153,19 @@
         if self._compression == Compression.Gzip:
             gzip_data = BytesIO()
             with gzip.GzipFile(fileobj=gzip_data, mode="w") as gzip_stream:
                 gzip_stream.write(serialized_data)
             data = gzip_data.getvalue()
         elif self._compression == Compression.Deflate:
             data = zlib.compress(bytes(serialized_data))
-
+        Telemetry().capture(
+            "span_exporter:_export",
+            {
+            },
+        )
         return self._session.post(
             url=self._endpoint,
             data=data,
             verify=self._certificate_file,
             timeout=self._timeout,
         )
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,29 +1,29 @@
 magic:    0xa70d0d0a
-moddate:  0xae090966 (Sun Mar 31 06:58:54 2024 UTC)
-files sz: 7151
+moddate:  0x82584366 (Tue May 14 12:26:42 2024 UTC)
+files sz: 7791
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       026c036d045a040100640064036c056d065a060100640064046c076d085a
       080100640064056c096d0a5a0a6d0b5a0b6d0c5a0c0100640064016c0d5a
       0d640064016c0e5a0e640064066c0f6d105a106d115a116d125a126d135a
       136d145a146d155a156d165a166d175a176d185a186d195a190100640064
       076c1a6d1b5a1b0100640064086c1c6d1d5a1d6d1e5a1e0100640064096c
       1f6d205a2001006400640a6c216d225a226d235a236d245a240100640064
-      0b6c256d265a260100020065016a2700000000000000006528a6010000ab
-      0100000000000000005a2965246a2a00000000000000005a2b640c5a2c64
-      0d5a2d640e5a2e020065016a2700000000000000006528a6010000ab0100
-      000000000000005a2f02004700640f84006410651da6030000ab03000000
-      00000000005a30641165246602641284045a316413653264116532660464
-      1484045a3364015300
+      0b6c256d265a2601006400640c6c276d285a280100020065016a29000000
+      0000000000652aa6010000ab0100000000000000005a2b65246a2c000000
+      00000000005a2d640d5a2e640e5a2f640f5a30020065016a290000000000
+      000000652aa6010000ab0100000000000000005a31020047006410840064
+      11651da6030000ab0300000000000000005a32641265246602641384045a
+      3364146534641265346604641584045a3564015300
      0           0 RESUME                   0
    
     15           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (gzip)
                  8 STORE_NAME               0 (gzip)
    
@@ -141,83 +141,91 @@
     46         206 LOAD_CONST               0 (0)
                208 LOAD_CONST              11 (('parse_env_headers',))
                210 IMPORT_NAME             37 (opentelemetry.util.re)
                212 IMPORT_FROM             38 (parse_env_headers)
                214 STORE_NAME              38 (parse_env_headers)
                216 POP_TOP
    
-    48         218 PUSH_NULL
-               220 LOAD_NAME                1 (logging)
-               222 LOAD_ATTR               39 (getLogger)
-               232 LOAD_NAME               40 (__name__)
-               234 PRECALL                  1
-               238 CALL                     1
-               248 STORE_NAME              41 (_logger)
-   
-    50         250 LOAD_NAME               36 (Compression)
-               252 LOAD_ATTR               42 (NoCompression)
-               262 STORE_NAME              43 (DEFAULT_COMPRESSION)
-   
-    51         264 LOAD_CONST              12 ('v1/traces')
-               266 STORE_NAME              44 (DEFAULT_TRACES_EXPORT_PATH)
-   
-    52         268 LOAD_CONST              13 (10)
-               270 STORE_NAME              45 (DEFAULT_TIMEOUT)
-   
-    53         272 LOAD_CONST              14 ((200, 202))
-               274 STORE_NAME              46 (REQUESTS_SUCCESS_STATUS_CODES)
-   
-    55         276 PUSH_NULL
-               278 LOAD_NAME                1 (logging)
-               280 LOAD_ATTR               39 (getLogger)
-               290 LOAD_NAME               40 (__name__)
-               292 PRECALL                  1
-               296 CALL                     1
-               306 STORE_NAME              47 (logger)
-   
-    58         308 PUSH_NULL
-               310 LOAD_BUILD_CLASS
-               312 LOAD_CONST              15 (<code object OTLPSpanExporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 58>)
-               314 MAKE_FUNCTION            0
-               316 LOAD_CONST              16 ('OTLPSpanExporter')
-               318 LOAD_NAME               29 (SpanExporter)
-               320 PRECALL                  3
-               324 CALL                     3
-               334 STORE_NAME              48 (OTLPSpanExporter)
-   
-   189         336 LOAD_CONST              17 ('return')
-               338 LOAD_NAME               36 (Compression)
-               340 BUILD_TUPLE              2
-               342 LOAD_CONST              18 (<code object _compression_from_env, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 189>)
-               344 MAKE_FUNCTION            4 (annotations)
-               346 STORE_NAME              49 (_compression_from_env)
-   
-   201         348 LOAD_CONST              19 ('endpoint')
-               350 LOAD_NAME               50 (str)
-               352 LOAD_CONST              17 ('return')
-               354 LOAD_NAME               50 (str)
-               356 BUILD_TUPLE              4
-               358 LOAD_CONST              20 (<code object _append_trace_path, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 201>)
-               360 MAKE_FUNCTION            4 (annotations)
-               362 STORE_NAME              51 (_append_trace_path)
-               364 LOAD_CONST               1 (None)
-               366 RETURN_VALUE
+    47         218 LOAD_CONST               0 (0)
+               220 LOAD_CONST              12 (('Telemetry',))
+               222 IMPORT_NAME             39 (syntrac.sdk)
+               224 IMPORT_FROM             40 (Telemetry)
+               226 STORE_NAME              40 (Telemetry)
+               228 POP_TOP
+   
+    49         230 PUSH_NULL
+               232 LOAD_NAME                1 (logging)
+               234 LOAD_ATTR               41 (getLogger)
+               244 LOAD_NAME               42 (__name__)
+               246 PRECALL                  1
+               250 CALL                     1
+               260 STORE_NAME              43 (_logger)
+   
+    51         262 LOAD_NAME               36 (Compression)
+               264 LOAD_ATTR               44 (NoCompression)
+               274 STORE_NAME              45 (DEFAULT_COMPRESSION)
+   
+    52         276 LOAD_CONST              13 ('v1/traces')
+               278 STORE_NAME              46 (DEFAULT_TRACES_EXPORT_PATH)
+   
+    53         280 LOAD_CONST              14 (10)
+               282 STORE_NAME              47 (DEFAULT_TIMEOUT)
+   
+    54         284 LOAD_CONST              15 ((200, 202))
+               286 STORE_NAME              48 (REQUESTS_SUCCESS_STATUS_CODES)
+   
+    56         288 PUSH_NULL
+               290 LOAD_NAME                1 (logging)
+               292 LOAD_ATTR               41 (getLogger)
+               302 LOAD_NAME               42 (__name__)
+               304 PRECALL                  1
+               308 CALL                     1
+               318 STORE_NAME              49 (logger)
+   
+    59         320 PUSH_NULL
+               322 LOAD_BUILD_CLASS
+               324 LOAD_CONST              16 (<code object OTLPSpanExporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 59>)
+               326 MAKE_FUNCTION            0
+               328 LOAD_CONST              17 ('OTLPSpanExporter')
+               330 LOAD_NAME               29 (SpanExporter)
+               332 PRECALL                  3
+               336 CALL                     3
+               346 STORE_NAME              50 (OTLPSpanExporter)
+   
+   213         348 LOAD_CONST              18 ('return')
+               350 LOAD_NAME               36 (Compression)
+               352 BUILD_TUPLE              2
+               354 LOAD_CONST              19 (<code object _compression_from_env, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 213>)
+               356 MAKE_FUNCTION            4 (annotations)
+               358 STORE_NAME              51 (_compression_from_env)
+   
+   225         360 LOAD_CONST              20 ('endpoint')
+               362 LOAD_NAME               52 (str)
+               364 LOAD_CONST              18 ('return')
+               366 LOAD_NAME               52 (str)
+               368 BUILD_TUPLE              4
+               370 LOAD_CONST              21 (<code object _append_trace_path, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 225>)
+               372 MAKE_FUNCTION            4 (annotations)
+               374 STORE_NAME              53 (_append_trace_path)
+               376 LOAD_CONST               1 (None)
+               378 RETURN_VALUE
    consts
       0
       None
       ('BytesIO',)
       ('defaultdict',)
       ('environ',)
       ('Dict', 'Optional', 'Sequence')
       ('OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE', 'OTEL_EXPORTER_OTLP_TRACES_COMPRESSION', 'OTEL_EXPORTER_OTLP_TRACES_ENDPOINT', 'OTEL_EXPORTER_OTLP_TRACES_HEADERS', 'OTEL_EXPORTER_OTLP_TRACES_TIMEOUT', 'OTEL_EXPORTER_OTLP_CERTIFICATE', 'OTEL_EXPORTER_OTLP_COMPRESSION', 'OTEL_EXPORTER_OTLP_ENDPOINT', 'OTEL_EXPORTER_OTLP_HEADERS', 'OTEL_EXPORTER_OTLP_TIMEOUT')
       ('SERVICE_NAME',)
       ('SpanExporter', 'SpanExportResult')
       ('ReadableSpan',)
       ('_OTLP_HTTP_HEADERS', 'DEFAULT_ENDPOINT', 'Compression')
       ('parse_env_headers',)
+      ('Telemetry',)
       'v1/traces'
       10
       (200, 202)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 14
@@ -228,120 +236,120 @@
             036505650465046602190000000000000000001900000000000000000064
             056503650619000000000000000000640665036507190000000000000000
             006407650365086a09000000000000000019000000000000000000660c64
             0884055a0a6409650b650c19000000000000000000640a650d6604640b84
             045a0e6415640c84045a0f6416640e6506640a65106604640f84055a1164
             1065046602641184045a126412650b650c19000000000000000000640a65
             046604641384045a1364015300
-          58           0 RESUME                   0
+          59           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('OTLPSpanExporter')
                        8 STORE_NAME               2 (__qualname__)
          
-          61          10 NOP
+          62          10 NOP
          
-          62          12 NOP
+          63          12 NOP
          
-          63          14 NOP
+          64          14 NOP
          
-          64          16 NOP
+          65          16 NOP
          
-          65          18 NOP
+          66          18 NOP
          
-          66          20 NOP
+          67          20 NOP
          
-          59          22 LOAD_CONST              20 ((None, None, None, None, None, None))
+          60          22 LOAD_CONST              20 ((None, None, None, None, None, None))
                       24 LOAD_CONST               2 ('endpoint')
          
-          61          26 LOAD_NAME                3 (Optional)
+          62          26 LOAD_NAME                3 (Optional)
                       28 LOAD_NAME                4 (str)
                       30 BINARY_SUBSCR
          
-          59          40 LOAD_CONST               3 ('certificate_file')
+          60          40 LOAD_CONST               3 ('certificate_file')
          
-          62          42 LOAD_NAME                3 (Optional)
+          63          42 LOAD_NAME                3 (Optional)
                       44 LOAD_NAME                4 (str)
                       46 BINARY_SUBSCR
          
-          59          56 LOAD_CONST               4 ('headers')
+          60          56 LOAD_CONST               4 ('headers')
          
-          63          58 LOAD_NAME                3 (Optional)
+          64          58 LOAD_NAME                3 (Optional)
                       60 LOAD_NAME                5 (Dict)
                       62 LOAD_NAME                4 (str)
                       64 LOAD_NAME                4 (str)
                       66 BUILD_TUPLE              2
                       68 BINARY_SUBSCR
                       78 BINARY_SUBSCR
          
-          59          88 LOAD_CONST               5 ('timeout')
+          60          88 LOAD_CONST               5 ('timeout')
          
-          64          90 LOAD_NAME                3 (Optional)
+          65          90 LOAD_NAME                3 (Optional)
                       92 LOAD_NAME                6 (int)
                       94 BINARY_SUBSCR
          
-          59         104 LOAD_CONST               6 ('compression')
+          60         104 LOAD_CONST               6 ('compression')
          
-          65         106 LOAD_NAME                3 (Optional)
+          66         106 LOAD_NAME                3 (Optional)
                      108 LOAD_NAME                7 (Compression)
                      110 BINARY_SUBSCR
          
-          59         120 LOAD_CONST               7 ('session')
+          60         120 LOAD_CONST               7 ('session')
          
-          66         122 LOAD_NAME                3 (Optional)
+          67         122 LOAD_NAME                3 (Optional)
                      124 LOAD_NAME                8 (requests)
                      126 LOAD_ATTR                9 (Session)
                      136 BINARY_SUBSCR
          
-          59         146 BUILD_TUPLE             12
-                     148 LOAD_CONST               8 (<code object __init__, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 59>)
+          60         146 BUILD_TUPLE             12
+                     148 LOAD_CONST               8 (<code object __init__, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 60>)
                      150 MAKE_FUNCTION            5 (defaults, annotations)
                      152 STORE_NAME              10 (__init__)
          
-          99         154 LOAD_CONST               9 ('spans')
+         108         154 LOAD_CONST               9 ('spans')
                      156 LOAD_NAME               11 (Sequence)
                      158 LOAD_NAME               12 (ReadableSpan)
                      160 BINARY_SUBSCR
                      170 LOAD_CONST              10 ('return')
                      172 LOAD_NAME               13 (SpanExportResult)
                      174 BUILD_TUPLE              4
-                     176 LOAD_CONST              11 (<code object export, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 99>)
+                     176 LOAD_CONST              11 (<code object export, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 108>)
                      178 MAKE_FUNCTION            4 (annotations)
                      180 STORE_NAME              14 (export)
          
-         120         182 LOAD_CONST              21 (('return', None))
-                     184 LOAD_CONST              12 (<code object shutdown, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 120>)
+         135         182 LOAD_CONST              21 (('return', None))
+                     184 LOAD_CONST              12 (<code object shutdown, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 135>)
                      186 MAKE_FUNCTION            4 (annotations)
                      188 STORE_NAME              15 (shutdown)
          
-         127         190 LOAD_CONST              22 ((30000,))
+         147         190 LOAD_CONST              22 ((30000,))
                      192 LOAD_CONST              14 ('timeout_millis')
                      194 LOAD_NAME                6 (int)
                      196 LOAD_CONST              10 ('return')
                      198 LOAD_NAME               16 (bool)
                      200 BUILD_TUPLE              4
-                     202 LOAD_CONST              15 (<code object force_flush, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 127>)
+                     202 LOAD_CONST              15 (<code object force_flush, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 147>)
                      204 MAKE_FUNCTION            5 (defaults, annotations)
                      206 STORE_NAME              17 (force_flush)
          
-         131         208 LOAD_CONST              16 ('serialized_data')
+         151         208 LOAD_CONST              16 ('serialized_data')
                      210 LOAD_NAME                4 (str)
                      212 BUILD_TUPLE              2
-                     214 LOAD_CONST              17 (<code object _export, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 131>)
+                     214 LOAD_CONST              17 (<code object _export, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 151>)
                      216 MAKE_FUNCTION            4 (annotations)
                      218 STORE_NAME              18 (_export)
          
-         148         220 LOAD_CONST              18 ('sdk_spans')
+         172         220 LOAD_CONST              18 ('sdk_spans')
                      222 LOAD_NAME               11 (Sequence)
                      224 LOAD_NAME               12 (ReadableSpan)
                      226 BINARY_SUBSCR
                      236 LOAD_CONST              10 ('return')
                      238 LOAD_NAME                4 (str)
                      240 BUILD_TUPLE              4
-                     242 LOAD_CONST              19 (<code object _serialize_spans, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 148>)
+                     242 LOAD_CONST              19 (<code object _serialize_spans, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 172>)
                      244 MAKE_FUNCTION            4 (annotations)
                      246 STORE_NAME              19 (_serialize_spans)
                      248 LOAD_CONST               1 (None)
                      250 RETURN_VALUE
          consts
             'OTLPSpanExporter'
             None
@@ -384,350 +392,418 @@
                   000000000001007c006a1700000000000000006a180000000000000000a0
                   190000000000000000000000000000000000000000743400000000000000
                   000000a6010000ab01000000000000000001007c006a1400000000000000
                   007436000000000000000000006a1c00000000000000007501722b7c006a
                   1700000000000000006a180000000000000000a019000000000000000000
                   000000000000000000000064037c006a1400000000000000006a1d000000
                   00000000006901a6010000ab010000000000000000010064047c005f1e00
-                  0000000000000064005300
-                59           0 RESUME                   0
+                  00000000000000743f00000000000000000000a6000000ab000000000000
+                  000000a020000000000000000000000000000000000000000064057c006a
+                  0600000000000000007c006a0900000000000000007c006a120000000000
+                  00000064069c03a6020000ab020000000000000000010064005300
+                60           0 RESUME                   0
                
-                68           2 LOAD_FAST                1 (endpoint)
+                69           2 LOAD_FAST                1 (endpoint)
                              4 JUMP_IF_TRUE_OR_POP     67 (to 140)
                              6 LOAD_GLOBAL              1 (NULL + environ)
                             18 LOAD_ATTR                1 (get)
                
-                69          28 LOAD_GLOBAL              4 (OTEL_EXPORTER_OTLP_TRACES_ENDPOINT)
+                70          28 LOAD_GLOBAL              4 (OTEL_EXPORTER_OTLP_TRACES_ENDPOINT)
                
-                70          40 LOAD_GLOBAL              7 (NULL + _append_trace_path)
+                71          40 LOAD_GLOBAL              7 (NULL + _append_trace_path)
                
-                71          52 LOAD_GLOBAL              1 (NULL + environ)
+                72          52 LOAD_GLOBAL              1 (NULL + environ)
                             64 LOAD_ATTR                1 (get)
                             74 LOAD_GLOBAL              8 (OTEL_EXPORTER_OTLP_ENDPOINT)
                             86 LOAD_GLOBAL             10 (DEFAULT_ENDPOINT)
                             98 PRECALL                  2
                            102 CALL                     2
                
-                70         112 PRECALL                  1
+                71         112 PRECALL                  1
                            116 CALL                     1
                
-                68         126 PRECALL                  2
+                69         126 PRECALL                  2
                            130 CALL                     2
                        >>  140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               6 (_endpoint)
                
-                74         152 LOAD_FAST                2 (certificate_file)
+                75         152 LOAD_FAST                2 (certificate_file)
                            154 JUMP_IF_TRUE_OR_POP     49 (to 254)
                            156 LOAD_GLOBAL              1 (NULL + environ)
                            168 LOAD_ATTR                1 (get)
                
-                75         178 LOAD_GLOBAL             14 (OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE)
+                76         178 LOAD_GLOBAL             14 (OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE)
                
-                76         190 LOAD_GLOBAL              1 (NULL + environ)
+                77         190 LOAD_GLOBAL              1 (NULL + environ)
                            202 LOAD_ATTR                1 (get)
                            212 LOAD_GLOBAL             16 (OTEL_EXPORTER_OTLP_CERTIFICATE)
                            224 LOAD_CONST               1 (True)
                            226 PRECALL                  2
                            230 CALL                     2
                
-                74         240 PRECALL                  2
+                75         240 PRECALL                  2
                            244 CALL                     2
                        >>  254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (_certificate_file)
                
-                78         266 LOAD_GLOBAL              1 (NULL + environ)
+                79         266 LOAD_GLOBAL              1 (NULL + environ)
                            278 LOAD_ATTR                1 (get)
                
-                79         288 LOAD_GLOBAL             20 (OTEL_EXPORTER_OTLP_TRACES_HEADERS)
+                80         288 LOAD_GLOBAL             20 (OTEL_EXPORTER_OTLP_TRACES_HEADERS)
                
-                80         300 LOAD_GLOBAL              1 (NULL + environ)
+                81         300 LOAD_GLOBAL              1 (NULL + environ)
                            312 LOAD_ATTR                1 (get)
                            322 LOAD_GLOBAL             22 (OTEL_EXPORTER_OTLP_HEADERS)
                            334 LOAD_CONST               2 ('')
                            336 PRECALL                  2
                            340 CALL                     2
                
-                78         350 PRECALL                  2
+                79         350 PRECALL                  2
                            354 CALL                     2
                            364 STORE_FAST               7 (headers_string)
                
-                82         366 LOAD_FAST                3 (headers)
+                83         366 LOAD_FAST                3 (headers)
                            368 JUMP_IF_TRUE_OR_POP     14 (to 398)
                            370 LOAD_GLOBAL             25 (NULL + parse_env_headers)
                            382 LOAD_FAST                7 (headers_string)
                            384 PRECALL                  1
                            388 CALL                     1
                        >>  398 LOAD_FAST                0 (self)
                            400 STORE_ATTR              13 (_headers)
                
-                83         410 LOAD_FAST                4 (timeout)
+                84         410 LOAD_FAST                4 (timeout)
                            412 JUMP_IF_TRUE_OR_POP     67 (to 548)
                            414 LOAD_GLOBAL             29 (NULL + int)
                
-                84         426 LOAD_GLOBAL              1 (NULL + environ)
+                85         426 LOAD_GLOBAL              1 (NULL + environ)
                            438 LOAD_ATTR                1 (get)
                
-                85         448 LOAD_GLOBAL             30 (OTEL_EXPORTER_OTLP_TRACES_TIMEOUT)
+                86         448 LOAD_GLOBAL             30 (OTEL_EXPORTER_OTLP_TRACES_TIMEOUT)
                
-                86         460 LOAD_GLOBAL              1 (NULL + environ)
+                87         460 LOAD_GLOBAL              1 (NULL + environ)
                            472 LOAD_ATTR                1 (get)
                            482 LOAD_GLOBAL             32 (OTEL_EXPORTER_OTLP_TIMEOUT)
                            494 LOAD_GLOBAL             34 (DEFAULT_TIMEOUT)
                            506 PRECALL                  2
                            510 CALL                     2
                
-                84         520 PRECALL                  2
+                85         520 PRECALL                  2
                            524 CALL                     2
                
-                83         534 PRECALL                  1
+                84         534 PRECALL                  1
                            538 CALL                     1
                        >>  548 LOAD_FAST                0 (self)
                            550 STORE_ATTR              18 (_timeout)
                
-                89         560 LOAD_FAST                5 (compression)
+                90         560 LOAD_FAST                5 (compression)
                            562 JUMP_IF_TRUE_OR_POP     13 (to 590)
                            564 LOAD_GLOBAL             39 (NULL + _compression_from_env)
                            576 PRECALL                  0
                            580 CALL                     0
                        >>  590 LOAD_FAST                0 (self)
                            592 STORE_ATTR              20 (_compression)
                
-                90         602 LOAD_FAST                6 (session)
+                91         602 LOAD_FAST                6 (session)
                            604 JUMP_IF_TRUE_OR_POP     18 (to 642)
                            606 LOAD_GLOBAL             43 (NULL + requests)
                            618 LOAD_ATTR               22 (Session)
                            628 PRECALL                  0
                            632 CALL                     0
                        >>  642 LOAD_FAST                0 (self)
                            644 STORE_ATTR              23 (_session)
                
-                91         654 LOAD_FAST                0 (self)
+                92         654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR               23 (_session)
                            666 LOAD_ATTR               24 (headers)
                            676 LOAD_METHOD             25 (update)
                            698 LOAD_FAST                0 (self)
                            700 LOAD_ATTR               13 (_headers)
                            710 PRECALL                  1
                            714 CALL                     1
                            724 POP_TOP
                
-                92         726 LOAD_FAST                0 (self)
+                93         726 LOAD_FAST                0 (self)
                            728 LOAD_ATTR               23 (_session)
                            738 LOAD_ATTR               24 (headers)
                            748 LOAD_METHOD             25 (update)
                            770 LOAD_GLOBAL             52 (_OTLP_HTTP_HEADERS)
                            782 PRECALL                  1
                            786 CALL                     1
                            796 POP_TOP
                
-                93         798 LOAD_FAST                0 (self)
+                94         798 LOAD_FAST                0 (self)
                            800 LOAD_ATTR               20 (_compression)
                            810 LOAD_GLOBAL             54 (Compression)
                            822 LOAD_ATTR               28 (NoCompression)
                            832 IS_OP                    1
                            834 POP_JUMP_FORWARD_IF_FALSE    43 (to 922)
                
-                94         836 LOAD_FAST                0 (self)
+                95         836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR               23 (_session)
                            848 LOAD_ATTR               24 (headers)
                            858 LOAD_METHOD             25 (update)
                
-                95         880 LOAD_CONST               3 ('Content-Encoding')
+                96         880 LOAD_CONST               3 ('Content-Encoding')
                            882 LOAD_FAST                0 (self)
                            884 LOAD_ATTR               20 (_compression)
                            894 LOAD_ATTR               29 (value)
                            904 BUILD_MAP                1
                
-                94         906 PRECALL                  1
+                95         906 PRECALL                  1
                            910 CALL                     1
                            920 POP_TOP
                
-                97     >>  922 LOAD_CONST               4 (False)
+                98     >>  922 LOAD_CONST               4 (False)
                            924 LOAD_FAST                0 (self)
                            926 STORE_ATTR              30 (_shutdown)
-                           936 LOAD_CONST               0 (None)
-                           938 RETURN_VALUE
+               
+                99         936 LOAD_GLOBAL             63 (NULL + Telemetry)
+                           948 PRECALL                  0
+                           952 CALL                     0
+                           962 LOAD_METHOD             32 (capture)
+               
+               100         984 LOAD_CONST               5 ('span_exporter:init')
+               
+               102         986 LOAD_FAST                0 (self)
+                           988 LOAD_ATTR                6 (_endpoint)
+               
+               103         998 LOAD_FAST                0 (self)
+                          1000 LOAD_ATTR                9 (_certificate_file)
+               
+               104        1010 LOAD_FAST                0 (self)
+                          1012 LOAD_ATTR               18 (_timeout)
+               
+               101        1022 LOAD_CONST               6 (('endpoint', 'certificate_file', 'timeout'))
+                          1024 BUILD_CONST_KEY_MAP      3
+               
+                99        1026 PRECALL                  2
+                          1030 CALL                     2
+                          1040 POP_TOP
+                          1042 LOAD_CONST               0 (None)
+                          1044 RETURN_VALUE
                consts
                   None
                   True
                   ''
                   'Content-Encoding'
                   False
-               names      ('environ', 'get', 'OTEL_EXPORTER_OTLP_TRACES_ENDPOINT', '_append_trace_path', 'OTEL_EXPORTER_OTLP_ENDPOINT', 'DEFAULT_ENDPOINT', '_endpoint', 'OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE', 'OTEL_EXPORTER_OTLP_CERTIFICATE', '_certificate_file', 'OTEL_EXPORTER_OTLP_TRACES_HEADERS', 'OTEL_EXPORTER_OTLP_HEADERS', 'parse_env_headers', '_headers', 'int', 'OTEL_EXPORTER_OTLP_TRACES_TIMEOUT', 'OTEL_EXPORTER_OTLP_TIMEOUT', 'DEFAULT_TIMEOUT', '_timeout', '_compression_from_env', '_compression', 'requests', 'Session', '_session', 'headers', 'update', '_OTLP_HTTP_HEADERS', 'Compression', 'NoCompression', 'value', '_shutdown')
+                  'span_exporter:init'
+                  ('endpoint', 'certificate_file', 'timeout')
+               names      ('environ', 'get', 'OTEL_EXPORTER_OTLP_TRACES_ENDPOINT', '_append_trace_path', 'OTEL_EXPORTER_OTLP_ENDPOINT', 'DEFAULT_ENDPOINT', '_endpoint', 'OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE', 'OTEL_EXPORTER_OTLP_CERTIFICATE', '_certificate_file', 'OTEL_EXPORTER_OTLP_TRACES_HEADERS', 'OTEL_EXPORTER_OTLP_HEADERS', 'parse_env_headers', '_headers', 'int', 'OTEL_EXPORTER_OTLP_TRACES_TIMEOUT', 'OTEL_EXPORTER_OTLP_TIMEOUT', 'DEFAULT_TIMEOUT', '_timeout', '_compression_from_env', '_compression', 'requests', 'Session', '_session', 'headers', 'update', '_OTLP_HTTP_HEADERS', 'Compression', 'NoCompression', 'value', '_shutdown', 'Telemetry', 'capture')
                varnames   ('self', 'endpoint', 'certificate_file', 'headers', 'timeout', 'compression', 'session', 'headers_string')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       '__init__'
-               firstlineno 59
+               firstlineno 60
                lnotab
                   0x02091a010c010c013cff0efe1a061a010c0132fe1a0416010c0132fe10
                   042c01100116010c013cfe0eff1a062a0134014801480126012c011aff10
-                  03
+                  030e01300102020c010c010cfd04fe
             'spans'
             'return'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
-                  0x97007c006a0000000000000000007226740200000000000000000000a0
-                  0200000000000000000000000000000000000000006401a6010000ab0100
-                  0000000000000001007406000000000000000000006a0400000000000000
-                  0053007c00a00500000000000000000000000000000000000000007c01a6
-                  010000ab0100000000000000007d027c00a0060000000000000000000000
-                  0000000000000000007c02a6010000ab0100000000000000007d037c036a
-                  070000000000000000720c7406000000000000000000006a080000000000
-                  0000005300741200000000000000000000a00a0000000000000000000000
-                  00000000000000000064027c036a0b00000000000000007c036a0c000000
-                  0000000000a6030000ab0300000000000000000100740600000000000000
-                  0000006a0400000000000000005300
-                99           0 RESUME                   0
-               
-               102           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (_shutdown)
-                            14 POP_JUMP_FORWARD_IF_FALSE    38 (to 92)
-               
-               103          16 LOAD_GLOBAL              2 (logger)
-                            28 LOAD_METHOD              2 (warning)
-                            50 LOAD_CONST               1 ('Exporter already shutdown, ignoring batch')
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-               
-               104          68 LOAD_GLOBAL              6 (SpanExportResult)
-                            80 LOAD_ATTR                4 (FAILURE)
-                            90 RETURN_VALUE
-               
-               106     >>   92 LOAD_FAST                0 (self)
-                            94 LOAD_METHOD              5 (_serialize_spans)
-                           116 LOAD_FAST                1 (spans)
-                           118 PRECALL                  1
-                           122 CALL                     1
-                           132 STORE_FAST               2 (serialized_data)
-               
-               107         134 LOAD_FAST                0 (self)
-                           136 LOAD_METHOD              6 (_export)
-                           158 LOAD_FAST                2 (serialized_data)
-                           160 PRECALL                  1
-                           164 CALL                     1
-                           174 STORE_FAST               3 (resp)
-               
-               110         176 LOAD_FAST                3 (resp)
-                           178 LOAD_ATTR                7 (ok)
-                           188 POP_JUMP_FORWARD_IF_FALSE    12 (to 214)
-               
-               111         190 LOAD_GLOBAL              6 (SpanExportResult)
-                           202 LOAD_ATTR                8 (SUCCESS)
-                           212 RETURN_VALUE
-               
-               113     >>  214 LOAD_GLOBAL             18 (_logger)
-                           226 LOAD_METHOD             10 (error)
-               
-               114         248 LOAD_CONST               2 ('Failed to export batch code: %s, reason: %s')
-               
-               115         250 LOAD_FAST                3 (resp)
-                           252 LOAD_ATTR               11 (status_code)
-               
-               116         262 LOAD_FAST                3 (resp)
-                           264 LOAD_ATTR               12 (text)
-               
-               113         274 PRECALL                  3
-                           278 CALL                     3
-                           288 POP_TOP
-               
-               118         290 LOAD_GLOBAL              6 (SpanExportResult)
-                           302 LOAD_ATTR                4 (FAILURE)
-                           312 RETURN_VALUE
+                  0x9700740100000000000000000000a6000000ab000000000000000000a0
+                  010000000000000000000000000000000000000000640164027c006a0200
+                  000000000000006901a6020000ab02000000000000000001007c006a0200
+                  000000000000007226740600000000000000000000a00400000000000000
+                  000000000000000000000000006403a6010000ab01000000000000000001
+                  00740a000000000000000000006a06000000000000000053007c00a00700
+                  000000000000000000000000000000000000007c01a6010000ab01000000
+                  00000000007d027c00a00800000000000000000000000000000000000000
+                  007c02a6010000ab0100000000000000007d037c036a0900000000000000
+                  00720c740a000000000000000000006a0a00000000000000005300741600
+                  000000000000000000a00c00000000000000000000000000000000000000
+                  0064047c036a0d00000000000000007c036a0e0000000000000000a60300
+                  00ab0300000000000000000100740a000000000000000000006a06000000
+                  00000000005300
+               108           0 RESUME                   0
+               
+               109           2 LOAD_GLOBAL              1 (NULL + Telemetry)
+                            14 PRECALL                  0
+                            18 CALL                     0
+                            28 LOAD_METHOD              1 (capture)
+               
+               110          50 LOAD_CONST               1 ('span_exporter:export')
+               
+               112          52 LOAD_CONST               2 ('shutdown')
+                            54 LOAD_FAST                0 (self)
+                            56 LOAD_ATTR                2 (_shutdown)
+               
+               111          66 BUILD_MAP                1
+               
+               109          68 PRECALL                  2
+                            72 CALL                     2
+                            82 POP_TOP
+               
+               117          84 LOAD_FAST                0 (self)
+                            86 LOAD_ATTR                2 (_shutdown)
+                            96 POP_JUMP_FORWARD_IF_FALSE    38 (to 174)
+               
+               118          98 LOAD_GLOBAL              6 (logger)
+                           110 LOAD_METHOD              4 (warning)
+                           132 LOAD_CONST               3 ('Exporter already shutdown, ignoring batch')
+                           134 PRECALL                  1
+                           138 CALL                     1
+                           148 POP_TOP
+               
+               119         150 LOAD_GLOBAL             10 (SpanExportResult)
+                           162 LOAD_ATTR                6 (FAILURE)
+                           172 RETURN_VALUE
+               
+               121     >>  174 LOAD_FAST                0 (self)
+                           176 LOAD_METHOD              7 (_serialize_spans)
+                           198 LOAD_FAST                1 (spans)
+                           200 PRECALL                  1
+                           204 CALL                     1
+                           214 STORE_FAST               2 (serialized_data)
+               
+               122         216 LOAD_FAST                0 (self)
+                           218 LOAD_METHOD              8 (_export)
+                           240 LOAD_FAST                2 (serialized_data)
+                           242 PRECALL                  1
+                           246 CALL                     1
+                           256 STORE_FAST               3 (resp)
+               
+               125         258 LOAD_FAST                3 (resp)
+                           260 LOAD_ATTR                9 (ok)
+                           270 POP_JUMP_FORWARD_IF_FALSE    12 (to 296)
+               
+               126         272 LOAD_GLOBAL             10 (SpanExportResult)
+                           284 LOAD_ATTR               10 (SUCCESS)
+                           294 RETURN_VALUE
+               
+               128     >>  296 LOAD_GLOBAL             22 (_logger)
+                           308 LOAD_METHOD             12 (error)
+               
+               129         330 LOAD_CONST               4 ('Failed to export batch code: %s, reason: %s')
+               
+               130         332 LOAD_FAST                3 (resp)
+                           334 LOAD_ATTR               13 (status_code)
+               
+               131         344 LOAD_FAST                3 (resp)
+                           346 LOAD_ATTR               14 (text)
+               
+               128         356 PRECALL                  3
+                           360 CALL                     3
+                           370 POP_TOP
+               
+               133         372 LOAD_GLOBAL             10 (SpanExportResult)
+                           384 LOAD_ATTR                6 (FAILURE)
+                           394 RETURN_VALUE
                consts
                   None
+                  'span_exporter:export'
+                  'shutdown'
                   'Exporter already shutdown, ignoring batch'
                   'Failed to export batch code: %s, reason: %s'
-               names      ('_shutdown', 'logger', 'warning', 'SpanExportResult', 'FAILURE', '_serialize_spans', '_export', 'ok', 'SUCCESS', '_logger', 'error', 'status_code', 'text')
+               names      ('Telemetry', 'capture', '_shutdown', 'logger', 'warning', 'SpanExportResult', 'FAILURE', '_serialize_spans', '_export', 'ok', 'SUCCESS', '_logger', 'error', 'status_code', 'text')
                varnames   ('self', 'spans', 'serialized_data', 'resp')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       'export'
-               firstlineno 99
-               lnotab 0x02030e01340118022a012a030e011802220102010c010cfd1005
+               firstlineno 108
+               lnotab
+                  0x0201300102020eff02fe10080e01340118022a012a030e011802220102
+                  010c010cfd1005
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 3
+               stacksize : 4
                flags     : 3
                code
-                  0x97007c006a000000000000000000721c740200000000000000000000a0
-                  0200000000000000000000000000000000000000006401a6010000ab0100
-                  000000000000000100640053007c006a030000000000000000a004000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  00010064027c005f00000000000000000064005300
-               120           0 RESUME                   0
+                  0x9700740100000000000000000000a6000000ab000000000000000000a0
+                  01000000000000000000000000000000000000000064016900a6020000ab
+                  02000000000000000001007c006a020000000000000000721c7406000000
+                  00000000000000a004000000000000000000000000000000000000000064
+                  02a6010000ab0100000000000000000100640053007c006a050000000000
+                  000000a0060000000000000000000000000000000000000000a6000000ab
+                  000000000000000000010064037c005f02000000000000000064005300
+               135           0 RESUME                   0
+               
+               136           2 LOAD_GLOBAL              1 (NULL + Telemetry)
+                            14 PRECALL                  0
+                            18 CALL                     0
+                            28 LOAD_METHOD              1 (capture)
+               
+               137          50 LOAD_CONST               1 ('span_exporter:shutdown')
+               
+               138          52 BUILD_MAP                0
+               
+               136          54 PRECALL                  2
+                            58 CALL                     2
+                            68 POP_TOP
+               
+               141          70 LOAD_FAST                0 (self)
+                            72 LOAD_ATTR                2 (_shutdown)
+                            82 POP_JUMP_FORWARD_IF_FALSE    28 (to 140)
+               
+               142          84 LOAD_GLOBAL              6 (logger)
+                            96 LOAD_METHOD              4 (warning)
+                           118 LOAD_CONST               2 ('Exporter already shutdown, ignoring call')
+                           120 PRECALL                  1
+                           124 CALL                     1
+                           134 POP_TOP
                
-               121           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (_shutdown)
-                            14 POP_JUMP_FORWARD_IF_FALSE    28 (to 72)
-               
-               122          16 LOAD_GLOBAL              2 (logger)
-                            28 LOAD_METHOD              2 (warning)
-                            50 LOAD_CONST               1 ('Exporter already shutdown, ignoring call')
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-               
-               123          68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
-               
-               124     >>   72 LOAD_FAST                0 (self)
-                            74 LOAD_ATTR                3 (_session)
-                            84 LOAD_METHOD              4 (close)
-                           106 PRECALL                  0
-                           110 CALL                     0
-                           120 POP_TOP
-               
-               125         122 LOAD_CONST               2 (True)
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               0 (_shutdown)
-                           136 LOAD_CONST               0 (None)
+               143         136 LOAD_CONST               0 (None)
                            138 RETURN_VALUE
+               
+               144     >>  140 LOAD_FAST                0 (self)
+                           142 LOAD_ATTR                5 (_session)
+                           152 LOAD_METHOD              6 (close)
+                           174 PRECALL                  0
+                           178 CALL                     0
+                           188 POP_TOP
+               
+               145         190 LOAD_CONST               3 (True)
+                           192 LOAD_FAST                0 (self)
+                           194 STORE_ATTR               2 (_shutdown)
+                           204 LOAD_CONST               0 (None)
+                           206 RETURN_VALUE
                consts
                   None
+                  'span_exporter:shutdown'
                   'Exporter already shutdown, ignoring call'
                   True
-               names      ('_shutdown', 'logger', 'warning', '_session', 'close')
+               names      ('Telemetry', 'capture', '_shutdown', 'logger', 'warning', '_session', 'close')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       'shutdown'
-               firstlineno 120
-               lnotab 0x02010e01340104013201
+               firstlineno 135
+               lnotab 0x02013001020102fe10050e01340104013201
             30000
             'timeout_millis'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064015300
-               127           0 RESUME                   0
+               147           0 RESUME                   0
                
-               129           2 LOAD_CONST               1 (True)
+               149           2 LOAD_CONST               1 (True)
                              4 RETURN_VALUE
                consts
                   'Nothing is buffered in this exporter, so this method does nothing.'
                   True
                names      ()
                varnames   ('self', 'timeout_millis')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       'force_flush'
-               firstlineno 127
+               firstlineno 147
                lnotab 0x0202
             'serialized_data'
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 6
                flags     : 3
@@ -740,53 +816,55 @@
                   010000ab0100000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007c03a0070000000000000000000000000000000000000000a6000000ab
                   0000000000000000007d026e367c006a0000000000000000007402000000
                   000000000000006a0800000000000000006b020000000072217413000000
                   000000000000006a0a00000000000000007417000000000000000000007c
                   01a6010000ab010000000000000000a6010000ab0100000000000000007d
-                  027c006a0c0000000000000000a00d000000000000000000000000000000
-                  00000000007c006a0e00000000000000007c027c006a0f00000000000000
-                  007c006a100000000000000000ac03a6040000ab04000000000000000053
-                  00
-               131           0 RESUME                   0
+                  02741900000000000000000000a6000000ab000000000000000000a00d00
+                  0000000000000000000000000000000000000064036900a6020000ab0200
+                  0000000000000001007c006a0e0000000000000000a00f00000000000000
+                  000000000000000000000000007c006a1000000000000000007c027c006a
+                  1100000000000000007c006a120000000000000000ac04a6040000ab0400
+                  000000000000005300
+               151           0 RESUME                   0
                
-               132           2 LOAD_FAST                1 (serialized_data)
+               152           2 LOAD_FAST                1 (serialized_data)
                              4 STORE_FAST               2 (data)
                
-               133           6 LOAD_FAST                0 (self)
+               153           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (_compression)
                             18 LOAD_GLOBAL              2 (Compression)
                             30 LOAD_ATTR                2 (Gzip)
                             40 COMPARE_OP               2 (==)
                             46 POP_JUMP_FORWARD_IF_FALSE   102 (to 252)
                
-               134          48 LOAD_GLOBAL              7 (NULL + BytesIO)
+               154          48 LOAD_GLOBAL              7 (NULL + BytesIO)
                             60 PRECALL                  0
                             64 CALL                     0
                             74 STORE_FAST               3 (gzip_data)
                
-               135          76 LOAD_GLOBAL              9 (NULL + gzip)
+               155          76 LOAD_GLOBAL              9 (NULL + gzip)
                             88 LOAD_ATTR                5 (GzipFile)
                             98 LOAD_FAST                3 (gzip_data)
                            100 LOAD_CONST               1 ('w')
                            102 KW_NAMES                 2
                            104 PRECALL                  2
                            108 CALL                     2
                            118 BEFORE_WITH
                            120 STORE_FAST               4 (gzip_stream)
                
-               136         122 LOAD_FAST                4 (gzip_stream)
+               156         122 LOAD_FAST                4 (gzip_stream)
                            124 LOAD_METHOD              6 (write)
                            146 LOAD_FAST                1 (serialized_data)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                
-               135         164 LOAD_CONST               0 (None)
+               155         164 LOAD_CONST               0 (None)
                            166 LOAD_CONST               0 (None)
                            168 LOAD_CONST               0 (None)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_TOP
                            186 JUMP_FORWARD            11 (to 210)
                        >>  188 PUSH_EXC_INFO
@@ -797,76 +875,90 @@
                            198 POP_EXCEPT
                            200 RERAISE                  1
                        >>  202 POP_TOP
                            204 POP_EXCEPT
                            206 POP_TOP
                            208 POP_TOP
                
-               137     >>  210 LOAD_FAST                3 (gzip_data)
+               157     >>  210 LOAD_FAST                3 (gzip_data)
                            212 LOAD_METHOD              7 (getvalue)
                            234 PRECALL                  0
                            238 CALL                     0
                            248 STORE_FAST               2 (data)
                            250 JUMP_FORWARD            54 (to 360)
                
-               138     >>  252 LOAD_FAST                0 (self)
+               158     >>  252 LOAD_FAST                0 (self)
                            254 LOAD_ATTR                0 (_compression)
                            264 LOAD_GLOBAL              2 (Compression)
                            276 LOAD_ATTR                8 (Deflate)
                            286 COMPARE_OP               2 (==)
                            292 POP_JUMP_FORWARD_IF_FALSE    33 (to 360)
                
-               139         294 LOAD_GLOBAL             19 (NULL + zlib)
+               159         294 LOAD_GLOBAL             19 (NULL + zlib)
                            306 LOAD_ATTR               10 (compress)
                            316 LOAD_GLOBAL             23 (NULL + bytes)
                            328 LOAD_FAST                1 (serialized_data)
                            330 PRECALL                  1
                            334 CALL                     1
                            344 PRECALL                  1
                            348 CALL                     1
                            358 STORE_FAST               2 (data)
                
-               141     >>  360 LOAD_FAST                0 (self)
-                           362 LOAD_ATTR               12 (_session)
-                           372 LOAD_METHOD             13 (post)
+               160     >>  360 LOAD_GLOBAL             25 (NULL + Telemetry)
+                           372 PRECALL                  0
+                           376 CALL                     0
+                           386 LOAD_METHOD             13 (capture)
+               
+               161         408 LOAD_CONST               3 ('span_exporter:_export')
+               
+               162         410 BUILD_MAP                0
+               
+               160         412 PRECALL                  2
+                           416 CALL                     2
+                           426 POP_TOP
+               
+               165         428 LOAD_FAST                0 (self)
+                           430 LOAD_ATTR               14 (_session)
+                           440 LOAD_METHOD             15 (post)
                
-               142         394 LOAD_FAST                0 (self)
-                           396 LOAD_ATTR               14 (_endpoint)
+               166         462 LOAD_FAST                0 (self)
+                           464 LOAD_ATTR               16 (_endpoint)
                
-               143         406 LOAD_FAST                2 (data)
+               167         474 LOAD_FAST                2 (data)
                
-               144         408 LOAD_FAST                0 (self)
-                           410 LOAD_ATTR               15 (_certificate_file)
+               168         476 LOAD_FAST                0 (self)
+                           478 LOAD_ATTR               17 (_certificate_file)
                
-               145         420 LOAD_FAST                0 (self)
-                           422 LOAD_ATTR               16 (_timeout)
+               169         488 LOAD_FAST                0 (self)
+                           490 LOAD_ATTR               18 (_timeout)
                
-               141         432 KW_NAMES                 3
-                           434 PRECALL                  4
-                           438 CALL                     4
-                           448 RETURN_VALUE
+               165         500 KW_NAMES                 4
+                           502 PRECALL                  4
+                           506 CALL                     4
+                           516 RETURN_VALUE
                ExceptionTable:
                  120 to 162 -> 188 [1] lasti
                  188 to 194 -> 196 [3] lasti
                  202 to 202 -> 196 [3] lasti
                consts
                   None
                   'w'
                   ('fileobj', 'mode')
+                  'span_exporter:_export'
                   ('url', 'data', 'verify', 'timeout')
-               names      ('_compression', 'Compression', 'Gzip', 'BytesIO', 'gzip', 'GzipFile', 'write', 'getvalue', 'Deflate', 'zlib', 'compress', 'bytes', '_session', 'post', '_endpoint', '_certificate_file', '_timeout')
+               names      ('_compression', 'Compression', 'Gzip', 'BytesIO', 'gzip', 'GzipFile', 'write', 'getvalue', 'Deflate', 'zlib', 'compress', 'bytes', 'Telemetry', 'capture', '_session', 'post', '_endpoint', '_certificate_file', '_timeout')
                varnames   ('self', 'serialized_data', 'data', 'gzip_data', 'gzip_stream')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       '_export'
-               firstlineno 131
+               firstlineno 151
                lnotab
-                  0x020104012a011c012e012aff2e022a012a01420222010c0102010c010c
-                  fc
+                  0x020104012a011c012e012aff2e022a012a0142013001020102fe100522
+                  010c0102010c010cfc
             'sdk_spans'
             code
                argcount  : 2
                nlocals   : 10
                stacksize : 8
                flags     : 3
                code
@@ -885,130 +977,130 @@
                   0000000000000064039c02a6010000ab01000000000000000001008c4c7c
                   06a0030000000000000000000000000000000000000000740b0000000000
                   00000000006a0600000000000000007c04a0070000000000000000000000
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   000000000000007c0864049c02a6010000ab01000000000000000001008c
                   a464057c0669017d09740b000000000000000000006a0800000000000000
                   007c09a6010000ab0100000000000000005300
-               148           0 RESUME                   0
+               172           0 RESUME                   0
                
-               160           2 LOAD_GLOBAL              1 (NULL + defaultdict)
-                            14 LOAD_CONST               1 (<code object <lambda>, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 160>)
+               184           2 LOAD_GLOBAL              1 (NULL + defaultdict)
+                            14 LOAD_CONST               1 (<code object <lambda>, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 184>)
                             16 MAKE_FUNCTION            0
                             18 PRECALL                  1
                             22 CALL                     1
                             32 STORE_FAST               2 (sdk_resource_spans)
                
-               161          34 LOAD_FAST                1 (sdk_spans)
+               185          34 LOAD_FAST                1 (sdk_spans)
                             36 GET_ITER
                        >>   38 FOR_ITER                49 (to 138)
                             40 STORE_FAST               3 (sdk_span)
                
-               162          42 LOAD_FAST                3 (sdk_span)
+               186          42 LOAD_FAST                3 (sdk_span)
                             44 LOAD_ATTR                1 (resource)
                             54 STORE_FAST               4 (sdk_resource)
                
-               163          56 LOAD_FAST                3 (sdk_span)
+               187          56 LOAD_FAST                3 (sdk_span)
                             58 LOAD_ATTR                2 (instrumentation_scope)
                             68 STORE_FAST               5 (sdk_instrumentation)
                
-               164          70 LOAD_FAST                2 (sdk_resource_spans)
+               188          70 LOAD_FAST                2 (sdk_resource_spans)
                             72 LOAD_FAST                4 (sdk_resource)
                             74 BINARY_SUBSCR
                             84 LOAD_FAST                5 (sdk_instrumentation)
                             86 BINARY_SUBSCR
                             96 LOAD_METHOD              3 (append)
                            118 LOAD_FAST                3 (sdk_span)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 POP_TOP
                            136 JUMP_BACKWARD           50 (to 38)
                
-               166     >>  138 BUILD_LIST               0
+               190     >>  138 BUILD_LIST               0
                            140 STORE_FAST               6 (resource_spans)
                
-               167         142 LOAD_FAST                2 (sdk_resource_spans)
+               191         142 LOAD_FAST                2 (sdk_resource_spans)
                            144 LOAD_METHOD              4 (items)
                            166 PRECALL                  0
                            170 CALL                     0
                            180 GET_ITER
                        >>  182 FOR_ITER               163 (to 510)
                            184 UNPACK_SEQUENCE          2
                            188 STORE_FAST               4 (sdk_resource)
                            190 STORE_FAST               7 (sdk_instrumentations)
                
-               168         192 BUILD_LIST               0
+               192         192 BUILD_LIST               0
                            194 STORE_FAST               8 (scope_spans)
                
-               169         196 LOAD_FAST                7 (sdk_instrumentations)
+               193         196 LOAD_FAST                7 (sdk_instrumentations)
                            198 LOAD_METHOD              4 (items)
                            220 PRECALL                  0
                            224 CALL                     0
                            234 GET_ITER
                        >>  236 FOR_ITER                75 (to 388)
                            238 UNPACK_SEQUENCE          2
                            242 STORE_FAST               5 (sdk_instrumentation)
                            244 STORE_FAST               1 (sdk_spans)
                
-               170         246 LOAD_FAST                8 (scope_spans)
+               194         246 LOAD_FAST                8 (scope_spans)
                            248 LOAD_METHOD              3 (append)
                
-               172         270 LOAD_GLOBAL             11 (NULL + json)
+               196         270 LOAD_GLOBAL             11 (NULL + json)
                            282 LOAD_ATTR                6 (loads)
                            292 LOAD_FAST                5 (sdk_instrumentation)
                            294 LOAD_METHOD              7 (to_json)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 PRECALL                  1
                            334 CALL                     1
                
-               173         344 LOAD_CONST               2 (<code object <listcomp>, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 173>)
+               197         344 LOAD_CONST               2 (<code object <listcomp>, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 197>)
                            346 MAKE_FUNCTION            0
                            348 LOAD_FAST                1 (sdk_spans)
                            350 GET_ITER
                            352 PRECALL                  0
                            356 CALL                     0
                
-               171         366 LOAD_CONST               3 (('scope', 'spans'))
+               195         366 LOAD_CONST               3 (('scope', 'spans'))
                            368 BUILD_CONST_KEY_MAP      2
                
-               170         370 PRECALL                  1
+               194         370 PRECALL                  1
                            374 CALL                     1
                            384 POP_TOP
                            386 JUMP_BACKWARD           76 (to 236)
                
-               176     >>  388 LOAD_FAST                6 (resource_spans)
+               200     >>  388 LOAD_FAST                6 (resource_spans)
                            390 LOAD_METHOD              3 (append)
                
-               178         412 LOAD_GLOBAL             11 (NULL + json)
+               202         412 LOAD_GLOBAL             11 (NULL + json)
                            424 LOAD_ATTR                6 (loads)
                            434 LOAD_FAST                4 (sdk_resource)
                            436 LOAD_METHOD              7 (to_json)
                            458 PRECALL                  0
                            462 CALL                     0
                            472 PRECALL                  1
                            476 CALL                     1
                
-               179         486 LOAD_FAST                8 (scope_spans)
+               203         486 LOAD_FAST                8 (scope_spans)
                
-               177         488 LOAD_CONST               4 (('resource', 'scope_spans'))
+               201         488 LOAD_CONST               4 (('resource', 'scope_spans'))
                            490 BUILD_CONST_KEY_MAP      2
                
-               176         492 PRECALL                  1
+               200         492 PRECALL                  1
                            496 CALL                     1
                            506 POP_TOP
                            508 JUMP_BACKWARD          164 (to 182)
                
-               184     >>  510 LOAD_CONST               5 ('resource_spans')
+               208     >>  510 LOAD_CONST               5 ('resource_spans')
                            512 LOAD_FAST                6 (resource_spans)
                
-               183         514 BUILD_MAP                1
+               207         514 BUILD_MAP                1
                            516 STORE_FAST               9 (data)
                
-               186         518 LOAD_GLOBAL             11 (NULL + json)
+               210         518 LOAD_GLOBAL             11 (NULL + json)
                            530 LOAD_ATTR                8 (dumps)
                            540 LOAD_FAST                9 (data)
                            542 PRECALL                  1
                            546 CALL                     1
                            556 RETURN_VALUE
                consts
                   None
@@ -1016,41 +1108,41 @@
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 3
                      flags     : 19
                      code
                         0x9700740100000000000000000000740200000000000000000000a60100
                         00ab0100000000000000005300
-                     160           0 RESUME                   0
+                     184           0 RESUME                   0
                                    2 LOAD_GLOBAL              1 (NULL + defaultdict)
                                   14 LOAD_GLOBAL              2 (list)
                                   26 PRECALL                  1
                                   30 CALL                     1
                                   40 RETURN_VALUE
                      consts
                         None
                      names      ('defaultdict', 'list')
                      varnames   ()
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                      name       '<lambda>'
-                     firstlineno 160
+                     firstlineno 184
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x970067007c005d287d017401000000000000000000006a010000000000
                         0000007c01a0020000000000000000000000000000000000000000a60000
                         00ab000000000000000000a6010000ab01000000000000000091028c2953
                         00
-                     173           0 RESUME                   0
+                     197           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                40 (to 88)
                                    8 STORE_FAST               1 (sdk_span)
                                   10 LOAD_GLOBAL              1 (NULL + json)
                                   22 LOAD_ATTR                1 (loads)
                                   32 LOAD_FAST                1 (sdk_span)
@@ -1065,42 +1157,42 @@
                      consts
                      names      ('json', 'loads', 'to_json')
                      varnames   ('.0', 'sdk_span')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                      name       '<listcomp>'
-                     firstlineno 173
+                     firstlineno 197
                      lnotab 0x
                   ('scope', 'spans')
                   ('resource', 'scope_spans')
                   'resource_spans'
                names      ('defaultdict', 'resource', 'instrumentation_scope', 'append', 'items', 'json', 'loads', 'to_json', 'dumps')
                varnames   ('self', 'sdk_spans', 'sdk_resource_spans', 'sdk_span', 'sdk_resource', 'sdk_instrumentation', 'resource_spans', 'sdk_instrumentations', 'scope_spans', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       '_serialize_spans'
-               firstlineno 148
+               firstlineno 172
                lnotab
                   0x020c200108010e010e014402040132010401320118024a0116fe04ff12
                   0618024a0102fe04ff120804ff0403
             (None, None, None, None, None, None)
             ('return', None)
             (30000,)
          names      ('__name__', '__module__', '__qualname__', 'Optional', 'str', 'Dict', 'int', 'Compression', 'requests', 'Session', '__init__', 'Sequence', 'ReadableSpan', 'SpanExportResult', 'export', 'shutdown', 'bool', 'force_flush', '_export', '_serialize_spans')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
          name       'OTLPSpanExporter'
-         firstlineno 58
+         firstlineno 59
          lnotab
             0x0a030201020102010201020102f904020efe02030efd02041efc02050e
-            fb02060efa020718f908281c15080712040c11
+            fb02060efa020718f908301c1b080c12040c15
       'OTLPSpanExporter'
       'return'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 7
          flags     : 3
@@ -1108,83 +1200,83 @@
             0x97007401000000000000000000006a0100000000000000007404000000
             000000000000007401000000000000000000006a01000000000000000074
             06000000000000000000006401a6020000ab020000000000000000a60200
             00ab020000000000000000a0040000000000000000000000000000000000
             000000a6000000ab000000000000000000a0050000000000000000000000
             000000000000000000a6000000ab0000000000000000007d00740d000000
             000000000000007c00a6010000ab0100000000000000005300
-         189           0 RESUME                   0
+         213           0 RESUME                   0
          
-         191           2 LOAD_GLOBAL              1 (NULL + environ)
+         215           2 LOAD_GLOBAL              1 (NULL + environ)
                       14 LOAD_ATTR                1 (get)
          
-         192          24 LOAD_GLOBAL              4 (OTEL_EXPORTER_OTLP_TRACES_COMPRESSION)
+         216          24 LOAD_GLOBAL              4 (OTEL_EXPORTER_OTLP_TRACES_COMPRESSION)
          
-         193          36 LOAD_GLOBAL              1 (NULL + environ)
+         217          36 LOAD_GLOBAL              1 (NULL + environ)
                       48 LOAD_ATTR                1 (get)
                       58 LOAD_GLOBAL              6 (OTEL_EXPORTER_OTLP_COMPRESSION)
                       70 LOAD_CONST               1 ('none')
                       72 PRECALL                  2
                       76 CALL                     2
          
-         191          86 PRECALL                  2
+         215          86 PRECALL                  2
                       90 CALL                     2
          
-         195         100 LOAD_METHOD              4 (lower)
+         219         100 LOAD_METHOD              4 (lower)
                      122 PRECALL                  0
                      126 CALL                     0
          
-         196         136 LOAD_METHOD              5 (strip)
+         220         136 LOAD_METHOD              5 (strip)
                      158 PRECALL                  0
                      162 CALL                     0
          
-         190         172 STORE_FAST               0 (compression)
+         214         172 STORE_FAST               0 (compression)
          
-         198         174 LOAD_GLOBAL             13 (NULL + Compression)
+         222         174 LOAD_GLOBAL             13 (NULL + Compression)
                      186 LOAD_FAST                0 (compression)
                      188 PRECALL                  1
                      192 CALL                     1
                      202 RETURN_VALUE
          consts
             None
             'none'
          names      ('environ', 'get', 'OTEL_EXPORTER_OTLP_TRACES_COMPRESSION', 'OTEL_EXPORTER_OTLP_COMPRESSION', 'lower', 'strip', 'Compression')
          varnames   ('compression',)
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
          name       '_compression_from_env'
-         firstlineno 189
+         firstlineno 213
          lnotab 0x020216010c0132fe0e04240124fa0208
       'endpoint'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007c00a00000000000000000000000000000000000000000006401a6
             010000ab010000000000000000720a7c007402000000000000000000007a
             00000053007c0064017402000000000000000000009b009d027a00000053
             00
-         201           0 RESUME                   0
+         225           0 RESUME                   0
          
-         202           2 LOAD_FAST                0 (endpoint)
+         226           2 LOAD_FAST                0 (endpoint)
                        4 LOAD_METHOD              0 (endswith)
                       26 LOAD_CONST               1 ('/')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 POP_JUMP_FORWARD_IF_FALSE    10 (to 64)
          
-         203          44 LOAD_FAST                0 (endpoint)
+         227          44 LOAD_FAST                0 (endpoint)
                       46 LOAD_GLOBAL              2 (DEFAULT_TRACES_EXPORT_PATH)
                       58 BINARY_OP                0 (+)
                       62 RETURN_VALUE
          
-         204     >>   64 LOAD_FAST                0 (endpoint)
+         228     >>   64 LOAD_FAST                0 (endpoint)
                       66 LOAD_CONST               1 ('/')
                       68 LOAD_GLOBAL              2 (DEFAULT_TRACES_EXPORT_PATH)
                       80 FORMAT_VALUE             0
                       82 BUILD_STRING             2
                       84 BINARY_OP                0 (+)
                       88 RETURN_VALUE
          consts
@@ -1192,19 +1284,19 @@
             '/'
          names      ('endswith', 'DEFAULT_TRACES_EXPORT_PATH')
          varnames   ('endpoint',)
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
          name       '_append_trace_path'
-         firstlineno 201
+         firstlineno 225
          lnotab 0x02012a011401
-   names      ('gzip', 'logging', 'zlib', 'io', 'BytesIO', 'collections', 'defaultdict', 'os', 'environ', 'typing', 'Dict', 'Optional', 'Sequence', 'json', 'requests', 'opentelemetry.sdk.environment_variables', 'OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE', 'OTEL_EXPORTER_OTLP_TRACES_COMPRESSION', 'OTEL_EXPORTER_OTLP_TRACES_ENDPOINT', 'OTEL_EXPORTER_OTLP_TRACES_HEADERS', 'OTEL_EXPORTER_OTLP_TRACES_TIMEOUT', 'OTEL_EXPORTER_OTLP_CERTIFICATE', 'OTEL_EXPORTER_OTLP_COMPRESSION', 'OTEL_EXPORTER_OTLP_ENDPOINT', 'OTEL_EXPORTER_OTLP_HEADERS', 'OTEL_EXPORTER_OTLP_TIMEOUT', 'opentelemetry.sdk.resources', 'SERVICE_NAME', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SpanExportResult', 'opentelemetry.sdk.trace', 'ReadableSpan', 'syntrac.sdk.otlp.json', '_OTLP_HTTP_HEADERS', 'DEFAULT_ENDPOINT', 'Compression', 'opentelemetry.util.re', 'parse_env_headers', 'getLogger', '__name__', '_logger', 'NoCompression', 'DEFAULT_COMPRESSION', 'DEFAULT_TRACES_EXPORT_PATH', 'DEFAULT_TIMEOUT', 'REQUESTS_SUCCESS_STATUS_CODES', 'logger', 'OTLPSpanExporter', '_compression_from_env', 'str', '_append_trace_path')
+   names      ('gzip', 'logging', 'zlib', 'io', 'BytesIO', 'collections', 'defaultdict', 'os', 'environ', 'typing', 'Dict', 'Optional', 'Sequence', 'json', 'requests', 'opentelemetry.sdk.environment_variables', 'OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE', 'OTEL_EXPORTER_OTLP_TRACES_COMPRESSION', 'OTEL_EXPORTER_OTLP_TRACES_ENDPOINT', 'OTEL_EXPORTER_OTLP_TRACES_HEADERS', 'OTEL_EXPORTER_OTLP_TRACES_TIMEOUT', 'OTEL_EXPORTER_OTLP_CERTIFICATE', 'OTEL_EXPORTER_OTLP_COMPRESSION', 'OTEL_EXPORTER_OTLP_ENDPOINT', 'OTEL_EXPORTER_OTLP_HEADERS', 'OTEL_EXPORTER_OTLP_TIMEOUT', 'opentelemetry.sdk.resources', 'SERVICE_NAME', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SpanExportResult', 'opentelemetry.sdk.trace', 'ReadableSpan', 'syntrac.sdk.otlp.json', '_OTLP_HTTP_HEADERS', 'DEFAULT_ENDPOINT', 'Compression', 'opentelemetry.util.re', 'parse_env_headers', 'syntrac.sdk', 'Telemetry', 'getLogger', '__name__', '_logger', 'NoCompression', 'DEFAULT_COMPRESSION', 'DEFAULT_TRACES_EXPORT_PATH', 'DEFAULT_TIMEOUT', 'REQUESTS_SUCCESS_STATUS_CODES', 'logger', 'OTLPSpanExporter', '_compression_from_env', 'str', '_append_trace_path')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020f0801080108010c010c010c01140108020802300c0c0110010c
-      0114050c0220020e0104010401040220031c7f00040c0c
+      0114050c010c0220020e0104010401040220031c7f001b0c0c
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/version.py` & `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/telemetry.py` & `syntrac_sdk-0.0.8/syntrac/sdk/telemetry.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/.DS_Store` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/.DS_Store`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3cf43e66 (Sat May 11 04:29:48 2024 UTC)
+moddate:  0x72174366 (Tue May 14 07:49:06 2024 UTC)
 files sz: 302
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb2193f66 (Sat May 11 07:09:38 2024 UTC)
+moddate:  0x72174366 (Tue May 14 07:49:06 2024 UTC)
 files sz: 2509
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa7193f66 (Sat May 11 07:09:27 2024 UTC)
+moddate:  0x72174366 (Tue May 14 07:49:06 2024 UTC)
 files sz: 1880
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x61f43e66 (Sat May 11 04:30:25 2024 UTC)
-files sz: 22217
+moddate:  0x29584366 (Tue May 14 12:25:13 2024 UTC)
+files sz: 22336
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -219,96 +219,96 @@
                350 LOAD_CONST              23 ('return')
                352 LOAD_NAME               27 (SpanExporter)
                354 BUILD_TUPLE              6
                356 LOAD_CONST              27 (<code object init_spans_exporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 336>)
                358 MAKE_FUNCTION            4 (annotations)
                360 STORE_NAME              56 (init_spans_exporter)
    
-   340         362 LOAD_CONST              28 ('resource')
+   346         362 LOAD_CONST              28 ('resource')
                364 LOAD_NAME               18 (Resource)
                366 LOAD_CONST              23 ('return')
                368 LOAD_NAME               20 (TracerProvider)
                370 BUILD_TUPLE              4
-               372 LOAD_CONST              29 (<code object init_tracer_provider, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 340>)
+               372 LOAD_CONST              29 (<code object init_tracer_provider, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 346>)
                374 MAKE_FUNCTION            4 (annotations)
                376 STORE_NAME              57 (init_tracer_provider)
    
-   358         378 LOAD_CONST              30 (<code object init_instrumentations, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 358>)
+   364         378 LOAD_CONST              30 (<code object init_instrumentations, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 364>)
                380 MAKE_FUNCTION            0
                382 STORE_NAME              58 (init_instrumentations)
    
-   379         384 LOAD_CONST              31 (<code object init_openai_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 379>)
+   385         384 LOAD_CONST              31 (<code object init_openai_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 385>)
                386 MAKE_FUNCTION            0
                388 STORE_NAME              59 (init_openai_instrumentor)
    
-   390         390 LOAD_CONST              32 (<code object init_anthropic_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 390>)
+   396         390 LOAD_CONST              32 (<code object init_anthropic_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 396>)
                392 MAKE_FUNCTION            0
                394 STORE_NAME              60 (init_anthropic_instrumentor)
    
-   401         396 LOAD_CONST              33 (<code object init_cohere_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 401>)
+   407         396 LOAD_CONST              33 (<code object init_cohere_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 407>)
                398 MAKE_FUNCTION            0
                400 STORE_NAME              61 (init_cohere_instrumentor)
    
-   412         402 LOAD_CONST              34 (<code object init_pinecone_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 412>)
+   418         402 LOAD_CONST              34 (<code object init_pinecone_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 418>)
                404 MAKE_FUNCTION            0
                406 STORE_NAME              62 (init_pinecone_instrumentor)
    
-   423         408 LOAD_CONST              35 (<code object init_qdrant_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 423>)
+   429         408 LOAD_CONST              35 (<code object init_qdrant_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 429>)
                410 MAKE_FUNCTION            0
                412 STORE_NAME              63 (init_qdrant_instrumentor)
    
-   433         414 LOAD_CONST              36 (<code object init_chroma_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 433>)
+   439         414 LOAD_CONST              36 (<code object init_chroma_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 439>)
                416 MAKE_FUNCTION            0
                418 STORE_NAME              64 (init_chroma_instrumentor)
    
-   444         420 LOAD_CONST              37 (<code object init_haystack_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 444>)
+   450         420 LOAD_CONST              37 (<code object init_haystack_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 450>)
                422 MAKE_FUNCTION            0
                424 STORE_NAME              65 (init_haystack_instrumentor)
    
-   455         426 LOAD_CONST              38 (<code object init_langchain_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 455>)
+   461         426 LOAD_CONST              38 (<code object init_langchain_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 461>)
                428 MAKE_FUNCTION            0
                430 STORE_NAME              66 (init_langchain_instrumentor)
    
-   466         432 LOAD_CONST              39 (<code object init_transformers_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 466>)
+   472         432 LOAD_CONST              39 (<code object init_transformers_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 472>)
                434 MAKE_FUNCTION            0
                436 STORE_NAME              67 (init_transformers_instrumentor)
    
-   477         438 LOAD_CONST              40 (<code object init_llama_index_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 477>)
+   483         438 LOAD_CONST              40 (<code object init_llama_index_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 483>)
                440 MAKE_FUNCTION            0
                442 STORE_NAME              68 (init_llama_index_instrumentor)
    
-   488         444 LOAD_CONST              41 (<code object init_requests_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 488>)
+   494         444 LOAD_CONST              41 (<code object init_requests_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 494>)
                446 MAKE_FUNCTION            0
                448 STORE_NAME              69 (init_requests_instrumentor)
    
-   498         450 LOAD_CONST              42 (<code object init_urllib3_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 498>)
+   504         450 LOAD_CONST              42 (<code object init_urllib3_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 504>)
                452 MAKE_FUNCTION            0
                454 STORE_NAME              70 (init_urllib3_instrumentor)
    
-   508         456 LOAD_CONST              43 (<code object init_pymysql_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 508>)
+   514         456 LOAD_CONST              43 (<code object init_pymysql_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 514>)
                458 MAKE_FUNCTION            0
                460 STORE_NAME              71 (init_pymysql_instrumentor)
    
-   518         462 LOAD_CONST              44 (<code object init_bedrock_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 518>)
+   524         462 LOAD_CONST              44 (<code object init_bedrock_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 524>)
                464 MAKE_FUNCTION            0
                466 STORE_NAME              72 (init_bedrock_instrumentor)
    
-   528         468 LOAD_CONST              45 (<code object init_replicate_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 528>)
+   534         468 LOAD_CONST              45 (<code object init_replicate_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 534>)
                470 MAKE_FUNCTION            0
                472 STORE_NAME              73 (init_replicate_instrumentor)
    
-   539         474 LOAD_CONST              46 (<code object init_vertexai_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 539>)
+   545         474 LOAD_CONST              46 (<code object init_vertexai_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 545>)
                476 MAKE_FUNCTION            0
                478 STORE_NAME              74 (init_vertexai_instrumentor)
    
-   550         480 LOAD_CONST              47 (<code object init_watsonx_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 550>)
+   556         480 LOAD_CONST              47 (<code object init_watsonx_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 556>)
                482 MAKE_FUNCTION            0
                484 STORE_NAME              75 (init_watsonx_instrumentor)
    
-   561         486 LOAD_CONST              48 (<code object init_weaviate_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 561>)
+   567         486 LOAD_CONST              48 (<code object init_weaviate_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 567>)
                488 MAKE_FUNCTION            0
                490 STORE_NAME              76 (init_weaviate_instrumentor)
                492 LOAD_CONST               1 (None)
                494 RETURN_VALUE
    consts
       0
       None
@@ -2000,43 +2000,63 @@
          firstlineno 332
          lnotab 0x0201
       'api_endpoint'
       'headers'
       code
          argcount  : 2
          nlocals   : 2
-         stacksize : 4
+         stacksize : 5
          flags     : 3
          code
-            0x97007401000000000000000000007c009b0064019d027c01ac02a60200
-            00ab0200000000000000005300
+            0x9700740100000000000000000000a6000000ab000000000000000000a0
+            010000000000000000000000000000000000000000640164027c006901a6
+            020000ab02000000000000000001007405000000000000000000007c009b
+            0064039d027c01ac04a6020000ab0200000000000000005300
          336           0 RESUME                   0
          
-         337           2 LOAD_GLOBAL              1 (NULL + OTLPSpanExporter)
-                      14 LOAD_FAST                0 (api_endpoint)
-                      16 FORMAT_VALUE             0
-                      18 LOAD_CONST               1 ('/v1/traces')
-                      20 BUILD_STRING             2
-                      22 LOAD_FAST                1 (headers)
-                      24 KW_NAMES                 2
-                      26 PRECALL                  2
-                      30 CALL                     2
-                      40 RETURN_VALUE
+         337           2 LOAD_GLOBAL              1 (NULL + Telemetry)
+                      14 PRECALL                  0
+                      18 CALL                     0
+                      28 LOAD_METHOD              1 (capture)
+         
+         338          50 LOAD_CONST               1 ('exporter:init')
+         
+         340          52 LOAD_CONST               2 ('api_endpoint')
+                      54 LOAD_FAST                0 (api_endpoint)
+         
+         339          56 BUILD_MAP                1
+         
+         337          58 PRECALL                  2
+                      62 CALL                     2
+                      72 POP_TOP
+         
+         343          74 LOAD_GLOBAL              5 (NULL + OTLPSpanExporter)
+                      86 LOAD_FAST                0 (api_endpoint)
+                      88 FORMAT_VALUE             0
+                      90 LOAD_CONST               3 ('/v1/traces')
+                      92 BUILD_STRING             2
+                      94 LOAD_FAST                1 (headers)
+                      96 KW_NAMES                 4
+                      98 PRECALL                  2
+                     102 CALL                     2
+                     112 RETURN_VALUE
          consts
             None
+            'exporter:init'
+            'api_endpoint'
             '/v1/traces'
             ('endpoint', 'headers')
-         names      ('OTLPSpanExporter',)
+         names      ('Telemetry', 'capture', 'OTLPSpanExporter')
          varnames   ('api_endpoint', 'headers')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_spans_exporter'
          firstlineno 336
-         lnotab 0x0201
+         lnotab 0x02013001020204ff02fe1006
       'resource'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
@@ -2044,82 +2064,82 @@
             0000007d027403000000000000000000007c027404000000000000000000
             00a6020000ab02000000000000000072257407000000000000000000007c
             00ac01a6010000ab0100000000000000007d017409000000000000000000
             006a0500000000000000007c01a6010000ab01000000000000000001006e
             28740d000000000000000000007c026402a6020000ab0200000000000000
             007316740f000000000000000000006a0800000000000000006403a60100
             00ab0100000000000000000100640053007c027d017c015300
-         340           0 RESUME                   0
+         346           0 RESUME                   0
          
-         341           2 LOAD_CONST               0 (None)
+         347           2 LOAD_CONST               0 (None)
                        4 STORE_FAST               1 (provider)
          
-         342           6 LOAD_GLOBAL              1 (NULL + get_tracer_provider)
+         348           6 LOAD_GLOBAL              1 (NULL + get_tracer_provider)
                       18 PRECALL                  0
                       22 CALL                     0
                       32 STORE_FAST               2 (default_provider)
          
-         344          34 LOAD_GLOBAL              3 (NULL + isinstance)
+         350          34 LOAD_GLOBAL              3 (NULL + isinstance)
                       46 LOAD_FAST                2 (default_provider)
                       48 LOAD_GLOBAL              4 (ProxyTracerProvider)
                       60 PRECALL                  2
                       64 CALL                     2
                       74 POP_JUMP_FORWARD_IF_FALSE    37 (to 150)
          
-         345          76 LOAD_GLOBAL              7 (NULL + TracerProvider)
+         351          76 LOAD_GLOBAL              7 (NULL + TracerProvider)
                       88 LOAD_FAST                0 (resource)
                       90 KW_NAMES                 1
                       92 PRECALL                  1
                       96 CALL                     1
                      106 STORE_FAST               1 (provider)
          
-         346         108 LOAD_GLOBAL              9 (NULL + trace)
+         352         108 LOAD_GLOBAL              9 (NULL + trace)
                      120 LOAD_ATTR                5 (set_tracer_provider)
                      130 LOAD_FAST                1 (provider)
                      132 PRECALL                  1
                      136 CALL                     1
                      146 POP_TOP
                      148 JUMP_FORWARD            40 (to 230)
          
-         347     >>  150 LOAD_GLOBAL             13 (NULL + hasattr)
+         353     >>  150 LOAD_GLOBAL             13 (NULL + hasattr)
                      162 LOAD_FAST                2 (default_provider)
                      164 LOAD_CONST               2 ('add_span_processor')
                      166 PRECALL                  2
                      170 CALL                     2
                      180 POP_JUMP_FORWARD_IF_TRUE    22 (to 226)
          
-         348         182 LOAD_GLOBAL             15 (NULL + logging)
+         354         182 LOAD_GLOBAL             15 (NULL + logging)
                      194 LOAD_ATTR                8 (error)
          
-         349         204 LOAD_CONST               3 ("Cannot add span processor to the default provider since it doesn't support it")
+         355         204 LOAD_CONST               3 ("Cannot add span processor to the default provider since it doesn't support it")
          
-         348         206 PRECALL                  1
+         354         206 PRECALL                  1
                      210 CALL                     1
                      220 POP_TOP
          
-         351         222 LOAD_CONST               0 (None)
+         357         222 LOAD_CONST               0 (None)
                      224 RETURN_VALUE
          
-         353     >>  226 LOAD_FAST                2 (default_provider)
+         359     >>  226 LOAD_FAST                2 (default_provider)
                      228 STORE_FAST               1 (provider)
          
-         355     >>  230 LOAD_FAST                1 (provider)
+         361     >>  230 LOAD_FAST                1 (provider)
                      232 RETURN_VALUE
          consts
             None
             ('resource',)
             'add_span_processor'
             "Cannot add span processor to the default provider since it doesn't support it"
          names      ('get_tracer_provider', 'isinstance', 'ProxyTracerProvider', 'TracerProvider', 'trace', 'set_tracer_provider', 'hasattr', 'logging', 'error')
          varnames   ('resource', 'provider', 'default_provider')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_tracer_provider'
-         firstlineno 340
+         firstlineno 346
          lnotab 0x020104011c022a0120012a012001160102ff100304020402
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
@@ -2137,116 +2157,116 @@
             000000000000000100741900000000000000000000a6000000ab00000000
             00000000000100741b00000000000000000000a6000000ab000000000000
             0000000100741d00000000000000000000a6000000ab0000000000000000
             000100741f00000000000000000000a6000000ab00000000000000000001
             00742100000000000000000000a6000000ab000000000000000000010074
             2300000000000000000000a6000000ab0000000000000000000100640053
             00
-         358           0 RESUME                   0
+         364           0 RESUME                   0
          
-         359           2 LOAD_GLOBAL              1 (NULL + init_openai_instrumentor)
+         365           2 LOAD_GLOBAL              1 (NULL + init_openai_instrumentor)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 POP_TOP
          
-         360          30 LOAD_GLOBAL              3 (NULL + init_anthropic_instrumentor)
+         366          30 LOAD_GLOBAL              3 (NULL + init_anthropic_instrumentor)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 POP_TOP
          
-         361          58 LOAD_GLOBAL              5 (NULL + init_cohere_instrumentor)
+         367          58 LOAD_GLOBAL              5 (NULL + init_cohere_instrumentor)
                       70 PRECALL                  0
                       74 CALL                     0
                       84 POP_TOP
          
-         362          86 LOAD_GLOBAL              7 (NULL + init_pinecone_instrumentor)
+         368          86 LOAD_GLOBAL              7 (NULL + init_pinecone_instrumentor)
                       98 PRECALL                  0
                      102 CALL                     0
                      112 POP_TOP
          
-         363         114 LOAD_GLOBAL              9 (NULL + init_qdrant_instrumentor)
+         369         114 LOAD_GLOBAL              9 (NULL + init_qdrant_instrumentor)
                      126 PRECALL                  0
                      130 CALL                     0
                      140 POP_TOP
          
-         364         142 LOAD_GLOBAL             11 (NULL + init_chroma_instrumentor)
+         370         142 LOAD_GLOBAL             11 (NULL + init_chroma_instrumentor)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 POP_TOP
          
-         365         170 LOAD_GLOBAL             13 (NULL + init_haystack_instrumentor)
+         371         170 LOAD_GLOBAL             13 (NULL + init_haystack_instrumentor)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 POP_TOP
          
-         366         198 LOAD_GLOBAL             15 (NULL + init_langchain_instrumentor)
+         372         198 LOAD_GLOBAL             15 (NULL + init_langchain_instrumentor)
                      210 PRECALL                  0
                      214 CALL                     0
                      224 POP_TOP
          
-         367         226 LOAD_GLOBAL             17 (NULL + init_llama_index_instrumentor)
+         373         226 LOAD_GLOBAL             17 (NULL + init_llama_index_instrumentor)
                      238 PRECALL                  0
                      242 CALL                     0
                      252 POP_TOP
          
-         368         254 LOAD_GLOBAL             19 (NULL + init_transformers_instrumentor)
+         374         254 LOAD_GLOBAL             19 (NULL + init_transformers_instrumentor)
                      266 PRECALL                  0
                      270 CALL                     0
                      280 POP_TOP
          
-         369         282 LOAD_GLOBAL             21 (NULL + init_requests_instrumentor)
+         375         282 LOAD_GLOBAL             21 (NULL + init_requests_instrumentor)
                      294 PRECALL                  0
                      298 CALL                     0
                      308 POP_TOP
          
-         370         310 LOAD_GLOBAL             23 (NULL + init_urllib3_instrumentor)
+         376         310 LOAD_GLOBAL             23 (NULL + init_urllib3_instrumentor)
                      322 PRECALL                  0
                      326 CALL                     0
                      336 POP_TOP
          
-         371         338 LOAD_GLOBAL             25 (NULL + init_pymysql_instrumentor)
+         377         338 LOAD_GLOBAL             25 (NULL + init_pymysql_instrumentor)
                      350 PRECALL                  0
                      354 CALL                     0
                      364 POP_TOP
          
-         372         366 LOAD_GLOBAL             27 (NULL + init_bedrock_instrumentor)
+         378         366 LOAD_GLOBAL             27 (NULL + init_bedrock_instrumentor)
                      378 PRECALL                  0
                      382 CALL                     0
                      392 POP_TOP
          
-         373         394 LOAD_GLOBAL             29 (NULL + init_replicate_instrumentor)
+         379         394 LOAD_GLOBAL             29 (NULL + init_replicate_instrumentor)
                      406 PRECALL                  0
                      410 CALL                     0
                      420 POP_TOP
          
-         374         422 LOAD_GLOBAL             31 (NULL + init_vertexai_instrumentor)
+         380         422 LOAD_GLOBAL             31 (NULL + init_vertexai_instrumentor)
                      434 PRECALL                  0
                      438 CALL                     0
                      448 POP_TOP
          
-         375         450 LOAD_GLOBAL             33 (NULL + init_watsonx_instrumentor)
+         381         450 LOAD_GLOBAL             33 (NULL + init_watsonx_instrumentor)
                      462 PRECALL                  0
                      466 CALL                     0
                      476 POP_TOP
          
-         376         478 LOAD_GLOBAL             35 (NULL + init_weaviate_instrumentor)
+         382         478 LOAD_GLOBAL             35 (NULL + init_weaviate_instrumentor)
                      490 PRECALL                  0
                      494 CALL                     0
                      504 POP_TOP
                      506 LOAD_CONST               0 (None)
                      508 RETURN_VALUE
          consts
             None
          names      ('init_openai_instrumentor', 'init_anthropic_instrumentor', 'init_cohere_instrumentor', 'init_pinecone_instrumentor', 'init_qdrant_instrumentor', 'init_chroma_instrumentor', 'init_haystack_instrumentor', 'init_langchain_instrumentor', 'init_llama_index_instrumentor', 'init_transformers_instrumentor', 'init_requests_instrumentor', 'init_urllib3_instrumentor', 'init_pymysql_instrumentor', 'init_bedrock_instrumentor', 'init_replicate_instrumentor', 'init_vertexai_instrumentor', 'init_watsonx_instrumentor', 'init_weaviate_instrumentor')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_instrumentations'
-         firstlineno 358
+         firstlineno 364
          lnotab
             0x02011c011c011c011c011c011c011c011c011c011c011c011c011c011c
             011c011c011c01
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
@@ -2256,59 +2276,59 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814e740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c006405ac
             06a6010000ab0100000000000000007d017c016a07000000000000000073
             147c01a0080000000000000000000000000000000000000000a6000000ab
             000000000000000000010064055300
-         379           0 RESUME                   0
+         385           0 RESUME                   0
          
-         380           2 LOAD_GLOBAL              0 (importlib)
+         386           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('openai')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    78 (to 220)
          
-         381          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         387          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:openai:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         382         130 LOAD_CONST               3 (0)
+         388         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('OpenAIInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.openai)
                      136 IMPORT_FROM              6 (OpenAIInstrumentor)
                      138 STORE_FAST               0 (OpenAIInstrumentor)
                      140 POP_TOP
          
-         384         142 PUSH_NULL
+         390         142 PUSH_NULL
                      144 LOAD_FAST                0 (OpenAIInstrumentor)
                      146 LOAD_CONST               5 (True)
                      148 KW_NAMES                 6
                      150 PRECALL                  1
                      154 CALL                     1
                      164 STORE_FAST               1 (instrumentor)
          
-         385         166 LOAD_FAST                1 (instrumentor)
+         391         166 LOAD_FAST                1 (instrumentor)
                      168 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      178 POP_JUMP_FORWARD_IF_TRUE    20 (to 220)
          
-         386         180 LOAD_FAST                1 (instrumentor)
+         392         180 LOAD_FAST                1 (instrumentor)
                      182 LOAD_METHOD              8 (instrument)
                      204 PRECALL                  0
                      208 CALL                     0
                      218 POP_TOP
          
-         387     >>  220 LOAD_CONST               5 (True)
+         393     >>  220 LOAD_CONST               5 (True)
                      222 RETURN_VALUE
          consts
             None
             'openai'
             'instrumentation:openai:init'
             0
             ('OpenAIInstrumentor',)
@@ -2316,15 +2336,15 @@
             ('enrich_assistant',)
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.openai', 'OpenAIInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('OpenAIInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_openai_instrumentor'
-         firstlineno 379
+         firstlineno 385
          lnotab 0x02013e0142010c0218010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2332,72 +2352,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         390           0 RESUME                   0
+         396           0 RESUME                   0
          
-         391           2 LOAD_GLOBAL              0 (importlib)
+         397           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('anthropic')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         392          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         398          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:anthropic:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         393         130 LOAD_CONST               3 (0)
+         399         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('AnthropicInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.anthropic)
                      136 IMPORT_FROM              6 (AnthropicInstrumentor)
                      138 STORE_FAST               0 (AnthropicInstrumentor)
                      140 POP_TOP
          
-         395         142 PUSH_NULL
+         401         142 PUSH_NULL
                      144 LOAD_FAST                0 (AnthropicInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         396         162 LOAD_FAST                1 (instrumentor)
+         402         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         397         176 LOAD_FAST                1 (instrumentor)
+         403         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         398     >>  216 LOAD_CONST               5 (True)
+         404     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'anthropic'
             'instrumentation:anthropic:init'
             0
             ('AnthropicInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.anthropic', 'AnthropicInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('AnthropicInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_anthropic_instrumentor'
-         firstlineno 390
+         firstlineno 396
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2405,72 +2425,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         401           0 RESUME                   0
+         407           0 RESUME                   0
          
-         402           2 LOAD_GLOBAL              0 (importlib)
+         408           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('cohere')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         403          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         409          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:cohere:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         404         130 LOAD_CONST               3 (0)
+         410         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('CohereInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.cohere)
                      136 IMPORT_FROM              6 (CohereInstrumentor)
                      138 STORE_FAST               0 (CohereInstrumentor)
                      140 POP_TOP
          
-         406         142 PUSH_NULL
+         412         142 PUSH_NULL
                      144 LOAD_FAST                0 (CohereInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         407         162 LOAD_FAST                1 (instrumentor)
+         413         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         408         176 LOAD_FAST                1 (instrumentor)
+         414         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         409     >>  216 LOAD_CONST               5 (True)
+         415     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'cohere'
             'instrumentation:cohere:init'
             0
             ('CohereInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.cohere', 'CohereInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('CohereInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_cohere_instrumentor'
-         firstlineno 401
+         firstlineno 407
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2478,72 +2498,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         412           0 RESUME                   0
+         418           0 RESUME                   0
          
-         413           2 LOAD_GLOBAL              0 (importlib)
+         419           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('pinecone')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         414          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         420          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:pinecone:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         415         130 LOAD_CONST               3 (0)
+         421         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('PineconeInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.pinecone)
                      136 IMPORT_FROM              6 (PineconeInstrumentor)
                      138 STORE_FAST               0 (PineconeInstrumentor)
                      140 POP_TOP
          
-         417         142 PUSH_NULL
+         423         142 PUSH_NULL
                      144 LOAD_FAST                0 (PineconeInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         418         162 LOAD_FAST                1 (instrumentor)
+         424         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         419         176 LOAD_FAST                1 (instrumentor)
+         425         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         420     >>  216 LOAD_CONST               5 (True)
+         426     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'pinecone'
             'instrumentation:pinecone:init'
             0
             ('PineconeInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.pinecone', 'PineconeInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('PineconeInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_pinecone_instrumentor'
-         firstlineno 412
+         firstlineno 418
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2551,76 +2571,76 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814e740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073187c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             00000000000100640053006400530064005300
-         423           0 RESUME                   0
+         429           0 RESUME                   0
          
-         424           2 LOAD_GLOBAL              0 (importlib)
+         430           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('qdrant_client')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    78 (to 220)
          
-         425          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         431          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:qdrant:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         426         130 LOAD_CONST               3 (0)
+         432         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('QdrantInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.qdrant)
                      136 IMPORT_FROM              6 (QdrantInstrumentor)
                      138 STORE_FAST               0 (QdrantInstrumentor)
                      140 POP_TOP
          
-         428         142 PUSH_NULL
+         434         142 PUSH_NULL
                      144 LOAD_FAST                0 (QdrantInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         429         162 LOAD_FAST                1 (instrumentor)
+         435         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    24 (to 224)
          
-         430         176 LOAD_FAST                1 (instrumentor)
+         436         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
                      216 LOAD_CONST               0 (None)
                      218 RETURN_VALUE
          
-         424     >>  220 LOAD_CONST               0 (None)
+         430     >>  220 LOAD_CONST               0 (None)
                      222 RETURN_VALUE
          
-         429     >>  224 LOAD_CONST               0 (None)
+         435     >>  224 LOAD_CONST               0 (None)
                      226 RETURN_VALUE
          consts
             None
             'qdrant_client'
             'instrumentation:qdrant:init'
             0
             ('QdrantInstrumentor',)
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.qdrant', 'QdrantInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('QdrantInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_qdrant_instrumentor'
-         firstlineno 423
+         firstlineno 429
          lnotab 0x02013e0142010c0214010e012cfa0405
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2628,72 +2648,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         433           0 RESUME                   0
+         439           0 RESUME                   0
          
-         434           2 LOAD_GLOBAL              0 (importlib)
+         440           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('chromadb')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         435          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         441          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:chromadb:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         436         130 LOAD_CONST               3 (0)
+         442         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('ChromaInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.chromadb)
                      136 IMPORT_FROM              6 (ChromaInstrumentor)
                      138 STORE_FAST               0 (ChromaInstrumentor)
                      140 POP_TOP
          
-         438         142 PUSH_NULL
+         444         142 PUSH_NULL
                      144 LOAD_FAST                0 (ChromaInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         439         162 LOAD_FAST                1 (instrumentor)
+         445         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         440         176 LOAD_FAST                1 (instrumentor)
+         446         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         441     >>  216 LOAD_CONST               5 (True)
+         447     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'chromadb'
             'instrumentation:chromadb:init'
             0
             ('ChromaInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.chromadb', 'ChromaInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('ChromaInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_chroma_instrumentor'
-         firstlineno 433
+         firstlineno 439
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2701,72 +2721,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         444           0 RESUME                   0
+         450           0 RESUME                   0
          
-         445           2 LOAD_GLOBAL              0 (importlib)
+         451           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('haystack')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         446          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         452          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:haystack:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         447         130 LOAD_CONST               3 (0)
+         453         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('HaystackInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.haystack)
                      136 IMPORT_FROM              6 (HaystackInstrumentor)
                      138 STORE_FAST               0 (HaystackInstrumentor)
                      140 POP_TOP
          
-         449         142 PUSH_NULL
+         455         142 PUSH_NULL
                      144 LOAD_FAST                0 (HaystackInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         450         162 LOAD_FAST                1 (instrumentor)
+         456         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         451         176 LOAD_FAST                1 (instrumentor)
+         457         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         452     >>  216 LOAD_CONST               5 (True)
+         458     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'haystack'
             'instrumentation:haystack:init'
             0
             ('HaystackInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.haystack', 'HaystackInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('HaystackInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_haystack_instrumentor'
-         firstlineno 444
+         firstlineno 450
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2774,72 +2794,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         455           0 RESUME                   0
+         461           0 RESUME                   0
          
-         456           2 LOAD_GLOBAL              0 (importlib)
+         462           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('langchain')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         457          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         463          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:langchain:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         458         130 LOAD_CONST               3 (0)
+         464         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('LangchainInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.langchain)
                      136 IMPORT_FROM              6 (LangchainInstrumentor)
                      138 STORE_FAST               0 (LangchainInstrumentor)
                      140 POP_TOP
          
-         460         142 PUSH_NULL
+         466         142 PUSH_NULL
                      144 LOAD_FAST                0 (LangchainInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         461         162 LOAD_FAST                1 (instrumentor)
+         467         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         462         176 LOAD_FAST                1 (instrumentor)
+         468         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         463     >>  216 LOAD_CONST               5 (True)
+         469     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'langchain'
             'instrumentation:langchain:init'
             0
             ('LangchainInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.langchain', 'LangchainInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('LangchainInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_langchain_instrumentor'
-         firstlineno 455
+         firstlineno 461
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2847,72 +2867,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         466           0 RESUME                   0
+         472           0 RESUME                   0
          
-         467           2 LOAD_GLOBAL              0 (importlib)
+         473           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('transformers')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         468          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         474          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:transformers:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         469         130 LOAD_CONST               3 (0)
+         475         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('TransformersInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.transformers)
                      136 IMPORT_FROM              6 (TransformersInstrumentor)
                      138 STORE_FAST               0 (TransformersInstrumentor)
                      140 POP_TOP
          
-         471         142 PUSH_NULL
+         477         142 PUSH_NULL
                      144 LOAD_FAST                0 (TransformersInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         472         162 LOAD_FAST                1 (instrumentor)
+         478         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         473         176 LOAD_FAST                1 (instrumentor)
+         479         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         474     >>  216 LOAD_CONST               5 (True)
+         480     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'transformers'
             'instrumentation:transformers:init'
             0
             ('TransformersInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.transformers', 'TransformersInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('TransformersInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_transformers_instrumentor'
-         firstlineno 466
+         firstlineno 472
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2920,322 +2940,322 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         477           0 RESUME                   0
+         483           0 RESUME                   0
          
-         478           2 LOAD_GLOBAL              0 (importlib)
+         484           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('llama_index')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         479          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         485          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:llamaindex:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         480         130 LOAD_CONST               3 (0)
+         486         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('LlamaIndexInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.llamaindex)
                      136 IMPORT_FROM              6 (LlamaIndexInstrumentor)
                      138 STORE_FAST               0 (LlamaIndexInstrumentor)
                      140 POP_TOP
          
-         482         142 PUSH_NULL
+         488         142 PUSH_NULL
                      144 LOAD_FAST                0 (LlamaIndexInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         483         162 LOAD_FAST                1 (instrumentor)
+         489         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         484         176 LOAD_FAST                1 (instrumentor)
+         490         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         485     >>  216 LOAD_CONST               5 (True)
+         491     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'llama_index'
             'instrumentation:llamaindex:init'
             0
             ('LlamaIndexInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.llamaindex', 'LlamaIndexInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('LlamaIndexInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_llama_index_instrumentor'
-         firstlineno 477
+         firstlineno 483
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000006401a6010000ab010000000000
             0000008132640264036c036d047d00010002007c00a6000000ab00000000
             00000000007d017c016a050000000000000000731b7c01a0060000000000
             000000000000000000000000000000740e00000000000000000000ac04a6
             010000ab010000000000000000010064055300
-         488           0 RESUME                   0
+         494           0 RESUME                   0
          
-         489           2 LOAD_GLOBAL              0 (importlib)
+         495           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('requests')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    50 (to 164)
          
-         490          64 LOAD_CONST               2 (0)
+         496          64 LOAD_CONST               2 (0)
                       66 LOAD_CONST               3 (('RequestsInstrumentor',))
                       68 IMPORT_NAME              3 (opentelemetry.instrumentation.requests)
                       70 IMPORT_FROM              4 (RequestsInstrumentor)
                       72 STORE_FAST               0 (RequestsInstrumentor)
                       74 POP_TOP
          
-         492          76 PUSH_NULL
+         498          76 PUSH_NULL
                       78 LOAD_FAST                0 (RequestsInstrumentor)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 STORE_FAST               1 (instrumentor)
          
-         493          96 LOAD_FAST                1 (instrumentor)
+         499          96 LOAD_FAST                1 (instrumentor)
                       98 LOAD_ATTR                5 (is_instrumented_by_opentelemetry)
                      108 POP_JUMP_FORWARD_IF_TRUE    27 (to 164)
          
-         494         110 LOAD_FAST                1 (instrumentor)
+         500         110 LOAD_FAST                1 (instrumentor)
                      112 LOAD_METHOD              6 (instrument)
                      134 LOAD_GLOBAL             14 (EXCLUDED_URLS)
                      146 KW_NAMES                 4
                      148 PRECALL                  1
                      152 CALL                     1
                      162 POP_TOP
          
-         495     >>  164 LOAD_CONST               5 (True)
+         501     >>  164 LOAD_CONST               5 (True)
                      166 RETURN_VALUE
          consts
             None
             'requests'
             0
             ('RequestsInstrumentor',)
             ('excluded_urls',)
             True
          names      ('importlib', 'util', 'find_spec', 'opentelemetry.instrumentation.requests', 'RequestsInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument', 'EXCLUDED_URLS')
          varnames   ('RequestsInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_requests_instrumentor'
-         firstlineno 488
+         firstlineno 494
          lnotab 0x02013e010c0214010e013601
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000006401a6010000ab010000000000
             0000008132640264036c036d047d00010002007c00a6000000ab00000000
             00000000007d017c016a050000000000000000731b7c01a0060000000000
             000000000000000000000000000000740e00000000000000000000ac04a6
             010000ab010000000000000000010064055300
-         498           0 RESUME                   0
+         504           0 RESUME                   0
          
-         499           2 LOAD_GLOBAL              0 (importlib)
+         505           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('urllib3')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    50 (to 164)
          
-         500          64 LOAD_CONST               2 (0)
+         506          64 LOAD_CONST               2 (0)
                       66 LOAD_CONST               3 (('URLLib3Instrumentor',))
                       68 IMPORT_NAME              3 (opentelemetry.instrumentation.urllib3)
                       70 IMPORT_FROM              4 (URLLib3Instrumentor)
                       72 STORE_FAST               0 (URLLib3Instrumentor)
                       74 POP_TOP
          
-         502          76 PUSH_NULL
+         508          76 PUSH_NULL
                       78 LOAD_FAST                0 (URLLib3Instrumentor)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 STORE_FAST               1 (instrumentor)
          
-         503          96 LOAD_FAST                1 (instrumentor)
+         509          96 LOAD_FAST                1 (instrumentor)
                       98 LOAD_ATTR                5 (is_instrumented_by_opentelemetry)
                      108 POP_JUMP_FORWARD_IF_TRUE    27 (to 164)
          
-         504         110 LOAD_FAST                1 (instrumentor)
+         510         110 LOAD_FAST                1 (instrumentor)
                      112 LOAD_METHOD              6 (instrument)
                      134 LOAD_GLOBAL             14 (EXCLUDED_URLS)
                      146 KW_NAMES                 4
                      148 PRECALL                  1
                      152 CALL                     1
                      162 POP_TOP
          
-         505     >>  164 LOAD_CONST               5 (True)
+         511     >>  164 LOAD_CONST               5 (True)
                      166 RETURN_VALUE
          consts
             None
             'urllib3'
             0
             ('URLLib3Instrumentor',)
             ('excluded_urls',)
             True
          names      ('importlib', 'util', 'find_spec', 'opentelemetry.instrumentation.urllib3', 'URLLib3Instrumentor', 'is_instrumented_by_opentelemetry', 'instrument', 'EXCLUDED_URLS')
          varnames   ('URLLib3Instrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_urllib3_instrumentor'
-         firstlineno 498
+         firstlineno 504
          lnotab 0x02013e010c0214010e013601
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000006401a6010000ab010000000000
             000000812b640264036c036d047d00010002007c00a6000000ab00000000
             00000000007d017c016a05000000000000000073147c01a0060000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             0064045300
-         508           0 RESUME                   0
+         514           0 RESUME                   0
          
-         509           2 LOAD_GLOBAL              0 (importlib)
+         515           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('sqlalchemy')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    43 (to 150)
          
-         510          64 LOAD_CONST               2 (0)
+         516          64 LOAD_CONST               2 (0)
                       66 LOAD_CONST               3 (('SQLAlchemyInstrumentor',))
                       68 IMPORT_NAME              3 (opentelemetry.instrumentation.sqlalchemy)
                       70 IMPORT_FROM              4 (SQLAlchemyInstrumentor)
                       72 STORE_FAST               0 (SQLAlchemyInstrumentor)
                       74 POP_TOP
          
-         512          76 PUSH_NULL
+         518          76 PUSH_NULL
                       78 LOAD_FAST                0 (SQLAlchemyInstrumentor)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 STORE_FAST               1 (instrumentor)
          
-         513          96 LOAD_FAST                1 (instrumentor)
+         519          96 LOAD_FAST                1 (instrumentor)
                       98 LOAD_ATTR                5 (is_instrumented_by_opentelemetry)
                      108 POP_JUMP_FORWARD_IF_TRUE    20 (to 150)
          
-         514         110 LOAD_FAST                1 (instrumentor)
+         520         110 LOAD_FAST                1 (instrumentor)
                      112 LOAD_METHOD              6 (instrument)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 POP_TOP
          
-         515     >>  150 LOAD_CONST               4 (True)
+         521     >>  150 LOAD_CONST               4 (True)
                      152 RETURN_VALUE
          consts
             None
             'sqlalchemy'
             0
             ('SQLAlchemyInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'opentelemetry.instrumentation.sqlalchemy', 'SQLAlchemyInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('SQLAlchemyInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_pymysql_instrumentor'
-         firstlineno 508
+         firstlineno 514
          lnotab 0x02013e010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000006401a6010000ab010000000000
             000000812b640264036c036d047d00010002007c00a6000000ab00000000
             00000000007d017c016a05000000000000000073147c01a0060000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             0064045300
-         518           0 RESUME                   0
+         524           0 RESUME                   0
          
-         519           2 LOAD_GLOBAL              0 (importlib)
+         525           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('boto3')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    43 (to 150)
          
-         520          64 LOAD_CONST               2 (0)
+         526          64 LOAD_CONST               2 (0)
                       66 LOAD_CONST               3 (('BedrockInstrumentor',))
                       68 IMPORT_NAME              3 (syntrac_opentelemetry.instrumentation.bedrock)
                       70 IMPORT_FROM              4 (BedrockInstrumentor)
                       72 STORE_FAST               0 (BedrockInstrumentor)
                       74 POP_TOP
          
-         522          76 PUSH_NULL
+         528          76 PUSH_NULL
                       78 LOAD_FAST                0 (BedrockInstrumentor)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 STORE_FAST               1 (instrumentor)
          
-         523          96 LOAD_FAST                1 (instrumentor)
+         529          96 LOAD_FAST                1 (instrumentor)
                       98 LOAD_ATTR                5 (is_instrumented_by_opentelemetry)
                      108 POP_JUMP_FORWARD_IF_TRUE    20 (to 150)
          
-         524         110 LOAD_FAST                1 (instrumentor)
+         530         110 LOAD_FAST                1 (instrumentor)
                      112 LOAD_METHOD              6 (instrument)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 POP_TOP
          
-         525     >>  150 LOAD_CONST               4 (True)
+         531     >>  150 LOAD_CONST               4 (True)
                      152 RETURN_VALUE
          consts
             None
             'boto3'
             0
             ('BedrockInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'syntrac_opentelemetry.instrumentation.bedrock', 'BedrockInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('BedrockInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_bedrock_instrumentor'
-         firstlineno 518
+         firstlineno 524
          lnotab 0x02013e010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3243,72 +3263,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         528           0 RESUME                   0
+         534           0 RESUME                   0
          
-         529           2 LOAD_GLOBAL              0 (importlib)
+         535           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('replicate')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         530          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         536          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:replicate:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         531         130 LOAD_CONST               3 (0)
+         537         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('ReplicateInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.replicate)
                      136 IMPORT_FROM              6 (ReplicateInstrumentor)
                      138 STORE_FAST               0 (ReplicateInstrumentor)
                      140 POP_TOP
          
-         533         142 PUSH_NULL
+         539         142 PUSH_NULL
                      144 LOAD_FAST                0 (ReplicateInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         534         162 LOAD_FAST                1 (instrumentor)
+         540         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         535         176 LOAD_FAST                1 (instrumentor)
+         541         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         536     >>  216 LOAD_CONST               5 (True)
+         542     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'replicate'
             'instrumentation:replicate:init'
             0
             ('ReplicateInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.replicate', 'ReplicateInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('ReplicateInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_replicate_instrumentor'
-         firstlineno 528
+         firstlineno 534
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3316,72 +3336,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         539           0 RESUME                   0
+         545           0 RESUME                   0
          
-         540           2 LOAD_GLOBAL              0 (importlib)
+         546           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('vertexai')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         541          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         547          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:vertexai:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         542         130 LOAD_CONST               3 (0)
+         548         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('VertexAIInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.vertexai)
                      136 IMPORT_FROM              6 (VertexAIInstrumentor)
                      138 STORE_FAST               0 (VertexAIInstrumentor)
                      140 POP_TOP
          
-         544         142 PUSH_NULL
+         550         142 PUSH_NULL
                      144 LOAD_FAST                0 (VertexAIInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         545         162 LOAD_FAST                1 (instrumentor)
+         551         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         546         176 LOAD_FAST                1 (instrumentor)
+         552         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         547     >>  216 LOAD_CONST               5 (True)
+         553     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'vertexai'
             'instrumentation:vertexai:init'
             0
             ('VertexAIInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.vertexai', 'VertexAIInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('VertexAIInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_vertexai_instrumentor'
-         firstlineno 539
+         firstlineno 545
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3389,72 +3409,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         550           0 RESUME                   0
+         556           0 RESUME                   0
          
-         551           2 LOAD_GLOBAL              0 (importlib)
+         557           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('ibm_watson_machine_learning')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         552          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         558          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:watsonx:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         553         130 LOAD_CONST               3 (0)
+         559         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('WatsonxInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.watsonx)
                      136 IMPORT_FROM              6 (WatsonxInstrumentor)
                      138 STORE_FAST               0 (WatsonxInstrumentor)
                      140 POP_TOP
          
-         555         142 PUSH_NULL
+         561         142 PUSH_NULL
                      144 LOAD_FAST                0 (WatsonxInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         556         162 LOAD_FAST                1 (instrumentor)
+         562         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         557         176 LOAD_FAST                1 (instrumentor)
+         563         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         558     >>  216 LOAD_CONST               5 (True)
+         564     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'ibm_watson_machine_learning'
             'instrumentation:watsonx:init'
             0
             ('WatsonxInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.watsonx', 'WatsonxInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('WatsonxInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_watsonx_instrumentor'
-         firstlineno 550
+         firstlineno 556
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3462,78 +3482,78 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         561           0 RESUME                   0
+         567           0 RESUME                   0
          
-         562           2 LOAD_GLOBAL              0 (importlib)
+         568           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('weaviate')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         563          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         569          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:weaviate:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         564         130 LOAD_CONST               3 (0)
+         570         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('WeaviateInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.weaviate)
                      136 IMPORT_FROM              6 (WeaviateInstrumentor)
                      138 STORE_FAST               0 (WeaviateInstrumentor)
                      140 POP_TOP
          
-         566         142 PUSH_NULL
+         572         142 PUSH_NULL
                      144 LOAD_FAST                0 (WeaviateInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         567         162 LOAD_FAST                1 (instrumentor)
+         573         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         568         176 LOAD_FAST                1 (instrumentor)
+         574         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         569     >>  216 LOAD_CONST               5 (True)
+         575     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'weaviate'
             'instrumentation:weaviate:init'
             0
             ('WeaviateInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.weaviate', 'WeaviateInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('WeaviateInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_weaviate_instrumentor'
-         firstlineno 561
+         firstlineno 567
          lnotab 0x02013e0142010c0214010e012801
    names      ('atexit', 'logging', 'os', 'importlib.util', 'importlib', 'colorama', 'Fore', 'opentelemetry', 'trace', 'syntrac.sdk.otlp.json.trace_exporter', 'OTLPSpanExporter', 'typing', 'Any', 'Callable', 'Dict', 'Optional', 'Set', 'opentelemetry.sdk.resources', 'Resource', 'opentelemetry.sdk.trace', 'TracerProvider', 'SpanProcessor', 'opentelemetry.propagators.textmap', 'TextMapPropagator', 'opentelemetry.propagate', 'set_global_textmap', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SimpleSpanProcessor', 'BatchSpanProcessor', 'opentelemetry.trace', 'get_tracer_provider', 'ProxyTracerProvider', 'syntrac_opentelemetry.semconv.ai', 'SpanAttributes', 'syntrac.sdk', 'Telemetry', 'syntrac.sdk.instruments', 'Instruments', 'syntrac.sdk.tracing.content_allow_list', 'ContentAllowList', 'syntrac.sdk.utils', 'is_notebook', 'syntrac.sdk.tracing.context', 'set_override_enable_context_tracing', 'get_association_properties', 'syntrac.sdk.tracing.span_from_context', 'set_workflow_name_from_context', 'set_prompt_attributes_from_context', 'TRACER_NAME', 'EXCLUDED_URLS', 'object', 'TracerWrapper', 'bool', 'is_llm_span', 'str', 'init_spans_exporter', 'init_tracer_provider', 'init_instrumentations', 'init_openai_instrumentor', 'init_anthropic_instrumentor', 'init_cohere_instrumentor', 'init_pinecone_instrumentor', 'init_qdrant_instrumentor', 'init_chroma_instrumentor', 'init_haystack_instrumentor', 'init_langchain_instrumentor', 'init_transformers_instrumentor', 'init_llama_index_instrumentor', 'init_requests_instrumentor', 'init_urllib3_instrumentor', 'init_pymysql_instrumentor', 'init_bedrock_instrumentor', 'init_replicate_instrumentor', 'init_vertexai_instrumentor', 'init_watsonx_instrumentor', 'init_weaviate_instrumentor')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010801080108030c010c010c031c010c0110010c010c0114
       0510020c010c010c010c010c0110011002040104101c7f007f001d0c0424
-      0410120615060b060b060b060b060a060b060b060b060b060b060a060a06
+      0a10120615060b060b060b060b060a060b060b060b060b060b060a060a06
       0a060a060b060b060b
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/content_allow_list.py` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/context.py` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/context.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/span_from_context.py` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/span_from_context.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/tracing/tracing.py` & `syntrac_sdk-0.0.8/syntrac/sdk/tracing/tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,14 +330,20 @@
 
 
 def is_llm_span(span) -> bool:
     return span.attributes.get(SpanAttributes.LLM_REQUEST_TYPE) is not None
 
 
 def init_spans_exporter(api_endpoint: str, headers: Dict[str, str]) -> SpanExporter:
+    Telemetry().capture(
+        "exporter:init",
+        {
+            "api_endpoint": api_endpoint,
+        },
+    )
     return OTLPSpanExporter(endpoint=f"{api_endpoint}/v1/traces", headers=headers)
 
 
 def init_tracer_provider(resource: Resource) -> TracerProvider:
     provider: Optional[TracerProvider] = None
     default_provider: TracerProvider = get_tracer_provider()
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/utils/__init__.py` & `syntrac_sdk-0.0.8/syntrac/sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.8/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x91193f66 (Sat May 11 07:09:05 2024 UTC)
+moddate:  0x72174366 (Tue May 14 07:49:06 2024 UTC)
 files sz: 878
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `syntrac_sdk-0.0.7/syntrac/sdk/utils/in_memory_span_exporter.py` & `syntrac_sdk-0.0.8/syntrac/sdk/utils/in_memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.7/PKG-INFO` & `syntrac_sdk-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntrac-sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: Syntrac Software Development Kit (SDK) for Python
 Home-page: https://github.com/syntracAI/syntrac
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

