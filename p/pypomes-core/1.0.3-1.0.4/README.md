# Comparing `tmp/pypomes_core-1.0.3.tar.gz` & `tmp/pypomes_core-1.0.4.tar.gz`

## Comparing `pypomes_core-1.0.3.tar` & `pypomes_core-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24661 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24661 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/PKG-INFO
```

### Comparing `pypomes_core-1.0.3/src/pypomes_core/.ruff.toml` & `pypomes_core-1.0.4/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/__init__.py` & `pypomes_core-1.0.4/src/pypomes_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 )
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
 )
 from .str_pomes import (
     str_as_list, str_sanitize, str_split_on_mark,
-    str_find_whitespace, str_get_between, str_get_positional,
+    str_find_whitespace, str_get_between, str_get_positional, str_rreplace,
 )
 from .validation_msgs import (
     validate_add_msgs, validate_set_msgs
 )
 from .validation_pomes import (
     VALIDATION_MSG_LANGUAGE, VALIDATION_MSG_PREFIX,
     validate_value, validate_bool, validate_int, validate_float, validate_str,
@@ -79,15 +79,15 @@
     # json_pomes
     "json_normalize_dict", "json_normalize_iterable",
     # list_pomes
     "list_compare", "list_flatten", "list_unflatten",
     "list_find_coupled", "list_elem_starting_with", "list_transform",
     # str_pomes
     "str_as_list", "str_sanitize", "str_split_on_mark",
-    "str_find_whitespace", "str_get_between", "str_get_positional",
+    "str_find_whitespace", "str_get_between", "str_get_positional", "str_rreplace",
     # validation_msgs
     "validate_add_msgs", "validate_set_msgs",
     # validation_pomes
     "VALIDATION_MSG_LANGUAGE", "VALIDATION_MSG_PREFIX",
     "validate_value", "validate_bool", "validate_int", "validate_float", "validate_str",
     "validate_date", "validate_datetime", "validate_ints", "validate_strs",
     "validate_format_error", "validate_format_errors", "validate_unformat_errors",
```

### Comparing `pypomes_core-1.0.3/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/email_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/env_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/file_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/json_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/list_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/str_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/str_pomes.py`

 * *Files 14% similar despite different names*

```diff
@@ -132,7 +132,20 @@
         result = list_dest[pos]
     except (ValueError, IndexError):
         result = None
 
     return result
 
 
+def str_rreplace(source: str, old: str, new: str, count: int = 1) -> str:
+    """
+    Replace at most *count* occurrences of substring *old* with string *new* in *source*, in reverse order.
+
+    :param source: the string to have a substring replaced
+    :param old: the substring to replace
+    :param new: the string replacement
+    :param count: the maximum number of replacements (defaults to 1)
+    :return: the modified string
+    """
+    return source[::-1].replace(old[::-1], new[::-1], count)[::-1]
+
+
```

### Comparing `pypomes_core-1.0.3/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.0.4/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.0.4/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/LICENSE` & `pypomes_core-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.3/pyproject.toml` & `pypomes_core-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.0.3/PKG-INFO` & `pypomes_core-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

