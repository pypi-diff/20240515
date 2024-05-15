# Comparing `tmp/titandevice-0.3.9.tar.gz` & `tmp/titandevice-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titandevice-0.3.9.tar", last modified: Sun Apr 28 08:06:46 2024, max compression
+gzip compressed data, was "titandevice-0.4.0.tar", last modified: Wed May 15 02:47:04 2024, max compression
```

## Comparing `titandevice-0.3.9.tar` & `titandevice-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:06:46.419641 titandevice-0.3.9/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-28 08:06:46.419641 titandevice-0.3.9/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 titandevice-0.3.9/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 08:06:46.419641 titandevice-0.3.9/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-28 08:05:29.000000 titandevice-0.3.9/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:06:46.419641 titandevice-0.3.9/titandevice/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4601 2024-04-28 08:04:48.000000 titandevice-0.3.9/titandevice/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1415 2024-04-26 10:24:31.000000 titandevice-0.3.9/titandevice/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7089 2024-04-28 01:52:55.000000 titandevice-0.3.9/titandevice/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      559 2024-04-25 06:30:48.000000 titandevice-0.3.9/titandevice/_device_models.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:06:46.419641 titandevice-0.3.9/titandevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      310 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.979767 titandevice-0.4.0/
+-rw-r--r--   0 mark      (1000) mark      (1000)      573 2024-05-15 02:47:04.979767 titandevice-0.4.0/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      161 2024-05-11 08:04:43.000000 titandevice-0.4.0/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-15 02:47:04.979767 titandevice-0.4.0/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-05-15 02:46:20.000000 titandevice-0.4.0/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.975767 titandevice-0.4.0/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2689 2024-05-15 02:46:20.000000 titandevice-0.4.0/tests/tests.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.979767 titandevice-0.4.0/titandevice/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       33 2024-05-14 09:13:44.000000 titandevice-0.4.0/titandevice/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1162 2024-05-14 11:10:29.000000 titandevice-0.4.0/titandevice/_titian_exception.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.979767 titandevice-0.4.0/titandevice/android/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-14 09:15:12.000000 titandevice-0.4.0/titandevice/android/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3288 2024-05-15 02:32:40.000000 titandevice-0.4.0/titandevice/android/_device.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3010 2024-05-15 01:20:19.000000 titandevice-0.4.0/titandevice/android/_frida.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2033 2024-05-15 02:35:37.000000 titandevice-0.4.0/titandevice/android/_frida_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1639 2024-05-14 08:57:29.000000 titandevice-0.4.0/titandevice/android/_package_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1240 2024-05-14 09:21:38.000000 titandevice-0.4.0/titandevice/android/device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       88 2024-05-14 07:18:06.000000 titandevice-0.4.0/titandevice/utils.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.979767 titandevice-0.4.0/titandevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      573 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      494 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/top_level.txt
```

### Comparing `titandevice-0.3.9/PKG-INFO` & `titandevice-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: titandevice
-Version: 0.3.9
+Version: 0.4.0
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: adbutils
 Requires-Dist: pydantic
 
 # Titan
 
-A Python library used for managing devices, including:
+A Python library used for managing devices(must root), including:
 
-- Obtaining information of all devices
-- Checking the status of a device
+- Getting information of all devices
 - Installing Frida
-- Installing APK
+- Installing `APK`
 - And more
```

### Comparing `titandevice-0.3.9/setup.py` & `titandevice-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="titandevice",
-    version="0.3.9",
+    version="0.4.0",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `titandevice-0.3.9/titandevice/_device_exception.py` & `titandevice-0.4.0/titandevice/_titian_exception.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 class TitanException(Exception):
     def __init__(self, message: str):
         super().__init__(message)
 
 
-class DeviceNoFoundException(TitanException):
-    def __init__(self, device_serial):
-        super().__init__(f"Device with serial {device_serial} not found")
+class AnyDeviceNoFoundException(TitanException):
+    def __init__(self):
+        super().__init__("Any device not found.")
 
 
-class DeviceMustBeRootedException(TitanException):
-    def __init__(self, device_serial):
-        super().__init__(
-            f'Device [{device_serial}] must be rooted to perform this operation'
-        )
+class DeviceNoFoundException(TitanException):
+    def __init__(self, device_serial: str):
+        super().__init__(f"Device with serial {device_serial} not found.")
 
 
-class FridaServerNotInstalledException(TitanException):
-    def __init__(self, device_serial, frida_server_path):
-        super().__init__(
-            f'Frida server is not installed in {frida_server_path} on device with serial {device_serial}'
-        )
+class PackageNoFoundException(TitanException):
+    def __init__(self, device_serial: str, package_name: str):
+        super().__init__(f"Package {package_name} not found on device {device_serial}.")
 
 
-class FridaServerNotRunningException(TitanException):
-    def __init__(self, device_serial, frida_server_name):
-        super().__init__(
-            f'Frida server [{frida_server_name}] is not running on device with serial {device_serial}'
-        )
+class DeviceMustBeRootedException(TitanException):
+    def __init__(self, device_serial: str):
+        super().__init__(f"Device with serial {device_serial} must be rooted.")
 
 
-class PackageNotInstalledException(TitanException):
-    def __init__(self, device_serial, package_name):
-        super().__init__(f'Package {package_name} is not installed in {device_serial}')
+class AnyFridaNotInstalledException(TitanException):
+    def __init__(self):
+        super().__init__("Any device frida not installed.")
 
 
-class InstallPackageMustUninstallFirstException(TitanException):
-    def __init__(self, device_serial, package_name):
+class FridaNotInstalledException(TitanException):
+    def __init__(self, device_serial: str, frida_server_path: str):
         super().__init__(
-            f'Package {package_name} is already installed in {device_serial}'
+            f"Frida not installed on device {device_serial} with path {frida_server_path}."
         )
```

### Comparing `titandevice-0.3.9/titandevice.egg-info/PKG-INFO` & `titandevice-0.4.0/titandevice.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: titandevice
-Version: 0.3.9
+Version: 0.4.0
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: adbutils
 Requires-Dist: pydantic
 
 # Titan
 
-A Python library used for managing devices, including:
+A Python library used for managing devices(must root), including:
 
-- Obtaining information of all devices
-- Checking the status of a device
+- Getting information of all devices
 - Installing Frida
-- Installing APK
+- Installing `APK`
 - And more
```

