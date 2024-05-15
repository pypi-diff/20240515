# Comparing `tmp/cvprocessor-0.6.0.tar.gz` & `tmp/cvprocessor-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.6.0.tar", last modified: Wed May 15 04:49:41 2024, max compression
+gzip compressed data, was "cvprocessor-0.6.1.tar", last modified: Wed May 15 05:14:15 2024, max compression
```

## Comparing `cvprocessor-0.6.0.tar` & `cvprocessor-0.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 04:49:41.189552 cvprocessor-0.6.0/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.6.0/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 04:49:41.188759 cvprocessor-0.6.0/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.6.0/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-15 04:48:58.000000 cvprocessor-0.6.0/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-15 04:49:41.189710 cvprocessor-0.6.0/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 04:49:41.163948 cvprocessor-0.6.0/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 04:49:41.183695 cvprocessor-0.6.0/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.6.0/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)    10464 2024-05-15 03:47:26.000000 cvprocessor-0.6.0/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-15 02:16:23.000000 cvprocessor-0.6.0/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     7888 2024-05-15 04:48:38.000000 cvprocessor-0.6.0/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     4882 2024-05-15 03:56:47.000000 cvprocessor-0.6.0/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     3758 2024-05-15 04:08:11.000000 cvprocessor-0.6.0/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     4051 2024-05-15 03:58:18.000000 cvprocessor-0.6.0/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     7113 2024-05-15 04:39:45.000000 cvprocessor-0.6.0/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-0.6.0/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1921 2024-05-15 04:10:03.000000 cvprocessor-0.6.0/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     4435 2024-05-15 04:11:19.000000 cvprocessor-0.6.0/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    16102 2024-05-15 04:47:01.000000 cvprocessor-0.6.0/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2697 2024-05-15 04:26:24.000000 cvprocessor-0.6.0/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-15 04:26:39.000000 cvprocessor-0.6.0/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2540 2024-05-15 04:27:18.000000 cvprocessor-0.6.0/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     3316 2024-05-15 04:27:50.000000 cvprocessor-0.6.0/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     4916 2024-05-15 04:39:59.000000 cvprocessor-0.6.0/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     5247 2024-05-15 04:39:23.000000 cvprocessor-0.6.0/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     5270 2024-05-15 02:19:52.000000 cvprocessor-0.6.0/src/cvprocessor/teaching.py
--rw-r--r--   0 fernando   (501) staff       (20)     3482 2024-05-15 02:26:14.000000 cvprocessor-0.6.0/src/cvprocessor/year_data.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 04:49:41.187940 cvprocessor-0.6.0/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      800 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-15 04:49:41.000000 cvprocessor-0.6.0/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 05:14:15.198000 cvprocessor-0.6.1/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.6.1/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 05:14:15.197326 cvprocessor-0.6.1/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.6.1/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-15 05:13:46.000000 cvprocessor-0.6.1/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-15 05:14:15.198120 cvprocessor-0.6.1/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 05:14:15.172019 cvprocessor-0.6.1/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 05:14:15.192234 cvprocessor-0.6.1/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.6.1/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)    10464 2024-05-15 03:47:26.000000 cvprocessor-0.6.1/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-15 02:16:23.000000 cvprocessor-0.6.1/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7742 2024-05-15 05:13:02.000000 cvprocessor-0.6.1/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4882 2024-05-15 03:56:47.000000 cvprocessor-0.6.1/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3758 2024-05-15 04:08:11.000000 cvprocessor-0.6.1/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4051 2024-05-15 03:58:18.000000 cvprocessor-0.6.1/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7113 2024-05-15 04:39:45.000000 cvprocessor-0.6.1/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-0.6.1/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1921 2024-05-15 04:10:03.000000 cvprocessor-0.6.1/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4435 2024-05-15 04:11:19.000000 cvprocessor-0.6.1/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    16444 2024-05-15 05:13:34.000000 cvprocessor-0.6.1/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2697 2024-05-15 04:26:24.000000 cvprocessor-0.6.1/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-15 04:26:39.000000 cvprocessor-0.6.1/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2540 2024-05-15 04:27:18.000000 cvprocessor-0.6.1/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3316 2024-05-15 04:27:50.000000 cvprocessor-0.6.1/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4916 2024-05-15 04:39:59.000000 cvprocessor-0.6.1/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5247 2024-05-15 04:39:23.000000 cvprocessor-0.6.1/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5270 2024-05-15 02:19:52.000000 cvprocessor-0.6.1/src/cvprocessor/teaching.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3482 2024-05-15 02:26:14.000000 cvprocessor-0.6.1/src/cvprocessor/year_data.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 05:14:15.196616 cvprocessor-0.6.1/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 05:14:15.000000 cvprocessor-0.6.1/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      800 2024-05-15 05:14:15.000000 cvprocessor-0.6.1/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-15 05:14:15.000000 cvprocessor-0.6.1/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-15 05:14:15.000000 cvprocessor-0.6.1/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-15 05:14:15.000000 cvprocessor-0.6.1/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.6.0/LICENSE` & `cvprocessor-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/PKG-INFO` & `cvprocessor-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.6.0
+Version: 0.6.1
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.6.0/README.md` & `cvprocessor-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/pyproject.toml` & `cvprocessor-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.6.0/src/cvprocessor/authors.py` & `cvprocessor-0.6.1/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/cv.py` & `cvprocessor-0.6.1/src/cvprocessor/cv.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,33 +162,21 @@
         authors_ids = []
         for author_id in authors_ids_affiliations_ids:
             authors_ids.append(author_id.get_author_id())
         authors_alias_short = []
         for author_id in authors_ids:
             author = self.personal.authors.get_author(author_id)
             if author is not None:
-                authors_alias_short.append(author.get_alias_short())
+                authors_alias_short.append(author.personal.get_alias_short())
         if len(authors_alias_short) > 1:
             authors_alias_short[-1] = "& " + authors_alias_short[-1]
         authors_alias_short = ", ".join(authors_alias_short)
         apa = authors_alias_short + apa
         return apa
 
-    def get_research_interests(self):
-        """
-        The get_research_interests method is used to get the research interests.
-        """
-        return self.academic.research_interests.get_interests()
-
-    def get_research_keywords(self):
-        """
-        The get_research_keywords method is used to get the research keywords.
-        """
-        return self.academic.research_interests.get_keywords()
-
     def _load_cv(self, filename):
         """
         The _load_cv method is used to load the CV file.
 
         :param filename: The filename of the CV file.
         :type filename: str
         """
@@ -227,8 +215,13 @@
             f"news={repr(self.news)})\n")
         return string
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
     print(str(cv.personal.references))
+    # Get the first publication
+    pub = cv.academic.publications.get_publications_by_index(0)
+    print(f"Publication title: {pub.details.get_title()}")
+    apa = cv.get_publications_apa_citation(pub.details.get_title())
+    print(f"APA Citation: {apa}")
     sys.exit(0)
```

### Comparing `cvprocessor-0.6.0/src/cvprocessor/education.py` & `cvprocessor-0.6.1/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/experience.py` & `cvprocessor-0.6.1/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/grants_awards.py` & `cvprocessor-0.6.1/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/institutes.py` & `cvprocessor-0.6.1/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/intro.py` & `cvprocessor-0.6.1/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/memberships.py` & `cvprocessor-0.6.1/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/news.py` & `cvprocessor-0.6.1/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/publications.py` & `cvprocessor-0.6.1/src/cvprocessor/publications.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,18 @@
 
     def load(self, filename):
         """
         Load the publication details from the file.
         """
         self.title = filename["Title"]
         self.year = filename["Year"]
+        if len(self.year.split()) == 1:
+            self.year = "Jan "+self.year
+        # To datetime month year format
+        self.year = pd.to_datetime(self.year, format="%b %Y").date()
         self.source.load(filename)
         self.pages.load(filename)
         self.document_type = filename["Document Type"]
         self.abstract = filename["Abstract"]
         self.keywords = filename["Keywords"]
 
     def __repr__(self):
@@ -466,14 +470,20 @@
 
     def get_publications_count(self):
         """
         Gets the number of publications.
         """
         return len(self.publications)
 
+    def get_publications_by_index(self, index):
+        """
+        Gets the publication by index.
+        """
+        return self.publications[index]
+
     def get_unique_sources(self):
         """
         Gets the number of unique sources.
         """
         sources = set()
         for publication in self.publications:
             sources.add(publication.details.source.get_source())
```

### Comparing `cvprocessor-0.6.0/src/cvprocessor/references.py` & `cvprocessor-0.6.1/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/research_interests.py` & `cvprocessor-0.6.1/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/service.py` & `cvprocessor-0.6.1/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/skills.py` & `cvprocessor-0.6.1/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/software.py` & `cvprocessor-0.6.1/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/supervision.py` & `cvprocessor-0.6.1/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/teaching.py` & `cvprocessor-0.6.1/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor/year_data.py` & `cvprocessor-0.6.1/src/cvprocessor/year_data.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.0/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.6.1/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.6.0
+Version: 0.6.1
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.6.0/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.6.1/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

