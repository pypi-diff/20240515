# Comparing `tmp/odex-0.0.1.tar.gz` & `tmp/odex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odex-0.0.1.tar", max compression
+gzip compressed data, was "odex-0.0.2.tar", max compression
```

## Comparing `odex-0.0.1.tar` & `odex-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1062 2024-05-14 21:49:28.493104 odex-0.0.1/LICENSE
--rw-r--r--   0        0        0      962 2024-05-14 21:49:28.493104 odex-0.0.1/README.md
--rw-r--r--   0        0        0      633 2024-05-14 21:49:28.493104 odex-0.0.1/odex/__init__.py
--rw-r--r--   0        0        0     7055 2024-05-14 21:49:28.493104 odex-0.0.1/odex/condition.py
--rw-r--r--   0        0        0      701 2024-05-14 21:49:28.493104 odex-0.0.1/odex/container.py
--rw-r--r--   0        0        0      829 2024-05-14 21:49:28.493104 odex-0.0.1/odex/context.py
--rw-r--r--   0        0        0     3530 2024-05-14 21:49:28.493104 odex-0.0.1/odex/index.py
--rw-r--r--   0        0        0     4528 2024-05-14 21:49:28.493104 odex-0.0.1/odex/optimize.py
--rw-r--r--   0        0        0     4340 2024-05-14 21:49:28.493104 odex-0.0.1/odex/parse.py
--rw-r--r--   0        0        0     3467 2024-05-14 21:49:28.493104 odex-0.0.1/odex/plan.py
--rw-r--r--   0        0        0     7698 2024-05-14 21:49:28.493104 odex-0.0.1/odex/set.py
--rw-r--r--   0        0        0        0 2024-05-14 21:49:28.493104 odex-0.0.1/odex/utils.py
--rw-r--r--   0        0        0      600 2024-05-14 21:49:28.493104 odex-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 odex-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-14 22:45:34.863882 odex-0.0.2/LICENSE
+-rw-r--r--   0        0        0      962 2024-05-14 22:45:34.863882 odex-0.0.2/README.md
+-rw-r--r--   0        0        0      633 2024-05-14 22:45:34.863882 odex-0.0.2/odex/__init__.py
+-rw-r--r--   0        0        0     7055 2024-05-14 22:45:34.863882 odex-0.0.2/odex/condition.py
+-rw-r--r--   0        0        0      701 2024-05-14 22:45:34.863882 odex-0.0.2/odex/container.py
+-rw-r--r--   0        0        0      829 2024-05-14 22:45:34.863882 odex-0.0.2/odex/context.py
+-rw-r--r--   0        0        0     3530 2024-05-14 22:45:34.863882 odex-0.0.2/odex/index.py
+-rw-r--r--   0        0        0     4528 2024-05-14 22:45:34.863882 odex-0.0.2/odex/optimize.py
+-rw-r--r--   0        0        0     4439 2024-05-14 22:45:34.863882 odex-0.0.2/odex/parse.py
+-rw-r--r--   0        0        0     3467 2024-05-14 22:45:34.863882 odex-0.0.2/odex/plan.py
+-rw-r--r--   0        0        0     7698 2024-05-14 22:45:34.863882 odex-0.0.2/odex/set.py
+-rw-r--r--   0        0        0      600 2024-05-14 22:45:34.863882 odex-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 odex-0.0.2/PKG-INFO
```

### Comparing `odex-0.0.1/LICENSE` & `odex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/README.md` & `odex-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/odex/__init__.py` & `odex-0.0.2/odex/__init__.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/odex/condition.py` & `odex-0.0.2/odex/condition.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/odex/container.py` & `odex-0.0.2/odex/container.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/odex/context.py` & `odex-0.0.2/odex/context.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/odex/index.py` & `odex-0.0.2/odex/index.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/odex/optimize.py` & `odex-0.0.2/odex/optimize.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/odex/parse.py` & `odex-0.0.2/odex/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
             exp.NEQ: lambda e: self._convert_binary(cond.Ne, e),
             exp.And: lambda e: self._convert_binary(cond.And, e),
             exp.Or: lambda e: self._convert_binary(cond.Or, e),
             exp.Not: lambda e: self._convert_unary(cond.Not, e),
             exp.Literal: self._convert_literal,
             exp.Column: self._convert_column,
             exp.In: self._convert_in,
+            exp.Null: lambda e: Literal(None),
+            exp.Boolean: lambda e: Literal(e.this),
         }
 
     def convert(self, expression: exp.Expression) -> Condition:
         converter = self.converters.get(expression.__class__)
         if not converter:
             raise ValueError(f"Unsupported sqlglot Expression: {expression.__class__}")
         return converter(expression)
```

### Comparing `odex-0.0.1/odex/plan.py` & `odex-0.0.2/odex/plan.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/odex/set.py` & `odex-0.0.2/odex/set.py`

 * *Files identical despite different names*

### Comparing `odex-0.0.1/pyproject.toml` & `odex-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odex"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python object index for fast, declarative retrieval"
 authors = ["Barak Alon"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/barakalon/odex"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `odex-0.0.1/PKG-INFO` & `odex-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odex
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python object index for fast, declarative retrieval
 Home-page: https://github.com/barakalon/odex
 License: MIT
 Author: Barak Alon
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

