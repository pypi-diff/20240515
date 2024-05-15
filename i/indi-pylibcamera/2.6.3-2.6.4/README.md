# Comparing `tmp/indi_pylibcamera-2.6.3.tar.gz` & `tmp/indi_pylibcamera-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indi_pylibcamera-2.6.3.tar", last modified: Wed May  8 08:10:33 2024, max compression
+gzip compressed data, was "indi_pylibcamera-2.6.4.tar", last modified: Wed May 15 12:01:34 2024, max compression
```

## Comparing `indi_pylibcamera-2.6.3.tar` & `indi_pylibcamera-2.6.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2423 2024-05-08 07:52:04.000000 indi_pylibcamera-2.6.3/CHANGELOG
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1074 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/LICENSE
--rw-r--r--   0 sbr       (1000) sbr       (1000)      187 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/MANIFEST.in
--rw-r--r--   0 sbr       (1000) sbr       (1000)    23165 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/PKG-INFO
--rw-r--r--   0 sbr       (1000) sbr       (1000)    19324 2024-05-08 08:08:34.000000 indi_pylibcamera-2.6.3/README.md
--rw-r--r--   0 sbr       (1000) sbr       (1000)       81 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/pyproject.toml
--rw-r--r--   0 sbr       (1000) sbr       (1000)      857 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/setup.cfg
--rw-r--r--   0 sbr       (1000) sbr       (1000)       40 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/setup.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.049916 indi_pylibcamera-2.6.3/src/
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.053250 indi_pylibcamera-2.6.3/src/indi_pylibcamera/
--rw-r--r--   0 sbr       (1000) sbr       (1000)    48830 2024-04-21 18:26:02.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraControl.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1397 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1903 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/IMX290.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2074 2024-02-23 15:06:38.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2654 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1960 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2621 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     3244 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/SnoopingManager.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)       75 2024-05-08 07:49:47.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/__init__.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2472 2024-02-27 18:59:44.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.ini
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    60404 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)      216 2024-05-08 07:49:47.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.xml
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2825 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera_postinstall.py
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    28758 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indidevice.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)      902 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/make_driver_xml.py
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)     1944 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/print_camera_information.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/src/indi_pylibcamera/testpattern/
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    19253 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/testpattern/RBG_testpattern.png
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/
--rw-r--r--   0 sbr       (1000) sbr       (1000)    23165 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/PKG-INFO
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1091 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/SOURCES.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)        1 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/dependency_links.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)      249 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/entry_points.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)       17 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/top_level.txt
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-15 12:01:34.394033 indi_pylibcamera-2.6.4/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2518 2024-05-15 11:59:34.000000 indi_pylibcamera-2.6.4/CHANGELOG
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1074 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/LICENSE
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      187 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/MANIFEST.in
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    23260 2024-05-15 12:01:34.394033 indi_pylibcamera-2.6.4/PKG-INFO
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    19324 2024-05-08 08:08:34.000000 indi_pylibcamera-2.6.4/README.md
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       81 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/pyproject.toml
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      857 2024-05-15 12:01:34.394033 indi_pylibcamera-2.6.4/setup.cfg
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       40 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/setup.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-15 12:01:34.377366 indi_pylibcamera-2.6.4/src/
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-15 12:01:34.384033 indi_pylibcamera-2.6.4/src/indi_pylibcamera/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    48832 2024-05-15 11:59:34.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraControl.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-15 12:01:34.390699 indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1397 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1903 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/IMX290.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2074 2024-02-23 15:06:38.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2654 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1960 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2621 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     3244 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/SnoopingManager.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       75 2024-05-15 11:59:34.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/__init__.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2472 2024-02-27 18:59:44.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/indi_pylibcamera.ini
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    60404 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/indi_pylibcamera.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      216 2024-05-15 11:59:34.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/indi_pylibcamera.xml
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2825 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/indi_pylibcamera_postinstall.py
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    28758 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/indidevice.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      902 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/make_driver_xml.py
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)     1944 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/print_camera_information.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-15 12:01:34.390699 indi_pylibcamera-2.6.4/src/indi_pylibcamera/testpattern/
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    19253 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera/testpattern/RBG_testpattern.png
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-15 12:01:34.394033 indi_pylibcamera-2.6.4/src/indi_pylibcamera.egg-info/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    23260 2024-05-15 12:01:34.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera.egg-info/PKG-INFO
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1091 2024-05-15 12:01:34.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera.egg-info/SOURCES.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)        1 2024-05-15 12:01:34.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera.egg-info/dependency_links.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      249 2024-05-15 12:01:34.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera.egg-info/entry_points.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       17 2024-05-15 12:01:34.000000 indi_pylibcamera-2.6.4/src/indi_pylibcamera.egg-info/top_level.txt
```

### Comparing `indi_pylibcamera-2.6.3/CHANGELOG` & `indi_pylibcamera-2.6.4/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2.6.4
+- fixed maximum exposure time for cameras reporting max < min (for instance for IMX296)
+
 2.6.3
 - fixed installation issues
 
 2.6.2
 - fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
   have the Bayer pattern in the correct order)
 - more details in install_requires of the wheel
```

### Comparing `indi_pylibcamera-2.6.3/LICENSE` & `indi_pylibcamera-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/PKG-INFO` & `indi_pylibcamera-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indi_pylibcamera
-Version: 2.6.3
+Version: 2.6.4
 Summary: An INDI driver for Raspberry Pi cameras supported by libcamera
 Home-page: https://github.com/scriptorron/indi_pylibcamera
 Author: Ronald Schreiber
 Author-email: ronald.schreiber01@gmx.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -351,14 +351,17 @@
 - Simon Šander
 - Aaron W Morris
 - Caden Gobat
 - anjok
 
 I hope I did not forget someone. If so please do not be angry and tell me.
 
+2.6.4
+- fixed maximum exposure time for cameras reporting max < min (for instance for IMX296)
+
 2.6.3
 - fixed installation issues
 
 2.6.2
 - fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
   have the Bayer pattern in the correct order)
 - more details in install_requires of the wheel
```

### Comparing `indi_pylibcamera-2.6.3/README.md` & `indi_pylibcamera-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/setup.cfg` & `indi_pylibcamera-2.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraControl.py` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
             self.RawModes = []
         # camera controls
         self.camera_controls = self.picam2.camera_controls
         # gain and exposure time range
         self.min_ExposureTime, self.max_ExposureTime, default_exp = self.camera_controls["ExposureTime"]
         self.min_AnalogueGain, self.max_AnalogueGain, default_again = self.camera_controls["AnalogueGain"]
         # workaround for cameras reporting max_ExposureTime=0 (IMX296)
-        self.max_ExposureTime = self.max_ExposureTime if self.min_ExposureTime < self.max_ExposureTime else 1000.0
+        self.max_ExposureTime = self.max_ExposureTime if self.min_ExposureTime < self.max_ExposureTime else 1000.0e6
         self.max_AnalogueGain = self.max_AnalogueGain if self.min_AnalogueGain < self.max_AnalogueGain else 1000.0
         # TODO
         force_Restart = self.config.get("driver", "force_Restart", fallback="auto").lower()
         if force_Restart == "yes":
             logger.info("INI setting forces camera restart")
             self.needs_Restarts = True
         elif force_Restart == "no":
```

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/IMX290.txt` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/IMX290.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/SnoopingManager.py` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/SnoopingManager.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.ini` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/indi_pylibcamera.ini`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.py` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/indi_pylibcamera.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera_postinstall.py` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/indi_pylibcamera_postinstall.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/indidevice.py` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/indidevice.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/make_driver_xml.py` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/make_driver_xml.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/print_camera_information.py` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/print_camera_information.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera/testpattern/RBG_testpattern.png` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera/testpattern/RBG_testpattern.png`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/PKG-INFO` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indi_pylibcamera
-Version: 2.6.3
+Version: 2.6.4
 Summary: An INDI driver for Raspberry Pi cameras supported by libcamera
 Home-page: https://github.com/scriptorron/indi_pylibcamera
 Author: Ronald Schreiber
 Author-email: ronald.schreiber01@gmx.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -351,14 +351,17 @@
 - Simon Šander
 - Aaron W Morris
 - Caden Gobat
 - anjok
 
 I hope I did not forget someone. If so please do not be angry and tell me.
 
+2.6.4
+- fixed maximum exposure time for cameras reporting max < min (for instance for IMX296)
+
 2.6.3
 - fixed installation issues
 
 2.6.2
 - fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
   have the Bayer pattern in the correct order)
 - more details in install_requires of the wheel
```

### Comparing `indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/SOURCES.txt` & `indi_pylibcamera-2.6.4/src/indi_pylibcamera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

