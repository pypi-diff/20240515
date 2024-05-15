# Comparing `tmp/polars_expr_transformer-0.1.3.3.tar.gz` & `tmp/polars_expr_transformer-0.1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_expr_transformer-0.1.3.3.tar", last modified: Wed May 15 11:27:56 2024, max compression
+gzip compressed data, was "polars_expr_transformer-0.1.3.4.tar", last modified: Wed May 15 15:59:37 2024, max compression
```

## Comparing `polars_expr_transformer-0.1.3.3.tar` & `polars_expr_transformer-0.1.3.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.766578 polars_expr_transformer-0.1.3.3/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3.3/LICENSE
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 11:27:56.766385 polars_expr_transformer-0.1.3.3/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3443 2024-05-15 11:01:56.000000 polars_expr_transformer-0.1.3.3/README.md
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.761077 polars_expr_transformer-0.1.3.3/polars_expr_transformer/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/__init__.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.762276 polars_expr_transformer-0.1.3.3/polars_expr_transformer/configs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       14 2024-05-15 08:14:06.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/configs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/configs/settings.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.763674 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8837 2024-05-15 09:39:41.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/date_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4219 2024-05-15 09:34:53.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/logic_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1165 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/math_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/special_funcs.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     7550 2024-05-15 10:37:45.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/string_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      333 2024-05-15 08:57:32.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/utils.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1980 2024-05-14 17:53:37.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/function_overview.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/main_module.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.765106 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6667 2024-05-15 09:30:09.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/models.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1512 2024-05-15 08:26:49.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/polars_expr_transformer.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/preprocess.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4805 2024-05-15 08:27:45.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/process_inline.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/standardize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3230 2024-05-15 11:26:35.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/tokenize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4977 2024-05-15 10:32:09.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/tree.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/schemas.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.765545 polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/settings.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/utils.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.765982 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/requires.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/top_level.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-15 11:27:56.766619 polars_expr_transformer-0.1.3.3/setup.cfg
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1836 2024-05-15 11:27:50.000000 polars_expr_transformer-0.1.3.3/setup.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.765787 polars_expr_transformer-0.1.3.3/tests/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     9690 2024-05-15 11:27:32.000000 polars_expr_transformer-0.1.3.3/tests/test.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 15:59:37.479180 polars_expr_transformer-0.1.3.4/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3.4/LICENSE
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 15:59:37.479007 polars_expr_transformer-0.1.3.4/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3443 2024-05-15 11:01:56.000000 polars_expr_transformer-0.1.3.4/README.md
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 15:59:37.473882 polars_expr_transformer-0.1.3.4/polars_expr_transformer/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/__init__.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 15:59:37.474912 polars_expr_transformer-0.1.3.4/polars_expr_transformer/configs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       14 2024-05-15 08:14:06.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/configs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/configs/settings.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 15:59:37.476313 polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8837 2024-05-15 09:39:41.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/date_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4123 2024-05-15 13:37:30.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/logic_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5704 2024-05-15 13:44:12.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/math_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/special_funcs.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    10141 2024-05-15 13:48:08.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/string_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      333 2024-05-15 08:57:32.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/utils.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1980 2024-05-14 17:53:37.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/function_overview.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/main_module.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 15:59:37.477783 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6667 2024-05-15 09:30:09.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/models.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1490 2024-05-15 13:19:43.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/polars_expr_transformer.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/preprocess.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4805 2024-05-15 08:27:45.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/process_inline.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/standardize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3217 2024-05-15 13:22:49.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/tokenize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4977 2024-05-15 10:32:09.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/tree.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/schemas.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 15:59:37.478214 polars_expr_transformer-0.1.3.4/polars_expr_transformer/utils/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/utils/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/utils/settings.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer/utils/utils.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 15:59:37.478644 polars_expr_transformer-0.1.3.4/polars_expr_transformer.egg-info/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 15:59:37.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-15 15:59:37.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-15 15:59:37.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-15 15:59:37.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer.egg-info/requires.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-15 15:59:37.000000 polars_expr_transformer-0.1.3.4/polars_expr_transformer.egg-info/top_level.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-15 15:59:37.479229 polars_expr_transformer-0.1.3.4/setup.cfg
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1836 2024-05-15 15:59:29.000000 polars_expr_transformer-0.1.3.4/setup.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 15:59:37.478458 polars_expr_transformer-0.1.3.4/tests/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    14285 2024-05-15 15:41:29.000000 polars_expr_transformer-0.1.3.4/tests/test.py
```

### Comparing `polars_expr_transformer-0.1.3.3/LICENSE` & `polars_expr_transformer-0.1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/PKG-INFO` & `polars_expr_transformer-0.1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_expr_transformer
-Version: 0.1.3.3
+Version: 0.1.3.4
 Summary: Transform string-based expressions into Polars DataFrame operations
 Home-page: https://github.com/edwardvaneechoud/polars_expr_transformer
 Author: Edward van Eehoud
 Author-email: evaneechoudl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polars_expr_transformer-0.1.3.3/README.md` & `polars_expr_transformer-0.1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/configs/settings.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/configs/settings.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/date_functions.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/date_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/logic_functions.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/logic_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,53 +5,53 @@
 
 
 def equals(s: Any, t: Any) -> pl.Expr:
     """
     Check if two expressions or values are equal.
 
     Parameters:
-    - s (Any): The first expression or value to compare. Can be a FlowFile expression or any other value.
-    - t (Any): The second expression or value to compare. Can be a FlowFile expression or any other value.
+    - s (Any): The first expression or value to compare. Can be a pl expression or any other value.
+    - t (Any): The second expression or value to compare. Can be a pl expression or any other value.
 
     Returns:
-    - pl.Expr: A FlowFile expression representing the equality of `s` and `t`.
+    - pl.Expr: A pl expression representing the equality of `s` and `t`.
 
-    Note: If `s` or `t` is not a FlowFile expression, it will be converted into one.
+    Note: If `s` or `t` is not a pl expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_col(s)
     t = t if is_polars_expr(t) else create_fix_col(t)
     return s.eq(t)
 
 
 def is_empty(s: pl.Expr) -> pl.Expr:
     """
     Check if a given expression is empty.
 
     Parameters:
-    - s (pl.Expr): The expression to check. Must be a FlowFile expression.
+    - s (pl.Expr): The expression to check. Must be a pl expression.
 
     Returns:
-    - pl.Expr: A FlowFile expression representing whether `s` is empty.
+    - pl.Expr: A pl expression representing whether `s` is empty.
 
-    Note: If `s` is not a FlowFile expression, a ValueError will be raised.
+    Note: If `s` is not a pl expression, a ValueError will be raised.
     """
     return s.is_null()
 
 
 def is_not_empty(s: pl.Expr) -> pl.Expr:
     """
     Check if a given expression is empty.
 
     Parameters:
-    - s (pl.Expr): The expression to check. Must be a FlowFile expression.
+    - s (pl.Expr): The expression to check. Must be a pl expression.
 
     Returns:
-    - pl.Expr: A FlowFile expression representing whether `s` is empty.
+    - pl.Expr: A pl expression representing whether `s` is empty.
 
-    Note: If `s` is not a FlowFile expression, a ValueError will be raised.
+    Note: If `s` is not a pl expression, a ValueError will be raised.
     """
     return s.is_not_null()
 
 
 def does_not_equal(s: Any, t: Any):
     s = s if is_polars_expr(s) else create_fix_col(s)
     t = t if is_polars_expr(t) else create_fix_col(t)
@@ -59,37 +59,37 @@
 
 
 def _not(s: Any) -> pl.Expr:
     """
     Negate a given expression.
 
     Parameters:
-    - s (pl.Expr): The expression to negate. Must be a FlowFile expression.
+    - s (pl.Expr): The expression to negate. Must be a pl expression.
 
     Returns:
-    - pl.Expr: A FlowFile expression representing the negation of `s`.
+    - pl.Expr: A pl expression representing the negation of `s`.
 
-    Note: If `s` is not a FlowFile expression, a ValueError will be raised.
+    Note: If `s` is not a pl expression, a ValueError will be raised.
     """
     if not is_polars_expr(s):
         s = pl.lit(s)
     return pl.Expr.not_(s)
 
 
 def is_string(val: Any) -> pl.Expr:
     """
     Check if a given expression or value is a string.
 
     Parameters:
-    - val (Any): The expression or value to check. Can be a FlowFile expression or any other value.
+    - val (Any): The expression or value to check. Can be a pl expression or any other value.
 
     Returns:
-    - pl.Expr: A FlowFile expression representing whether `val` is a string.
+    - pl.Expr: A pl expression representing whether `val` is a string.
 
-    Note: If `val` is a FlowFile expression, its dtype will be checked. Otherwise, Python's isinstance will be used.
+    Note: If `val` is a pl expression, its dtype will be checked. Otherwise, Python's isinstance will be used.
     """
     if is_polars_expr(val):
         dtype = pl.select(val).dtypes[0]
         return pl.lit(dtype.is_(pl.Utf8))
     return pl.lit(isinstance(val, str))
```

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/string_functions.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/funcs/string_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
 def __left(row: Dict):
     v, l = row.values()
     if v is not None:
         return v[:l]
     return None
 
+
 def left(column: PlStringType, length: pl.Expr | int) -> pl.Expr:
     """
     Extracts a substring from a column or string, starting from the beginning.
 
     Parameters:
     - column: The column or string from which to extract the substring.
     - length: The length of the substring to extract.
@@ -187,52 +188,136 @@
 
 
 def to_date(s: PlStringType, date_format: str = "%Y-%m-%d") -> pl.Expr:
     """
     Convert a string to a date.
 
     Parameters:
-    - s (Any): The string to convert to a date. Can be a FlowFile expression or any other value.
+    - s (Any): The string to convert to a date. Can be a pl expression or any other value.
     - format (str): The format of the date string. Default is "%Y-%m-%d".
 
     Returns:
-    - pl.Expr: A FlowFile expression representing the converted date.
+    - pl.Expr: A pl expression representing the converted date.
 
-    Note: If `s` is not a FlowFile expression, it will be converted into one.
+    Note: If `s` is not a pl expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_col(s)
     return s.str.to_date(date_format, strict=False)
 
 
 def to_datetime(s: PlStringType, date_format: str = "%Y-%m-%d %H:%M:%S") -> pl.Expr:
     """
     Convert a string to a datetime.
 
     Parameters:
-    - s (Any): The string to convert to a datetime. Can be a FlowFile expression or any other value.
+    - s (Any): The string to convert to a datetime. Can be a pl expression or any other value.
     - format (str): The format of the datetime string. Default is "%Y-%m-%d %H:%M:%S".
 
     Returns:
-    - pl.Expr: A FlowFile expression representing the converted datetime.
+    - pl.Expr: A pl expression representing the converted datetime.
 
-    Note: If `s` is not a FlowFile expression, it will be converted into one.
+    Note: If `s` is not a pl expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_col(s)
     return s.str.to_datetime(date_format, strict=False)
 
 
 def find_position(s: PlStringType, sub: PlStringType) -> pl.Expr:
     """
     Find the position of a substring within a string.
 
     Parameters:
-    - s (Any): The string in which to find the position of the substring. Can be a FlowFile expression or any other value.
-    - sub (Any): The substring to find the position of. Can be a FlowFile expression or any other value.
+    - s (Any): The string in which to find the position of the substring. Can be a pl expression or any other value.
+    - sub (Any): The substring to find the position of. Can be a pl expression or any other value.
 
     Returns:
-    - pl.Expr: A FlowFile expression representing the position of the substring within the string.
+    - pl.Expr: A pl expression representing the position of the substring within the string.
 
-    Note: If `s` or `sub` is not a FlowFile expression, it will be converted into one.
+    Note: If `s` or `sub` is not a pl expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_col(s)
     sub = sub if is_polars_expr(sub) else create_fix_col(sub)
-    return s.str(sub)
+    return s.str(sub)
+
+
+def pad_left(s: PlStringType, _length: int, pad: str = " ") -> pl.Expr:
+    """
+    Pad a string on the left side with a specified character to reach a certain length.
+
+    Parameters:
+    - s (Any): The string to pad. Can be a pl expression or any other value.
+    - length (int): The desired length of the padded string.
+    - pad (str): The character to use for padding. Default is " ".
+
+    Returns:
+    - pl.Expr: A pl expression representing the padded string.
+
+    Note: If `s` is not a pl expression, it will be converted into one.
+    """
+    s = s if is_polars_expr(s) else create_fix_col(s)
+    return s.str.pad_start(_length, pad)
+
+
+def pad_right(s: PlStringType, _length: int, pad: str = " ") -> pl.Expr:
+    """
+    Pad a string on the right side with a specified character to reach a certain length.
+
+    Parameters:
+    - s (Any): The string to pad. Can be a pl expression or any other value.
+    - length (int): The desired length of the padded string.
+    - pad (str): The character to use for padding. Default is " ".
+
+    Returns:
+    - pl.Expr: A pl expression representing the padded string.
+
+    Note: If `s` is not a pl expression, it will be converted into one.
+    """
+    s = s if is_polars_expr(s) else create_fix_col(s)
+    return s.str.pad_end(_length, pad)
+
+
+def trim(s: PlStringType) -> pl.Expr:
+    """
+    Remove leading and trailing whitespace from a string.
+
+    Parameters:
+    - s (Any): The string to trim. Can be a pl expression or any other value.
+
+    Returns:
+    - pl.Expr: A pl expression representing the trimmed string.
+
+    Note: If `s` is not a pl expression, it will be converted into one.
+    """
+    s = s if is_polars_expr(s) else create_fix_col(s)
+    return s.str.strip_chars_end().str.strip_chars_start()
+
+
+def left_trim(s: PlStringType) -> pl.Expr:
+    """
+    Remove leading whitespace from a string.
+
+    Parameters:
+    - s (Any): The string to trim. Can be a pl expression or any other value.
+
+    Returns:
+    - pl.Expr: A pl expression representing the trimmed string.
+
+    Note: If `s` is not a pl expression, it will be converted into one.
+    """
+    s = s if is_polars_expr(s) else create_fix_col(s)
+    return s.str.strip_chars_start()
+
+
+def right_trim(s: PlStringType) -> pl.Expr:
+    """
+    Remove trailing whitespace from a string.
+
+    Parameters:
+    - s (Any): The string to trim. Can be a pl expression or any other value.
+
+    Returns:
+    - pl.Expr: A pl expression representing the trimmed string.
+
+    Note: If `s` is not a pl expression, it will be converted into one.
+    """
+    s = s if is_polars_expr(s) else create_fix_col(s)
+    return s.str.strip_chars_end()
```

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/function_overview.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/function_overview.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/models.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/models.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/preprocess.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/preprocess.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/process_inline.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/process_inline.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/standardize.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/standardize.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/tokenize.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/tokenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     output = []
     v = ''
     in_string = False  # Flag to track if we're inside a string literal
     in_brackets = False  # Flag to track if we're inside square brackets
     i = 0
     string_indicator = None
     while i < len(r):
-
         current_val = r[i]
         # print(i, v[::-1])
         if current_val == string_indicator:
             output.append(v+current_val)
             v = ''
             string_indicator = None
             in_string = False
@@ -47,16 +46,16 @@
                         temp_v += r[temp_i]
                         temp_i += 1
 
                     other_split = next((f for f in all_functions.keys() if temp_v[::-1] == f))
                     next_value = r[temp_i] if temp_i<len(r) else None
                     if next_value in [None, ' '] + list(set(v[0] for v in all_split_vals if len(v)>0)) and other_split is not None:
                         output.append(temp_v)
-                        v = next_value
-                        i = temp_i + 1
+                        v = ''
+                        i = temp_i
                         continue
             for toks in (v+current_val).split(splitter):
                 if len(toks) > 0:
                     output.append(toks)
             output.append(splitter)
             v = ''
         else:
```

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/tree.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/process/tree.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/utils.py` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/PKG-INFO` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_expr_transformer
-Version: 0.1.3.3
+Version: 0.1.3.4
 Summary: Transform string-based expressions into Polars DataFrame operations
 Home-page: https://github.com/edwardvaneechoud/polars_expr_transformer
 Author: Edward van Eehoud
 Author-email: evaneechoudl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/SOURCES.txt` & `polars_expr_transformer-0.1.3.4/polars_expr_transformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.3/setup.py` & `polars_expr_transformer-0.1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """Load requirements from a pip requirements file."""
     with open(filename, 'r') as file:
         lines = file.readlines()
     return [line.strip() for line in lines if line and not line.startswith("#")]
 
 setup(
     name='polars_expr_transformer',  # Package name
-    version='0.1.3.3',  # Package version
+    version='0.1.3.4',  # Package version
     description='Transform string-based expressions into Polars DataFrame operations',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',  # Use markdown format for long description
     author='Edward van Eehoud',  # Replace with your name
     author_email='evaneechoudl@gmail.com',  # Replace with your email
     url='https://github.com/edwardvaneechoud/polars_expr_transformer',  # Replace with the URL to your package repository
     packages=find_packages(include=['polars_expr_transformer', 'polars_expr_transformer.*']),  # Automatically find package directories
```

### Comparing `polars_expr_transformer-0.1.3.3/tests/test.py` & `polars_expr_transformer-0.1.3.4/tests/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 
 def test_simple_constant_expression():
     df = pl.from_dicts([{'a': 'edward', 'b': 'courtney'}, {'a': 'courtney', 'b': 'edward'}])
     result = df.select(simple_function_to_expr("'hallo world'"))
     expected = pl.DataFrame({'literal': ['hallo world']})
     assert result.equals(expected)
 
+
 def test_combining_columns_expression():
     df = pl.from_dicts([{'a': 'edward', 'b': 'courtney'}, {'a': 'courtney', 'b': 'edward'}])
     result = df.select(simple_function_to_expr('[a] + " loves " + [b]').alias('literal'))
     expected = pl.DataFrame({'literal': ['edward loves courtney', 'courtney loves edward']})
     assert result.equals(expected)
 
+
 def test_condition_expression():
     df = pl.from_dicts([{'a': 'edward', 'b': 'courtney'}, {'a': 'courtney', 'b': 'edward'}])
     result = df.select(simple_function_to_expr('"a" in [a]').alias('literal'))
     expected = pl.DataFrame({'literal': [True, False]})
     assert result.equals(expected)
 
+
 def test_complex_conditional_expression():
     df = pl.from_dicts([{'a': 'edward', 'b': 'courtney'}, {'a': 'courtney', 'b': 'edward'}])
     result = df.select(simple_function_to_expr('concat("result:", if "a" in [a] then "A has been found" else "not found" endif)'))
     expected = pl.DataFrame({'literal': ['result:A has been found', 'result:not found']})
     assert result.equals(expected)
 
 
@@ -220,9 +223,127 @@
 def test_to_string_concat():
     df = pl.DataFrame({'numbers': [1, 2, 3], 'more_numbers': [4, 5, 6]})
     result = df.select(simple_function_to_expr('to_string([numbers]) + to_string([more_numbers])'))
     expected = pl.DataFrame({'numbers': ['14', '25', '36']})
     assert result.equals(expected)
 
 
+def test_date_func_concat():
+    df = pl.DataFrame({'date': ['2021-01-01', '2021-01-02', '2021-01-03']})
+    df_with_dates = df.select(pl.col('date').str.to_date())
+    func_str = 'to_date(to_string(year([date])) + "-"+ to_string(month([date])) + "-" + to_string(day([date])))'
+    result = df_with_dates.select(simple_function_to_expr(func_str))
+    expected = df_with_dates
+    assert result.equals(expected)
+
+
+def test_ceil():
+    df = pl.DataFrame({'numbers': [1.1, 2.2, 3.3]})
+    result = df.select(simple_function_to_expr('ceil([numbers])'))
+    expected = pl.DataFrame({'numbers': [2, 3, 4]})
+    assert result.equals(expected)
+
+
+def test_floor():
+    df = pl.DataFrame({'numbers': [1.1, 2.2, 3.3]})
+    result = df.select(simple_function_to_expr('floor([numbers])'))
+    expected = pl.DataFrame({'numbers': [1, 2, 3]})
+    assert result.equals(expected)
+
+
+def test_tanh():
+    df = pl.DataFrame({'numbers': [1.1, 2.2, 3.3]})
+    result = df.select(simple_function_to_expr('tanh([numbers])'))
+    expected = df.select(pl.col('numbers').tanh())
+    assert result.equals(expected)
+
+
+def test_sqrt():
+    df = pl.DataFrame({'numbers': [1.1, 2.2, 3.3]})
+    result = df.select(simple_function_to_expr('sqrt([numbers])'))
+    expected = df.select(pl.col('numbers').sqrt())
+    assert result.equals(expected)
+
+
+def test_abs():
+    df = pl.DataFrame({'numbers': [1.1, -2.2, 3.3]})
+    result = df.select(simple_function_to_expr('abs([numbers])'))
+    expected = df.select(pl.col('numbers').abs())
+    assert result.equals(expected)
+
+
+def test_sin():
+    df = pl.DataFrame({'numbers': [1.1, 2.2, 3.3]})
+    result = df.select(simple_function_to_expr('sin([numbers])'))
+    expected = df.select(pl.col('numbers').sin())
+    assert result.equals(expected)
+
+
+def test_cos():
+    df = pl.DataFrame({'numbers': [1.1, 2.2, 3.3]})
+    result = df.select(simple_function_to_expr('cos([numbers])'))
+    expected = df.select(pl.col('numbers').cos())
+    assert result.equals(expected)
+
+
+def test_tan():
+    df = pl.DataFrame({'numbers': [1.1, 2.2, 3.3]})
+    result = df.select(simple_function_to_expr('tan([numbers])'))
+    expected = df.select(pl.col('numbers').tan())
+    assert result.equals(expected)
+
+
+def test_pad_left():
+    df = pl.DataFrame({'names': ['ham', 'sandwich with spam', 'eggs']})
+    result = df.select(simple_function_to_expr('pad_left([names], 10, " ")'))
+    expected = pl.DataFrame({'names': ['       ham', 'sandwich with spam', '      eggs']})
+    assert result.equals(expected)
+
+
+def test_trim():
+    df = pl.DataFrame({'names': ['   ham', 'sandwich with spam   ', 'eggs   ']})
+    result = df.select(simple_function_to_expr('trim([names])'))
+    expected = pl.DataFrame({'names': ['ham', 'sandwich with spam', 'eggs']})
+    assert result.equals(expected)
+
+
+def test_pad_right():
+    df = pl.DataFrame({'names': ['ham', 'sandwich with spam', 'eggs']})
+    result = df.select(simple_function_to_expr('pad_right([names], 10, " ")'))
+    expected = pl.DataFrame({'names': ['ham       ', 'sandwich with spam', 'eggs      ']})
+    assert result.equals(expected)
+
+def test_multiply_if_else():
+    df = pl.DataFrame({'names': ['ham', 'sandwich with spam', 'eggs']})
+    result = df.select(simple_function_to_expr('if contains([names], "a") then 10 else 20 endif') * 2)
+    expected = pl.DataFrame({'literal': [20, 20, 40]})
+    assert result.equals(expected)
+
+
+def test_if_elseif_else_multiply():
+    df = pl.DataFrame({'names': ['ham', 'sandwich with spam', 'eggs']})
+    result = df.select(simple_function_to_expr('if contains([names], "an") then 10 elseif contains([names], "s") then 20 else 30 endif') * 2)
+    expected = pl.DataFrame({'literal': [60, 20, 40]})
+    assert result.equals(expected)
+
+
+def test_combination_add():
+    sf1 = 'if contains([names], "an") then 10 elseif contains([names], "s") then 20 else 30 endif'
+    sf2 = 'if contains([names], "a") then 10 else 20 endif'
+    combined = f'({sf1}) + ({sf2})'
+    df = pl.DataFrame({'names': ['ham', 'sandwich with spam', 'eggs']})
+    result = df.select(simple_function_to_expr(combined))
+    expected = pl.DataFrame({'literal': [40, 20, 40]})
+    assert result.equals(expected)
+
+
+def test_build_on_combination():
+    sf1 = 'if contains([names], "anw") then 10 elseif contains([names], "s") then 20 else 30 endif'
+    combined = 'concat("result: ", ' + sf1 + ')'
+    df = pl.DataFrame({'names': ['ham', 'sandwich with spam', 'eggs']})
+    result = df.select(simple_function_to_expr(combined))
+    expected = pl.DataFrame({'literal': ['result: 30', 'result: 20', 'result: 20']})
+    assert result.equals(expected)
+
+
 if __name__ == '__main__':
     pytest.main()
```

