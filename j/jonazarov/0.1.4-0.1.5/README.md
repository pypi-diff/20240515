# Comparing `tmp/jonazarov-0.1.4.tar.gz` & `tmp/jonazarov-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jonazarov-0.1.4.tar", last modified: Wed May 15 15:05:37 2024, max compression
+gzip compressed data, was "jonazarov-0.1.5.tar", last modified: Wed May 15 15:18:36 2024, max compression
```

## Comparing `jonazarov-0.1.4.tar` & `jonazarov-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 15:05:37.702538 jonazarov-0.1.4/
--rw-rw-rw-   0        0        0     1087 2023-08-16 08:45:41.000000 jonazarov-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      666 2024-05-15 15:05:37.701532 jonazarov-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-15 13:46:04.000000 jonazarov-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 15:05:37.642510 jonazarov-0.1.4/jonazarov/
--rw-rw-rw-   0        0        0    55498 2024-05-15 15:01:30.000000 jonazarov-0.1.4/jonazarov/AtlassianCloudRest.py
--rw-rw-rw-   0        0        0       77 2024-05-15 15:05:20.000000 jonazarov-0.1.4/jonazarov/__init__.py
--rw-rw-rw-   0        0        0     3716 2024-05-15 15:04:54.000000 jonazarov-0.1.4/jonazarov/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:05:37.700224 jonazarov-0.1.4/jonazarov.egg-info/
--rw-rw-rw-   0        0        0      666 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 15:05:37.702538 jonazarov-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-05-15 15:05:11.000000 jonazarov-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:18:36.335767 jonazarov-0.1.5/
+-rw-rw-rw-   0        0        0     1087 2023-08-16 08:45:41.000000 jonazarov-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      666 2024-05-15 15:18:36.334373 jonazarov-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2024-05-15 15:06:16.000000 jonazarov-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 15:18:36.295730 jonazarov-0.1.5/jonazarov/
+-rw-rw-rw-   0        0        0    55498 2024-05-15 15:01:30.000000 jonazarov-0.1.5/jonazarov/AtlassianCloudRest.py
+-rw-rw-rw-   0        0        0       77 2024-05-15 15:18:09.000000 jonazarov-0.1.5/jonazarov/__init__.py
+-rw-rw-rw-   0        0        0     3728 2024-05-15 15:18:14.000000 jonazarov-0.1.5/jonazarov/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:18:36.334209 jonazarov-0.1.5/jonazarov.egg-info/
+-rw-rw-rw-   0        0        0      666 2024-05-15 15:18:36.000000 jonazarov-0.1.5/jonazarov.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-15 15:18:36.000000 jonazarov-0.1.5/jonazarov.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:18:36.000000 jonazarov-0.1.5/jonazarov.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-15 15:18:36.000000 jonazarov-0.1.5/jonazarov.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 15:18:36.000000 jonazarov-0.1.5/jonazarov.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 15:18:36.336692 jonazarov-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-05-15 15:18:23.000000 jonazarov-0.1.5/setup.py
```

### Comparing `jonazarov-0.1.4/LICENSE` & `jonazarov-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jonazarov-0.1.4/PKG-INFO` & `jonazarov-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jonazarov
-Version: 0.1.4
+Version: 0.1.5
 Summary: Verschiedene Python-Tools, vor allem für Atlassian Cloud
 Home-page: https://github.com/jonazarov/pytools
 Author: Johannes Nazarov
 Author-email: johannes.nazarov+dev@gmail.com
 License: GNU
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `jonazarov-0.1.4/jonazarov/AtlassianCloudRest.py` & `jonazarov-0.1.5/jonazarov/AtlassianCloudRest.py`

 * *Files identical despite different names*

### Comparing `jonazarov-0.1.4/jonazarov/utils.py` & `jonazarov-0.1.5/jonazarov/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         '''
         return Utils.loads(Utils.dumps(data))
     
     def dumps(data: dict | list | str | int) -> json:
         return json.dumps(Utils.normalize(data))
     
     def log(current_filename: str|None = None):
-        if configfile == None:
-            configfile = pathlib.Path(inspect.stack()[1][1]).resolve()
+        if current_filename == None:
+            current_filename = pathlib.Path(inspect.stack()[1][1]).resolve()
         now = time.localtime()
         logfilename = current_filename + time.strftime(".%Y-%m-%d.log", now)
         logfile = codecs.open(logfilename, 'a', encoding='utf-8')
         logfile.write("NewLogEntry "+time.strftime("%Y-%m-%d %H:%M:%S", now) + "\n")
         sys.stdout = Unbuffered(logfile, sys.stdout)
 
     def getconfig(confdef: dict, conffile: str) -> SimpleNamespace:
```

### Comparing `jonazarov-0.1.4/jonazarov.egg-info/PKG-INFO` & `jonazarov-0.1.5/jonazarov.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jonazarov
-Version: 0.1.4
+Version: 0.1.5
 Summary: Verschiedene Python-Tools, vor allem für Atlassian Cloud
 Home-page: https://github.com/jonazarov/pytools
 Author: Johannes Nazarov
 Author-email: johannes.nazarov+dev@gmail.com
 License: GNU
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `jonazarov-0.1.4/setup.py` & `jonazarov-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='jonazarov',
-    version='0.1.4',    
+    version='0.1.5',    
     description='Verschiedene Python-Tools, vor allem für Atlassian Cloud',
     url='https://github.com/jonazarov/pytools',
     author='Johannes Nazarov',
     author_email='johannes.nazarov+dev@gmail.com',
     license='GNU',
     packages=['jonazarov'],
     install_requires=['requests>=2.31.0',
```

