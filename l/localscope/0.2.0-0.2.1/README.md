# Comparing `tmp/localscope-0.2.0.tar.gz` & `tmp/localscope-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localscope-0.2.0.tar", last modified: Sat Feb 17 03:06:44 2024, max compression
+gzip compressed data, was "localscope-0.2.1.tar", last modified: Wed May 15 13:40:18 2024, max compression
```

## Comparing `localscope-0.2.0.tar` & `localscope-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 03:06:44.232693 localscope-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-17 03:06:20.000000 localscope-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-17 03:06:44.232693 localscope-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-02-17 03:06:20.000000 localscope-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 03:06:44.228693 localscope-0.2.0/localscope/
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-02-17 03:06:20.000000 localscope-0.2.0/localscope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 03:06:44.232693 localscope-0.2.0/localscope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-17 03:06:44.000000 localscope-0.2.0/localscope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-17 03:06:44.000000 localscope-0.2.0/localscope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 03:06:44.000000 localscope-0.2.0/localscope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-17 03:06:44.000000 localscope-0.2.0/localscope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-17 03:06:20.000000 localscope-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-17 03:06:44.232693 localscope-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 03:06:44.232693 localscope-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-02-17 03:06:20.000000 localscope-0.2.0/tests/test_localscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:18.014648 localscope-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 13:39:51.000000 localscope-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 13:40:18.014648 localscope-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-15 13:39:51.000000 localscope-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:18.014648 localscope-0.2.1/localscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-15 13:39:51.000000 localscope-0.2.1/localscope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:18.014648 localscope-0.2.1/localscope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 13:40:18.000000 localscope-0.2.1/localscope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 13:40:18.000000 localscope-0.2.1/localscope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:40:18.000000 localscope-0.2.1/localscope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 13:40:18.000000 localscope-0.2.1/localscope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-15 13:39:51.000000 localscope-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 13:40:18.014648 localscope-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:18.014648 localscope-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-15 13:39:51.000000 localscope-0.2.1/tests/test_localscope.py
```

### Comparing `localscope-0.2.0/LICENSE` & `localscope-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `localscope-0.2.0/PKG-INFO` & `localscope-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localscope
-Version: 0.2.0
+Version: 0.2.1
 Summary: Restrict the scope of functions for reproducible code execution and peace of mind.
 Author: Till Hoffmann
 Project-URL: Documentation, https://localscope.readthedocs.io
 Project-URL: Repository, https://github.com/tillahoffmann/localscope.git
 Project-URL: Issues, https://github.com/tillahoffmann/localscope/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `localscope-0.2.0/README.rst` & `localscope-0.2.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
    >>> a = 'hello world'
    >>> @localscope
    ... def print_a():
    ...     print(a)
    Traceback (most recent call last):
      ...
-   localscope.LocalscopeException: `a` is not a permitted global (file "...", line 1, in print_a)
+   localscope.LocalscopeException: `a` is not a permitted global (file "...",
+      line 1, in print_a)
 
 Motivation and detailed example
 -------------------------------
 
 Suppose you are evaluating the mean squared error between two lists of numbers, including a scale factor ``sigma``.
 
 .. doctest::
@@ -61,13 +62,14 @@
 
    >>> from localscope import localscope
    >>> @localscope
    ... def evaluate_mse(xs, ys):  # missing argument sigma
    ...     return sum(((x - y) / sigma) ** 2 for x, y in zip(xs, ys))
    Traceback (most recent call last):
      ...
-   localscope.LocalscopeException: `sigma` is not a permitted global (file "...", line 3, in <genexpr>)
+   localscope.LocalscopeException: `sigma` is not a permitted global (file "...",
+      line 3, in <genexpr>)
 
 Interface
 ---------
 
 .. autofunction:: localscope.localscope
```

### Comparing `localscope-0.2.0/localscope/__init__.py` & `localscope-0.2.1/localscope/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import builtins
 import dis
 import functools as ft
 import inspect
 import logging
 import types
-from typing import Any, Callable, Dict, Optional, Set, Union
+from typing import Any, Callable, Dict, Iterable, Optional, Set, Union
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def localscope(
     func: Optional[Union[types.FunctionType, types.CodeType]] = None,
     *,
     predicate: Optional[Callable] = None,
-    allowed: Optional[Set[str]] = None,
+    allowed: Optional[Union[Iterable[str], str]] = None,
     allow_closure: bool = False,
 ):
     """
     Restrict the scope of a callable to local variables to avoid unintentional
     information ingress.
 
     Args:
@@ -40,16 +40,16 @@
         ... def print_a():
         ...     print(a)
         Traceback (most recent call last):
         ...
         localscope.LocalscopeException: `a` is not a permitted global (file "...",
             line 1, in print_a)
 
-        The scope of a function can be extended by providing a list of allowed
-        exceptions.
+        The scope of a function can be extended by providing an iterable of allowed
+        variable names or a string of space-separated allowed variable names.
 
         >>> a = 'hello world'
         >>> @localscope(allowed=['a'])
         ... def print_a():
         ...     print(a)
         >>> print_a()
         hello world
@@ -83,14 +83,16 @@
         blocks) at the time of declaration because static analysis has a minimal impact
         on performance and it is easier to implement.
     """
     # Set defaults and construct partial if the callable has not yet been provided for
     # parameterized decorators, e.g., @localscope(allowed={"foo", "bar"}). This is a
     # thin wrapper around the actual implementation `_localscope`. The wrapper
     # reconstructs an informative traceback.
+    if isinstance(allowed, str):
+        allowed = allowed.split()
     allowed = set(allowed) if allowed else set()
     predicate = predicate or inspect.ismodule
     if not func:
         return ft.partial(
             localscope,
             allow_closure=allow_closure,
             allowed=allowed,
```

### Comparing `localscope-0.2.0/localscope.egg-info/PKG-INFO` & `localscope-0.2.1/localscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localscope
-Version: 0.2.0
+Version: 0.2.1
 Summary: Restrict the scope of functions for reproducible code execution and peace of mind.
 Author: Till Hoffmann
 Project-URL: Documentation, https://localscope.readthedocs.io
 Project-URL: Repository, https://github.com/tillahoffmann/localscope.git
 Project-URL: Issues, https://github.com/tillahoffmann/localscope/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `localscope-0.2.0/pyproject.toml` & `localscope-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "localscope"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.8"
 authors = [
     {name = "Till Hoffmann"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `localscope-0.2.0/tests/test_localscope.py` & `localscope-0.2.1/tests/test_localscope.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,14 +51,20 @@
 def test_allowed():
     @localscope(allowed=["allowed_global"])
     def return_allowed_global():
         return allowed_global
 
     assert return_allowed_global() == allowed_global
 
+    @localscope(allowed="allowed_global integer_global")
+    def return_allowed_global():
+        return allowed_global, integer_global
+
+    assert return_allowed_global() == (allowed_global, integer_global)
+
 
 def test_closure():
     def wrapper():
         forbidden_closure = uuid.uuid4()
 
         @localscope
         def return_forbidden_closure():
@@ -198,7 +204,23 @@
 def test_local_deref():
     @localscope
     def identity(x):
         return x
         lambda: x
 
     assert identity(42) == 42
+
+
+def test_method():
+    x = 1
+
+    with pytest.raises(LocalscopeException, match="`x` is not a permitted"):
+
+        class MyClass:
+            @localscope
+            def my_func(self, a):
+                return a + x
+
+    class MyOtherClass:
+        @localscope(allowed=["x"])
+        def my_func(self, a):
+            return a + x
```

