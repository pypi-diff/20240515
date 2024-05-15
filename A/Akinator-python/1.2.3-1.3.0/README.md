# Comparing `tmp/Akinator-python-1.2.3.tar.gz` & `tmp/Akinator-python-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akinator-python-1.2.3.tar", last modified: Wed May 15 11:53:28 2024, max compression
+gzip compressed data, was "Akinator-python-1.3.0.tar", last modified: Wed May 15 16:42:15 2024, max compression
```

## Comparing `Akinator-python-1.2.3.tar` & `Akinator-python-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 11:53:28.075366 Akinator-python-1.2.3/
-drwxrwxrwx   0        0        0        0 2024-05-15 11:53:28.062821 Akinator-python-1.2.3/Akinator_python.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-15 11:53:27.000000 Akinator-python-1.2.3/Akinator_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-15 11:53:27.000000 Akinator-python-1.2.3/Akinator_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 11:53:27.000000 Akinator-python-1.2.3/Akinator_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-15 11:53:27.000000 Akinator-python-1.2.3/Akinator_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3914 2024-05-15 11:53:28.072765 Akinator-python-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 11:53:28.072765 Akinator-python-1.2.3/akinator_python/
--rw-rw-rw-   0        0        0      121 2024-05-15 11:52:34.000000 Akinator-python-1.2.3/akinator_python/__init__.py
--rw-rw-rw-   0        0        0     4570 2024-05-15 11:51:06.000000 Akinator-python-1.2.3/akinator_python/main.py
--rw-rw-rw-   0        0        0       42 2024-05-15 11:53:28.075366 Akinator-python-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      742 2024-05-15 11:52:51.000000 Akinator-python-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:15.136895 Akinator-python-1.3.0/
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:15.122640 Akinator-python-1.3.0/Akinator_python.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-15 16:42:15.000000 Akinator-python-1.3.0/Akinator_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-15 16:42:15.000000 Akinator-python-1.3.0/Akinator_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:42:15.000000 Akinator-python-1.3.0/Akinator_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 16:42:15.000000 Akinator-python-1.3.0/Akinator_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3914 2024-05-15 16:42:15.135882 Akinator-python-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 16:42:15.134453 Akinator-python-1.3.0/akinator_python/
+-rw-rw-rw-   0        0        0      121 2024-05-15 16:41:10.000000 Akinator-python-1.3.0/akinator_python/__init__.py
+-rw-rw-rw-   0        0        0     4566 2024-05-15 16:40:33.000000 Akinator-python-1.3.0/akinator_python/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:42:15.136895 Akinator-python-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      742 2024-05-15 16:40:58.000000 Akinator-python-1.3.0/setup.py
```

### Comparing `Akinator-python-1.2.3/Akinator_python.egg-info/PKG-INFO` & `Akinator-python-1.3.0/Akinator_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akinator-python
-Version: 1.2.3
+Version: 1.3.0
 Summary: A API wrapper for the AkinatorAPI
 Home-page: https://github.com/taka-4602/Akinator-python
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: akinator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Akinator-python-1.2.3/PKG-INFO` & `Akinator-python-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akinator-python
-Version: 1.2.3
+Version: 1.3.0
 Summary: A API wrapper for the AkinatorAPI
 Home-page: https://github.com/taka-4602/Akinator-python
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: akinator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Akinator-python-1.2.3/README.md` & `Akinator-python-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `Akinator-python-1.2.3/akinator_python/main.py` & `Akinator-python-1.3.0/akinator_python/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,16 +106,16 @@
         self.photo=None
         self.answer_id=None
         if "answer" in self.json:
             del self.json["answer"]
         try:
             exclude=requests.post(f"{self.ENDPOINT}exclude",json=self.json)
             exclude=exclude.json()
-            self.json["step"]=int(self.json["step"])
-            self.json["progression"]=float(self.json["progression"])
+            self.json["step"]=int(exclude["step"])
+            self.json["progression"]=float(exclude["progression"])
             self.step=int(exclude["step"])
             self.progression=float(exclude["progression"])
             self.question=exclude["question"]
             self.question_id=exclude["question_id"]
             return exclude
         except:
             raise AkinatorError(exclude)
```

### Comparing `Akinator-python-1.2.3/setup.py` & `Akinator-python-1.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 def load_readme() -> str:
     with open("README.md",encoding="utf-8_sig") as fin:
         return fin.read()
 setup(
     name='Akinator-python',
-    version='1.2.3',
+    version='1.3.0',
     keywords = "akinator",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     author='taka4602',
     author_email='shun4602@gmail.com',
     url='https://github.com/taka-4602/Akinator-python',
     description='A API wrapper for the AkinatorAPI',
```

