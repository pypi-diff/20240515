# Comparing `tmp/Akinator-python-1.2.2.tar.gz` & `tmp/Akinator-python-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akinator-python-1.2.2.tar", last modified: Wed May 15 10:30:15 2024, max compression
+gzip compressed data, was "Akinator-python-1.2.3.tar", last modified: Wed May 15 11:53:28 2024, max compression
```

## Comparing `Akinator-python-1.2.2.tar` & `Akinator-python-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 10:30:15.462037 Akinator-python-1.2.2/
-drwxrwxrwx   0        0        0        0 2024-05-15 10:30:15.446258 Akinator-python-1.2.2/Akinator_python.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-15 10:30:15.000000 Akinator-python-1.2.2/Akinator_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-15 10:30:15.000000 Akinator-python-1.2.2/Akinator_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 10:30:15.000000 Akinator-python-1.2.2/Akinator_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-15 10:30:15.000000 Akinator-python-1.2.2/Akinator_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3914 2024-05-15 10:30:15.462037 Akinator-python-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 10:30:15.462037 Akinator-python-1.2.2/akinator_python/
--rw-rw-rw-   0        0        0      121 2024-05-15 10:29:31.000000 Akinator-python-1.2.2/akinator_python/__init__.py
--rw-rw-rw-   0        0        0     4585 2024-05-15 10:28:56.000000 Akinator-python-1.2.2/akinator_python/main.py
--rw-rw-rw-   0        0        0       42 2024-05-15 10:30:15.462037 Akinator-python-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      742 2024-05-15 10:29:18.000000 Akinator-python-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:53:28.075366 Akinator-python-1.2.3/
+drwxrwxrwx   0        0        0        0 2024-05-15 11:53:28.062821 Akinator-python-1.2.3/Akinator_python.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-15 11:53:27.000000 Akinator-python-1.2.3/Akinator_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-15 11:53:27.000000 Akinator-python-1.2.3/Akinator_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 11:53:27.000000 Akinator-python-1.2.3/Akinator_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 11:53:27.000000 Akinator-python-1.2.3/Akinator_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3914 2024-05-15 11:53:28.072765 Akinator-python-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 11:53:28.072765 Akinator-python-1.2.3/akinator_python/
+-rw-rw-rw-   0        0        0      121 2024-05-15 11:52:34.000000 Akinator-python-1.2.3/akinator_python/__init__.py
+-rw-rw-rw-   0        0        0     4570 2024-05-15 11:51:06.000000 Akinator-python-1.2.3/akinator_python/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 11:53:28.075366 Akinator-python-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      742 2024-05-15 11:52:51.000000 Akinator-python-1.2.3/setup.py
```

### Comparing `Akinator-python-1.2.2/Akinator_python.egg-info/PKG-INFO` & `Akinator-python-1.2.3/Akinator_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akinator-python
-Version: 1.2.2
+Version: 1.2.3
 Summary: A API wrapper for the AkinatorAPI
 Home-page: https://github.com/taka-4602/Akinator-python
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: akinator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Akinator-python-1.2.2/PKG-INFO` & `Akinator-python-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akinator-python
-Version: 1.2.2
+Version: 1.2.3
 Summary: A API wrapper for the AkinatorAPI
 Home-page: https://github.com/taka-4602/Akinator-python
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: akinator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Akinator-python-1.2.2/README.md` & `Akinator-python-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `Akinator-python-1.2.2/akinator_python/main.py` & `Akinator-python-1.2.3/akinator_python/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             except:
                 self.name=progression["name_proposition"]
                 self.description=progression["description_proposition"]
                 self.photo=progression["photo"]
                 self.answer_id=progression["id_proposition"]
             return progression
         except:
-            raise AkinatorError(progression.text)
+            raise AkinatorError(progression)
 
     def go_back(self):
         self.name=None
         self.description=None
         self.photo=None
         self.answer_id=None
         if self.json["step"]==0:
@@ -94,15 +94,15 @@
             self.json["progression"]=float(goback["progression"])
             self.step=int(goback["step"])
             self.progression=float(goback["progression"])
             self.question=goback["question"]
             self.question_id=goback["question_id"]
             return goback
         except:
-            raise AkinatorError(goback.text)
+            raise AkinatorError(goback)
 
     def exclude(self):
         self.name=None
         self.description=None
         self.photo=None
         self.answer_id=None
         if "answer" in self.json:
@@ -114,8 +114,8 @@
             self.json["progression"]=float(self.json["progression"])
             self.step=int(exclude["step"])
             self.progression=float(exclude["progression"])
             self.question=exclude["question"]
             self.question_id=exclude["question_id"]
             return exclude
         except:
-            raise AkinatorError(exclude.text)
+            raise AkinatorError(exclude)
```

### Comparing `Akinator-python-1.2.2/setup.py` & `Akinator-python-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 def load_readme() -> str:
     with open("README.md",encoding="utf-8_sig") as fin:
         return fin.read()
 setup(
     name='Akinator-python',
-    version='1.2.2',
+    version='1.2.3',
     keywords = "akinator",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     author='taka4602',
     author_email='shun4602@gmail.com',
     url='https://github.com/taka-4602/Akinator-python',
     description='A API wrapper for the AkinatorAPI',
```

