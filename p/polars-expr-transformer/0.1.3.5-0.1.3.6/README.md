# Comparing `tmp/polars_expr_transformer-0.1.3.5.tar.gz` & `tmp/polars_expr_transformer-0.1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_expr_transformer-0.1.3.5.tar", last modified: Wed May 15 16:07:13 2024, max compression
+gzip compressed data, was "polars_expr_transformer-0.1.3.6.tar", last modified: Wed May 15 16:35:50 2024, max compression
```

## Comparing `polars_expr_transformer-0.1.3.5.tar` & `polars_expr_transformer-0.1.3.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:07:13.928426 polars_expr_transformer-0.1.3.5/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3.5/LICENSE
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 16:07:13.928218 polars_expr_transformer-0.1.3.5/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3443 2024-05-15 11:01:56.000000 polars_expr_transformer-0.1.3.5/README.md
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:07:13.922823 polars_expr_transformer-0.1.3.5/polars_expr_transformer/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/__init__.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:07:13.923802 polars_expr_transformer-0.1.3.5/polars_expr_transformer/configs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       14 2024-05-15 08:14:06.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/configs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/configs/settings.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:07:13.925231 polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8837 2024-05-15 09:39:41.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/date_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4123 2024-05-15 13:37:30.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/logic_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5704 2024-05-15 13:44:12.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/math_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/special_funcs.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    10141 2024-05-15 13:48:08.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/string_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      333 2024-05-15 08:57:32.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/utils.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     2004 2024-05-15 16:06:59.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/function_overview.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/main_module.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:07:13.926852 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6667 2024-05-15 09:30:09.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/models.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1490 2024-05-15 13:19:43.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/polars_expr_transformer.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/preprocess.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4805 2024-05-15 08:27:45.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/process_inline.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/standardize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3217 2024-05-15 13:22:49.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/tokenize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4977 2024-05-15 10:32:09.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/tree.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/schemas.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:07:13.927321 polars_expr_transformer-0.1.3.5/polars_expr_transformer/utils/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/utils/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/utils/settings.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer/utils/utils.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:07:13.927813 polars_expr_transformer-0.1.3.5/polars_expr_transformer.egg-info/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 16:07:13.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer.egg-info/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-15 16:07:13.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-15 16:07:13.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-15 16:07:13.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer.egg-info/requires.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-15 16:07:13.000000 polars_expr_transformer-0.1.3.5/polars_expr_transformer.egg-info/top_level.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-15 16:07:13.928470 polars_expr_transformer-0.1.3.5/setup.cfg
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1836 2024-05-15 16:07:11.000000 polars_expr_transformer-0.1.3.5/setup.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:07:13.927526 polars_expr_transformer-0.1.3.5/tests/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    14285 2024-05-15 15:41:29.000000 polars_expr_transformer-0.1.3.5/tests/test.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:35:50.705511 polars_expr_transformer-0.1.3.6/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3.6/LICENSE
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 16:35:50.705313 polars_expr_transformer-0.1.3.6/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3443 2024-05-15 11:01:56.000000 polars_expr_transformer-0.1.3.6/README.md
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:35:50.700898 polars_expr_transformer-0.1.3.6/polars_expr_transformer/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/__init__.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:35:50.702322 polars_expr_transformer-0.1.3.6/polars_expr_transformer/configs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       14 2024-05-15 08:14:06.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/configs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/configs/settings.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:35:50.703283 polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    10607 2024-05-15 16:35:08.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/date_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4123 2024-05-15 13:37:30.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/logic_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5704 2024-05-15 13:44:12.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/math_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/special_funcs.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    10141 2024-05-15 13:48:08.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/string_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      333 2024-05-15 08:57:32.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/utils.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     2004 2024-05-15 16:06:59.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/function_overview.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/main_module.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:35:50.704256 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6667 2024-05-15 09:30:09.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/models.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1490 2024-05-15 13:19:43.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/polars_expr_transformer.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/preprocess.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4805 2024-05-15 08:27:45.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/process_inline.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/standardize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3217 2024-05-15 13:22:49.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/tokenize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4977 2024-05-15 10:32:09.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/tree.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/schemas.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:35:50.704580 polars_expr_transformer-0.1.3.6/polars_expr_transformer/utils/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/utils/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/utils/settings.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer/utils/utils.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:35:50.704877 polars_expr_transformer-0.1.3.6/polars_expr_transformer.egg-info/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 16:35:50.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-15 16:35:50.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-15 16:35:50.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-15 16:35:50.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer.egg-info/requires.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-15 16:35:50.000000 polars_expr_transformer-0.1.3.6/polars_expr_transformer.egg-info/top_level.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-15 16:35:50.705551 polars_expr_transformer-0.1.3.6/setup.cfg
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1836 2024-05-15 16:35:22.000000 polars_expr_transformer-0.1.3.6/setup.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 16:35:50.704698 polars_expr_transformer-0.1.3.6/tests/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    14285 2024-05-15 15:41:29.000000 polars_expr_transformer-0.1.3.6/tests/test.py
```

### Comparing `polars_expr_transformer-0.1.3.5/LICENSE` & `polars_expr_transformer-0.1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/PKG-INFO` & `polars_expr_transformer-0.1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_expr_transformer
-Version: 0.1.3.5
+Version: 0.1.3.6
 Summary: Transform string-based expressions into Polars DataFrame operations
 Home-page: https://github.com/edwardvaneechoud/polars_expr_transformer
 Author: Edward van Eehoud
 Author-email: evaneechoudl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polars_expr_transformer-0.1.3.5/README.md` & `polars_expr_transformer-0.1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/configs/settings.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/configs/settings.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/date_functions.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/date_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -254,8 +254,52 @@
     Returns:
     - pl.Expr: A FlowFile expression representing the difference in days between `s1` and `s2`.
 
     Note: If `s1` and `s2` are not FlowFile expressions, they will be converted into one.
     """
     s1 = s1 if is_polars_expr(s1) else create_fix_date_col(s1)
     s2 = s2 if is_polars_expr(s2) else create_fix_date_col(s2)
-    return (s1 - s2).dt.total_days()
+    return (s1 - s2).dt.total_days()
+
+
+def date_trim(s1: Any, part: str):
+    """
+    Trim a date to a specified part. So for example 2023-01-12 12:34:56.123 with part 'day' will return 2023-01-12 00:00:00.000
+
+    Parameters:
+    - s1 (Any): The date to trim. Can be a FlowFile expression or any other value.
+    - part (str): The part of the date to trim to. Can be 'year', 'month', 'day', 'hour', 'minute', or 'second'.
+
+    Returns:
+    - pl.Expr: A FlowFile expression representing the date trimmed to the specified part.
+
+    Note: If `s1` is not a FlowFile expression, it will be converted into one.
+    """
+    s1 = s1 if isinstance(s1, pl.Expr) else pl.col(s1)
+    if part == 'year':
+        return s1.dt.truncate('1y')
+    elif part == 'month':
+        return s1.dt.truncate('1mo')
+    elif part == 'day':
+        return s1.dt.truncate('1d')
+    elif part == 'hour':
+        return s1.dt.truncate('1h')
+    elif part == 'minute':
+        return s1.dt.truncate('1min')
+    elif part == 'second':
+        return s1.dt.truncate('1s')
+    else:
+        raise ValueError(f"Invalid part '{part}' specified. Must be 'year', 'month', 'day', 'hour', 'minute', or 'second'.")
+
+
+def date_truncate(s1: Any, truncate_by: str):
+    """
+    Truncate a date to a specified part. So for example 2023-01-12 12:34:56.123 with part '1day' will return 2023-01-12 00:00:00.000
+    Parameters:
+    - s1 (Any): The date to truncate. Can be a FlowFile expression or any other value.
+    - truncate_by (str): The part of the date to truncate to. Can be 'Nyear', 'Nmonth', 'Nday', 'Nhour', 'Nminute', or 'Nsecond'.
+    Returns:
+    - pl.Expr: A FlowFile expression representing the date truncated to the specified part.
+    """
+
+    s1 = s1 if isinstance(s1, pl.Expr) else pl.col(s1)
+    return s1.dt.truncate(truncate_by)
```

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/logic_functions.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/logic_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/math_functions.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/math_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/funcs/string_functions.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/funcs/string_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/function_overview.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/function_overview.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/models.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/models.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/polars_expr_transformer.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/polars_expr_transformer.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/preprocess.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/preprocess.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/process_inline.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/process_inline.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/standardize.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/standardize.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/tokenize.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/tokenize.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/process/tree.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/process/tree.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer/utils/utils.py` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer.egg-info/PKG-INFO` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_expr_transformer
-Version: 0.1.3.5
+Version: 0.1.3.6
 Summary: Transform string-based expressions into Polars DataFrame operations
 Home-page: https://github.com/edwardvaneechoud/polars_expr_transformer
 Author: Edward van Eehoud
 Author-email: evaneechoudl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polars_expr_transformer-0.1.3.5/polars_expr_transformer.egg-info/SOURCES.txt` & `polars_expr_transformer-0.1.3.6/polars_expr_transformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.5/setup.py` & `polars_expr_transformer-0.1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """Load requirements from a pip requirements file."""
     with open(filename, 'r') as file:
         lines = file.readlines()
     return [line.strip() for line in lines if line and not line.startswith("#")]
 
 setup(
     name='polars_expr_transformer',  # Package name
-    version='0.1.3.5',  # Package version
+    version='0.1.3.6',  # Package version
     description='Transform string-based expressions into Polars DataFrame operations',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',  # Use markdown format for long description
     author='Edward van Eehoud',  # Replace with your name
     author_email='evaneechoudl@gmail.com',  # Replace with your email
     url='https://github.com/edwardvaneechoud/polars_expr_transformer',  # Replace with the URL to your package repository
     packages=find_packages(include=['polars_expr_transformer', 'polars_expr_transformer.*']),  # Automatically find package directories
```

### Comparing `polars_expr_transformer-0.1.3.5/tests/test.py` & `polars_expr_transformer-0.1.3.6/tests/test.py`

 * *Files identical despite different names*

