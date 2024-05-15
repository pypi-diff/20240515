# Comparing `tmp/metricsreport-2024.4.20.tar.gz` & `tmp/metricsreport-2024.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricsreport-2024.4.20.tar", max compression
+gzip compressed data, was "metricsreport-2024.5.15.tar", max compression
```

## Comparing `metricsreport-2024.4.20.tar` & `metricsreport-2024.5.15.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-12 13:44:26.925841 metricsreport-2024.4.20/LICENSE
--rw-r--r--   0        0        0     2322 2024-04-12 13:44:26.925841 metricsreport-2024.4.20/README.md
--rw-r--r--   0        0        0       99 2024-04-12 14:13:35.841878 metricsreport-2024.4.20/metricsreport/__init__.py
--rw-r--r--   0        0        0     2749 2024-04-12 13:44:26.949841 metricsreport-2024.4.20/metricsreport/custom_metrics.py
--rw-r--r--   0        0        0    30080 2024-04-12 14:09:44.817364 metricsreport-2024.4.20/metricsreport/metricsreport.py
--rw-r--r--   0        0        0      577 2024-04-12 14:13:26.421857 metricsreport-2024.4.20/pyproject.toml
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 metricsreport-2024.4.20/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-12 13:44:26.925841 metricsreport-2024.5.15/LICENSE
+-rw-r--r--   0        0        0     2322 2024-04-12 13:44:26.925841 metricsreport-2024.5.15/README.md
+-rw-r--r--   0        0        0       98 2024-05-15 20:12:08.662664 metricsreport-2024.5.15/metricsreport/__init__.py
+-rw-r--r--   0        0        0     2749 2024-04-12 13:44:26.949841 metricsreport-2024.5.15/metricsreport/custom_metrics.py
+-rw-r--r--   0        0        0    50176 2024-05-15 20:23:07.887542 metricsreport-2024.5.15/metricsreport/metricsreport.py
+-rw-r--r--   0        0        0      564 2024-05-15 18:16:48.679241 metricsreport-2024.5.15/pyproject.toml
+-rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 metricsreport-2024.5.15/PKG-INFO
```

### Comparing `metricsreport-2024.4.20/LICENSE` & `metricsreport-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `metricsreport-2024.4.20/README.md` & `metricsreport-2024.5.15/README.md`

 * *Files identical despite different names*

### Comparing `metricsreport-2024.4.20/metricsreport/custom_metrics.py` & `metricsreport-2024.5.15/metricsreport/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `metricsreport-2024.4.20/PKG-INFO` & `metricsreport-2024.5.15/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: metricsreport
-Version: 2024.4.20
+Version: 2024.5.15
 Summary: Generating reports on metrics for Machine Learning models
 Home-page: https://github.com/Alex-Lekov/metricsreport
 Author: Alex Lekov
 Author-email: 11148364-AlexLekov@users.noreply.gitlab.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: plot-metric (>=0.0.6,<0.0.7)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
-Requires-Dist: scikit-plot (>=0.3.7,<0.4.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Project-URL: Repository, https://github.com/Alex-Lekov/metricsreport
 Description-Content-Type: text/markdown
 
 # Metrics Report
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/metricsreport) 
 ![PyPI](https://img.shields.io/pypi/v/metricsreport)
```

