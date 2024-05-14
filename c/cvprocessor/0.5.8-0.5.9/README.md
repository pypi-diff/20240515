# Comparing `tmp/cvprocessor-0.5.8.tar.gz` & `tmp/cvprocessor-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.5.8.tar", last modified: Tue May 14 08:07:22 2024, max compression
+gzip compressed data, was "cvprocessor-0.5.9.tar", last modified: Tue May 14 08:11:25 2024, max compression
```

## Comparing `cvprocessor-0.5.8.tar` & `cvprocessor-0.5.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:07:22.108686 cvprocessor-0.5.8/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.8/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:07:22.107955 cvprocessor-0.5.8/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.8/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 08:06:50.000000 cvprocessor-0.5.8/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 08:07:22.108809 cvprocessor-0.5.8/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:07:22.092789 cvprocessor-0.5.8/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:07:22.104161 cvprocessor-0.5.8/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.8/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)    10569 2024-05-14 06:57:49.000000 cvprocessor-0.5.8/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.8/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     9312 2024-05-14 08:06:44.000000 cvprocessor-0.5.8/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.8/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.8/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.8/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     6731 2024-05-14 06:59:18.000000 cvprocessor-0.5.8/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.8/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.8/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.8/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    18348 2024-05-14 08:03:10.000000 cvprocessor-0.5.8/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.8/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-14 08:06:36.000000 cvprocessor-0.5.8/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.8/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.8/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     6050 2024-05-14 07:37:26.000000 cvprocessor-0.5.8/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.8/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.8/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:07:22.107141 cvprocessor-0.5.8/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 08:07:22.000000 cvprocessor-0.5.8/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:11:25.218123 cvprocessor-0.5.9/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.5.9/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:11:25.217465 cvprocessor-0.5.9/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.5.9/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-14 08:10:44.000000 cvprocessor-0.5.9/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-14 08:11:25.218239 cvprocessor-0.5.9/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:11:25.200479 cvprocessor-0.5.9/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:11:25.213076 cvprocessor-0.5.9/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.5.9/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)    10569 2024-05-14 06:57:49.000000 cvprocessor-0.5.9/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-13 06:25:00.000000 cvprocessor-0.5.9/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9312 2024-05-14 08:06:44.000000 cvprocessor-0.5.9/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5199 2024-05-14 06:09:41.000000 cvprocessor-0.5.9/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5577 2024-05-14 06:10:28.000000 cvprocessor-0.5.9/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3317 2024-05-14 06:24:49.000000 cvprocessor-0.5.9/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6731 2024-05-14 06:59:18.000000 cvprocessor-0.5.9/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1547 2024-05-14 04:41:36.000000 cvprocessor-0.5.9/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1630 2024-05-14 06:28:31.000000 cvprocessor-0.5.9/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3458 2024-05-14 06:21:07.000000 cvprocessor-0.5.9/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    18348 2024-05-14 08:03:10.000000 cvprocessor-0.5.9/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2147 2024-05-14 06:29:12.000000 cvprocessor-0.5.9/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-14 08:06:36.000000 cvprocessor-0.5.9/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2123 2024-05-14 06:27:58.000000 cvprocessor-0.5.9/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2938 2024-05-14 06:27:29.000000 cvprocessor-0.5.9/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6111 2024-05-14 08:10:16.000000 cvprocessor-0.5.9/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4702 2024-05-14 06:26:31.000000 cvprocessor-0.5.9/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7223 2024-05-14 06:25:31.000000 cvprocessor-0.5.9/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-14 08:11:25.216785 cvprocessor-0.5.9/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-14 08:11:25.000000 cvprocessor-0.5.9/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.5.8/LICENSE` & `cvprocessor-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/PKG-INFO` & `cvprocessor-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.8
+Version: 0.5.9
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.8/README.md` & `cvprocessor-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/pyproject.toml` & `cvprocessor-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.5.8"
+version = "0.5.9"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.5.8/src/cvprocessor/authors.py` & `cvprocessor-0.5.9/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/cv.py` & `cvprocessor-0.5.9/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/education.py` & `cvprocessor-0.5.9/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/experience.py` & `cvprocessor-0.5.9/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/grants_awards.py` & `cvprocessor-0.5.9/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/institutes.py` & `cvprocessor-0.5.9/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/intro.py` & `cvprocessor-0.5.9/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/memberships.py` & `cvprocessor-0.5.9/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/news.py` & `cvprocessor-0.5.9/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/publications.py` & `cvprocessor-0.5.9/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/references.py` & `cvprocessor-0.5.9/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/research_interests.py` & `cvprocessor-0.5.9/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/service.py` & `cvprocessor-0.5.9/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/skills.py` & `cvprocessor-0.5.9/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/software.py` & `cvprocessor-0.5.9/src/cvprocessor/software.py`

 * *Files 4% similar despite different names*

```diff
@@ -229,7 +229,10 @@
         for software in self.softwares:
             string += str(software) + "\n"
         return string
 
     def __repr__(self) -> str:
         string = f"Software(software={repr(self.softwares)})"
         return string
+
+    def __iter__(self):
+        return iter(self.softwares)
```

### Comparing `cvprocessor-0.5.8/src/cvprocessor/supervision.py` & `cvprocessor-0.5.9/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor/teaching.py` & `cvprocessor-0.5.9/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.5.8/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.5.9/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.5.8
+Version: 0.5.9
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.5.8/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.5.9/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

