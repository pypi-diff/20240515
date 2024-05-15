# Comparing `tmp/isotree-0.6.1.post2.tar.gz` & `tmp/isotree-0.6.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isotree-0.6.1.post2.tar", last modified: Sat Feb 24 09:40:45 2024, max compression
+gzip compressed data, was "isotree-0.6.1.post3.tar", last modified: Wed May 15 15:35:26 2024, max compression
```

## Comparing `isotree-0.6.1.post2.tar` & `isotree-0.6.1.post3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-24 09:40:45.266133 isotree-0.6.1.post2/
--rw-r--r--   0 david     (1000) david     (1000)      434 2024-02-08 21:16:17.000000 isotree-0.6.1.post2/.gitignore
--rw-r--r--   0 david     (1000) david     (1000)     1327 2024-01-13 18:37:47.000000 isotree-0.6.1.post2/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     1070 2022-02-12 16:38:44.000000 isotree-0.6.1.post2/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      266 2024-02-24 09:40:45.262133 isotree-0.6.1.post2/PKG-INFO
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-24 09:40:45.262133 isotree-0.6.1.post2/isotree/
--rw-r--r--   0 david     (1000) david     (1000)   235993 2024-02-24 09:28:01.000000 isotree-0.6.1.post2/isotree/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    79170 2024-02-08 21:05:22.000000 isotree-0.6.1.post2/isotree/cpp_interface.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-24 09:40:45.262133 isotree-0.6.1.post2/isotree.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      266 2024-02-24 09:40:45.000000 isotree-0.6.1.post2/isotree.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      913 2024-02-24 09:40:45.000000 isotree-0.6.1.post2/isotree.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2024-02-24 09:40:45.000000 isotree-0.6.1.post2/isotree.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)        8 2024-02-24 09:40:45.000000 isotree-0.6.1.post2/isotree.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       82 2023-07-18 17:26:20.000000 isotree-0.6.1.post2/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       55 2023-07-18 17:25:53.000000 isotree-0.6.1.post2/requirements.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2024-02-24 09:40:45.266133 isotree-0.6.1.post2/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    14950 2024-02-24 09:07:40.000000 isotree-0.6.1.post2/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-24 09:40:45.262133 isotree-0.6.1.post2/src/
--rw-r--r--   0 david     (1000) david     (1000)   165890 2023-06-25 12:50:10.000000 isotree-0.6.1.post2/src/crit.hpp
--rw-r--r--   0 david     (1000) david     (1000)     6047 2023-02-09 16:54:59.000000 isotree-0.6.1.post2/src/digamma.hpp
--rw-r--r--   0 david     (1000) david     (1000)    88088 2023-12-01 17:28:02.000000 isotree-0.6.1.post2/src/dist.hpp
--rw-r--r--   0 david     (1000) david     (1000)    11715 2022-02-12 15:02:28.000000 isotree-0.6.1.post2/src/exp_depth_table.hpp
--rw-r--r--   0 david     (1000) david     (1000)    73015 2022-02-11 17:02:46.000000 isotree-0.6.1.post2/src/extended.hpp
--rw-r--r--   0 david     (1000) david     (1000)   138108 2023-12-01 17:28:39.000000 isotree-0.6.1.post2/src/fit_model.hpp
--rw-r--r--   0 david     (1000) david     (1000)    42221 2024-01-24 19:00:56.000000 isotree-0.6.1.post2/src/formatted_exporters.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4327 2022-01-17 02:22:39.000000 isotree-0.6.1.post2/src/headers_joined.hpp
--rw-r--r--   0 david     (1000) david     (1000)    40171 2023-06-25 12:50:21.000000 isotree-0.6.1.post2/src/helpers_iforest.hpp
--rw-r--r--   0 david     (1000) david     (1000)    58458 2023-12-01 17:30:07.000000 isotree-0.6.1.post2/src/impute.hpp
--rw-r--r--   0 david     (1000) david     (1000)    18580 2024-01-21 18:14:39.000000 isotree-0.6.1.post2/src/indexer.cpp
--rw-r--r--   0 david     (1000) david     (1000)    13338 2022-02-12 00:01:04.000000 isotree-0.6.1.post2/src/instantiate_template_headers.hpp
--rw-r--r--   0 david     (1000) david     (1000)    94130 2024-02-08 19:57:07.000000 isotree-0.6.1.post2/src/isoforest.hpp
--rw-r--r--   0 david     (1000) david     (1000)   124488 2024-02-08 20:10:14.000000 isotree-0.6.1.post2/src/isotree.hpp
--rw-r--r--   0 david     (1000) david     (1000)    14049 2024-01-13 18:55:29.000000 isotree-0.6.1.post2/src/merge_models.cpp
--rw-r--r--   0 david     (1000) david     (1000)    48374 2024-01-13 19:21:15.000000 isotree-0.6.1.post2/src/mult.hpp
--rw-r--r--   0 david     (1000) david     (1000)     9764 2022-03-28 19:16:28.000000 isotree-0.6.1.post2/src/other_helpers.hpp
--rw-r--r--   0 david     (1000) david     (1000)    90971 2024-02-08 20:43:55.000000 isotree-0.6.1.post2/src/predict.hpp
--rw-r--r--   0 david     (1000) david     (1000)     4435 2023-07-21 16:27:45.000000 isotree-0.6.1.post2/src/python_helpers.hpp
--rw-r--r--   0 david     (1000) david     (1000)     7886 2024-01-21 18:16:42.000000 isotree-0.6.1.post2/src/ref_indexer.hpp
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-24 09:40:45.262133 isotree-0.6.1.post2/src/robinmap/
--rw-r--r--   0 david     (1000) david     (1000)     1102 2021-07-16 23:59:38.000000 isotree-0.6.1.post2/src/robinmap/LICENSE
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-24 09:40:45.262133 isotree-0.6.1.post2/src/robinmap/include/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-24 09:40:45.262133 isotree-0.6.1.post2/src/robinmap/include/tsl/
--rw-r--r--   0 david     (1000) david     (1000)    11776 2022-05-13 19:14:51.000000 isotree-0.6.1.post2/src/robinmap/include/tsl/robin_growth_policy.h
--rw-r--r--   0 david     (1000) david     (1000)    54583 2024-01-24 20:05:52.000000 isotree-0.6.1.post2/src/robinmap/include/tsl/robin_hash.h
--rw-r--r--   0 david     (1000) david     (1000)    28414 2022-05-13 19:14:51.000000 isotree-0.6.1.post2/src/robinmap/include/tsl/robin_map.h
--rw-r--r--   0 david     (1000) david     (1000)    23593 2021-07-16 23:59:38.000000 isotree-0.6.1.post2/src/robinmap/include/tsl/robin_set.h
--rw-r--r--   0 david     (1000) david     (1000)   135986 2023-12-01 17:30:16.000000 isotree-0.6.1.post2/src/serialize.cpp
--rw-r--r--   0 david     (1000) david     (1000)    30994 2024-01-18 19:22:06.000000 isotree-0.6.1.post2/src/sql.cpp
--rw-r--r--   0 david     (1000) david     (1000)     9378 2024-01-13 18:56:13.000000 isotree-0.6.1.post2/src/subset_models.cpp
--rw-r--r--   0 david     (1000) david     (1000)   129953 2024-01-13 19:26:19.000000 isotree-0.6.1.post2/src/utils.hpp
--rw-r--r--   0 david     (1000) david     (1000)    14648 2023-11-08 20:02:48.000000 isotree-0.6.1.post2/src/xoshiro.hpp
--rw-r--r--   0 david     (1000) david     (1000)    24394 2022-02-10 01:40:29.000000 isotree-0.6.1.post2/src/ziggurat.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-05-15 15:35:26.545972 isotree-0.6.1.post3/
+-rw-r--r--   0 david     (1000) david     (1000)      434 2024-02-08 21:16:17.000000 isotree-0.6.1.post3/.gitignore
+-rw-r--r--   0 david     (1000) david     (1000)     1327 2024-01-13 18:37:47.000000 isotree-0.6.1.post3/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)     1070 2022-02-12 16:38:44.000000 isotree-0.6.1.post3/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      266 2024-05-15 15:35:26.545972 isotree-0.6.1.post3/PKG-INFO
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-05-15 15:35:26.541972 isotree-0.6.1.post3/isotree/
+-rw-r--r--   0 david     (1000) david     (1000)   236216 2024-05-15 15:34:38.000000 isotree-0.6.1.post3/isotree/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)    79170 2024-02-08 21:05:22.000000 isotree-0.6.1.post3/isotree/cpp_interface.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-05-15 15:35:26.541972 isotree-0.6.1.post3/isotree.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      266 2024-05-15 15:35:26.000000 isotree-0.6.1.post3/isotree.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      913 2024-05-15 15:35:26.000000 isotree-0.6.1.post3/isotree.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2024-05-15 15:35:26.000000 isotree-0.6.1.post3/isotree.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)        8 2024-05-15 15:35:26.000000 isotree-0.6.1.post3/isotree.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       82 2023-07-18 17:26:20.000000 isotree-0.6.1.post3/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       55 2023-07-18 17:25:53.000000 isotree-0.6.1.post3/requirements.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2024-05-15 15:35:26.545972 isotree-0.6.1.post3/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    14950 2024-05-15 15:34:38.000000 isotree-0.6.1.post3/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-05-15 15:35:26.541972 isotree-0.6.1.post3/src/
+-rw-r--r--   0 david     (1000) david     (1000)   165890 2023-06-25 12:50:10.000000 isotree-0.6.1.post3/src/crit.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     6047 2023-02-09 16:54:59.000000 isotree-0.6.1.post3/src/digamma.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    88088 2023-12-01 17:28:02.000000 isotree-0.6.1.post3/src/dist.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    11715 2022-02-12 15:02:28.000000 isotree-0.6.1.post3/src/exp_depth_table.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    73015 2022-02-11 17:02:46.000000 isotree-0.6.1.post3/src/extended.hpp
+-rw-r--r--   0 david     (1000) david     (1000)   138108 2023-12-01 17:28:39.000000 isotree-0.6.1.post3/src/fit_model.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    42221 2024-01-24 19:00:56.000000 isotree-0.6.1.post3/src/formatted_exporters.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4327 2022-01-17 02:22:39.000000 isotree-0.6.1.post3/src/headers_joined.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    40171 2023-06-25 12:50:21.000000 isotree-0.6.1.post3/src/helpers_iforest.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    58458 2023-12-01 17:30:07.000000 isotree-0.6.1.post3/src/impute.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    18580 2024-01-21 18:14:39.000000 isotree-0.6.1.post3/src/indexer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13338 2022-02-12 00:01:04.000000 isotree-0.6.1.post3/src/instantiate_template_headers.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    94130 2024-02-08 19:57:07.000000 isotree-0.6.1.post3/src/isoforest.hpp
+-rw-r--r--   0 david     (1000) david     (1000)   124620 2024-04-12 09:45:31.000000 isotree-0.6.1.post3/src/isotree.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    14049 2024-01-13 18:55:29.000000 isotree-0.6.1.post3/src/merge_models.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    48374 2024-01-13 19:21:15.000000 isotree-0.6.1.post3/src/mult.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     9764 2022-03-28 19:16:28.000000 isotree-0.6.1.post3/src/other_helpers.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    90971 2024-02-08 20:43:55.000000 isotree-0.6.1.post3/src/predict.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     4435 2023-07-21 16:27:45.000000 isotree-0.6.1.post3/src/python_helpers.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     7886 2024-01-21 18:16:42.000000 isotree-0.6.1.post3/src/ref_indexer.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-05-15 15:35:26.541972 isotree-0.6.1.post3/src/robinmap/
+-rw-r--r--   0 david     (1000) david     (1000)     1102 2021-07-16 23:59:38.000000 isotree-0.6.1.post3/src/robinmap/LICENSE
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-05-15 15:35:26.541972 isotree-0.6.1.post3/src/robinmap/include/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-05-15 15:35:26.545972 isotree-0.6.1.post3/src/robinmap/include/tsl/
+-rw-r--r--   0 david     (1000) david     (1000)    11776 2022-05-13 19:14:51.000000 isotree-0.6.1.post3/src/robinmap/include/tsl/robin_growth_policy.h
+-rw-r--r--   0 david     (1000) david     (1000)    54583 2024-01-24 20:05:52.000000 isotree-0.6.1.post3/src/robinmap/include/tsl/robin_hash.h
+-rw-r--r--   0 david     (1000) david     (1000)    28414 2022-05-13 19:14:51.000000 isotree-0.6.1.post3/src/robinmap/include/tsl/robin_map.h
+-rw-r--r--   0 david     (1000) david     (1000)    23593 2021-07-16 23:59:38.000000 isotree-0.6.1.post3/src/robinmap/include/tsl/robin_set.h
+-rw-r--r--   0 david     (1000) david     (1000)   135986 2023-12-01 17:30:16.000000 isotree-0.6.1.post3/src/serialize.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    30994 2024-01-18 19:22:06.000000 isotree-0.6.1.post3/src/sql.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     9378 2024-01-13 18:56:13.000000 isotree-0.6.1.post3/src/subset_models.cpp
+-rw-r--r--   0 david     (1000) david     (1000)   129953 2024-01-13 19:26:19.000000 isotree-0.6.1.post3/src/utils.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    14648 2023-11-08 20:02:48.000000 isotree-0.6.1.post3/src/xoshiro.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    24394 2022-02-10 01:40:29.000000 isotree-0.6.1.post3/src/ziggurat.hpp
```

### Comparing `isotree-0.6.1.post2/LICENSE` & `isotree-0.6.1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/MANIFEST.in` & `isotree-0.6.1.post3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/isotree/__init__.py` & `isotree-0.6.1.post3/isotree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4262,9 +4262,17 @@
                     msg += " Be sure to change these parameters if refitting this model or adding trees."
                 warnings.warn(msg)
 
         self.is_fitted_ = True
         self._is_extended_ = self.ndim_ > 1
         return self
 
-    def __is_fitted__(self):
+    def __sklearn_is_fitted__(self):
         return self.is_fitted_
+
+    @property
+    def _doc_link_module(self):
+        return "isotree"
+
+    @property
+    def _doc_link_template(self):
+        return f"https://isotree.readthedocs.io/en/latest/#isotree.{self.__class__.__name__}"
```

### Comparing `isotree-0.6.1.post2/isotree/cpp_interface.pyx` & `isotree-0.6.1.post3/isotree/cpp_interface.pyx`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/isotree.egg-info/SOURCES.txt` & `isotree-0.6.1.post3/isotree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/setup.py` & `isotree-0.6.1.post3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
             for e in self.extensions:
                 e.define_macros += [("SUPPORTS_RESTRICT", "1")]
 
 
 setup(
     name  = "isotree",
     packages = ["isotree"],
-    version = '0.6.1-2',
+    version = '0.6.1-3',
     description = 'Isolation-Based Outlier Detection, Distance, and NA imputation',
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/isotree',
     keywords = ['isolation-forest', 'anomaly', 'outlier'],
     cmdclass = {'build_ext': build_ext_subclass},
     ext_modules = [Extension(
                                 "isotree._cpp_interface",
```

### Comparing `isotree-0.6.1.post2/src/crit.hpp` & `isotree-0.6.1.post3/src/crit.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/digamma.hpp` & `isotree-0.6.1.post3/src/digamma.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/dist.hpp` & `isotree-0.6.1.post3/src/dist.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/exp_depth_table.hpp` & `isotree-0.6.1.post3/src/exp_depth_table.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/extended.hpp` & `isotree-0.6.1.post3/src/extended.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/fit_model.hpp` & `isotree-0.6.1.post3/src/fit_model.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/formatted_exporters.cpp` & `isotree-0.6.1.post3/src/formatted_exporters.cpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/headers_joined.hpp` & `isotree-0.6.1.post3/src/headers_joined.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/helpers_iforest.hpp` & `isotree-0.6.1.post3/src/helpers_iforest.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/impute.hpp` & `isotree-0.6.1.post3/src/impute.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/indexer.cpp` & `isotree-0.6.1.post3/src/indexer.cpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/instantiate_template_headers.hpp` & `isotree-0.6.1.post3/src/instantiate_template_headers.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/isoforest.hpp` & `isotree-0.6.1.post3/src/isoforest.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/isotree.hpp` & `isotree-0.6.1.post3/src/isotree.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -263,28 +263,31 @@
         #define size_t_for size_t
     #endif
 #else
     #define size_t_for size_t
 #endif
 
 #if defined(_FOR_R) || defined(_FOR_PYTHON)
-    #define ISOTREE_EXPORTED 
+    #define ISOTREE_EXPORTED
+    #define ISOTREE_EXPORTED_FRIEND
 #else
     #if defined(_WIN32)
         #ifdef ISOTREE_COMPILE_TIME
             #define ISOTREE_EXPORTED __declspec(dllexport)
         #else
             #define ISOTREE_EXPORTED __declspec(dllimport)
         #endif
+        #define ISOTREE_EXPORTED_FRIEND ISOTREE_EXPORTED
     #else
         #if defined(EXPLICITLTY_EXPORT_SYMBOLS) && defined(ISOTREE_COMPILE_TIME)
             #define ISOTREE_EXPORTED [[gnu::visibility("default")]]
         #else
             #define ISOTREE_EXPORTED 
         #endif
+        #define ISOTREE_EXPORTED_FRIEND
     #endif
 #endif
 
 #ifndef unreachable
 #   if (__cplusplus >= 202309L)
 #       include <utility>
         using std::unreachable;
```

### Comparing `isotree-0.6.1.post2/src/merge_models.cpp` & `isotree-0.6.1.post3/src/merge_models.cpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/mult.hpp` & `isotree-0.6.1.post3/src/mult.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/other_helpers.hpp` & `isotree-0.6.1.post3/src/other_helpers.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/predict.hpp` & `isotree-0.6.1.post3/src/predict.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/python_helpers.hpp` & `isotree-0.6.1.post3/src/python_helpers.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/ref_indexer.hpp` & `isotree-0.6.1.post3/src/ref_indexer.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/robinmap/LICENSE` & `isotree-0.6.1.post3/src/robinmap/LICENSE`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/robinmap/include/tsl/robin_growth_policy.h` & `isotree-0.6.1.post3/src/robinmap/include/tsl/robin_growth_policy.h`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/robinmap/include/tsl/robin_hash.h` & `isotree-0.6.1.post3/src/robinmap/include/tsl/robin_hash.h`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/robinmap/include/tsl/robin_map.h` & `isotree-0.6.1.post3/src/robinmap/include/tsl/robin_map.h`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/robinmap/include/tsl/robin_set.h` & `isotree-0.6.1.post3/src/robinmap/include/tsl/robin_set.h`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/serialize.cpp` & `isotree-0.6.1.post3/src/serialize.cpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/sql.cpp` & `isotree-0.6.1.post3/src/sql.cpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/subset_models.cpp` & `isotree-0.6.1.post3/src/subset_models.cpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/utils.hpp` & `isotree-0.6.1.post3/src/utils.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/xoshiro.hpp` & `isotree-0.6.1.post3/src/xoshiro.hpp`

 * *Files identical despite different names*

### Comparing `isotree-0.6.1.post2/src/ziggurat.hpp` & `isotree-0.6.1.post3/src/ziggurat.hpp`

 * *Files identical despite different names*

