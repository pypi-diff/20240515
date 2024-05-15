# Comparing `tmp/as7262-0.1.0.tar.gz` & `tmp/as7262-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/as7262-0.1.0.tar", last modified: Fri Sep 13 10:46:56 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `as7262-0.1.0.tar` & `as7262-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 10:46:56.000000 as7262-0.1.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     2488 2019-09-13 10:46:56.000000 as7262-0.1.0/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 10:46:56.000000 as7262-0.1.0/as7262/
--rw-r--r--   0 pi        (1000) pi        (1000)      781 2019-09-13 10:26:38.000000 as7262-0.1.0/as7262/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9549 2019-09-13 10:38:47.000000 as7262-0.1.0/as7262/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      108 2019-09-13 10:26:38.000000 as7262-0.1.0/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)     1189 2019-09-13 10:26:38.000000 as7262-0.1.0/README.rst
--rw-r--r--   0 pi        (1000) pi        (1000)      185 2019-09-13 10:38:47.000000 as7262-0.1.0/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2019-09-13 10:26:38.000000 as7262-0.1.0/LICENSE.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 10:46:56.000000 as7262-0.1.0/as7262.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2019-09-13 10:46:56.000000 as7262-0.1.0/as7262.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     2488 2019-09-13 10:46:56.000000 as7262-0.1.0/as7262.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2019-09-13 10:46:56.000000 as7262-0.1.0/as7262.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       17 2019-09-13 10:46:56.000000 as7262-0.1.0/as7262.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      254 2019-09-13 10:46:56.000000 as7262-0.1.0/as7262.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      165 2019-09-13 10:46:56.000000 as7262-0.1.0/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     2170 2019-09-13 10:38:47.000000 as7262-0.1.0/setup.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 as7262-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 as7262-1.0.0/Makefile
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 as7262-1.0.0/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 as7262-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 as7262-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 as7262-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 as7262-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 as7262-1.0.0/uninstall.sh
+-rw-r--r--   0        0        0     9551 2020-02-02 00:00:00.000000 as7262-1.0.0/as7262/__init__.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 as7262-1.0.0/as7262/__main__.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 as7262-1.0.0/examples/bargraph.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 as7262-1.0.0/examples/spectrum.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 as7262-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 as7262-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 as7262-1.0.0/tests/test_features.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 as7262-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 as7262-1.0.0/tests/tools.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 as7262-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 as7262-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 as7262-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 as7262-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `as7262-0.1.0/as7262/__main__.py` & `as7262-1.0.0/as7262/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Library for the AS7262 Visble Light Spectral Sensor."""
+"""Library for the AS7262 Viisble Light Spectral Sensor."""
 import as7262
 
 if __name__ == '__main__':
     as7262.soft_reset()
 
     hw_type, hw_version, fw_version = as7262.get_version()
```

### Comparing `as7262-0.1.0/as7262/__init__.py` & `as7262-1.0.0/as7262/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""Library for the AS7262 Visble Light Spectral Sensor."""
-import time
+"""Library for the AS7262 Visible Light Spectral Sensor."""
 import struct
+import time
 
-from i2cdevice import Device, Register, BitField, _int_to_bytes
+from i2cdevice import BitField, Device, Register, _int_to_bytes
 from i2cdevice.adapter import Adapter, LookupAdapter
 
-__version__ = '0.1.0'
+__version__ = '1.0.0'
 
 
 class as7262VirtualRegisterBus():
     """AS7262 Virtual Register.
 
     This class implements the wacky virtual register setup
-    of the AS7262 annd allows i2cdevice.Device to "just work"
+    of the AS7262 and allows i2cdevice.Device to "just work"
     without having to worry about how registers are actually
     read or written under the hood.
 
     """
 
     def __init__(self, i2c_dev=None):
         """Initialise virtual register class.
 
         :param bus: SMBus bus ID
 
         """
         if i2c_dev is None:
-            import smbus
-            self._i2c_bus = smbus.SMBus(1)
+            import smbus2
+            self._i2c_bus = smbus2.SMBus(1)
         else:
             self._i2c_bus = i2c_dev
 
     def get_status(self, address):
         """Return the AS7262 status register."""
         return self._i2c_bus.read_byte_data(address, 0x00)
```

### Comparing `as7262-0.1.0/LICENSE.txt` & `as7262-1.0.0/LICENSE`

 * *Files identical despite different names*

