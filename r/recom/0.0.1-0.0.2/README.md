# Comparing `tmp/recom-0.0.1.tar.gz` & `tmp/recom-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recom-0.0.1.tar", last modified: Sat Mar 23 20:26:51 2024, max compression
+gzip compressed data, was "recom-0.0.2.tar", last modified: Wed May 15 00:39:03 2024, max compression
```

## Comparing `recom-0.0.1.tar` & `recom-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-23 20:26:51.198435 recom-0.0.1/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      349 2024-03-23 20:26:51.198435 recom-0.0.1/PKG-INFO
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-23 20:26:51.198435 recom-0.0.1/recom/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      248 2024-03-23 20:26:19.000000 recom-0.0.1/recom/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      424 2024-03-23 19:16:06.000000 recom-0.0.1/recom/__main__.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-23 20:26:51.198435 recom-0.0.1/recom/backend/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2024-03-23 19:16:06.000000 recom-0.0.1/recom/backend/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      166 2024-03-23 19:16:06.000000 recom-0.0.1/recom/backend/uart.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4734 2024-03-23 19:16:06.000000 recom-0.0.1/recom/backend/usb.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1558 2024-03-23 19:16:06.000000 recom-0.0.1/recom/cli.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4682 2024-03-23 19:16:06.000000 recom-0.0.1/recom/device.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1785 2024-03-23 19:16:06.000000 recom-0.0.1/recom/interface.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-23 20:26:51.198435 recom-0.0.1/recom.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      349 2024-03-23 20:26:51.000000 recom-0.0.1/recom.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      347 2024-03-23 20:26:51.000000 recom-0.0.1/recom.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-03-23 20:26:51.000000 recom-0.0.1/recom.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       46 2024-03-23 20:26:51.000000 recom-0.0.1/recom.egg-info/entry_points.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       15 2024-03-23 20:26:51.000000 recom-0.0.1/recom.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        6 2024-03-23 20:26:51.000000 recom-0.0.1/recom.egg-info/top_level.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      122 2024-03-23 20:26:51.198435 recom-0.0.1/setup.cfg
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      778 2024-03-23 20:26:40.000000 recom-0.0.1/setup.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-15 00:39:03.057713 recom-0.0.2/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      395 2024-05-15 00:39:03.057713 recom-0.0.2/PKG-INFO
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-15 00:39:03.057713 recom-0.0.2/recom/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      258 2024-05-15 00:37:17.000000 recom-0.0.2/recom/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      424 2024-03-29 21:20:09.000000 recom-0.0.2/recom/__main__.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-15 00:39:03.057713 recom-0.0.2/recom/backend/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      938 2024-05-15 00:37:17.000000 recom-0.0.2/recom/backend/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      743 2024-05-15 00:37:17.000000 recom-0.0.2/recom/backend/backend.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      691 2024-05-15 00:37:17.000000 recom-0.0.2/recom/backend/uart.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     9296 2024-05-15 00:37:17.000000 recom-0.0.2/recom/backend/usb.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     7239 2024-05-15 00:37:17.000000 recom-0.0.2/recom/cli.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     6267 2024-05-15 00:37:17.000000 recom-0.0.2/recom/device.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1793 2024-05-15 00:37:17.000000 recom-0.0.2/recom/interface.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1981 2024-05-15 00:37:17.000000 recom-0.0.2/recom/util.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-15 00:39:03.057713 recom-0.0.2/recom.egg-info/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      395 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      386 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       46 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/entry_points.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       31 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        6 2024-05-15 00:39:03.000000 recom-0.0.2/recom.egg-info/top_level.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      122 2024-05-15 00:39:03.057713 recom-0.0.2/setup.cfg
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      800 2024-05-15 00:37:17.000000 recom-0.0.2/setup.py
```

### Comparing `recom-0.0.1/recom/interface.py` & `recom-0.0.2/recom/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 class RecomInterface:
 
     def __init__(self, deviceHandle, interfaceHandle):
         self._parentDevice = deviceHandle
         self._handle = interfaceHandle
 
     def __repr__(self):
-        return f"Interface: {self.name} (Sub={self._handle.subclass}/Prot={self._handle.protocol})"
+        return f"Interface: {self.name} (Sub={self._handle.itf_subclass}/Prot={self._handle.itf_protocol})"
 
     def read(self, dataLen=-1):
         """
         Reads data from the interface's data endpoint
         
         dataLen specifies how many bytes should be read. If not speciied, any
         available bytes will be returned
```

### Comparing `recom-0.0.1/setup.py` & `recom-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='recom',
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     setup_requires=['setuptools_scm'],
     license='MIT',
     author='Adrian Rothenbuhler',
     author_email='adrian@redhill-embedded.com',
     description='Embedded communication backend',
     keywords='embedded communication backedn usb serial',
@@ -15,14 +15,14 @@
     #download_url='https://github.com/redhill-embedded/sertool/archive/v_010.tar.gz',
     package_data={
         "recom": [
             "package_version"
         ]
     },
     python_requires=">=3.8",
-    install_requires=["pyusb", "pyserial"],
+    install_requires=["libusb1", "pyserial", "pyudev", "psutil"],
     entry_points={
         "console_scripts": [
             "recom=recom.__main__:main",
         ]
     },
 )
```

