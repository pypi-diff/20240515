# Comparing `tmp/configzen-0.9.0.tar.gz` & `tmp/configzen-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.9.0.tar", max compression
+gzip compressed data, was "configzen-1.0.0a0.tar", max compression
```

## Comparing `configzen-0.9.0.tar` & `configzen-1.0.0a0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
--rw-r--r--   0        0        0     1062 2023-08-22 06:18:50.949295 configzen-0.9.0/LICENSE
--rw-r--r--   0        0        0    16349 2023-08-22 06:18:50.949295 configzen-0.9.0/README.md
--rw-r--r--   0        0        0      721 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/__init__.py
--rw-r--r--   0        0        0      929 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/__main__.py
--rw-r--r--   0        0        0     1849 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/_detach.py
--rw-r--r--   0        0        0     3980 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/_setup.py
--rw-r--r--   0        0        0     6774 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/decorators.py
--rw-r--r--   0        0        0     4338 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/errors.py
--rw-r--r--   0        0        0      475 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/field.py
--rw-r--r--   0        0        0    14650 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/interpolation.py
--rw-r--r--   0        0        0    78749 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/model.py
--rw-r--r--   0        0        0     3761 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/module.py
--rw-r--r--   0        0        0    25912 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/py.typed
--rw-r--r--   0        0        0     4603 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/route.py
--rw-r--r--   0        0        0     1453 2023-08-22 06:18:50.949295 configzen-0.9.0/configzen/typedefs.py
--rw-r--r--   0        0        0     5850 2023-08-22 06:18:50.953295 configzen-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    17925 1970-01-01 00:00:00.000000 configzen-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-15 02:41:10.031376 configzen-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0    11297 2024-05-15 02:41:10.031376 configzen-1.0.0a0/README.md
+-rw-r--r--   0        0        0      718 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/__init__.py
+-rw-r--r--   0        0        0    21273 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/config.py
+-rw-r--r--   0        0        0     2095 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/context.py
+-rw-r--r--   0        0        0       85 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/contrib/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/contrib/pyproject.py
+-rw-r--r--   0        0        0       54 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/contrib/setup.py
+-rw-r--r--   0        0        0    10406 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/data.py
+-rw-r--r--   0        0        0     2145 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/errors.py
+-rw-r--r--   0        0        0      379 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/formats/__init__.py
+-rw-r--r--   0        0        0     3980 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/formats/std_json.py
+-rw-r--r--   0        0        0     2839 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/formats/std_plist.py
+-rw-r--r--   0        0        0     2241 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/formats/toml.py
+-rw-r--r--   0        0        0     3459 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/formats/yaml.py
+-rw-r--r--   0        0        0     6258 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/module_proxy.py
+-rw-r--r--   0        0        0    10315 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/processor.py
+-rw-r--r--   0        0        0        0 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/py.typed
+-rw-r--r--   0        0        0    15164 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/routes.py
+-rw-r--r--   0        0        0    12965 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/sources.py
+-rw-r--r--   0        0        0      255 2024-05-15 02:41:10.031376 configzen-1.0.0a0/configzen/typedefs.py
+-rw-r--r--   0        0        0     6183 2024-05-15 02:41:10.031376 configzen-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0    12527 1970-01-01 00:00:00.000000 configzen-1.0.0a0/PKG-INFO
```

### Comparing `configzen-0.9.0/configzen/_detach.py` & `configzen-1.0.0a0/configzen/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,78 @@
+"""Facilities for [contextual][contextvars] processing."""
+
 from __future__ import annotations
 
 import asyncio
 import contextvars
-import functools
-from typing import TYPE_CHECKING, cast, no_type_check
+from functools import wraps
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Coroutine
+    from typing import TypeVar
+
+    from typing_extensions import ParamSpec
 
-    from configzen.typedefs import P, T
+    _T = TypeVar("_T")
+    _P = ParamSpec("_P")
 
-# pyright: reportGeneralTypeIssues=false
 
+__all__ = (
+    "isolated_context_function",
+    "isolated_context_coroutine",
+    "run_isolated",
+    "async_run_isolated",
+)
 
-@no_type_check
-def detached_context_function(
-    func: Callable[P, T],
-) -> Callable[P, T]:
+
+def isolated_context_function(func: Callable[_P, _T]) -> Callable[_P, _T]:
     """
-    Copy a function call context automatically (context isolation)
-    to prevent collisions.
+    Copy the context automatically on function call.
+
+    Allows to isolate the library context from the user context.
 
-    This decorator will copy the current context and run the function
-    in this new isolated context.
+    Used as a decorator.
     """
     if isinstance(func, (classmethod, staticmethod)):
-        return type(func)(detached_context_function(func.__func__))
+        return type(func)(isolated_context_function(func.__func__))
+
+    @wraps(func)
+    def copy(*args: _P.args, **kwargs: _P.kwargs) -> _T:
+        return run_isolated(func, *args, **kwargs)
+
+    return copy
+
+
+def isolated_context_coroutine(
+    func: Callable[_P, Coroutine[object, object, _T]],
+) -> Callable[_P, Coroutine[object, object, _T]]:
+    """
+    Copy the context automatically on coroutine execution.
+
+    Allows to isolate library context from the user context.
+
+    Used as a decorator.
+    """
+    if isinstance(func, (classmethod, staticmethod)):
+        return type(func)(isolated_context_coroutine(func.__func__))
+
+    @wraps(func)
+    async def copy_async(*args: _P.args, **kwargs: _P.kwargs) -> _T:
+        return await async_run_isolated(func, *args, **kwargs)
+
+    return copy_async
 
-    if asyncio.iscoroutinefunction(func):
 
-        @no_type_check
-        @functools.wraps(func)
-        def _detaching_async_wrapper(
-            *args: object,
-            **kwargs: object,
-        ) -> asyncio.Task[T]:
-            return detached_context_await(
-                cast("Callable[P, Coroutine[object, object, T]]", func),
-                *args,
-                **kwargs,
-            )
-
-        return _detaching_async_wrapper
-
-    @functools.wraps(func)
-    def _detaching_wrapper(*args: object, **kwargs: object) -> T:
-        return detached_context_run(func, *args, **kwargs)
-
-    return _detaching_wrapper
-
-
-def detached_context_run(
-    func: Callable[..., T],
-    *args: object,
-    **kwargs: object,
-) -> T:
+def run_isolated(func: Callable[_P, _T], *args: _P.args, **kwargs: _P.kwargs) -> _T:
     """Run a function in an isolated context."""
     context = contextvars.copy_context()
     return context.run(func, *args, **kwargs)
 
 
-def detached_context_await(
-    func: Callable[..., Coroutine[object, object, T]],
-    *args: object,
-    **kwargs: object,
-) -> asyncio.Task[T]:
+def async_run_isolated(
+    func: Callable[_P, Coroutine[object, object, _T]],
+    *args: _P.args,
+    **kwargs: _P.kwargs,
+) -> asyncio.Task[_T]:
     """Await a coroutine in an isolated context."""
     return asyncio.create_task(func(*args, **kwargs))
```

