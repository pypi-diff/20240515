# Comparing `tmp/that_depends-1.6.6.tar.gz` & `tmp/that_depends-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.6.6.tar", max compression
+gzip compressed data, was "that_depends-1.7.0.tar", max compression
```

## Comparing `that_depends-1.6.6.tar` & `that_depends-1.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.6.6/LICENSE
--rw-r--r--   0        0        0     7277 2024-05-10 11:45:17.705570 that_depends-1.6.6/README.md
--rw-r--r--   0        0        0     1482 2024-05-11 10:28:58.661919 that_depends-1.6.6/pyproject.toml
--rw-r--r--   0        0        0      164 2024-05-09 18:37:39.636094 that_depends-1.6.6/that_depends/__init__.py
--rw-r--r--   0        0        0     1984 2024-05-11 10:19:08.451499 that_depends-1.6.6/that_depends/container.py
--rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.6/that_depends/injection.py
--rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.6.6/that_depends/providers/__init__.py
--rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.6/that_depends/providers/base.py
--rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.6/that_depends/providers/collections.py
--rw-r--r--   0        0        0     3792 2024-04-28 07:52:26.186980 that_depends-1.6.6/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.6/that_depends/providers/factories.py
--rw-r--r--   0        0        0     2948 2024-04-21 21:10:28.406639 that_depends-1.6.6/that_depends/providers/resources.py
--rw-r--r--   0        0        0      993 2024-05-09 12:45:32.587857 that_depends-1.6.6/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.6/that_depends/py.typed
--rw-r--r--   0        0        0     7757 1970-01-01 00:00:00.000000 that_depends-1.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.7.0/LICENSE
+-rw-r--r--   0        0        0     1710 2024-05-12 20:23:56.338518 that_depends-1.7.0/README.md
+-rw-r--r--   0        0        0     1515 2024-05-15 16:11:20.814470 that_depends-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-05-09 18:37:39.636094 that_depends-1.7.0/that_depends/__init__.py
+-rw-r--r--   0        0        0     1990 2024-05-13 16:35:18.245230 that_depends-1.7.0/that_depends/container.py
+-rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.7.0/that_depends/injection.py
+-rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.7.0/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0      775 2024-05-13 16:35:18.256594 that_depends-1.7.0/that_depends/providers/base.py
+-rw-r--r--   0        0        0      608 2024-05-13 16:35:18.258303 that_depends-1.7.0/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.7.0/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.7.0/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     4071 2024-05-15 16:03:10.739869 that_depends-1.7.0/that_depends/providers/resources.py
+-rw-r--r--   0        0        0     1547 2024-05-13 16:35:20.477615 that_depends-1.7.0/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.7.0/that_depends/py.typed
+-rw-r--r--   0        0        0     2190 1970-01-01 00:00:00.000000 that_depends-1.7.0/PKG-INFO
```

### Comparing `that_depends-1.6.6/LICENSE` & `that_depends-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.6/pyproject.toml` & `that_depends-1.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.6.6"
+version = "1.7.0"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
@@ -28,14 +28,17 @@
 strict = true
 
 [tool.ruff]
 fix = true
 unsafe-fixes = true
 line-length = 120
 target-version = "py310"
+extend-exclude = [
+    "docs",
+]
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "D1", # allow missing docstrings
     "S101", # allow asserts
     "TCH", # ignore flake8-type-checking
```

### Comparing `that_depends-1.6.6/that_depends/container.py` & `that_depends-1.7.0/that_depends/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
             if field_value.default is not inspect.Parameter.empty or field_name in ("_", "__"):
                 continue
 
             if field_name not in providers:
                 msg = f"Provider is not found, {field_name=}"
                 raise RuntimeError(msg)
 
-            kwargs[field_name] = await providers[field_name].resolve()
+            kwargs[field_name] = await providers[field_name].async_resolve()
 
         return object_to_resolve(**kwargs)
```

### Comparing `that_depends-1.6.6/that_depends/injection.py` & `that_depends-1.7.0/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.6/that_depends/providers/__init__.py` & `that_depends-1.7.0/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.6/that_depends/providers/context_resources.py` & `that_depends-1.7.0/that_depends/providers/context_resources.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,14 +43,22 @@
         self.app = app
 
     @container_context()
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         return await self.app(scope, receive, send)
 
 
+def _get_context() -> dict[str, AbstractResource[typing.Any]]:
+    try:
+        return context.get()
+    except LookupError as exc:
+        msg = "Context is not set. Use container_context"
+        raise RuntimeError(msg) from exc
+
+
 class ContextResource(AbstractProvider[T]):
     def __init__(
         self,
         creator: typing.Callable[P, typing.Iterator[T]],
         *args: P.args,
         **kwargs: P.kwargs,
     ) -> None:
@@ -60,29 +68,33 @@
 
         self._creator = creator
         self._args = args
         self._kwargs = kwargs
         self._override = None
         self._internal_name = f"{type(self).__name__}-{uuid.uuid4()}"
 
-    async def resolve(self) -> T:
+    def _get_or_create_resource(self) -> AbstractResource[T]:
+        context_obj = _get_context()
+        if not (resource := context_obj.get(self._internal_name)):
+            resource = Resource(self._creator, *self._args, **self._kwargs)
+            context_obj[self._internal_name] = resource
+
+        return resource
+
+    async def async_resolve(self) -> T:
         if self._override:
             return typing.cast(T, self._override)
 
-        try:
-            context_obj = context.get()
-        except LookupError as exc:
-            msg = "Context is not set. Use container_context"
-            raise RuntimeError(msg) from exc
-
-        if not (_resource := context_obj.get(self._internal_name)):
-            _resource = Resource(self._creator, *self._args, **self._kwargs)
-            context_obj[self._internal_name] = _resource
+        return await self._get_or_create_resource().async_resolve()
+
+    def sync_resolve(self) -> T:
+        if self._override:
+            return typing.cast(T, self._override)
 
-        return typing.cast(T, await _resource.resolve())
+        return self._get_or_create_resource().sync_resolve()
 
 
 class AsyncContextResource(AbstractProvider[T]):
     def __init__(
         self,
         creator: typing.Callable[P, typing.AsyncIterator[T]],
         *args: P.args,
@@ -94,22 +106,26 @@
 
         self._creator = creator
         self._args = args
         self._kwargs = kwargs
         self._override = None
         self._internal_name = f"{type(self).__name__}-{uuid.uuid4()}"
 
-    async def resolve(self) -> T:
+    def _get_or_create_resource(self) -> AbstractResource[T]:
+        context_obj = _get_context()
+        if not (resource := context_obj.get(self._internal_name)):
+            resource = AsyncResource(self._creator, *self._args, **self._kwargs)
+            context_obj[self._internal_name] = resource
+
+        return resource
+
+    async def async_resolve(self) -> T:
         if self._override:
             return typing.cast(T, self._override)
 
-        try:
-            context_obj = context.get()
-        except LookupError as exc:
-            msg = "Context is not set. Use container_context"
-            raise RuntimeError(msg) from exc
-
-        if not (_resource := context_obj.get(self._internal_name)):
-            _resource = AsyncResource(self._creator, *self._args, **self._kwargs)
-            context_obj[self._internal_name] = _resource
+        return await self._get_or_create_resource().async_resolve()
+
+    def sync_resolve(self) -> T:
+        if self._override:
+            return typing.cast(T, self._override)
 
-        return typing.cast(T, await _resource.resolve())
+        return self._get_or_create_resource().sync_resolve()
```

### Comparing `that_depends-1.6.6/that_depends/providers/factories.py` & `that_depends-1.7.0/that_depends/providers/singleton.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,39 +3,43 @@
 from that_depends.providers.base import AbstractProvider
 
 
 T = typing.TypeVar("T")
 P = typing.ParamSpec("P")
 
 
-class Factory(AbstractProvider[T]):
+class Singleton(AbstractProvider[T]):
     def __init__(self, factory: type[T] | typing.Callable[P, T], *args: P.args, **kwargs: P.kwargs) -> None:
         self._factory = factory
         self._args = args
         self._kwargs = kwargs
         self._override = None
+        self._instance: T | None = None
 
-    async def resolve(self) -> T:
-        if self._override:
+    async def async_resolve(self) -> T:
+        if self._override is not None:
             return typing.cast(T, self._override)
 
-        return self._factory(
-            *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
-            **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
-        )
+        if self._instance is None:
+            self._instance = self._factory(
+                *[await x.async_resolve() if isinstance(x, AbstractProvider) else x for x in self._args],
+                **{
+                    k: await v.async_resolve() if isinstance(v, AbstractProvider) else v
+                    for k, v in self._kwargs.items()
+                },
+            )
+        return self._instance
 
-
-class AsyncFactory(AbstractProvider[T]):
-    def __init__(self, factory: typing.Callable[P, typing.Awaitable[T]], *args: P.args, **kwargs: P.kwargs) -> None:
-        self._factory = factory
-        self._args = args
-        self._kwargs = kwargs
-        self._override = None
-
-    async def resolve(self) -> T:
-        if self._override:
+    def sync_resolve(self) -> T:
+        if self._override is not None:
             return typing.cast(T, self._override)
 
-        return await self._factory(
-            *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
-            **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
-        )
+        if self._instance is None:
+            self._instance = self._factory(
+                *[x.sync_resolve() if isinstance(x, AbstractProvider) else x for x in self._args],
+                **{k: v.sync_resolve() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
+            )
+        return self._instance
+
+    async def tear_down(self) -> None:
+        if self._instance is not None:
+            self._instance = None
```

### Comparing `that_depends-1.6.6/that_depends/providers/resources.py` & `that_depends-1.7.0/that_depends/providers/resources.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,25 +29,47 @@
 
     async def tear_down(self) -> None:
         if self._context_stack:
             self._context_stack.close()
         if self._instance is not None:
             self._instance = None
 
-    async def resolve(self) -> T:
+    async def async_resolve(self) -> T:
         if self._override:
             return typing.cast(T, self._override)
 
         if self._instance is None:
             self._instance = typing.cast(
                 T,
                 self._context_stack.enter_context(
                     contextlib.contextmanager(self._creator)(
-                        *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
-                        **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
+                        *[await x.async_resolve() if isinstance(x, AbstractProvider) else x for x in self._args],
+                        **{
+                            k: await v.async_resolve() if isinstance(v, AbstractProvider) else v
+                            for k, v in self._kwargs.items()
+                        },
+                    ),
+                ),
+            )
+        return self._instance
+
+    def sync_resolve(self) -> T:
+        if self._override:
+            return typing.cast(T, self._override)
+
+        if self._instance is None:
+            self._instance = typing.cast(
+                T,
+                self._context_stack.enter_context(
+                    contextlib.contextmanager(self._creator)(
+                        *[x.sync_resolve() if isinstance(x, AbstractProvider) else x for x in self._args],
+                        **{
+                            k: v.sync_resolve() if isinstance(v, AbstractProvider) else v
+                            for k, v in self._kwargs.items()
+                        },
                     ),
                 ),
             )
         return self._instance
 
 
 class AsyncResource(AbstractResource[T]):
@@ -70,22 +92,32 @@
 
     async def tear_down(self) -> None:
         if self._context_stack:
             await self._context_stack.aclose()
         if self._instance is not None:
             self._instance = None
 
-    async def resolve(self) -> T:
+    async def async_resolve(self) -> T:
         if self._override:
             return typing.cast(T, self._override)
 
         if self._instance is None:
             self._instance = typing.cast(
                 T,
                 await self._context_stack.enter_async_context(
                     contextlib.asynccontextmanager(self._creator)(
                         *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
                         **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
                     ),
                 ),
             )
         return self._instance
+
+    def sync_resolve(self) -> T:
+        if self._override:
+            return typing.cast(T, self._override)
+
+        if self._instance is None:
+            msg = "AsyncResource cannot be resolved synchronously"
+            raise RuntimeError(msg)
+
+        return self._instance
```

