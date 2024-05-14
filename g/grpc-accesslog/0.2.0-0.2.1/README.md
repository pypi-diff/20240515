# Comparing `tmp/grpc_accesslog-0.2.0.tar.gz` & `tmp/grpc_accesslog-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc_accesslog-0.2.0.tar", max compression
+gzip compressed data, was "grpc_accesslog-0.2.1.tar", max compression
```

## Comparing `grpc_accesslog-0.2.0.tar` & `grpc_accesslog-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/LICENSE.rst
--rw-r--r--   0        0        0     3009 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/README.rst
--rw-r--r--   0        0        0     1973 2023-08-04 02:37:00.635139 grpc_accesslog-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      161 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/__init__.py
--rw-r--r--   0        0        0      339 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/_context.py
--rw-r--r--   0        0        0     6379 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/_server.py
--rw-r--r--   0        0        0     3357 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/handlers.py
--rw-r--r--   0        0        0        0 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/py.typed
--rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 grpc_accesslog-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/LICENSE.rst
+-rw-r--r--   0        0        0     3009 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/README.rst
+-rw-r--r--   0        0        0     1965 2024-05-14 23:27:56.451378 grpc_accesslog-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      162 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/__init__.py
+-rw-r--r--   0        0        0      340 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/_context.py
+-rw-r--r--   0        0        0     6750 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/_server.py
+-rw-r--r--   0        0        0     3358 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/handlers.py
+-rw-r--r--   0        0        0        0 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/py.typed
+-rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 grpc_accesslog-0.2.1/PKG-INFO
```

### Comparing `grpc_accesslog-0.2.0/LICENSE.rst` & `grpc_accesslog-0.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `grpc_accesslog-0.2.0/README.rst` & `grpc_accesslog-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `grpc_accesslog-0.2.0/pyproject.toml` & `grpc_accesslog-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grpc-accesslog"
-version = "0.2.0"
+version = "0.2.1"
 description = "gRPC Access Log"
 authors = ["Michael Morgan <git@morgan83.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/villainy/grpc-accesslog"
 repository = "https://github.com/villainy/grpc-accesslog"
 documentation = "https://grpc-accesslog.readthedocs.io"
@@ -17,19 +17,19 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 grpcio = "^1.56.2"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
-black = ">=21.10b0"
+bandit = ">=1.7.7"
+black = ">=24.1.0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
-flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.930"
 pep8-naming = ">=0.12.1"
```

### Comparing `grpc_accesslog-0.2.0/src/grpc_accesslog/_server.py` & `grpc_accesslog-0.2.1/src/grpc_accesslog/_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 """gRPC access log server interceptor."""
+
 import logging
 from datetime import datetime
 from datetime import timezone
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import Iterator
 from typing import Optional
+from typing import Union
 
 import grpc
 
 from . import handlers as _handlers
 from ._context import LogContext
 
 
 def _wrap_rpc_behavior(
-    handler: grpc.RpcMethodHandler,
+    handler: Union[grpc.RpcMethodHandler, None],
     continuation: Callable[
         [
             Callable[[Any, grpc.ServicerContext], Any],
             bool,
             bool,
         ],
         Callable[[Any, grpc.ServicerContext], Any],
     ],
-) -> grpc.RpcMethodHandler:
+) -> Union[grpc.RpcMethodHandler, None]:
     """Wrap an RPC call.
 
     From https://github.com/grpc/grpc/issues/18191#issuecomment-574735994
     """
+    if handler is None:
+        return None
+
     if handler.request_streaming and handler.response_streaming:
         behavior_fn = handler.stream_stream
         handler_factory = grpc.stream_stream_rpc_method_handler
     elif handler.request_streaming and not handler.response_streaming:
         behavior_fn = handler.stream_unary
         handler_factory = grpc.stream_unary_rpc_method_handler
     elif not handler.request_streaming and handler.response_streaming:
@@ -59,34 +64,40 @@
     def __init__(
         self,
         level: int = logging.INFO,
         name: str = __name__,
         handlers: Optional[Iterable[Callable[[LogContext], str]]] = None,
         separator: str = " ",
         propagate: bool = False,
+        logger: Optional[logging.Logger] = None,
     ) -> None:
         """Create a logging interceptor.
 
         Each provided handler will be called in order with a LogContext as
         the single positional argument. The resulting strings are joined
         using the provided separator to form the access log message.
 
         Args:
             level (int): Log level. Defaults to logging.INFO.
             name (str): Logger name. Defaults to __name__.
             handlers (Iterable[Callable[[LogContext], str]]): LogContext
                 handlers collected in order. Defaults to None.
             separator (str): Log message separator. Defaults to " ".
             propagate (bool): Enable propagation to parent loggers. Defaults to False.
+            logger (logging.Logger): The logger instance to use for access
+                logs. Optional, defaults to None.
         """
         super().__init__()
 
-        self._logger = logging.getLogger(name)
-        self._logger.propagate = propagate
-        self._logger.addHandler(logging.StreamHandler())
+        if logger is None:
+            self._logger = logging.getLogger(name)
+            self._logger.propagate = propagate
+            self._logger.addHandler(logging.StreamHandler())
+        else:
+            self._logger = logger
 
         self._level = level
         self._format = format
         self._handlers = handlers
         self._separator = separator
 
         if handlers is None:
@@ -131,15 +142,15 @@
     def intercept_service(
         self,
         continuation: Callable[
             [grpc.HandlerCallDetails],
             grpc.RpcMethodHandler,
         ],
         handler_call_details: grpc.HandlerCallDetails,
-    ) -> grpc.RpcMethodHandler:
+    ) -> Union[grpc.RpcMethodHandler, None]:
         """Intercept an RPC."""
 
         def logging_wrapper(
             behavior: Callable[[Any, grpc.ServicerContext], Any],
             request_streaming: bool,
             response_streaming: bool,
         ) -> Callable[[Any, grpc.ServicerContext], Any]:
```

### Comparing `grpc_accesslog-0.2.0/src/grpc_accesslog/handlers.py` & `grpc_accesslog-0.2.1/src/grpc_accesslog/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """gRPC access log handlers."""
+
 from datetime import timedelta
 from typing import Callable
 
 import grpc
 
 from ._context import LogContext
```

### Comparing `grpc_accesslog-0.2.0/PKG-INFO` & `grpc_accesslog-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpc-accesslog
-Version: 0.2.0
+Version: 0.2.1
 Summary: gRPC Access Log
 Home-page: https://github.com/villainy/grpc-accesslog
 License: MIT
 Author: Michael Morgan
 Author-email: git@morgan83.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

