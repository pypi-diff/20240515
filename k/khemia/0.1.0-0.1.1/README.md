# Comparing `tmp/khemia-0.1.0.tar.gz` & `tmp/khemia-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khemia-0.1.0.tar", max compression
+gzip compressed data, was "khemia-0.1.1.tar", max compression
```

## Comparing `khemia-0.1.0.tar` & `khemia-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1058 2023-12-12 09:35:35.036310 khemia-0.1.0/LICENSE
--rw-r--r--   0        0        0       52 2023-12-12 09:35:35.036310 khemia-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-12-12 09:35:35.036310 khemia-0.1.0/khemia/__init__.py
--rw-r--r--   0        0        0    16042 2023-12-12 09:35:35.036310 khemia-0.1.0/khemia/cache.py
--rw-r--r--   0        0        0     4199 2023-12-12 09:35:35.036310 khemia-0.1.0/khemia/typing.py
--rw-r--r--   0        0        0     2464 2023-12-12 09:35:35.036310 khemia-0.1.0/khemia/utils.py
--rw-r--r--   0        0        0     1431 2023-12-12 09:35:35.036310 khemia-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 khemia-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-15 09:49:36.671900 khemia-0.1.1/LICENSE
+-rw-r--r--   0        0        0       52 2024-05-15 09:49:36.671900 khemia-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 09:49:36.671900 khemia-0.1.1/khemia/__init__.py
+-rw-r--r--   0        0        0    16042 2024-05-15 09:49:36.671900 khemia-0.1.1/khemia/cache.py
+-rw-r--r--   0        0        0     4602 2024-05-15 09:49:36.671900 khemia-0.1.1/khemia/typing.py
+-rw-r--r--   0        0        0     2464 2024-05-15 09:49:36.671900 khemia-0.1.1/khemia/utils.py
+-rw-r--r--   0        0        0     1453 2024-05-15 09:49:36.671900 khemia-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 khemia-0.1.1/PKG-INFO
```

### Comparing `khemia-0.1.0/LICENSE` & `khemia-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `khemia-0.1.0/khemia/cache.py` & `khemia-0.1.1/khemia/cache.py`

 * *Files identical despite different names*

### Comparing `khemia-0.1.0/khemia/typing.py` & `khemia-0.1.1/khemia/typing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,72 @@
+from collections.abc import Iterable, Mapping, Sequence
 import contextlib
 from dataclasses import is_dataclass as is_dataclass
 import sys
 import typing
-from typing import Callable, ClassVar, ForwardRef, Iterable, Mapping, Optional, Sequence, Tuple, Type, Union
-from typing_extensions import (
+from typing import (
     Annotated,
+    Callable,
+    ClassVar,
+    ForwardRef,
+    Optional,
+    TYPE_CHECKING,
+    Union,
+)
+from typing_extensions import (
     Any,
     get_args as _typing_get_args,
     get_origin as _typing_get_origin,
     is_protocol as is_protocol,
     is_typeddict as is_typeddict,
     Literal,
+    TypeGuard,
 )
 
 LITERAL_TYPES: set[Any] = {Literal}
 if hasattr(typing, "Literal"):
     LITERAL_TYPES.add(typing.Literal)
 
 NoneType = type(None)
 NONE_TYPES: tuple[Any, ...] = (None, NoneType, *(tp[None] for tp in LITERAL_TYPES))
 
+if TYPE_CHECKING:
+    check_isinstance = isinstance
+else:
 
-def check_isinstance(value: Any, class_or_tuple: type[Any] | tuple[type[Any], ...] | None) -> bool:
-    try:
-        return isinstance(value, class_or_tuple)  # type: ignore[arg-type]
-    except TypeError:
-        return False
+    def check_isinstance(value: Any, class_or_tuple: Union[type[Any], tuple[type[Any], ...], None]) -> bool:
+        try:
+            return isinstance(value, class_or_tuple)
+        except TypeError:
+            return False
 
 
-def check_issubclass(cls: Any, class_or_tuple: Any) -> bool:
-    try:
-        return isinstance(cls, type) and issubclass(cls, class_or_tuple)
-    except TypeError:
-        return False
+if TYPE_CHECKING:
+    check_issubclass = issubclass
+else:
+
+    def check_issubclass(cls: Any, class_or_tuple: Any) -> bool:
+        try:
+            return isinstance(cls, type) and issubclass(cls, class_or_tuple)
+        except TypeError:
+            return False
 
 
-def get_origin(tp: Type[Any]):
+def get_origin(tp: type[Any]):
     return _typing_get_origin(tp) or getattr(tp, "__origin__", None)
 
 
-def _generic_get_args(tp: Type[Any]) -> Tuple[Any, ...]:
+def _generic_get_args(tp: type[Any]) -> tuple[Any, ...]:
     with contextlib.suppress(TypeError):
-        if tp == Tuple[()] or sys.version_info >= (3, 9) and tp == tuple[()]:
+        if tp == tuple[()] or sys.version_info >= (3, 9) and tp == tuple[()]:
             return ((),)
     return ()
 
 
-def get_args(tp: Type[Any]) -> Tuple[Any, ...]:
+def get_args(tp: type[Any]) -> tuple[Any, ...]:
     return _typing_get_args(tp) or getattr(tp, "__args__", ()) or _generic_get_args(tp)
 
 
 def is_none_type(type_: Any):
     return type_ in NONE_TYPES
 
 
@@ -78,15 +94,15 @@
     return get_origin(type_) is Annotated
 
 
 def is_namedtuple(type_: type[Any]) -> bool:
     return check_issubclass(type_, tuple) and hasattr(type_, "_fields")
 
 
-def _check_classvar(v: type[Any] | None) -> bool:
+def _check_classvar(v: Union[type[Any], None]) -> bool:
     if v is None:
         return False
 
     return v.__class__ == ClassVar.__class__ and getattr(v, "_name", None) == "ClassVar"
 
 
 def is_classvar(type_: type[Any]) -> bool:
@@ -96,54 +112,54 @@
         return True
 
     return False
 
 
 if sys.version_info < (3, 10):
 
-    def is_union(type_: Optional[Type[Any]]) -> bool:
+    def is_union(type_: Optional[type[Any]]) -> bool:
         return type_ is Union
 
 
 else:
     import types
 
-    def is_union(type_: Optional[Type[Any]]) -> bool:
+    def is_union(type_: Optional[type[Any]]) -> bool:
         return type_ is Union or type_ is types.UnionType
 
 
-def is_optional(type: Type[Any]) -> bool:
-    return is_union(get_origin(type)) and any(is_none_type(tp) for tp in get_args(type))
+def is_optional(type_: type[Any]) -> bool:
+    return is_none_type(type_) or (is_union(get_origin(type_)) and any(is_none_type(tp) for tp in get_args(type_)))
 
 
-def get_type_from_optional(type: Type[Any]) -> Tuple[bool, Type[Any]]:
-    if not is_optional(type):
-        return False, type
-    return True, next(tp for tp in get_args(type) if not is_none_type(tp))
+def get_args_without_none(type_: type[Any]) -> tuple[bool, tuple[type[Any], ...]]:
+    if is_none_type(type_):
+        return True, ()
+    if is_union(get_origin(type_)):
+        args = get_args(type_)
+        is_optional_ = any(is_none_type(tp) for tp in args)
+        return is_optional_, tuple(tp for tp in args if not is_none_type(tp))
+    return False, (type_,)
 
 
-def is_sequence_type(type: Type[Any]) -> bool:
-    return check_issubclass(type, Sequence) or check_issubclass(get_origin(type), Sequence)
+def is_sequence_type(type_: type[Any]) -> TypeGuard[type[Sequence]]:
+    return check_issubclass(type_, Sequence) or check_issubclass(get_origin(type_), Sequence)  # type: ignore
 
 
-def is_sequence(value: Any) -> bool:
+def is_sequence(value: Any) -> TypeGuard[Sequence]:
     return check_isinstance(value, Sequence)
 
 
-def is_iterable_type(type: Type[Any]) -> bool:
-    return check_issubclass(type, Iterable) or check_issubclass(get_origin(type), Iterable)
+def is_iterable_type(type_: type[Any]) -> TypeGuard[type[Iterable]]:
+    return check_issubclass(type_, Iterable) or check_issubclass(get_origin(type_), Iterable)  # type: ignore
 
 
-def is_iterable(value: Any) -> bool:
+def is_iterable(value: Any) -> TypeGuard[Iterable]:
     return check_isinstance(value, Iterable)
 
 
-def is_mapping_type(type: Type[Any]) -> bool:
-    return check_issubclass(type, Mapping) or check_issubclass(get_origin(type), Mapping)
+def is_mapping_type(type_: type[Any]) -> TypeGuard[type[Mapping]]:
+    return check_issubclass(type_, Mapping) or check_issubclass(get_origin(type_), Mapping)  # type: ignore
 
 
-def is_mapping(value: Any) -> bool:
+def is_mapping(value: Any) -> TypeGuard[Mapping]:
     return check_isinstance(value, Mapping)
-
-
-def is_json_like_type(type_: Type[Any]) -> bool:
-    return check_issubclass(type_, (Mapping, Sequence)) or check_issubclass(get_origin(type_), (Mapping, Sequence))
```

### Comparing `khemia-0.1.0/khemia/utils.py` & `khemia-0.1.1/khemia/utils.py`

 * *Files identical despite different names*

### Comparing `khemia-0.1.0/pyproject.toml` & `khemia-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "khemia"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python tools for typing and memory cache."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "khemia" }]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 typing-extensions = "^4.8.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.7"
+pre-commit = "^3.7.0"
 
 [tool.ruff]
 select = [
     "E",
     "W",   # pycodestyle
     "F",   # pyflakes
     "UP",  # pyupgrade
@@ -31,15 +32,15 @@
     "ISC", # flake8-implicit-str-concat
     "C4",  # flake8-comprehensions
     "COM", # flake8-commas
     "B",   # flake8-bugbear
 ]
 ignore = ["E402", "B008", "F403", "F405", "B005"]
 line-length = 120
-target-version = "py38"
+target-version = "py39"
 ignore-init-module-imports = true
 
 [tool.ruff.isort]
 force-sort-within-sections = true
 extra-standard-library = ["typing_extensions"]
 force-wrap-aliases = true
 combine-as-imports = true
```

### Comparing `khemia-0.1.0/PKG-INFO` & `khemia-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: khemia
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python tools for typing and memory cache.
 License: MIT
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Description-Content-Type: text/markdown
```

