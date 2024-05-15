# Comparing `tmp/plingenn-0.0.8.tar.gz` & `tmp/plingenn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plingenn-0.0.8.tar", last modified: Wed May 15 19:53:26 2024, max compression
+gzip compressed data, was "plingenn-0.0.9.tar", last modified: Wed May 15 20:08:28 2024, max compression
```

## Comparing `plingenn-0.0.8.tar` & `plingenn-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:53:26.704702 plingenn-0.0.8/
--rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.8/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      646 2024-05-15 19:53:26.662757 plingenn-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:53:25.944435 plingenn-0.0.8/plingenn/
--rw-rw-rw-   0        0        0     1705 2024-05-15 19:52:19.000000 plingenn-0.0.8/plingenn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:53:26.519026 plingenn-0.0.8/plingenn/plingenn.egg-info/
--rw-rw-rw-   0        0        0        0 2024-05-15 19:27:48.000000 plingenn-0.0.8/plingenn/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:27:48.000000 plingenn-0.0.8/plingenn/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:27:48.000000 plingenn-0.0.8/plingenn/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:27:48.000000 plingenn-0.0.8/plingenn/plingenn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:53:26.597178 plingenn-0.0.8/plingenn.egg-info/
--rw-rw-rw-   0        0        0      646 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 19:53:26.704702 plingenn-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-15 19:52:58.000000 plingenn-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:08:28.097090 plingenn-0.0.9/
+-rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.9/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      672 2024-05-15 20:08:28.054968 plingenn-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 20:08:27.336255 plingenn-0.0.9/plingenn/
+-rw-rw-rw-   0        0        0     2294 2024-05-15 20:07:14.000000 plingenn-0.0.9/plingenn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:08:27.910755 plingenn-0.0.9/plingenn/plingenn.egg-info/
+-rw-rw-rw-   0        0        0        0 2024-05-15 19:27:48.000000 plingenn-0.0.9/plingenn/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:27:48.000000 plingenn-0.0.9/plingenn/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:27:48.000000 plingenn-0.0.9/plingenn/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:27:48.000000 plingenn-0.0.9/plingenn/plingenn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 20:08:27.990537 plingenn-0.0.9/plingenn.egg-info/
+-rw-rw-rw-   0        0        0      672 2024-05-15 20:08:26.000000 plingenn-0.0.9/plingenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-05-15 20:08:26.000000 plingenn-0.0.9/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:08:26.000000 plingenn-0.0.9/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-15 20:08:26.000000 plingenn-0.0.9/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 20:08:26.000000 plingenn-0.0.9/plingenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:08:28.097090 plingenn-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      742 2024-05-15 20:07:22.000000 plingenn-0.0.9/setup.py
```

### Comparing `plingenn-0.0.8/LICENCE.txt` & `plingenn-0.0.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plingenn-0.0.8/PKG-INFO` & `plingenn-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.8
+Version: 0.0.9
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
-Requires-Dist: requests
-Requires-Dist: numpy
+Requires-Dist: colorama
+Requires-Dist: datetime
+Requires-Dist: ctypes
 
 This is a very simple library.
 
 Change Log
 ==========
 
 0.0.1 (Date)
```

### Comparing `plingenn-0.0.8/plingenn/__init__.py` & `plingenn-0.0.9/plingenn/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import os
 from colorama import Fore
 from datetime import datetime
+import ctypes
+
+BASE_DIR = os.getenv('LOCALAPPDATA')
 
 class LogManager:
-    def __init__(self, level):
+    text_cache = {}
+
+    def __init__(self, level, info_color=None):
         self.level = level
+        self.info_color = info_color if info_color else Fore.CYAN
         self.color_map = {
-            "info": (Fore.LIGHTWHITE_EX, "<*>"),
+            "info": (self.info_color, "<*>"),
             "warning": (Fore.YELLOW, "<->"),
             "bad": (Fore.RED, "<!>"),
             "good": (Fore.GREEN, "<+>"),
             "dbg": (Fore.MAGENTA, "</>"),
         }
 
     def notime(self, *args, **kwargs):
@@ -31,25 +37,35 @@
         for arg in args:
             base += f" {arg}"
 
         if kwargs:
             for key, value in kwargs.items():
                 base += f" {key}={value}"
         print(base)
-
-PROGRAM_NAME = "Plingenn"
-VERSION = "1.0"
-
-BASE_DIR = os.getenv('LOCALAPPDATA')
-
-def getver():
-    return VERSION
-
-def getname():
-    return PROGRAM_NAME
+        
+    @staticmethod
+    def st(text):
+        system = os.name
+        
+        if system == 'nt':
+            if text in LogManager.text_cache:
+                cached_text = LogManager.text_cache[text]
+            else:
+                cached_text = text
+                LogManager.text_cache[text] = cached_text
+
+            ctypes.windll.kernel32.SetConsoleTitleW(f"{text} - {cached_text}")
+        elif system == 'posix':
+            print(f"\033]0;{text}\007")
+        else:
+            pass
+
+    @staticmethod
+    def cc():
+        LogManager.text_cache.clear()
 
 def rf(file_name):
     try:
         os.remove(file_name)
         print("File removed successfully:", file_name)
     except OSError as e:
         print(f"Error: {file_name} : {e.strerror}")
```

### Comparing `plingenn-0.0.8/plingenn.egg-info/PKG-INFO` & `plingenn-0.0.9/plingenn.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.8
+Version: 0.0.9
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
-Requires-Dist: requests
-Requires-Dist: numpy
+Requires-Dist: colorama
+Requires-Dist: datetime
+Requires-Dist: ctypes
 
 This is a very simple library.
 
 Change Log
 ==========
 
 0.0.1 (Date)
```

### Comparing `plingenn-0.0.8/setup.py` & `plingenn-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='plingenn',
-    version='0.0.8',
+    version='0.0.9',
     description='A very basic package',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Plingenn Plingsson',
     author_email='Plingenn12@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='none',
     packages=['plingenn'],
-    install_requires=['requests', 'numpy']
+    install_requires=['colorama', 'datetime', 'ctypes']
 )
```

