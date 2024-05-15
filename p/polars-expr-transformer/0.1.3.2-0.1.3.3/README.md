# Comparing `tmp/polars_expr_transformer-0.1.3.2.tar.gz` & `tmp/polars_expr_transformer-0.1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_expr_transformer-0.1.3.2.tar", last modified: Wed May 15 11:11:58 2024, max compression
+gzip compressed data, was "polars_expr_transformer-0.1.3.3.tar", last modified: Wed May 15 11:27:56 2024, max compression
```

## Comparing `polars_expr_transformer-0.1.3.2.tar` & `polars_expr_transformer-0.1.3.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:11:58.932378 polars_expr_transformer-0.1.3.2/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3.2/LICENSE
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 11:11:58.932171 polars_expr_transformer-0.1.3.2/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3443 2024-05-15 11:01:56.000000 polars_expr_transformer-0.1.3.2/README.md
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:11:58.926632 polars_expr_transformer-0.1.3.2/polars_expr_transformer/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/__init__.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:11:58.927905 polars_expr_transformer-0.1.3.2/polars_expr_transformer/configs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       14 2024-05-15 08:14:06.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/configs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/configs/settings.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:11:58.929371 polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8837 2024-05-15 09:39:41.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/date_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4219 2024-05-15 09:34:53.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/logic_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1165 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/math_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/special_funcs.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     7550 2024-05-15 10:37:45.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/string_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      333 2024-05-15 08:57:32.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/utils.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1980 2024-05-14 17:53:37.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/function_overview.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/main_module.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:11:58.930761 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6667 2024-05-15 09:30:09.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/models.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1512 2024-05-15 08:26:49.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/polars_expr_transformer.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/preprocess.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4805 2024-05-15 08:27:45.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/process_inline.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/standardize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3186 2024-05-15 11:11:31.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/tokenize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4977 2024-05-15 10:32:09.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/tree.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/schemas.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:11:58.931225 polars_expr_transformer-0.1.3.2/polars_expr_transformer/utils/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/utils/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/utils/settings.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer/utils/utils.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:11:58.931724 polars_expr_transformer-0.1.3.2/polars_expr_transformer.egg-info/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 11:11:58.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer.egg-info/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-15 11:11:58.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-15 11:11:58.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-15 11:11:58.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer.egg-info/requires.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-15 11:11:58.000000 polars_expr_transformer-0.1.3.2/polars_expr_transformer.egg-info/top_level.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-15 11:11:58.932423 polars_expr_transformer-0.1.3.2/setup.cfg
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1836 2024-05-15 11:11:55.000000 polars_expr_transformer-0.1.3.2/setup.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:11:58.931429 polars_expr_transformer-0.1.3.2/tests/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     9390 2024-05-15 10:29:32.000000 polars_expr_transformer-0.1.3.2/tests/test.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.766578 polars_expr_transformer-0.1.3.3/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3.3/LICENSE
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 11:27:56.766385 polars_expr_transformer-0.1.3.3/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3443 2024-05-15 11:01:56.000000 polars_expr_transformer-0.1.3.3/README.md
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.761077 polars_expr_transformer-0.1.3.3/polars_expr_transformer/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/__init__.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.762276 polars_expr_transformer-0.1.3.3/polars_expr_transformer/configs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       14 2024-05-15 08:14:06.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/configs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/configs/settings.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.763674 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8837 2024-05-15 09:39:41.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/date_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4219 2024-05-15 09:34:53.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/logic_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1165 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/math_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/special_funcs.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     7550 2024-05-15 10:37:45.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/string_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      333 2024-05-15 08:57:32.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/utils.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1980 2024-05-14 17:53:37.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/function_overview.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/main_module.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.765106 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6667 2024-05-15 09:30:09.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/models.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1512 2024-05-15 08:26:49.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/polars_expr_transformer.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/preprocess.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4805 2024-05-15 08:27:45.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/process_inline.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/standardize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3230 2024-05-15 11:26:35.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/tokenize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4977 2024-05-15 10:32:09.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/tree.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/schemas.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.765545 polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/settings.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/utils.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.765982 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4252 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/requires.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-15 11:27:56.000000 polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/top_level.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-15 11:27:56.766619 polars_expr_transformer-0.1.3.3/setup.cfg
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1836 2024-05-15 11:27:50.000000 polars_expr_transformer-0.1.3.3/setup.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-15 11:27:56.765787 polars_expr_transformer-0.1.3.3/tests/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     9690 2024-05-15 11:27:32.000000 polars_expr_transformer-0.1.3.3/tests/test.py
```

### Comparing `polars_expr_transformer-0.1.3.2/LICENSE` & `polars_expr_transformer-0.1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/PKG-INFO` & `polars_expr_transformer-0.1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_expr_transformer
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: Transform string-based expressions into Polars DataFrame operations
 Home-page: https://github.com/edwardvaneechoud/polars_expr_transformer
 Author: Edward van Eehoud
 Author-email: evaneechoudl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polars_expr_transformer-0.1.3.2/README.md` & `polars_expr_transformer-0.1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/configs/settings.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/configs/settings.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/date_functions.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/date_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/logic_functions.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/logic_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/math_functions.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/math_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/funcs/string_functions.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/funcs/string_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/function_overview.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/function_overview.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/models.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/models.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/polars_expr_transformer.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/polars_expr_transformer.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/preprocess.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/preprocess.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/process_inline.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/process_inline.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/standardize.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/standardize.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/tokenize.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/tokenize.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                     temp_i, temp_v = i, v
                     while temp_i<len(r) and len([f for f in all_functions.keys() if (temp_v+r[temp_i])[::-1] in f])>0:
                         temp_v += r[temp_i]
                         temp_i += 1
 
                     other_split = next((f for f in all_functions.keys() if temp_v[::-1] == f))
                     next_value = r[temp_i] if temp_i<len(r) else None
-                    if next_value in (None, ' ', '(', '$') and other_split is not None:
+                    if next_value in [None, ' '] + list(set(v[0] for v in all_split_vals if len(v)>0)) and other_split is not None:
                         output.append(temp_v)
                         v = next_value
                         i = temp_i + 1
                         continue
             for toks in (v+current_val).split(splitter):
                 if len(toks) > 0:
                     output.append(toks)
```

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/process/tree.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/process/tree.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer/utils/utils.py` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer.egg-info/PKG-INFO` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_expr_transformer
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: Transform string-based expressions into Polars DataFrame operations
 Home-page: https://github.com/edwardvaneechoud/polars_expr_transformer
 Author: Edward van Eehoud
 Author-email: evaneechoudl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polars_expr_transformer-0.1.3.2/polars_expr_transformer.egg-info/SOURCES.txt` & `polars_expr_transformer-0.1.3.3/polars_expr_transformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.3.2/setup.py` & `polars_expr_transformer-0.1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """Load requirements from a pip requirements file."""
     with open(filename, 'r') as file:
         lines = file.readlines()
     return [line.strip() for line in lines if line and not line.startswith("#")]
 
 setup(
     name='polars_expr_transformer',  # Package name
-    version='0.1.3.2',  # Package version
+    version='0.1.3.3',  # Package version
     description='Transform string-based expressions into Polars DataFrame operations',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',  # Use markdown format for long description
     author='Edward van Eehoud',  # Replace with your name
     author_email='evaneechoudl@gmail.com',  # Replace with your email
     url='https://github.com/edwardvaneechoud/polars_expr_transformer',  # Replace with the URL to your package repository
     packages=find_packages(include=['polars_expr_transformer', 'polars_expr_transformer.*']),  # Automatically find package directories
```

### Comparing `polars_expr_transformer-0.1.3.2/tests/test.py` & `polars_expr_transformer-0.1.3.3/tests/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -213,9 +213,16 @@
     df = pl.DataFrame({'names': ['ham', 'sandwich with spam', 'eggs'],
                        'subnames': ['bread', 'spam', 'breakfast']})
     result = df.select(simple_function_to_expr('if contains([names], "a") then "found" else "not found" endif'))
     expected = pl.DataFrame({'literal': ['found', 'found', 'not found']})
     assert result.equals(expected)
 
 
+def test_to_string_concat():
+    df = pl.DataFrame({'numbers': [1, 2, 3], 'more_numbers': [4, 5, 6]})
+    result = df.select(simple_function_to_expr('to_string([numbers]) + to_string([more_numbers])'))
+    expected = pl.DataFrame({'numbers': ['14', '25', '36']})
+    assert result.equals(expected)
+
+
 if __name__ == '__main__':
     pytest.main()
```

