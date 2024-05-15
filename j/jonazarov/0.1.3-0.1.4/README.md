# Comparing `tmp/jonazarov-0.1.3.tar.gz` & `tmp/jonazarov-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jonazarov-0.1.3.tar", last modified: Wed May 15 13:35:55 2024, max compression
+gzip compressed data, was "jonazarov-0.1.4.tar", last modified: Wed May 15 15:05:37 2024, max compression
```

## Comparing `jonazarov-0.1.3.tar` & `jonazarov-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 13:35:55.529454 jonazarov-0.1.3/
--rw-rw-rw-   0        0        0     1087 2023-08-16 08:45:41.000000 jonazarov-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      666 2024-05-15 13:35:55.527547 jonazarov-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1277 2024-05-15 12:41:56.000000 jonazarov-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 13:35:55.434836 jonazarov-0.1.3/jonazarov/
--rw-rw-rw-   0        0        0    55422 2024-05-15 11:33:26.000000 jonazarov-0.1.3/jonazarov/AtlassianCloudRest.py
--rw-rw-rw-   0        0        0       77 2024-05-15 13:29:58.000000 jonazarov-0.1.3/jonazarov/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-09-12 14:44:09.000000 jonazarov-0.1.3/jonazarov/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 13:35:55.524732 jonazarov-0.1.3/jonazarov.egg-info/
--rw-rw-rw-   0        0        0      666 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 13:35:55.530480 jonazarov-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-05-15 13:30:04.000000 jonazarov-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:05:37.702538 jonazarov-0.1.4/
+-rw-rw-rw-   0        0        0     1087 2023-08-16 08:45:41.000000 jonazarov-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      666 2024-05-15 15:05:37.701532 jonazarov-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-15 13:46:04.000000 jonazarov-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 15:05:37.642510 jonazarov-0.1.4/jonazarov/
+-rw-rw-rw-   0        0        0    55498 2024-05-15 15:01:30.000000 jonazarov-0.1.4/jonazarov/AtlassianCloudRest.py
+-rw-rw-rw-   0        0        0       77 2024-05-15 15:05:20.000000 jonazarov-0.1.4/jonazarov/__init__.py
+-rw-rw-rw-   0        0        0     3716 2024-05-15 15:04:54.000000 jonazarov-0.1.4/jonazarov/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:05:37.700224 jonazarov-0.1.4/jonazarov.egg-info/
+-rw-rw-rw-   0        0        0      666 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 15:05:37.000000 jonazarov-0.1.4/jonazarov.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 15:05:37.702538 jonazarov-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-05-15 15:05:11.000000 jonazarov-0.1.4/setup.py
```

### Comparing `jonazarov-0.1.3/LICENSE` & `jonazarov-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jonazarov-0.1.3/PKG-INFO` & `jonazarov-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jonazarov
-Version: 0.1.3
+Version: 0.1.4
 Summary: Verschiedene Python-Tools, vor allem für Atlassian Cloud
 Home-page: https://github.com/jonazarov/pytools
 Author: Johannes Nazarov
 Author-email: johannes.nazarov+dev@gmail.com
 License: GNU
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `jonazarov-0.1.3/README.md` & `jonazarov-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 https://betterscientificsoftware.github.io/python-for-hpc/tutorials/python-pypi-packaging
 
 ## Package Update
 * Code aktualisieren
 * Version in `__init__.py` aktualisieren
 * Version in `setup.py` aktualisieren
 ```shell
-# Vorbereiten der Dateien und Upload in test.pypi.org
+# Vorbereiten der Dateien und Upload in https://test.pypi.org/project/jonazarov/
 deploy.bat
-# Installation des Test-Packages
-pip install --index-url https://test.pypi.org/simple/ jonazarov
 # Wenn alles funktioniert, Upload ins produktive pypi
 upload.bat
 # Installation der produktiven Packages
 pip install jonazarov
 ```
```

### Comparing `jonazarov-0.1.3/jonazarov/AtlassianCloudRest.py` & `jonazarov-0.1.4/jonazarov/AtlassianCloudRest.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
     try:
         u = jira.usersGetByName(config.orgadmin.user)
         if u == []:
             print('Die angegebenen Authentifizierungsdaten sind ungültig! Bitte Eingaben wiederholen!')
             config = ut.normalize(config)
             del config['orgadmin']
             with open(configfile, "w") as file:
-                json.dump(config, file, indent=3)
+                json.dump(config, file, ensure_ascii=False, indent=3)
             return loadAtlassianAuth(configfile)
     except objectNotExists as e:
         print('Die angegebene Cloud-Instanz kann nicht erreicht werden! Bitte Eingaben wiederholen!')
         config = ut.normalize(config)
         del config['base_urls']
-        with open(configfile, "w") as file:
+        with open(configfile, "w", encoding="utf-8") as file:
             json.dump(config, file, indent=3)
         return loadAtlassianAuth(configfile)
     _config = ut.normalize(config)
     _config['orgadmin']['accountId'] = u[0].accountId
     config = ut.simplifize(_config)
-    with open(configfile, "w") as file:
-        json.dump(ut.normalize(config), file, indent=3)
+    with open(configfile, "w", encoding="utf-8") as file:
+        json.dump(ut.normalize(config), file, ensure_ascii=False, indent=3)
     return config
 
 class objectNotExists(Exception):
     pass
 
 class AtlassianCloud:
     """
```

### Comparing `jonazarov-0.1.3/jonazarov/utils.py` & `jonazarov-0.1.4/jonazarov/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import json, pathlib, inspect
 from types import SimpleNamespace
 
 class NamespaceEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, (list, tuple)):
             return super(NamespaceEncoder,self).iterencode(o)
         return o.__dict__ 
@@ -77,22 +77,24 @@
         Verwandelt normale Python-Größen in SimpleNamespace
         '''
         return Utils.loads(Utils.dumps(data))
     
     def dumps(data: dict | list | str | int) -> json:
         return json.dumps(Utils.normalize(data))
     
-    def log(current_filename: str):
+    def log(current_filename: str|None = None):
+        if configfile == None:
+            configfile = pathlib.Path(inspect.stack()[1][1]).resolve()
         now = time.localtime()
         logfilename = current_filename + time.strftime(".%Y-%m-%d.log", now)
         logfile = codecs.open(logfilename, 'a', encoding='utf-8')
         logfile.write("NewLogEntry "+time.strftime("%Y-%m-%d %H:%M:%S", now) + "\n")
         sys.stdout = Unbuffered(logfile, sys.stdout)
 
     def getconfig(confdef: dict, conffile: str) -> SimpleNamespace:
         config = {}
-        with open(conffile, "r") as file:
+        with open(conffile, "r", encoding="utf-8") as file:
             try:
                 config = json.load(file)
             except:
                 pass
         return Utils.simplifize(confunpack(confdef, config))
```

### Comparing `jonazarov-0.1.3/jonazarov.egg-info/PKG-INFO` & `jonazarov-0.1.4/jonazarov.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jonazarov
-Version: 0.1.3
+Version: 0.1.4
 Summary: Verschiedene Python-Tools, vor allem für Atlassian Cloud
 Home-page: https://github.com/jonazarov/pytools
 Author: Johannes Nazarov
 Author-email: johannes.nazarov+dev@gmail.com
 License: GNU
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `jonazarov-0.1.3/setup.py` & `jonazarov-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='jonazarov',
-    version='0.1.3',    
+    version='0.1.4',    
     description='Verschiedene Python-Tools, vor allem für Atlassian Cloud',
     url='https://github.com/jonazarov/pytools',
     author='Johannes Nazarov',
     author_email='johannes.nazarov+dev@gmail.com',
     license='GNU',
     packages=['jonazarov'],
     install_requires=['requests>=2.31.0',
```

