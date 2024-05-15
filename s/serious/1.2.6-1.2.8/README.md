# Comparing `tmp/serious-1.2.6.tar.gz` & `tmp/serious-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serious-1.2.6.tar", last modified: Mon Dec  4 14:38:40 2023, max compression
+gzip compressed data, was "serious-1.2.8.tar", last modified: Wed May 15 17:28:03 2024, max compression
```

## Comparing `serious-1.2.6.tar` & `serious-1.2.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-04 14:38:40.176859 serious-1.2.6/
--rw-r--r--   0 vsts      (1001) docker     (127)     1069 2023-12-04 14:38:15.000000 serious-1.2.6/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     6866 2023-12-04 14:38:40.176859 serious-1.2.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5701 2023-12-04 14:38:15.000000 serious-1.2.6/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-04 14:38:40.172858 serious-1.2.6/serious/
--rw-r--r--   0 vsts      (1001) docker     (127)      773 2023-12-04 14:38:15.000000 serious-1.2.6/serious/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      389 2023-12-04 14:38:15.000000 serious-1.2.6/serious/checks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7650 2023-12-04 14:38:15.000000 serious-1.2.6/serious/descriptors.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-04 14:38:40.172858 serious-1.2.6/serious/dict/
--rw-r--r--   0 vsts      (1001) docker     (127)      159 2023-12-04 14:38:15.000000 serious-1.2.6/serious/dict/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4052 2023-12-04 14:38:15.000000 serious-1.2.6/serious/dict/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6218 2023-12-04 14:38:15.000000 serious-1.2.6/serious/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-04 14:38:40.172858 serious-1.2.6/serious/json/
--rw-r--r--   0 vsts      (1001) docker     (127)      131 2023-12-04 14:38:15.000000 serious-1.2.6/serious/json/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1443 2023-12-04 14:38:15.000000 serious-1.2.6/serious/json/checks.py
--rw-r--r--   0 vsts      (1001) docker     (127)      235 2023-12-04 14:38:15.000000 serious-1.2.6/serious/json/errors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5702 2023-12-04 14:38:15.000000 serious-1.2.6/serious/json/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      558 2023-12-04 14:38:15.000000 serious-1.2.6/serious/json/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-04 14:38:15.000000 serious-1.2.6/serious/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-04 14:38:40.176859 serious-1.2.6/serious/serialization/
--rw-r--r--   0 vsts      (1001) docker     (127)     1416 2023-12-04 14:38:15.000000 serious-1.2.6/serious/serialization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1411 2023-12-04 14:38:15.000000 serious-1.2.6/serious/serialization/check_immutable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3052 2023-12-04 14:38:15.000000 serious-1.2.6/serious/serialization/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24540 2023-12-04 14:38:15.000000 serious-1.2.6/serious/serialization/field_serializers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1229 2023-12-04 14:38:15.000000 serious-1.2.6/serious/serialization/key_mapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9493 2023-12-04 14:38:15.000000 serious-1.2.6/serious/serialization/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1844 2023-12-04 14:38:15.000000 serious-1.2.6/serious/serialization/serializer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      790 2023-12-04 14:38:15.000000 serious-1.2.6/serious/test_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6969 2023-12-04 14:38:15.000000 serious-1.2.6/serious/types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      294 2023-12-04 14:38:15.000000 serious-1.2.6/serious/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1617 2023-12-04 14:38:15.000000 serious-1.2.6/serious/validation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-04 14:38:40.172858 serious-1.2.6/serious.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     6866 2023-12-04 14:38:40.000000 serious-1.2.6/serious.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      770 2023-12-04 14:38:40.000000 serious-1.2.6/serious.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-04 14:38:40.000000 serious-1.2.6/serious.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-04 14:38:40.000000 serious-1.2.6/serious.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)        8 2023-12-04 14:38:40.000000 serious-1.2.6/serious.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-12-04 14:38:40.176859 serious-1.2.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1573 2023-12-04 14:38:15.000000 serious-1.2.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 17:28:03.263974 serious-1.2.8/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1069 2024-05-15 17:27:40.000000 serious-1.2.8/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     6866 2024-05-15 17:28:03.263974 serious-1.2.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5701 2024-05-15 17:27:40.000000 serious-1.2.8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 17:28:03.259974 serious-1.2.8/serious/
+-rw-r--r--   0 vsts      (1001) docker     (127)      773 2024-05-15 17:27:40.000000 serious-1.2.8/serious/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      389 2024-05-15 17:27:40.000000 serious-1.2.8/serious/checks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7650 2024-05-15 17:27:40.000000 serious-1.2.8/serious/descriptors.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 17:28:03.259974 serious-1.2.8/serious/dict/
+-rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-05-15 17:27:40.000000 serious-1.2.8/serious/dict/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4052 2024-05-15 17:27:40.000000 serious-1.2.8/serious/dict/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6196 2024-05-15 17:27:40.000000 serious-1.2.8/serious/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 17:28:03.259974 serious-1.2.8/serious/json/
+-rw-r--r--   0 vsts      (1001) docker     (127)      131 2024-05-15 17:27:40.000000 serious-1.2.8/serious/json/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1443 2024-05-15 17:27:40.000000 serious-1.2.8/serious/json/checks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      235 2024-05-15 17:27:40.000000 serious-1.2.8/serious/json/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5702 2024-05-15 17:27:40.000000 serious-1.2.8/serious/json/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-05-15 17:27:40.000000 serious-1.2.8/serious/json/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-15 17:27:40.000000 serious-1.2.8/serious/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 17:28:03.263974 serious-1.2.8/serious/serialization/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1416 2024-05-15 17:27:40.000000 serious-1.2.8/serious/serialization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1411 2024-05-15 17:27:40.000000 serious-1.2.8/serious/serialization/check_immutable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2808 2024-05-15 17:27:40.000000 serious-1.2.8/serious/serialization/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24540 2024-05-15 17:27:40.000000 serious-1.2.8/serious/serialization/field_serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-05-15 17:27:40.000000 serious-1.2.8/serious/serialization/key_mapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9493 2024-05-15 17:27:40.000000 serious-1.2.8/serious/serialization/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1844 2024-05-15 17:27:40.000000 serious-1.2.8/serious/serialization/serializer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-15 17:27:40.000000 serious-1.2.8/serious/test_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6969 2024-05-15 17:27:40.000000 serious-1.2.8/serious/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-05-15 17:27:40.000000 serious-1.2.8/serious/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1617 2024-05-15 17:27:40.000000 serious-1.2.8/serious/validation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-15 17:28:03.259974 serious-1.2.8/serious.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6866 2024-05-15 17:28:03.000000 serious-1.2.8/serious.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      770 2024-05-15 17:28:03.000000 serious-1.2.8/serious.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-15 17:28:03.000000 serious-1.2.8/serious.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-15 17:28:03.000000 serious-1.2.8/serious.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-05-15 17:28:03.000000 serious-1.2.8/serious.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-15 17:28:03.263974 serious-1.2.8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1573 2024-05-15 17:27:40.000000 serious-1.2.8/setup.py
```

### Comparing `serious-1.2.6/LICENSE` & `serious-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/PKG-INFO` & `serious-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serious
-Version: 1.2.6
+Version: 1.2.8
 Summary: Easily serialize dataclasses to and from JSON
 Home-page: https://github.com/mdrachuk/serious
 Author: mdrachuk
 Author-email: misha@drach.uk
 License: MIT
 Project-URL: Pipelines, https://dev.azure.com/misha-drachuk/serious
 Project-URL: Source, https://github.com/mdrachuk/serious/
```

### Comparing `serious-1.2.6/README.md` & `serious-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/__init__.py` & `serious-1.2.8/serious/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 from .dict import DictModel
 from .errors import ModelError, ValidationError, LoadError, DumpError
 from .json import JsonModel
 from .types import Timestamp, Email, FrozenList, FrozenDict
 from .validation import validate
 
-__version__ = '1.2.6'
+__version__ = '1.2.8'
```

### Comparing `serious-1.2.6/serious/descriptors.py` & `serious-1.2.8/serious/descriptors.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/dict/model.py` & `serious-1.2.8/serious/dict/model.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/errors.py` & `serious-1.2.8/serious/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.cls = cls
         self._path = self.__parse_stack(serializer_stack)
 
     @staticmethod
     def __parse_stack(serializer_stack: Collection[SerializationStep]) -> str:
         if len(serializer_stack) == 0:
             return ''
-        return ''.join(step.name for step in serializer_stack)[1:]
+        return ''.join(serializer_stack)[1:]
 
     @property
     def message(self):
         return f'Error during serialization of "{self.cls}"'
 
     def __str__(self):
         exc_type = super().__str__()
```

### Comparing `serious-1.2.6/serious/json/checks.py` & `serious-1.2.8/serious/json/checks.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/json/model.py` & `serious-1.2.8/serious/json/model.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/json/utils.py` & `serious-1.2.8/serious/json/utils.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/serialization/__init__.py` & `serious-1.2.8/serious/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/serialization/check_immutable.py` & `serious-1.2.8/serious/serialization/check_immutable.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/serialization/context.py` & `serious-1.2.8/serious/serialization/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 """Loading/dumping context holding the current execution stack, calling serializers and validators."""
 from __future__ import annotations
 
 __all__ = ['Context', 'Loading', 'Dumping']
 
 from abc import ABC, abstractmethod
-from contextlib import contextmanager
-from typing import List, Any, NamedTuple, TypeVar
+from collections import deque
+from typing import Any, TypeVar, Deque
 
 from serious.serialization.serializer import Serializer
 from serious.types import FrozenList
 from serious.validation import validate
 
 M = TypeVar('M')  # Python model value
 S = TypeVar('S')  # Serialized value
 
+SerializationStep = str
+
 
 class Context(ABC):
     """An abstract base class for the serialization context.
 
     Serialization context is created when executing `SeriousModel` load or dump and is passed inside
     all nested serializers.
 
     All of serializers are called via context to include them in stack and to perform
     all the necessary validation and processing
     """
-
-    def __init__(self):
-        self._steps: List[SerializationStep] = list()
-
-    @contextmanager
-    def _entering(self, step: str, serializer: Serializer):
-        self._steps.append(SerializationStep(step, serializer))
-        yield
-        self._steps.pop()
+    _steps: Deque[SerializationStep]
 
     @property
     def stack(self) -> FrozenList[SerializationStep]:
         """The stack is included in errors, mentioning the fields, array indexes, dictionary keys, etc."""
         return FrozenList(self._steps)
 
     def __repr__(self):
-        return f"<Context: {'.'.join([step.name for step in self._steps])}>"
+        return f"<Context: {'.'.join(self._steps)}>"
 
     @abstractmethod
     def run(self, step: str, serializer: Serializer, value: Any) -> Any:
         """Execute serializer in context.
 
         Implementations:
         - includes the current step in the stack,
@@ -59,33 +53,34 @@
 
 
 class Loading(Context):
     """Context used during **load** operations."""
 
     def __init__(self, *, validating: bool):
         super().__init__()
+        self._steps = deque()
         self.validating = validating
 
     def run(self, step: str, serializer: Serializer[M, S], value: S) -> M:
-        with self._entering(step, serializer):
-            result = serializer.load(value, self)
-            if self.validating:
-                validate(result)
-            return result
+        self._steps.append(step)
+        result = serializer.load(value, self)
+        if self.validating:
+            validate(result)
+        self._steps.pop()
+        return result
 
 
 class Dumping(Context):
     """Context used during **dump** operations."""
+
     def __init__(self, *, validating: bool):
         super().__init__()
+        self._steps = deque()
         self.validating = validating
 
     def run(self, step: str, serializer: Serializer[M, S], o: M) -> S:
-        with self._entering(step, serializer):
-            if self.validating:
-                validate(o)
-            return serializer.dump(o, self)
-
-
-class SerializationStep(NamedTuple):
-    name: str
-    serializer: Serializer
+        self._steps.append(step)
+        if self.validating:
+            validate(o)
+        result = serializer.dump(o, self)
+        self._steps.pop()
+        return result
```

### Comparing `serious-1.2.6/serious/serialization/field_serializers.py` & `serious-1.2.8/serious/serialization/field_serializers.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/serialization/key_mapper.py` & `serious-1.2.8/serious/serialization/key_mapper.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/serialization/model.py` & `serious-1.2.8/serious/serialization/model.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/serialization/serializer.py` & `serious-1.2.8/serious/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/test_utils.py` & `serious-1.2.8/serious/test_utils.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/types.py` & `serious-1.2.8/serious/types.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious/validation.py` & `serious-1.2.8/serious/validation.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/serious.egg-info/PKG-INFO` & `serious-1.2.8/serious.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serious
-Version: 1.2.6
+Version: 1.2.8
 Summary: Easily serialize dataclasses to and from JSON
 Home-page: https://github.com/mdrachuk/serious
 Author: mdrachuk
 Author-email: misha@drach.uk
 License: MIT
 Project-URL: Pipelines, https://dev.azure.com/misha-drachuk/serious
 Project-URL: Source, https://github.com/mdrachuk/serious/
```

### Comparing `serious-1.2.6/serious.egg-info/SOURCES.txt` & `serious-1.2.8/serious.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serious-1.2.6/setup.py` & `serious-1.2.8/setup.py`

 * *Files identical despite different names*

