# Comparing `tmp/cvprocessor-0.6.2.tar.gz` & `tmp/cvprocessor-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.6.2.tar", last modified: Wed May 15 07:10:53 2024, max compression
+gzip compressed data, was "cvprocessor-0.6.3.tar", last modified: Wed May 15 07:14:11 2024, max compression
```

## Comparing `cvprocessor-0.6.2.tar` & `cvprocessor-0.6.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:10:53.447674 cvprocessor-0.6.2/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.6.2/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 07:10:53.446960 cvprocessor-0.6.2/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.6.2/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-15 07:10:41.000000 cvprocessor-0.6.2/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-15 07:10:53.447801 cvprocessor-0.6.2/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:10:53.423473 cvprocessor-0.6.2/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:10:53.443017 cvprocessor-0.6.2/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.6.2/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)    10464 2024-05-15 03:47:26.000000 cvprocessor-0.6.2/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-15 02:16:23.000000 cvprocessor-0.6.2/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     7750 2024-05-15 05:44:19.000000 cvprocessor-0.6.2/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     4882 2024-05-15 03:56:47.000000 cvprocessor-0.6.2/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     3758 2024-05-15 04:08:11.000000 cvprocessor-0.6.2/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     4051 2024-05-15 03:58:18.000000 cvprocessor-0.6.2/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     7113 2024-05-15 04:39:45.000000 cvprocessor-0.6.2/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-0.6.2/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1921 2024-05-15 04:10:03.000000 cvprocessor-0.6.2/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     4435 2024-05-15 04:11:19.000000 cvprocessor-0.6.2/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    16444 2024-05-15 07:10:24.000000 cvprocessor-0.6.2/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2697 2024-05-15 04:26:24.000000 cvprocessor-0.6.2/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-15 04:26:39.000000 cvprocessor-0.6.2/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2540 2024-05-15 04:27:18.000000 cvprocessor-0.6.2/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     3316 2024-05-15 04:27:50.000000 cvprocessor-0.6.2/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     4916 2024-05-15 04:39:59.000000 cvprocessor-0.6.2/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     5247 2024-05-15 04:39:23.000000 cvprocessor-0.6.2/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     5270 2024-05-15 02:19:52.000000 cvprocessor-0.6.2/src/cvprocessor/teaching.py
--rw-r--r--   0 fernando   (501) staff       (20)     3482 2024-05-15 02:26:14.000000 cvprocessor-0.6.2/src/cvprocessor/year_data.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:10:53.446337 cvprocessor-0.6.2/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 07:10:53.000000 cvprocessor-0.6.2/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      800 2024-05-15 07:10:53.000000 cvprocessor-0.6.2/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-15 07:10:53.000000 cvprocessor-0.6.2/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-15 07:10:53.000000 cvprocessor-0.6.2/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-15 07:10:53.000000 cvprocessor-0.6.2/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:14:11.199509 cvprocessor-0.6.3/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.6.3/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 07:14:11.198949 cvprocessor-0.6.3/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.6.3/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-15 07:14:00.000000 cvprocessor-0.6.3/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-15 07:14:11.199616 cvprocessor-0.6.3/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:14:11.178081 cvprocessor-0.6.3/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:14:11.195120 cvprocessor-0.6.3/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.6.3/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)    10464 2024-05-15 03:47:26.000000 cvprocessor-0.6.3/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-15 02:16:23.000000 cvprocessor-0.6.3/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7750 2024-05-15 05:44:19.000000 cvprocessor-0.6.3/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4882 2024-05-15 03:56:47.000000 cvprocessor-0.6.3/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3758 2024-05-15 04:08:11.000000 cvprocessor-0.6.3/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4051 2024-05-15 03:58:18.000000 cvprocessor-0.6.3/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7113 2024-05-15 04:39:45.000000 cvprocessor-0.6.3/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-0.6.3/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1921 2024-05-15 04:10:03.000000 cvprocessor-0.6.3/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4435 2024-05-15 04:11:19.000000 cvprocessor-0.6.3/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    16444 2024-05-15 07:13:13.000000 cvprocessor-0.6.3/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2697 2024-05-15 04:26:24.000000 cvprocessor-0.6.3/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-15 04:26:39.000000 cvprocessor-0.6.3/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2540 2024-05-15 04:27:18.000000 cvprocessor-0.6.3/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3316 2024-05-15 04:27:50.000000 cvprocessor-0.6.3/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4916 2024-05-15 04:39:59.000000 cvprocessor-0.6.3/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5247 2024-05-15 04:39:23.000000 cvprocessor-0.6.3/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5270 2024-05-15 02:19:52.000000 cvprocessor-0.6.3/src/cvprocessor/teaching.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3482 2024-05-15 02:26:14.000000 cvprocessor-0.6.3/src/cvprocessor/year_data.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:14:11.198349 cvprocessor-0.6.3/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 07:14:11.000000 cvprocessor-0.6.3/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      800 2024-05-15 07:14:11.000000 cvprocessor-0.6.3/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-15 07:14:11.000000 cvprocessor-0.6.3/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-15 07:14:11.000000 cvprocessor-0.6.3/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-15 07:14:11.000000 cvprocessor-0.6.3/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.6.2/LICENSE` & `cvprocessor-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/PKG-INFO` & `cvprocessor-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.6.2
+Version: 0.6.3
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.6.2/README.md` & `cvprocessor-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/pyproject.toml` & `cvprocessor-0.6.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.6.2/src/cvprocessor/authors.py` & `cvprocessor-0.6.3/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/cv.py` & `cvprocessor-0.6.3/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/education.py` & `cvprocessor-0.6.3/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/experience.py` & `cvprocessor-0.6.3/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/grants_awards.py` & `cvprocessor-0.6.3/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/institutes.py` & `cvprocessor-0.6.3/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/intro.py` & `cvprocessor-0.6.3/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/memberships.py` & `cvprocessor-0.6.3/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/news.py` & `cvprocessor-0.6.3/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/publications.py` & `cvprocessor-0.6.3/src/cvprocessor/publications.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,15 +554,15 @@
         publications_df = pd.read_excel(
             filename, sheet_name="Publications")
         for _, row in publications_df.iterrows():
             self.publications.append(PublicationsData())
             self.publications[-1].load(row)
         self.publications = sorted(
             self.publications, key=lambda x: (
-                x.details.get_year(), x.details.get_title()), reverse=True
+                x.details.get_date(), x.details.get_title()), reverse=True
         )
 
     def __str__(self):
         string = ""
         for publication in self.publications:
             string += str(publication) + "\n\n"
         return string
```

### Comparing `cvprocessor-0.6.2/src/cvprocessor/references.py` & `cvprocessor-0.6.3/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/research_interests.py` & `cvprocessor-0.6.3/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/service.py` & `cvprocessor-0.6.3/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/skills.py` & `cvprocessor-0.6.3/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/software.py` & `cvprocessor-0.6.3/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/supervision.py` & `cvprocessor-0.6.3/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/teaching.py` & `cvprocessor-0.6.3/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor/year_data.py` & `cvprocessor-0.6.3/src/cvprocessor/year_data.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.2/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.6.3/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.6.2
+Version: 0.6.3
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.6.2/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.6.3/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

