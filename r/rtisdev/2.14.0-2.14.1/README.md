# Comparing `tmp/rtisdev-2.14.0.tar.gz` & `tmp/rtisdev-2.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\woute\Projects\rtisdev\dist\.tmp-s19io4xe\rtisdev-2.14.0.tar", last modified: Mon May 13 14:54:29 2024, max compression
+gzip compressed data, was "C:\Users\woute\Projects\rtisdev\dist\.tmp-ya_uu946\rtisdev-2.14.1.tar", last modified: Wed May 15 14:28:13 2024, max compression
```

## Comparing `rtisdev-2.14.0.tar` & `rtisdev-2.14.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/
--rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdev-2.14.0/LICENSE
--rw-rw-rw-   0        0        0       52 2024-04-05 08:40:05.000000 rtisdev-2.14.0/MANIFEST.in
--rw-rw-rw-   0        0        0    34213 2024-05-13 14:54:29.000000 rtisdev-2.14.0/PKG-INFO
--rw-rw-rw-   0        0        0     8123 2024-04-05 08:00:27.000000 rtisdev-2.14.0/README.md
--rw-rw-rw-   0        0        0     1832 2024-05-13 14:42:14.000000 rtisdev-2.14.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/
--rw-rw-rw-   0        0        0   224997 2024-05-13 14:42:14.000000 rtisdev-2.14.0/rtisdev/RTISDev.py
--rw-rw-rw-   0        0        0    11927 2024-05-13 14:33:14.000000 rtisdev-2.14.0/rtisdev/RTISGenerateSettings.py
--rw-rw-rw-   0        0        0     4457 2024-05-13 14:42:14.000000 rtisdev-2.14.0/rtisdev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2/
--rw-rw-rw-   0        0        0      700 2023-03-24 10:15:41.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2REC/
--rw-rw-rw-   0        0        0      281 2023-04-27 11:51:07.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2REC/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/
--rw-rw-rw-   0        0        0      699 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/
--rw-rw-rw-   0        0        0      266 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/uRTIS_v1/
--rw-rw-rw-   0        0        0      259 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/uRTIS_v1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/xRTIS_v1/
--rw-rw-rw-   0        0        0      318 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/xRTIS_v1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/
--rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/2D_5m_181.json
--rw-rw-rw-   0        0        0      114 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/2D_5m_91.json
--rw-rw-rw-   0        0        0      117 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_10m_3000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_5m_1000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_5m_3000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_5m_4000.json
--rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_5m_500.json
--rw-rw-rw-   0        0        0      182 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/custom_example_2D_5m_91.json
--rw-rw-rw-   0        0        0     8056 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/delaymatrix.csv
--rw-rw-rw-   0        0        0     1992 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/directions.csv
--rw-rw-rw-   0        0        0     8277 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/ranges.csv
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/default_20_80.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/default_25_50.json
--rw-rw-rw-   0        0        0    29236 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/flutter.csv
--rw-rw-rw-   0        0        0      180 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/flutter.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/long_20_80.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/long_25_50.json
--rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/short_20_80.json
--rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/short_25_50.json
--rw-rw-rw-   0        0        0   655360 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/simulate.bin
-drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/
--rw-rw-rw-   0        0        0    34213 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3402 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:54:29.000000 rtisdev-2.14.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/
+-rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdev-2.14.1/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-04-05 08:40:05.000000 rtisdev-2.14.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    34213 2024-05-15 14:28:13.000000 rtisdev-2.14.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8123 2024-04-05 08:00:27.000000 rtisdev-2.14.1/README.md
+-rw-rw-rw-   0        0        0     1832 2024-05-15 14:21:18.000000 rtisdev-2.14.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/
+-rw-rw-rw-   0        0        0   225706 2024-05-15 14:21:18.000000 rtisdev-2.14.1/rtisdev/RTISDev.py
+-rw-rw-rw-   0        0        0    11927 2024-05-13 14:33:14.000000 rtisdev-2.14.1/rtisdev/RTISGenerateSettings.py
+-rw-rw-rw-   0        0        0     4457 2024-05-15 14:21:18.000000 rtisdev-2.14.1/rtisdev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v2/
+-rw-rw-rw-   0        0        0      700 2023-03-24 10:15:41.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v2REC/
+-rw-rw-rw-   0        0        0      281 2023-04-27 11:51:07.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v2REC/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v3D1/
+-rw-rw-rw-   0        0        0      699 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/
+-rw-rw-rw-   0        0        0      266 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/uRTIS_v1/
+-rw-rw-rw-   0        0        0      259 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/uRTIS_v1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/xRTIS_v1/
+-rw-rw-rw-   0        0        0      318 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/microphoneLayouts/xRTIS_v1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/
+-rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/2D_5m_181.json
+-rw-rw-rw-   0        0        0      114 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/2D_5m_91.json
+-rw-rw-rw-   0        0        0      117 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/3D_10m_3000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/3D_5m_1000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/3D_5m_3000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/3D_5m_4000.json
+-rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/3D_5m_500.json
+-rw-rw-rw-   0        0        0      182 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/custom_example_2D_5m_91.json
+-rw-rw-rw-   0        0        0     8056 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/delaymatrix.csv
+-rw-rw-rw-   0        0        0     1992 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/directions.csv
+-rw-rw-rw-   0        0        0     8277 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/ranges.csv
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/default_20_80.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/default_25_50.json
+-rw-rw-rw-   0        0        0    29236 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/flutter.csv
+-rw-rw-rw-   0        0        0      180 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/flutter.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/long_20_80.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/long_25_50.json
+-rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/short_20_80.json
+-rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/short_25_50.json
+-rw-rw-rw-   0        0        0   655360 2023-03-22 13:54:21.000000 rtisdev-2.14.1/rtisdev/simulate.bin
+drwxrwxrwx   0        0        0        0 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev.egg-info/
+-rw-rw-rw-   0        0        0    34213 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3402 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-15 14:28:13.000000 rtisdev-2.14.1/rtisdev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:28:13.000000 rtisdev-2.14.1/setup.cfg
```

### Comparing `rtisdev-2.14.0/LICENSE` & `rtisdev-2.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/PKG-INFO` & `rtisdev-2.14.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdev
-Version: 2.14.0
+Version: 2.14.1
 Summary: Python module to make it easy to code with RTIS devices
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>, Arne Aerts <arne.aerts@uantwerpen.be>, Dennis Laurijssen <dennis.laurijssen@uantwerpen.be>, Jan Steckel <jan.steckel@uantwerpen.be>
 Maintainer-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `rtisdev-2.14.0/README.md` & `rtisdev-2.14.1/README.md`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/pyproject.toml` & `rtisdev-2.14.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rtisdev"
-version = "2.14.0"
+version = "2.14.1"
 description = "Python module to make it easy to code with RTIS devices"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{ name = "Wouter Jansen", email = "wouter.jansen@uantwerpen.be" },
            { name = "Arne Aerts", email = "arne.aerts@uantwerpen.be"},
            { name = "Dennis Laurijssen", email = "dennis.laurijssen@uantwerpen.be"},
            { name = "Jan Steckel", email = "jan.steckel@uantwerpen.be"}]
 maintainers = [{name = "Wouter Jansen", email = "wouter.jansen@uantwerpen.be"}]
```

### Comparing `rtisdev-2.14.0/rtisdev/RTISDev.py` & `rtisdev-2.14.1/rtisdev/RTISDev.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 SETTINGS = {}
 WORKERS = []
 CUDA_USED = False
 PACKAGE_DIRECTORY = os.path.dirname(os.path.abspath(__file__))
 BEHAVIOUR = False
 AMPLIFIER_ACTIVE = False
 DEBUG_COUNTER = 0
-VERSION = "v2.14.0"
+VERSION = "v2.14.1"
 CURRENT_RECORDING_CONFIG = ""
 
 
 class CustomFormatter(logging.Formatter):
     grey = "\x1b[38m"
     green = "\x1b[32m"
     yellow = "\x1b[33m"
@@ -605,16 +605,16 @@
             yield 'enveloppeEnable', self.enveloppeEnable
             yield 'cleanEnable', self.cleanEnable
             yield 'processingEnable', self.processingEnable
             yield 'minRange', self.minRange
             yield 'maxRange', self.maxRange
             yield "ranges" , self.ranges.tolist()
             yield 'nDirections', self.nDirections
-            yield "directions_azimuth" , self.directions[:, 0].tolist()
-            yield "directions_elevation" , self.directions[:, 1].tolist()
+            yield "directionsAzimuth" , self.directions[:, 0].tolist()
+            yield "directionsElevation" , self.directions[:, 1].tolist()
             yield 'energyscapeSplStart', self.energyscapeSplStart
             yield 'energyscapeSplStop', self.energyscapeSplStop
             yield 'pdmFc', self.pdmFc
             yield 'pdmb', self.pdmb.tolist()
             yield 'pdma', self.pdma.tolist()
             yield 'lpfesb', self.lpfesb.tolist()
             yield 'lpfesb', self.lpfesb.tolist()
@@ -1896,15 +1896,18 @@
                 if configName in SETTINGS:
                     curSettings = SETTINGS[configName]
                 else:
                     raise RTISSettingsByIDNotFoundError
 
             if not curSettings.processingSettings:
                 raise RTISProcessingSettingsError
-            inputData = packageIn.rawData
+            if curSettings.pdmEnable:
+                inputData = packageIn.rawData
+            else:
+                inputData = packageIn.processedData
             try:
                 outputData = rtiscuda.processing(inputData, int(curSettings.pdmEnable),
                                                  curSettings.processingDataDimensionOne,
                                                  curSettings.processingDataDimensionTwo,
                                                  curSettings.configName)
             except NameError:
                 raise RTISCUDAError
@@ -1920,30 +1923,36 @@
                 if configName in SETTINGS:
                     curSettings = SETTINGS[configName]
                 else:
                     raise RTISSettingsByIDNotFoundError
 
             if not curSettings.processingSettings:
                 raise RTISProcessingSettingsError
-            inputData = packageIn.rawData
+            if curSettings.pdmEnable:
+                inputData = packageIn.rawData
+            else:
+                inputData = packageIn.processedData
             try:
                 __preload(curSettings)
                 outputData = rtiscuda.processing(inputData, int(curSettings.pdmEnable),
                                                  curSettings.processingDataDimensionOne,
                                                  curSettings.processingDataDimensionTwo,
                                                  curSettings.configName)
                 __unload_one(curSettings.configName)
             except NameError:
                 raise RTISCUDAError
         elif settings is not None:
             if not settings.processingSettings:
                 raise RTISProcessingSettingsError
             try:
                 __preload(settings)
-                inputData = packageIn.rawData
+                if settings.pdmEnable:
+                    inputData = packageIn.rawData
+                else:
+                    inputData = packageIn.processedData
                 outputData = rtiscuda.processing(inputData, int(settings.pdmEnable),
                                                  settings.processingDataDimensionOne,
                                                  settings.processingDataDimensionTwo,
                                                  settings.configName)
                 __unload_one(settings.configName)
             except NameError:
                 raise RTISCUDAError
@@ -1960,33 +1969,38 @@
                 else:
                     raise RTISMultipleSettingsFoundError
             else:
                 if configName in SETTINGS:
                     curSettings = SETTINGS[configName]
                 else:
                     raise RTISSettingsByIDNotFoundError
-
-            inputData = packageIn.rawData
             settingsSignal = deepcopy(curSettings)
             settingsSignal.configName = settingsSignal.configName + "_signal"
             settingsSignal.set_signal_processing_only()
+            if settingsSignal.pdmEnable:
+                inputData = packageIn.rawData
+            else:
+                inputData = packageIn.processedData
             try:
                 __preload(settingsSignal)
                 outputData = rtiscuda.processing(inputData, int(settingsSignal.pdmEnable),
                                                  settingsSignal.processingDataDimensionOne,
                                                  settingsSignal.processingDataDimensionTwo,
                                                  settingsSignal.configName)
                 __unload_one(settingsSignal.configName)
             except NameError:
                 raise RTISCUDAError
         else:
-            inputData = packageIn.rawData
             settingsSignal = deepcopy(settings)
             settingsSignal.configName = settingsSignal.configName + "_signal"
             settingsSignal.set_signal_processing_only()
+            if settingsSignal.pdmEnable:
+                inputData = packageIn.rawData
+            else:
+                inputData = packageIn.processedData
             try:
                 __preload(settingsSignal)
                 outputData = rtiscuda.processing(inputData, int(settingsSignal.pdmEnable),
                                                  settingsSignal.processingDataDimensionOne,
                                                  settingsSignal.processingDataDimensionTwo,
                                                  settingsSignal.configName)
                 __unload_one(settingsSignal.configName)
@@ -2086,15 +2100,18 @@
                          int(settings.enveloppeEnable), int(settings.cleanEnable),
                          disableList.astype(dtype=np.uint32))
         localLogger.info("Started a processing worker.")
 
         while True:
             packageIn = inputQueue.get()
             start = time.perf_counter()
-            inputData = packageIn.rawData
+            if settings.pdmEnable:
+                inputData = packageIn.rawData
+            else:
+                inputData = packageIn.processedData
             outputData = rtiscuda.processing(inputData, int(settings.pdmEnable),
                                              settings.processingDataDimensionOne,
                                              settings.processingDataDimensionTwo,
                                              settings.configName)
             localLogger.debug("Processing with RTIS CUDA took %0.4fs", time.perf_counter() - start)
             packageIn.update_processed_data(outputData)
             packageOut = packageIn
@@ -3236,15 +3253,15 @@
                                     "Please make sure to use correct path and filename.")
 
 
 def set_processing_settings(configName: str, premade: str = None, jsonPath: str = None, customPath: str = None,
                             microphoneLayout: str = "eRTIS_v3D1", mode: int = 1, directions: int = 181,
                             azimuthLowLimit : float = -90, azimuthHighLimit : float = 90,
                             elevationLowLimit : float = -90, elevationHighLimit : float = 90,
-                            elevation2DAngle : float =0, minRange: float = 0.5, maxRange: float = 5,
+                            elevation2DAngle : float = 0, minRange: float = 0.5, maxRange: float = 5,
                             pdmEnable: bool = True, preFilterEnable: bool = False, matchedFilterEnable: bool = True,
                             beamformingEnable: bool = True, postFilterEnable: bool = False,
                             enveloppeEnable: bool = True, cleanEnable: bool = True, preloadToggle: bool = True,
                             preFilter: np.ndarray = None, postFilter: np.ndarray = None,
                             meanEnergyRangeMultiplier: float = 2,
                             maxEnergyRangeThresholdMultiplier: float = 0.5) -> bool:
     """Set the processing settings. All parameters are optional and most have default values.
@@ -4183,15 +4200,15 @@
     if configName == "":
         if len(SETTINGS) == 1:
             configName = list(SETTINGS.values())[0].configName
         else:
             raise RTISMultipleSettingsFoundError
 
     if SETTINGS[configName].processingSettings:
-        return __process(measurement, None, configName, False)
+        return __process(deepcopy(measurement), None, configName, False)
     else:
         raise RTISProcessingSettingsError
 
 
 def set_counter(newCount: int = 0) -> bool:
     """Set the internal measurement counter of the sonar hardware.
```

### Comparing `rtisdev-2.14.0/rtisdev/RTISGenerateSettings.py` & `rtisdev-2.14.1/rtisdev/RTISGenerateSettings.py`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/rtisdev/__init__.py` & `rtisdev-2.14.1/rtisdev/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,8 +96,8 @@
     ...             axs[microphone_index_i, microphone_index_j].set_xlabel("Time (Samples)")
     ...         if microphone_index_j == 0:
     ...             axs[microphone_index_i, microphone_index_j].set_ylabel("Amplitude")
     >>> plt.show()
     >>> fig.suptitle("RTIS Dev - Microphone Signals")
 """
 from .RTISDev import *
-__version__ = "2.14.0"
+__version__ = "2.14.1"
```

### Comparing `rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat` & `rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat` & `rtisdev-2.14.1/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/delaymatrix.csv` & `rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/delaymatrix.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/directions.csv` & `rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/directions.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/ranges.csv` & `rtisdev-2.14.1/rtisdev/config/premadeSettings/processing/ranges.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/flutter.csv` & `rtisdev-2.14.1/rtisdev/config/premadeSettings/recording/flutter.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/rtisdev/simulate.bin` & `rtisdev-2.14.1/rtisdev/simulate.bin`

 * *Files identical despite different names*

### Comparing `rtisdev-2.14.0/rtisdev.egg-info/PKG-INFO` & `rtisdev-2.14.1/rtisdev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdev
-Version: 2.14.0
+Version: 2.14.1
 Summary: Python module to make it easy to code with RTIS devices
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>, Arne Aerts <arne.aerts@uantwerpen.be>, Dennis Laurijssen <dennis.laurijssen@uantwerpen.be>, Jan Steckel <jan.steckel@uantwerpen.be>
 Maintainer-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `rtisdev-2.14.0/rtisdev.egg-info/SOURCES.txt` & `rtisdev-2.14.1/rtisdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

