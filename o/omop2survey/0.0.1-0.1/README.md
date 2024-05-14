# Comparing `tmp/omop2survey-0.0.1.tar.gz` & `tmp/omop2survey-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omop2survey-0.0.1.tar", max compression
+gzip compressed data, was "omop2survey-0.1.tar", max compression
```

## Comparing `omop2survey-0.0.1.tar` & `omop2survey-0.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     5296 2024-05-14 21:03:51.967987 omop2survey-0.0.1/README.md
--rw-r--r--   0        0        0      277 2024-05-14 21:03:51.980323 omop2survey-0.0.1/omop2survey/__init__.py
--rw-r--r--   0        0        0     4077 2024-05-14 20:57:26.446629 omop2survey-0.0.1/omop2survey/codebooks.py
--rw-r--r--   0        0        0     1567 2024-05-14 19:38:37.534134 omop2survey-0.0.1/omop2survey/pivot_data.py
--rw-r--r--   0        0        0      872 2024-05-11 22:10:49.324160 omop2survey-0.0.1/omop2survey/recode_missing.py
--rw-r--r--   0        0        0     7436 2024-05-14 07:33:20.872482 omop2survey-0.0.1/omop2survey/response_set.py
--rw-r--r--   0        0        0      725 2024-05-14 21:05:00.645223 omop2survey-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6315 1970-01-01 00:00:00.000000 omop2survey-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5296 2024-05-14 21:03:51.967987 omop2survey-0.1/README.md
+-rw-r--r--   0        0        0      277 2024-05-14 21:03:51.980323 omop2survey-0.1/omop2survey/__init__.py
+-rw-r--r--   0        0        0     4077 2024-05-14 20:57:26.446629 omop2survey-0.1/omop2survey/codebooks.py
+-rw-r--r--   0        0        0     1567 2024-05-14 19:38:37.534134 omop2survey-0.1/omop2survey/pivot_data.py
+-rw-r--r--   0        0        0      872 2024-05-11 22:10:49.324160 omop2survey-0.1/omop2survey/recode_missing.py
+-rw-r--r--   0        0        0     7436 2024-05-14 07:33:20.872482 omop2survey-0.1/omop2survey/response_set.py
+-rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omop2survey-0.1/omop2survey/survey_key.csv
+-rw-r--r--   0        0        0      723 2024-05-14 21:29:11.843933 omop2survey-0.1/pyproject.toml
+-rw-r--r--   0        0        0     6313 1970-01-01 00:00:00.000000 omop2survey-0.1/PKG-INFO
```

### Comparing `omop2survey-0.0.1/README.md` & `omop2survey-0.1/README.md`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.1/omop2survey/codebooks.py` & `omop2survey-0.1/omop2survey/codebooks.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.1/omop2survey/pivot_data.py` & `omop2survey-0.1/omop2survey/pivot_data.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.1/omop2survey/recode_missing.py` & `omop2survey-0.1/omop2survey/recode_missing.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.1/omop2survey/response_set.py` & `omop2survey-0.1/omop2survey/response_set.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.1/pyproject.toml` & `omop2survey-0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omop2survey"
-version = "0.0.1"
+version = "0.1"
 description = "The 'omop2survey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
 repository = "https://github.com/elifdy/omop2survey.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `omop2survey-0.0.1/PKG-INFO` & `omop2survey-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omop2survey
-Version: 0.0.1
+Version: 0.1
 Summary: The 'omop2survey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omop2survey.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

