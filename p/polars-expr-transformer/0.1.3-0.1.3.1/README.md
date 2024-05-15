# Comparing `tmp/polars_expr_transformer-0.1.3.tar.gz` & `tmp/polars_expr_transformer-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_expr_transformer-0.1.3.tar", last modified: Tue May 14 20:14:11 2024, max compression
+gzip compressed data, was "polars_expr_transformer-0.1.3.1.tar", last modified: Wed May 15 11:09:09 2024, max compression
```

## Comparing `polars_expr_transformer-0.1.3.tar` & `polars_expr_transformer-0.1.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.089948 polars_expr_transformer-0.1.3/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3/LICENSE
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     2291 2024-05-14 20:14:11.089780 polars_expr_transformer-0.1.3/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1485 2024-05-14 20:00:49.000000 polars_expr_transformer-0.1.3/README.md
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.086177 polars_expr_transformer-0.1.3/polars_expr_transformer/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/__init__.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.087029 polars_expr_transformer-0.1.3/polars_expr_transformer/configs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:27.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/configs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/configs/settings.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.087896 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8014 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/date_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4155 2024-05-14 18:00:47.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/logic_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1165 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/math_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/special_funcs.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6622 2024-05-14 18:01:02.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/string_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      276 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/utils.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1980 2024-05-14 17:53:37.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/function_overview.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/main_module.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.088813 polars_expr_transformer-0.1.3/polars_expr_transformer/process/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5237 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/models.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1512 2024-05-14 17:59:40.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/polars_expr_transformer.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/preprocess.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4511 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/process_inline.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/standardize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3148 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/tokenize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5038 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/tree.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/schemas.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.089106 polars_expr_transformer-0.1.3/polars_expr_transformer/utils/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/utils/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/utils/settings.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/utils/utils.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.089384 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     2291 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/requires.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/top_level.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-14 20:14:11.089987 polars_expr_transformer-0.1.3/setup.cfg
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1834 2024-05-14 20:14:05.000000 polars_expr_transformer-0.1.3/setup.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.089214 polars_expr_transformer-0.1.3/tests/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1518 2024-05-14 19:53:33.000000 polars_expr_transformer-0.1.3/tests/test.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:09:09.186927 polars_expr_transformer-0.1.3.1/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3.1/LICENSE
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 11:09:09.186712 polars_expr_transformer-0.1.3.1/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3443 2024-05-15 11:01:56.000000 polars_expr_transformer-0.1.3.1/README.md
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:09:09.181359 polars_expr_transformer-0.1.3.1/polars_expr_transformer/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/__init__.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:09:09.182308 polars_expr_transformer-0.1.3.1/polars_expr_transformer/configs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       14 2024-05-15 08:14:06.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/configs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/configs/settings.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:09:09.183626 polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8837 2024-05-15 09:39:41.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/date_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4219 2024-05-15 09:34:53.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/logic_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1165 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/math_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/special_funcs.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     7550 2024-05-15 10:37:45.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/string_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      333 2024-05-15 08:57:32.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/utils.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1980 2024-05-14 17:53:37.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/function_overview.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/main_module.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:09:09.185323 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6667 2024-05-15 09:30:09.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/models.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1512 2024-05-15 08:26:49.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/polars_expr_transformer.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/preprocess.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4805 2024-05-15 08:27:45.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/process_inline.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/standardize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3184 2024-05-15 10:35:16.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/tokenize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4977 2024-05-15 10:32:09.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/tree.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/schemas.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:09:09.185787 polars_expr_transformer-0.1.3.1/polars_expr_transformer/utils/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/utils/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/utils/settings.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer/utils/utils.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:09:09.186282 polars_expr_transformer-0.1.3.1/polars_expr_transformer.egg-info/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 11:09:09.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-15 11:09:09.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-15 11:09:09.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-15 11:09:09.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer.egg-info/requires.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-15 11:09:09.000000 polars_expr_transformer-0.1.3.1/polars_expr_transformer.egg-info/top_level.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-15 11:09:09.186966 polars_expr_transformer-0.1.3.1/setup.cfg
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1836 2024-05-15 11:08:59.000000 polars_expr_transformer-0.1.3.1/setup.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:09:09.186011 polars_expr_transformer-0.1.3.1/tests/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     9390 2024-05-15 10:29:32.000000 polars_expr_transformer-0.1.3.1/tests/test.py
```

### Comparing `polars_expr_transformer-0.1.3/LICENSE` & `polars_expr_transformer-0.1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/configs/settings.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/configs/settings.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/date_functions.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/date_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import polars as pl
 from typing import Any
 from polars_expr_transformer.funcs.utils import is_polars_expr, create_fix_col, create_fix_date_col
 from datetime import datetime
-
-string_type = pl.Expr | str
+from polars_expr_transformer.funcs.utils import PlStringType, PlIntType
 
 
 def now() -> pl.Expr:
     """
     Get the current timestamp.
 
     Returns:
@@ -54,15 +53,15 @@
 
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_col(s).str.to_datetime()
     return s.dt.month()
 
 
-def day(s: Any) -> pl.Expr:
+def day(s: PlStringType) -> pl.Expr:
     """
     Extract the day from a date or timestamp.
 
     Parameters:
     - s (Any): The date or timestamp to extract the day from. Can be a FlowFile expression or any other value.
 
     Returns:
@@ -70,15 +69,15 @@
 
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_date_col(s)
     return s.dt.day()
 
 
-def hour(s: Any) -> pl.Expr:
+def hour(s: PlStringType) -> pl.Expr:
     """
     Extract the hour from a timestamp.
 
     Parameters:
     - s (Any): The timestamp to extract the hour from. Can be a FlowFile expression or any other value.
 
     Returns:
@@ -86,15 +85,15 @@
 
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_date_col(s)
     return s.dt.hour()
 
 
-def minute(s: Any) -> pl.Expr:
+def minute(s: PlStringType) -> pl.Expr:
     """
     Extract the minute from a timestamp.
 
     Parameters:
     - s (Any): The timestamp to extract the minute from. Can be a FlowFile expression or any other value.
 
     Returns:
@@ -102,15 +101,15 @@
 
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_date_col(s)
     return s.dt.minute()
 
 
-def second(s: Any) -> pl.Expr:
+def second(s: PlStringType) -> pl.Expr:
     """
     Extract the second from a timestamp.
 
     Parameters:
     - s (Any): The timestamp to extract the second from. Can be a FlowFile expression or any other value.
 
     Returns:
@@ -118,33 +117,51 @@
 
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_date_col(s)
     return s.dt.second()
 
 
-def add_days(s: Any, days: Any) -> pl.Expr:
+def add_days(s: PlStringType, days: PlIntType) -> pl.Expr:
     """
     Add a specified number of days to a date or timestamp.
 
     Parameters:
     - s (Any): The date or timestamp to add days to. Can be a FlowFile expression or any other value.
     - days (int): The number of days to add.
 
     Returns:
     - pl.Expr: A FlowFile expression representing the result of adding `days` to `s`.
 
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_date_col(s)
-    days = days if is_polars_expr(days) else create_fix_date_col(days)
+    days = days if is_polars_expr(days) else create_fix_col(days)
     return s + pl.duration(days=days)
 
 
-def add_hours(s: Any, hours: any) -> pl.Expr:
+def add_years(s: PlStringType, years: PlIntType) -> pl.Expr:
+    """
+    Add a specified number of days to a date or timestamp.
+
+    Parameters:
+    - s (Any): The date or timestamp to add days to. Can be a FlowFile expression or any other value.
+    - days (int): The number of days to add.
+
+    Returns:
+    - pl.Expr: A FlowFile expression representing the result of adding `days` to `s`.
+
+    Note: If `s` is not a FlowFile expression, it will be converted into one.
+    """
+    s = s if is_polars_expr(s) else create_fix_date_col(s)
+    years = years if is_polars_expr(years) else create_fix_col(years)
+    return s + pl.duration(days=years*365)
+
+
+def add_hours(s: PlStringType, hours: PlIntType) -> pl.Expr:
     """
     Add a specified number of hours to a timestamp.
 
     Parameters:
     - s (Any): The timestamp to add hours to. Can be a FlowFile expression or any other value.
     - hours (int): The number of hours to add.
 
@@ -154,15 +171,15 @@
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_date_col(s)
     hours = hours if is_polars_expr(hours) else create_fix_col(hours)
     return s + pl.duration(hours=hours)
 
 
-def add_minutes(s: Any, minutes: Any) -> pl.Expr:
+def add_minutes(s: PlStringType, minutes: PlIntType) -> pl.Expr:
     """
     Add a specified number of minutes to a timestamp.
 
     Parameters:
     - s (Any): The timestamp to add minutes to. Can be a FlowFile expression or any other value.
     - minutes (int): The number of minutes to add.
 
@@ -172,15 +189,15 @@
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_date_col(s)
     minutes = minutes if is_polars_expr(minutes) else create_fix_col(minutes)
     return s + pl.duration(minutes=minutes)
 
 
-def add_seconds(s: Any, seconds: Any) -> pl.Expr:
+def add_seconds(s: PlStringType, seconds: PlIntType) -> pl.Expr:
     """
     Add a specified number of seconds to a timestamp.
 
     Parameters:
     - s (Any): The timestamp to add seconds to. Can be a FlowFile expression or any other value.
     - seconds (int): The number of seconds to add.
 
@@ -190,15 +207,15 @@
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_date_col(s)
     seconds = seconds if is_polars_expr(seconds) else create_fix_col(seconds)
     return s + pl.duration(seconds=seconds)
 
 
-def datetime_diff_seconds(s1: Any, s2: Any) -> pl.Expr:
+def datetime_diff_seconds(s1: PlStringType, s2: PlStringType) -> pl.Expr:
     """
     Calculate the difference in seconds between two timestamps.
 
     Parameters:
     - s1 (Any): The first timestamp. Can be a FlowFile expression or any other value.
     - s2 (Any): The second timestamp. Can be a FlowFile expression or any other value.
 
@@ -208,15 +225,15 @@
     Note: If `s1` and `s2` are not FlowFile expressions, they will be converted into one.
     """
     s1 = s1 if is_polars_expr(s1) else create_fix_date_col(s1)
     s2 = s2 if is_polars_expr(s2) else create_fix_date_col(s2)
     return (s1 - s2).dt.total_seconds()
 
 
-def datetime_diff_nanoseconds(s1: Any, s2: Any):
+def datetime_diff_nanoseconds(s1: PlStringType, s2: PlStringType):
     """ Calculate the difference in days between two dates.
     Parameters:
     - s1 (Any): The first date. Can be a FlowFile expression or any other value.
     - s2 (Any): The second date. Can be a FlowFile expression or any other value.
     Returns:
     - pl.Expr: A FlowFile expression representing the difference in days between `s1` and `s2`.
     Note: If `s1` and `s2` are not FlowFile expressions, they will be converted into one.
```

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/logic_functions.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/logic_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from polars_expr_transformer.funcs.utils import is_polars_expr, create_fix_col
 from typing import Any, Dict
 import polars as pl
+from polars_expr_transformer.funcs.utils import PlStringType, PlIntType
 
 
 def equals(s: Any, t: Any) -> pl.Expr:
     """
     Check if two expressions or values are equal.
 
     Parameters:
@@ -88,15 +89,15 @@
     """
     if is_polars_expr(val):
         dtype = pl.select(val).dtypes[0]
         return pl.lit(dtype.is_(pl.Utf8))
     return pl.lit(isinstance(val, str))
 
 
-def contains(base: pl.Expr | str, pattern: pl.Expr | str) -> pl.Expr:
+def contains(base: PlStringType, pattern: Any) -> pl.Expr:
     """
     Check if a pattern is contained within a base string or expression.
 
     Parameters:
     - base (Union[Expr, str]): The base string or expression where the pattern is to be searched.
     - pattern (Union[Expr, str]): The pattern string or expression to search for within the base.
 
@@ -110,19 +111,19 @@
     """
     def _contain(_row: Dict):
         base_val, pattern_val = _row.values()
         return pattern_val in base_val
 
     if isinstance(base, pl.Expr):
         if isinstance(pattern, pl.Expr):
-            return pl.struct([base, pattern]).apply(lambda r: _contain(r), return_dtype=pl.Boolean)
+            return pl.struct([base, pattern]).map_elements(lambda r: _contain(r), return_dtype=pl.Boolean)
         else:
             return base.str.contains(pattern)
     else:
         if isinstance(pattern, pl.Expr):
-            return pl.struct([pattern]).apply(lambda x: next(iter(x.values())) in base)
+            return pl.struct([pattern]).map_elements(lambda x: next(iter(x.values())) in base)
         else:
             return pl.lit(pattern in base)
 
 
-def _in(pattern: pl.Expr | str, base: pl.Expr | str) -> pl.Expr:
+def _in(pattern: Any, base: PlStringType) -> pl.Expr:
     return contains(base, pattern)
```

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/math_functions.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/math_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/string_functions.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/funcs/string_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import polars as pl
 from typing import List, Tuple, Callable, Dict, Any
 from polars_expr_transformer.funcs.utils import is_polars_expr, create_fix_col
-
-
-string_type = pl.Expr | str
+from polars_expr_transformer.funcs.utils import PlStringType, PlIntType
 
 
 def concat(*columns) -> pl.Expr:
     """
     Concatenate the values of multiple columns into a single string.
 
     Parameters:
@@ -16,77 +14,78 @@
     Returns:
     - An expression representing the concatenated string.
     """
     columns = [create_fix_col(c) if not is_polars_expr(c) else c for c in columns]
     return pl.concat_str(columns)
 
 
-def count_match(column: pl.Expr | str, value: str) -> pl.Expr:
+def count_match(column: PlStringType, value: str) -> pl.Expr:
 
     """
     Count the number of occurrences of a given value in a column.
 
     Parameters:
     - column: The column in which to count the occurrences.
     - value: The value to count.
 
     Returns:
     - An expression representing the number of occurrences.
     """
     if isinstance(column, pl.Expr):
-        return column.str.count_match(value)
-    return pl.lit(column).str.count_match(value)
+        return column.str.count_matches(value)
+    return pl.lit(column).str.count_matches(value)
 
 
-def length(column: pl.Expr | str) -> pl.Expr:
+def length(column: PlStringType) -> pl.Expr:
     """
     Calculate the length of a given column or string.
 
     Parameters:
     - column: The column or string for which to calculate the length.
 
     Returns:
     - An expression representing the length.
     """
     if isinstance(column, str):
         return pl.lit(len(column))
-    return column.str.lengths()
+    column: pl.Expr
+    return column.str.len_chars()
 
 
-def uppercase(_v: pl.Expr | str) -> pl.Expr:
+def uppercase(_v: PlStringType) -> pl.Expr:
     """
     Convert the characters in a given column or string to uppercase.
 
     Parameters:
     - _v: The column or string to convert.
 
     Returns:
     - An expression representing the uppercase conversion.
     """
     if isinstance(_v, pl.Expr):
         return _v.str.to_uppercase()
     return pl.lit(_v.__str__().upper())
 
 
-def to_string(_v: pl.Expr | str) -> pl.Expr:
+def to_string(_v: PlStringType) -> pl.Expr:
     """
     Convert a given column or value to its string representation.
 
     Parameters:
     - _v: The column or value to convert.
 
     Returns:
     - An expression representing the string conversion.
     """
     if isinstance(_v, pl.Expr):
         return _v.cast(str)
     return pl.lit(_v.__str__())
 
 
-def lowercase(_v: pl.Expr | str) -> pl.Expr:
+def lowercase(_v: PlStringType) -> pl.Expr:
     """
     Convert the characters in a given column or string to lowercase.
 
     Parameters:
     - _v: The column or string to convert.
 
     Returns:
@@ -99,78 +98,78 @@
 
 def __left(row: Dict):
     v, l = row.values()
     if v is not None:
         return v[:l]
     return None
 
-def left(column: string_type, length: pl.Expr | int) -> pl.Expr:
+def left(column: PlStringType, length: pl.Expr | int) -> pl.Expr:
     """
     Extracts a substring from a column or string, starting from the beginning.
 
     Parameters:
     - column: The column or string from which to extract the substring.
     - length: The length of the substring to extract.
 
     Returns:
     - An expression representing the substring.
     """
     if is_polars_expr(column):
         if is_polars_expr(length):
             print(' pl.struct([column, length]).apply(lambda r: __left(r))')
-            return pl.struct([column, length]).apply(lambda r: __left(r))
+            return pl.struct([column, length]).map_elements(lambda r: __left(r), return_dtype=pl.String)
         else:
             print('column.str.slice(0, length)')
             return column.str.slice(0, length)
     elif is_polars_expr(length):
         print('pl.struct([length]).apply(lambda r: column[:list(r.values)[0]])')
-        return pl.struct([length]).apply(lambda r: column[:list(r.values)[0]])
+        return pl.struct([length]).map_elements(lambda r: column[:list(r.values)[0]], return_dtype=pl.String)
     else:
         print('pl.lit(column[:length])')
         return pl.lit(column[:length])
 
 
 def __right(row: Dict):
     v, l = row.values()
     if v is not None:
         return v[-l:]
 
 
-def right(column: string_type, length: pl.Expr | int) -> pl.Expr:
+def right(column: PlStringType, length: PlIntType) -> pl.Expr:
     """
     Extracts a substring from a column or string, starting from the end.
 
     Parameters:
     - column: The column or string from which to extract the substring.
     - length: The length of the substring to extract.
 
     Returns:
     - An expression representing the substring.
     """
 
     if is_polars_expr(column):
         if is_polars_expr(length):
-            return pl.struct([column, length]).apply(__right)
+            return pl.struct([column, length]).map_elements(__right, return_dtype=pl.String)
         else:
             return column.str.slice(-length)
     elif is_polars_expr(length):
-        return pl.struct([length]).apply(lambda r: column[-next(iter(r.values())):])
+        return pl.struct([length]).map_elements(lambda r: column[-next(iter(r.values())):], return_dtype=pl.String)
     else:
         return pl.lit(column[-length:])
 
 
 def __apply_replace(row, replace_by=None):
     v = list(row.values())
     main_str = v[0]
     other_str = v[1] if len(v) > 1 else None
     replace_str = v[2] if len(v) > 2 else replace_by
     return main_str.replace(other_str, replace_str)
 
 
-def replace(main: string_type, other: string_type, replace_by: string_type) -> pl.Expr:
+def replace(main: PlStringType, other: PlStringType, replace_by: PlStringType) -> pl.Expr:
     """
        Replaces occurrences of a substring within a main string with another string.
 
        Parameters:
        - main: The main string or expression where the replacement will occur.
        - other: The substring or expression that needs to be replaced.
        - replace_by: The string or expression that will replace the 'other' substring in 'main'.
@@ -183,39 +182,57 @@
        The function will return "Hello, there!"
        """
     if not is_polars_expr(main):
         main = pl.lit(main)
     return main.str.replace_all(other, replace_by, literal=True).cast(pl.Utf8)
 
 
-def to_date(s: Any, date_format: str = "%Y-%m-%d") -> pl.Expr:
+def to_date(s: PlStringType, date_format: str = "%Y-%m-%d") -> pl.Expr:
     """
     Convert a string to a date.
 
     Parameters:
     - s (Any): The string to convert to a date. Can be a FlowFile expression or any other value.
     - format (str): The format of the date string. Default is "%Y-%m-%d".
 
     Returns:
     - pl.Expr: A FlowFile expression representing the converted date.
 
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_col(s)
-    return s.str.to_date(date_format, strict=True)
+    return s.str.to_date(date_format, strict=False)
 
 
-def to_datetime(s: Any, date_format: str = "%Y-%m-%d %H:%M:%S") -> pl.Expr:
+def to_datetime(s: PlStringType, date_format: str = "%Y-%m-%d %H:%M:%S") -> pl.Expr:
     """
     Convert a string to a datetime.
 
     Parameters:
     - s (Any): The string to convert to a datetime. Can be a FlowFile expression or any other value.
     - format (str): The format of the datetime string. Default is "%Y-%m-%d %H:%M:%S".
 
     Returns:
     - pl.Expr: A FlowFile expression representing the converted datetime.
 
     Note: If `s` is not a FlowFile expression, it will be converted into one.
     """
     s = s if is_polars_expr(s) else create_fix_col(s)
     return s.str.to_datetime(date_format, strict=False)
+
+
+def find_position(s: PlStringType, sub: PlStringType) -> pl.Expr:
+    """
+    Find the position of a substring within a string.
+
+    Parameters:
+    - s (Any): The string in which to find the position of the substring. Can be a FlowFile expression or any other value.
+    - sub (Any): The substring to find the position of. Can be a FlowFile expression or any other value.
+
+    Returns:
+    - pl.Expr: A FlowFile expression representing the position of the substring within the string.
+
+    Note: If `s` or `sub` is not a FlowFile expression, it will be converted into one.
+    """
+    s = s if is_polars_expr(s) else create_fix_col(s)
+    sub = sub if is_polars_expr(sub) else create_fix_col(sub)
+    return s.str(sub)
```

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/function_overview.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/function_overview.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/process/models.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 from polars_expr_transformer.configs.settings import PRECEDENCE
-from typing import TypeAlias, Literal, List, Union, Optional, Any
+from typing import TypeAlias, Literal, List, Union, Optional, Any, Callable
+from polars_expr_transformer.funcs.utils import PlStringType, PlIntType
 from polars_expr_transformer.configs.settings import operators, funcs
+from polars_expr_transformer.configs import logging
 from dataclasses import dataclass, field
 import polars as pl
+from types import NotImplementedType
+import inspect
+
+
+def get_types_from_func(func: Callable):
+    return [param.annotation for param in inspect.signature(func).parameters.values()]
+
+
+def allow_expressions(_type):
+    return _type in [PlStringType, PlIntType, pl.Expr, Any, inspect._empty]
+
+
+def allow_non_pl_expressions(_type):
+    return _type in [str, int, float, bool, PlIntType, PlStringType, Any, inspect._empty]
 
 
 value_type: TypeAlias = Literal['string', 'number', 'boolean', 'operator', 'function', 'column', 'empty', 'case_when',
                                 'prio', 'sep', 'special']
 
 
 @dataclass
@@ -64,43 +80,64 @@
 
     def __eq__(self, other):
         return self.val == other
 
     def __hash__(self):
         return hash(self.val)
 
+    def get_readable_pl_function(self):
+        return self.val
+
 
 @dataclass
 class Func:
     func_ref: Union[Classifier, "IfFunc"]
     args: List[Union["Func", Classifier, "IfFunc"]] = field(default_factory=list)
     parent: Optional["Func"] = field(repr=False, default=None)
 
+    def get_readable_pl_function(self):
+        return f'{self.func_ref.val}({", ".join([arg.get_readable_pl_function() for arg in self.args])})'
+
     def add_arg(self, arg: Union["Func", Classifier, "IfFunc"]):
         self.args.append(arg)
         arg.parent = self
 
     def get_pl_func(self):
         if self.func_ref == 'pl.lit':
             if len(self.args)!=1:
                 raise Exception('Expected must contain 1 argument not more not less')
             if isinstance(self.args[0].get_pl_func(), pl.expr.Expr):
                 return self.args[0].get_pl_func()
             return funcs[self.func_ref.val](self.args[0].get_pl_func())
         args = [arg.get_pl_func() for arg in self.args]
+        func = funcs[self.func_ref.val]
         if any(isinstance(arg, pl.Expr) for arg in args) and any(not isinstance(arg, pl.Expr) for arg in args):
+            func_types = get_types_from_func(func)
             standardized_args = []
-            for arg in args:
-                if not isinstance(arg, pl.Expr):
-                    standardized_args.append(pl.lit(arg))
-                else:
-                    standardized_args.append(arg)
+            if len(func_types) == len(args):
+                for func_type, arg in zip(func_types, args):
+                    if not isinstance(arg, pl.Expr) and allow_expressions(func_type):
+                        standardized_args.append(pl.lit(arg))
+                    else:
+                        standardized_args.append(arg)
+            else:
+                standardized_args = [pl.lit(arg) if not isinstance(arg, pl.Expr) else arg for arg in args]
+
         else:
             standardized_args = args
-        return funcs[self.func_ref.val](*standardized_args)
+        r = func(*standardized_args)
+
+        if isinstance(r, NotImplementedType):
+            try:
+                readable_pl_function = self.get_readable_pl_function()
+                logging.warning(f'Not implemented type: {self.get_readable_pl_function()}')
+            except:
+                logging.warning('Not implemented type')
+            return False
+        return r
 
 
 @dataclass
 class ConditionVal:
     func_ref: Union[Classifier, "IfFunc", "Func"] = None
     condition: Func = None
     val: Func = None
```

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/process/polars_expr_transformer.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/polars_expr_transformer.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/process/preprocess.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/preprocess.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/process/process_inline.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/process_inline.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,23 +90,28 @@
         parsed_prefixed_formula = parse_formula(prefixed_formula)
         evaluated_prefix_formula = evaluate_prefix_formula(parsed_prefixed_formula)
         return flatten_inline_formula(evaluated_prefix_formula)
     return inline_formula_tokens
 
 
 def parse_inline_functions(_hierarchical_formula: Func):
-    if any([a.val_type == 'operator' for a in _hierarchical_formula.args if isinstance(a, Classifier)]):
-        prefixed_formula = inline_to_prefix_formula(_hierarchical_formula.args)
-        parsed_prefixed_formula = parse_formula(prefixed_formula)
-        evaluated_prefix_formula = evaluate_prefix_formula(parsed_prefixed_formula)
-        flattened_prefix_formula = flatten_inline_formula(evaluated_prefix_formula)
-        _hierarchical_formula.args = [build_hierarchy(flattened_prefix_formula)]
-    else:
-        for arg in _hierarchical_formula.args:
-            if isinstance(arg, Func):
-                parse_inline_functions(arg)
-            elif isinstance(arg, IfFunc):
-                for condition in arg.conditions:
-                    parse_inline_functions(condition.condition)
-                    parse_inline_functions(condition.val)
-                parse_inline_functions(arg.else_val)
-
+    run = [True]
+    def parse_inline_function_worker(_hierarchical_formula: Func):
+        if any([a.val_type == 'operator' for a in _hierarchical_formula.args if isinstance(a, Classifier)]):
+            prefixed_formula = inline_to_prefix_formula(_hierarchical_formula.args)
+            parsed_prefixed_formula = parse_formula(prefixed_formula)
+            evaluated_prefix_formula = evaluate_prefix_formula(parsed_prefixed_formula)
+            flattened_prefix_formula = flatten_inline_formula(evaluated_prefix_formula)
+            _hierarchical_formula.args = [build_hierarchy(flattened_prefix_formula)]
+            run[0] = True
+        else:
+            for arg in _hierarchical_formula.args:
+                if isinstance(arg, Func):
+                    parse_inline_function_worker(arg)
+                elif isinstance(arg, IfFunc):
+                    for condition in arg.conditions:
+                        parse_inline_function_worker(condition.condition)
+                        parse_inline_function_worker(condition.val)
+                    parse_inline_function_worker(arg.else_val)
+    while run[0]:
+        run[0] = False
+        parse_inline_function_worker(_hierarchical_formula)
```

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/process/standardize.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/standardize.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/process/tokenize.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/tokenize.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     output = []
     v = ''
     in_string = False  # Flag to track if we're inside a string literal
     in_brackets = False  # Flag to track if we're inside square brackets
     i = 0
     string_indicator = None
     while i < len(r):
+
         current_val = r[i]
+        print(i, v[::-1])
         if current_val == string_indicator:
             output.append(v+current_val)
             v = ''
             string_indicator = None
             in_string = False
             i += 1
             continue
@@ -25,33 +27,33 @@
             in_brackets = not in_brackets  # Toggle the in_brackets flag
         elif current_val == '=' and not in_brackets and not in_string:
             if len(r) > i + 1:
                 two_character_inline = r[i + 1] in ('<', '>', '=', '!')
                 if two_character_inline:
                     current_val += r[i + 1]
                     i += 1
-
         if not in_string and not in_brackets and current_val[::-1] in all_split_vals:
             if i > 0:
                 output.append(v)
             output.append(current_val)
             v = ''
         elif any([vv[::-1] in v+current_val for vv in all_split_vals if len(vv) > 1]) and not in_string:
             splitter = next(vv[::-1] for vv in all_split_vals if len(vv) > 1 and vv[::-1] in v+current_val)
             if splitter:
                 # check for longer possiblities
                 longer_options = [f for f in all_functions.keys() if (v+current_val)[::-1] in f]
                 if len(longer_options)>0:
                     temp_i, temp_v = i, v
-                    while len([f for f in all_functions.keys() if temp_v[::-1] in f])>0 and temp_i<len(r):
+                    while temp_i<len(r) and len([f for f in all_functions.keys() if (temp_v+r[temp_i])[::-1] in f])>0:
                         temp_v += r[temp_i]
                         temp_i += 1
-                    other_split = next((f for f in all_functions.keys() if temp_v[::-1] == f), None)
-                    next_value = r[temp_i+1] if temp_i<len(r) else None
-                    if next_value in (None, ' ', '(') and other_split is not None:
+
+                    other_split = next((f for f in all_functions.keys() if temp_v[::-1] == f))
+                    next_value = r[temp_i] if temp_i<len(r) else None
+                    if next_value in (None, ' ', '(', '$') and other_split is not None:
                         output.append(temp_v)
                         v = next_value
                         i = temp_i + 1
                         continue
             for toks in (v+current_val).split(splitter):
                 if len(toks) > 0:
                     output.append(toks)
```

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/process/tree.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/process/tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from polars_expr_transformer.process.models import Classifier, Func, IfFunc, TempFunc, ConditionVal
 from copy import deepcopy
 
 
 def handle_opening_bracket(current_func: Func, previous_val: Classifier) -> Func:
     if previous_val and previous_val.val_type == 'function':
         pass
-    elif isinstance(current_func, IfFunc) and previous_val.val == '$if$':
+    elif isinstance(current_func, IfFunc) and previous_val.val in ('$if$', '$elseif$'):
         condition = Func(Classifier('pl.lit'))
         val = Func(Classifier('pl.lit'))
         condition_val = ConditionVal(condition=condition, val=val)
-        else_val = Func(Classifier('pl.lit'))
-        current_func.add_else_val(else_val)
+        if previous_val.val == '$if$':
+            else_val = Func(Classifier('pl.lit'))
+            current_func.add_else_val(else_val)
         current_func.add_condition(condition_val)
         current_func = condition
     else:
         new_func = Func(Classifier('pl.lit'))
         current_func.add_arg(new_func)
         current_func = new_func
     return current_func
@@ -36,24 +37,22 @@
 
 def handle_else(current_func: Func, next_val: Optional[Classifier], pos: int) -> (Func, int):
     current_func = current_func.parent
     if isinstance(current_func, IfFunc):
         current_func = current_func.else_val
         if next_val and next_val.val == '(':
             pos += 1
+    else:
+        raise Exception('Expected if')
     return current_func, pos
 
 def handle_elseif(current_func: Func) -> Func:
     current_func = current_func.parent
-    if isinstance(current_func, IfFunc):
-        condition = Func(Classifier('pl.lit'))
-        val = Func(Classifier('pl.lit'))
-        condition_val = ConditionVal(condition=condition, val=val)
-        current_func.add_condition(condition_val)
-        current_func = condition
+    if not isinstance(current_func, IfFunc):
+        raise Exception('Expected if')
     return current_func
 
 def handle_endif(current_func: Func) -> Func:
     if isinstance(current_func, IfFunc):
         current_func = current_func.parent
     else:
         raise Exception('Expected if')
@@ -105,19 +104,20 @@
                 current_func, pos = handle_else(current_func, next_val, pos)
             elif current_val.val == '$elseif$':
                 current_func = handle_elseif(current_func)
             elif current_val.val == '$endif$':
                 current_func = handle_endif(current_func)
             elif current_val.val == ')':
                 if next_val is None:
+                    pass
                     break
                 current_func, main_func = handle_closing_bracket(current_func, main_func)
             elif current_val.val_type == 'function':
                 current_func = handle_function(current_func, current_val)
             elif current_val.val_type in ('string', 'number', 'boolean', 'operator'):
                 handle_literal(current_func, current_val)
             elif current_val.val == '__negative()':
                 handle_literal(current_func, Classifier('-1'))
         else:
             handle_literal(current_func, current_val)
         pos += 1
-    return main_func
+    return main_func
```

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer/utils/utils.py` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/SOURCES.txt` & `polars_expr_transformer-0.1.3.1/polars_expr_transformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3/setup.py` & `polars_expr_transformer-0.1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """Load requirements from a pip requirements file."""
     with open(filename, 'r') as file:
         lines = file.readlines()
     return [line.strip() for line in lines if line and not line.startswith("#")]
 
 setup(
     name='polars_expr_transformer',  # Package name
-    version='0.1.3',  # Package version
+    version='0.1.3.1',  # Package version
     description='Transform string-based expressions into Polars DataFrame operations',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',  # Use markdown format for long description
     author='Edward van Eehoud',  # Replace with your name
     author_email='evaneechoudl@gmail.com',  # Replace with your email
     url='https://github.com/edwardvaneechoud/polars_expr_transformer',  # Replace with the URL to your package repository
     packages=find_packages(include=['polars_expr_transformer', 'polars_expr_transformer.*']),  # Automatically find package directories
```

