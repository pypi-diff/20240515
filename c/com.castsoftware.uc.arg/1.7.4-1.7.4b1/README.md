# Comparing `tmp/com_castsoftware_uc_arg-1.7.4.tar.gz` & `tmp/com_castsoftware_uc_arg-1.7.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com_castsoftware_uc_arg-1.7.4.tar", last modified: Wed May 15 21:31:44 2024, max compression
+gzip compressed data, was "com_castsoftware_uc_arg-1.7.4b1.tar", last modified: Wed May 15 21:23:03 2024, max compression
```

## Comparing `com_castsoftware_uc_arg-1.7.4.tar` & `com_castsoftware_uc_arg-1.7.4b1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 21:31:44.142768 com_castsoftware_uc_arg-1.7.4/
--rw-rw-rw-   0        0        0     2326 2024-05-15 21:31:44.129766 com_castsoftware_uc_arg-1.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 21:31:43.887040 com_castsoftware_uc_arg-1.7.4/cast_arg/
--rw-rw-rw-   0        0        0     1429 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/Effort.csv
--rw-rw-rw-   0        0        0        0 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/__init__.py
--rw-rw-rw-   0        0        0     8669 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/actionPlan.py
--rw-rw-rw-   0        0        0     1004 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/cause.json
--rw-rw-rw-   0        0        0     7689 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/config.py
--rw-rw-rw-   0        0        0    28583 2024-05-07 15:10:56.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/convert.py
--rw-rw-rw-   0        0        0     1105 2024-04-29 21:58:10.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/main.py
-drwxrwxrwx   0        0        0        0 2024-05-15 21:31:44.046685 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/
--rw-rw-rw-   0        0        0        0 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/__init__.py
--rw-rw-rw-   0        0        0     6344 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_benchmark.py
--rw-rw-rw-   0        0        0     5044 2024-05-09 16:55:39.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_cloud.py
--rw-rw-rw-   0        0        0     4567 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_greenIt.py
--rw-rw-rw-   0        0        0     2344 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_report.py
--rw-rw-rw-   0        0        0    11296 2024-05-07 18:27:33.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_summary.py
--rw-rw-rw-   0        0        0     3191 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_grades.py
--rw-rw-rw-   0        0        0     1084 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_overview.py
--rw-rw-rw-   0        0        0      890 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_report.py
--rw-rw-rw-   0        0        0     4593 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_sizing.py
--rw-rw-rw-   0        0        0     1780 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_strengh_improvement.py
--rw-rw-rw-   0        0        0     3582 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_tech_detail_table.py
--rw-rw-rw-   0        0        0     8800 2024-05-07 15:30:59.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/powerpoint.py
--rw-rw-rw-   0        0        0    34636 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/restCall.py
--rw-rw-rw-   0        0        0     7182 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4/cast_arg/stats.py
-drwxrwxrwx   0        0        0        0 2024-05-15 21:31:44.117762 com_castsoftware_uc_arg-1.7.4/com.castsoftware.uc.arg.egg-info/
--rw-rw-rw-   0        0        0     2326 2024-05-15 21:31:43.000000 com_castsoftware_uc_arg-1.7.4/com.castsoftware.uc.arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      840 2024-05-15 21:31:43.000000 com_castsoftware_uc_arg-1.7.4/com.castsoftware.uc.arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 21:31:43.000000 com_castsoftware_uc_arg-1.7.4/com.castsoftware.uc.arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2024-05-15 21:31:43.000000 com_castsoftware_uc_arg-1.7.4/com.castsoftware.uc.arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 21:31:43.000000 com_castsoftware_uc_arg-1.7.4/com.castsoftware.uc.arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      817 2024-05-15 21:27:36.000000 com_castsoftware_uc_arg-1.7.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 21:31:44.142768 com_castsoftware_uc_arg-1.7.4/setup.cfg
--rw-rw-rw-   0        0        0      422 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:23:03.115862 com_castsoftware_uc_arg-1.7.4b1/
+-rw-rw-rw-   0        0        0     2328 2024-05-15 21:23:03.101658 com_castsoftware_uc_arg-1.7.4b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 21:23:02.822434 com_castsoftware_uc_arg-1.7.4b1/cast_arg/
+-rw-rw-rw-   0        0        0     1429 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/Effort.csv
+-rw-rw-rw-   0        0        0        0 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/__init__.py
+-rw-rw-rw-   0        0        0     8669 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/actionPlan.py
+-rw-rw-rw-   0        0        0     1004 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/cause.json
+-rw-rw-rw-   0        0        0     7689 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/config.py
+-rw-rw-rw-   0        0        0    28583 2024-05-07 15:10:56.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/convert.py
+-rw-rw-rw-   0        0        0     1105 2024-04-29 21:58:10.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:23:02.974808 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/
+-rw-rw-rw-   0        0        0        0 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_benchmark.py
+-rw-rw-rw-   0        0        0     5044 2024-05-09 16:55:39.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_cloud.py
+-rw-rw-rw-   0        0        0     4567 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_greenIt.py
+-rw-rw-rw-   0        0        0     2344 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_report.py
+-rw-rw-rw-   0        0        0    11296 2024-05-07 18:27:33.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_summary.py
+-rw-rw-rw-   0        0        0     3191 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_grades.py
+-rw-rw-rw-   0        0        0     1084 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_overview.py
+-rw-rw-rw-   0        0        0      890 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_report.py
+-rw-rw-rw-   0        0        0     4593 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_sizing.py
+-rw-rw-rw-   0        0        0     1780 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_strengh_improvement.py
+-rw-rw-rw-   0        0        0     3582 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_tech_detail_table.py
+-rw-rw-rw-   0        0        0     8800 2024-05-07 15:30:59.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/powerpoint.py
+-rw-rw-rw-   0        0        0    34636 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/restCall.py
+-rw-rw-rw-   0        0        0     7182 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/stats.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:23:03.091066 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/
+-rw-rw-rw-   0        0        0     2328 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      819 2024-05-15 21:22:26.000000 com_castsoftware_uc_arg-1.7.4b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 21:23:03.115862 com_castsoftware_uc_arg-1.7.4b1/setup.cfg
+-rw-rw-rw-   0        0        0      422 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/setup.py
```

### Comparing `com_castsoftware_uc_arg-1.7.4/PKG-INFO` & `com_castsoftware_uc_arg-1.7.4b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.7.4
+Version: 1.7.4b1
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Author-email: Nevin Kaplan <n.kaplan@castsoftware.com>, DD Assessment Team <Team.ddassessments@castsoftware.com>
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: documentation, https://github.com/CAST-Extend/com.castsoftware.uc.arg/wiki
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `com_castsoftware_uc_arg-1.7.4/README.md` & `com_castsoftware_uc_arg-1.7.4b1/README.md`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/Effort.csv` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/Effort.csv`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/actionPlan.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/actionPlan.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/cause.json` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/cause.json`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/config.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/config.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/convert.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/convert.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/main.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/main.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_benchmark.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_benchmark.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_cloud.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_cloud.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_greenIt.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_greenIt.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_report.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_report.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/hl_summary.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_summary.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_grades.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_grades.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_overview.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_overview.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_report.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_report.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_sizing.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_sizing.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_strengh_improvement.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_strengh_improvement.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/pages/mri_tech_detail_table.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_tech_detail_table.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/powerpoint.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/powerpoint.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/restCall.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/restCall.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/cast_arg/stats.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/stats.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/com.castsoftware.uc.arg.egg-info/PKG-INFO` & `com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.7.4
+Version: 1.7.4b1
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Author-email: Nevin Kaplan <n.kaplan@castsoftware.com>, DD Assessment Team <Team.ddassessments@castsoftware.com>
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: documentation, https://github.com/CAST-Extend/com.castsoftware.uc.arg/wiki
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `com_castsoftware_uc_arg-1.7.4/com.castsoftware.uc.arg.egg-info/SOURCES.txt` & `com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.4/pyproject.toml` & `com_castsoftware_uc_arg-1.7.4b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name='com.castsoftware.uc.arg'
 description="Assessment Report Generator (ARG)"
-version='1.7.4' #prod version
+version='1.7.4b1' #prod version
 authors= [
     {name="Nevin Kaplan",email="n.kaplan@castsoftware.com"},
     {name="DD Assessment Team",email="Team.ddassessments@castsoftware.com"}
 ]
 readme="README.md"
 dependencies = ['pandas', 'python-pptx==0.6.19', 'com.castsoftware.uc.python.common>=1.1.12', 'IPython', 'requests', 'Jinja2','setuptools','inflect']
 classifiers = [
```

