# Comparing `tmp/zhlyr-4.3.tar.gz` & `tmp/zhlyr-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhlyr-4.3.tar", last modified: Wed May 15 16:42:06 2024, max compression
+gzip compressed data, was "zhlyr-4.4.tar", last modified: Wed May 15 17:32:34 2024, max compression
```

## Comparing `zhlyr-4.3.tar` & `zhlyr-4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 16:42:06.428885 zhlyr-4.3/
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     4083 2024-05-15 16:42:06.421884 zhlyr-4.3/PKG-INFO
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     3411 2024-05-13 08:54:58.000000 zhlyr-4.3/README.md
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)       38 2024-05-15 16:42:06.430396 zhlyr-4.3/setup.cfg
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1146 2024-05-15 16:42:04.000000 zhlyr-4.3/setup.py
-drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 16:42:06.322035 zhlyr-4.3/zhlyr/
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)      134 2024-05-15 16:36:48.000000 zhlyr-4.3/zhlyr/__init__.py
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1847 2024-05-13 08:30:55.000000 zhlyr-4.3/zhlyr/recosnize.py
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1931 2024-05-15 14:38:07.000000 zhlyr-4.3/zhlyr/serialize.pyx
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     2179 2024-05-10 18:26:37.000000 zhlyr-4.3/zhlyr/zhlyr.py
-drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 16:42:06.414858 zhlyr-4.3/zhlyr.egg-info/
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)     4083 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/PKG-INFO
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)      234 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/SOURCES.txt
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)        1 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/dependency_links.txt
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)       32 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/requires.txt
--rwxrwxrwx   0 whoami    (1000) whoami    (1000)        6 2024-05-15 16:42:06.000000 zhlyr-4.3/zhlyr.egg-info/top_level.txt
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 17:32:34.281216 zhlyr-4.4/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     4083 2024-05-15 17:32:34.273164 zhlyr-4.4/PKG-INFO
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     3411 2024-05-13 08:54:58.000000 zhlyr-4.4/README.md
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)       38 2024-05-15 17:32:34.282217 zhlyr-4.4/setup.cfg
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1433 2024-05-15 17:32:27.000000 zhlyr-4.4/setup.py
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 17:32:34.181035 zhlyr-4.4/zhlyr/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)      134 2024-05-15 16:36:48.000000 zhlyr-4.4/zhlyr/__init__.py
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1847 2024-05-13 08:30:55.000000 zhlyr-4.4/zhlyr/recosnize.py
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1931 2024-05-15 14:38:07.000000 zhlyr-4.4/zhlyr/serialize.pyx
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     2179 2024-05-10 18:26:37.000000 zhlyr-4.4/zhlyr/zhlyr.py
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-15 17:32:34.265164 zhlyr-4.4/zhlyr.egg-info/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     4083 2024-05-15 17:32:33.000000 zhlyr-4.4/zhlyr.egg-info/PKG-INFO
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)      234 2024-05-15 17:32:34.000000 zhlyr-4.4/zhlyr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)        1 2024-05-15 17:32:33.000000 zhlyr-4.4/zhlyr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)       32 2024-05-15 17:32:33.000000 zhlyr-4.4/zhlyr.egg-info/requires.txt
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)        6 2024-05-15 17:32:33.000000 zhlyr-4.4/zhlyr.egg-info/top_level.txt
```

### Comparing `zhlyr-4.3/PKG-INFO` & `zhlyr-4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 4.3
+Version: 4.4
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
```

### Comparing `zhlyr-4.3/README.md` & `zhlyr-4.4/README.md`

 * *Files identical despite different names*

### Comparing `zhlyr-4.3/setup.py` & `zhlyr-4.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from setuptools import setup, find_packages
 from Cython.Build import cythonize
-
+from setuptools import setup, Extension
+from glob import glob 
+import os
 with open('README.md', 'r') as file:
     long_description = file.read()
+    
+cython_files = glob("*.pyx")
+# Create extension objects for each .pyx file
+extensions = [Extension(name=os.path.splitext(file)[0], sources=[file]) for file in cython_files]
+
 
 setup(
     name='zhlyr',
-    version='4.3',
+    version='4.4',
     packages=find_packages(),
     install_requires=['requests', 'shazamio', 'shazam', 'cython'],
+    ext_modules=extensions,
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='Python library for music handling',
     author='Mtsky',
     author_email='secon2636@gmail.com',
     url='https://gaoc3.github.io/zhlyr/',
     license='MIT',
```

### Comparing `zhlyr-4.3/zhlyr/recosnize.py` & `zhlyr-4.4/zhlyr/recosnize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-4.3/zhlyr/serialize.pyx` & `zhlyr-4.4/zhlyr/serialize.pyx`

 * *Files identical despite different names*

### Comparing `zhlyr-4.3/zhlyr/zhlyr.py` & `zhlyr-4.4/zhlyr/zhlyr.py`

 * *Files identical despite different names*

### Comparing `zhlyr-4.3/zhlyr.egg-info/PKG-INFO` & `zhlyr-4.4/zhlyr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 4.3
+Version: 4.4
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
```

