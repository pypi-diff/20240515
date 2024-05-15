# Comparing `tmp/titandevice-0.4.0.tar.gz` & `tmp/titandevice-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titandevice-0.4.0.tar", last modified: Wed May 15 02:47:04 2024, max compression
+gzip compressed data, was "titandevice-0.4.1.tar", last modified: Wed May 15 03:10:52 2024, max compression
```

## Comparing `titandevice-0.4.0.tar` & `titandevice-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.979767 titandevice-0.4.0/
--rw-r--r--   0 mark      (1000) mark      (1000)      573 2024-05-15 02:47:04.979767 titandevice-0.4.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      161 2024-05-11 08:04:43.000000 titandevice-0.4.0/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-15 02:47:04.979767 titandevice-0.4.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-05-15 02:46:20.000000 titandevice-0.4.0/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.975767 titandevice-0.4.0/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2689 2024-05-15 02:46:20.000000 titandevice-0.4.0/tests/tests.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.979767 titandevice-0.4.0/titandevice/
--rw-rw-r--   0 mark      (1000) mark      (1000)       33 2024-05-14 09:13:44.000000 titandevice-0.4.0/titandevice/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1162 2024-05-14 11:10:29.000000 titandevice-0.4.0/titandevice/_titian_exception.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.979767 titandevice-0.4.0/titandevice/android/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-14 09:15:12.000000 titandevice-0.4.0/titandevice/android/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3288 2024-05-15 02:32:40.000000 titandevice-0.4.0/titandevice/android/_device.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3010 2024-05-15 01:20:19.000000 titandevice-0.4.0/titandevice/android/_frida.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2033 2024-05-15 02:35:37.000000 titandevice-0.4.0/titandevice/android/_frida_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1639 2024-05-14 08:57:29.000000 titandevice-0.4.0/titandevice/android/_package_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1240 2024-05-14 09:21:38.000000 titandevice-0.4.0/titandevice/android/device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       88 2024-05-14 07:18:06.000000 titandevice-0.4.0/titandevice/utils.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 02:47:04.979767 titandevice-0.4.0/titandevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      573 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      494 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-05-15 02:47:04.000000 titandevice-0.4.0/titandevice.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:10:52.882012 titandevice-0.4.1/
+-rw-r--r--   0 mark      (1000) mark      (1000)      573 2024-05-15 03:10:52.882012 titandevice-0.4.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      161 2024-05-11 08:04:43.000000 titandevice-0.4.1/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-15 03:10:52.882012 titandevice-0.4.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-05-15 03:10:23.000000 titandevice-0.4.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:10:52.882012 titandevice-0.4.1/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2689 2024-05-15 02:46:20.000000 titandevice-0.4.1/tests/tests.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:10:52.882012 titandevice-0.4.1/titandevice/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       33 2024-05-14 09:13:44.000000 titandevice-0.4.1/titandevice/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1162 2024-05-14 11:10:29.000000 titandevice-0.4.1/titandevice/_titian_exception.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:10:52.882012 titandevice-0.4.1/titandevice/android/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-14 09:15:12.000000 titandevice-0.4.1/titandevice/android/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3280 2024-05-15 03:09:28.000000 titandevice-0.4.1/titandevice/android/device.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1234 2024-05-15 03:09:28.000000 titandevice-0.4.1/titandevice/android/device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3006 2024-05-15 03:09:28.000000 titandevice-0.4.1/titandevice/android/frida.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2026 2024-05-15 03:09:55.000000 titandevice-0.4.1/titandevice/android/frida_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1638 2024-05-15 03:09:28.000000 titandevice-0.4.1/titandevice/android/package_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       88 2024-05-14 07:18:06.000000 titandevice-0.4.1/titandevice/utils.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:10:52.882012 titandevice-0.4.1/titandevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      573 2024-05-15 03:10:52.000000 titandevice-0.4.1/titandevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      490 2024-05-15 03:10:52.000000 titandevice-0.4.1/titandevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-15 03:10:52.000000 titandevice-0.4.1/titandevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-05-15 03:10:52.000000 titandevice-0.4.1/titandevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-05-15 03:10:52.000000 titandevice-0.4.1/titandevice.egg-info/top_level.txt
```

### Comparing `titandevice-0.4.0/PKG-INFO` & `titandevice-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titandevice
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `titandevice-0.4.0/setup.py` & `titandevice-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="titandevice",
-    version="0.4.0",
+    version="0.4.1",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `titandevice-0.4.0/tests/tests.py` & `titandevice-0.4.1/tests/tests.py`

 * *Files identical despite different names*

### Comparing `titandevice-0.4.0/titandevice/_titian_exception.py` & `titandevice-0.4.1/titandevice/_titian_exception.py`

 * *Files identical despite different names*

### Comparing `titandevice-0.4.0/titandevice/android/_device.py` & `titandevice-0.4.1/titandevice/android/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from adbutils import adb
 
 from titandevice._titian_exception import DeviceMustBeRootedException
-from titandevice.android._package_manager import _AndroidPackageManager
+from titandevice.android.package_manager import AndroidPackageManager
 
 
-class _AndroidDevice:
+class AndroidDevice:
 
     def __init__(self, device_serial: str):
         self.__adb_device = adb.device(device_serial)
         self.device_serial = device_serial
         self.device_ip = self.__adb_device.wlan_ip()
         self.device_is_root = self.__is_root()
         self.device_device = self.__adb_device.prop.device
         self.device_model = self.__adb_device.prop.model
         self.device_product = self.__adb_device.prop.name
-        self.__package_manager = _AndroidPackageManager(self.__adb_device)
+        self.__package_manager = AndroidPackageManager(self.__adb_device)
 
-    def get_package_manager(self) -> _AndroidPackageManager:
+    def get_package_manager(self) -> AndroidPackageManager:
         return self.__package_manager
 
     def get_frida_manager(
             self, frida_server_file_name_prefix, frida_server_install_path
     ):
         if not self.device_is_root:
             raise DeviceMustBeRootedException(self.device_serial)
-        from titandevice.android._frida_manager import _AndroidFridaManager
-        return _AndroidFridaManager(
+        from titandevice.android.frida_manager import AndroidFridaManager
+        return AndroidFridaManager(
             self, frida_server_file_name_prefix, frida_server_install_path
         )
 
     def __is_root(self):
         return self.file_exists("/system/xbin/su") or self.file_exists(
             "/system/bin/su"
         )
```

### Comparing `titandevice-0.4.0/titandevice/android/_frida.py` & `titandevice-0.4.1/titandevice/android/frida.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 from adbutils import adb_path
 
 from titandevice import FridaNotInstalledException
 from titandevice.utils import get_file_name_from_path
 
 
-class _AndroidFrida:
+class AndroidFrida:
 
     @staticmethod
     def __check_is_installed(func):
 
         def wrapper(self, *args, **kwargs):
             if not self.__android_device.file_exists(self.__frida_server_full_path):
                 raise FridaNotInstalledException(
                     self.__android_device.device_serial, self.__frida_server_full_path
                 )
             return func(self, *args, **kwargs)
 
         return wrapper
 
     def __init__(self, android_device, frida_server_executable_file_path):
-        from titandevice.android._device import _AndroidDevice
-        self.__android_device: _AndroidDevice = android_device
+        from titandevice.android.device import AndroidDevice
+        self.__android_device: AndroidDevice = android_device
         self.__frida_server_full_path = frida_server_executable_file_path
         self.__frida_server_path = os.path.abspath(frida_server_executable_file_path)
         self.__frida_server_name = get_file_name_from_path(
             frida_server_executable_file_path
         )
         self.__version = self.__get_version()
         self.__is_running = self.__check_if_running()
```

### Comparing `titandevice-0.4.0/titandevice/android/_frida_manager.py` & `titandevice-0.4.1/titandevice/android/frida_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from titandevice.android._device import _AndroidDevice
+from titandevice.android.device import AndroidDevice
 
 
-class _AndroidFridaManager:
+class AndroidFridaManager:
     def __init__(
-            self, android_device: _AndroidDevice, frida_server_file_name_prefix: str,
+            self, android_device: AndroidDevice, frida_server_file_name_prefix: str,
             frida_server_install_path: str
     ):
         self.__android_device = android_device
         self.__frida_server_file_name_prefix = frida_server_file_name_prefix
         if not frida_server_install_path.endswith('/'):
             frida_server_install_path += '/'
         self.__frida_server_install_path = frida_server_install_path
 
     def get_all_frida(self):
-        from titandevice.android._frida import _AndroidFrida
+        from titandevice.android.frida import AndroidFrida
         return [
-            _AndroidFrida(self.__android_device, frida_server_path) for
+            AndroidFrida(self.__android_device, frida_server_path) for
             frida_server_path in
             self.get_all_frida_executable_file_path()
         ]
 
     def get_all_frida_executable_file_path(self) -> list[str]:
         files = self.__android_device.get_all_files(self.__frida_server_install_path)
         return [self.__get_frida_server_path(file) for file in files if
```

### Comparing `titandevice-0.4.0/titandevice/android/_package_manager.py` & `titandevice-0.4.1/titandevice/android/package_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import apkutils2
 from adbutils import AdbDevice, RunningAppInfo
 from titandevice._titian_exception import *
 
 
-class _AndroidPackageManager:
+class AndroidPackageManager:
     __adb_device: AdbDevice
 
     def __init__(self, adb_device):
         self.__adb_device = adb_device
 
     def get_installed_packages(self) -> list[str]:
         return self.__adb_device.list_packages()
```

### Comparing `titandevice-0.4.0/titandevice/android/device_manager.py` & `titandevice-0.4.1/titandevice/android/device_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import threading
 
 import adbutils
 
-from titandevice.android._device import _AndroidDevice
+from titandevice.android.device import AndroidDevice
 
 
 class AndroidDeviceManager(object):
     __instance: 'AndroidDeviceManager' = None
     __lock = threading.Lock()
-    __all_devices: list[_AndroidDevice] = None
+    __all_devices: list[AndroidDevice] = None
 
     def __new__(cls, *args, **kwargs):
         with cls.__lock:
             if not cls.__instance:
                 cls.__instance = super(AndroidDeviceManager, cls).__new__(cls)
         return cls.__instance
 
-    def get_all_devices(self) -> list[_AndroidDevice]:
+    def get_all_devices(self) -> list[AndroidDevice]:
         if self.__all_devices is None:
             self.__all_devices = [
-                _AndroidDevice(device.serial)
+                AndroidDevice(device.serial)
                 for device in adbutils.adb.device_list()
             ]
             if len(self.__all_devices) == 0:
                 from titandevice._titian_exception import AnyDeviceNoFoundException
                 raise AnyDeviceNoFoundException()
         return self.__all_devices
 
-    def get_device(self, device_serial: str) -> _AndroidDevice:
+    def get_device(self, device_serial: str) -> AndroidDevice:
         for device in self.get_all_devices():
             if device.device_serial == device_serial:
                 return device
         from titandevice._titian_exception import DeviceNoFoundException
         raise DeviceNoFoundException(device_serial)
```

### Comparing `titandevice-0.4.0/titandevice.egg-info/PKG-INFO` & `titandevice-0.4.1/titandevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titandevice
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

