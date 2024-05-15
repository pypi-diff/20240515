# Comparing `tmp/pynanovna-0.0.6.tar.gz` & `tmp/pynanovna-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynanovna-0.0.6.tar", last modified: Mon May  6 16:31:42 2024, max compression
+gzip compressed data, was "pynanovna-0.0.7.tar", last modified: Wed May 15 12:36:17 2024, max compression
```

## Comparing `pynanovna-0.0.6.tar` & `pynanovna-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.725478 pynanovna-0.0.6/
--rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.6/LICENCE
--rw-r--r--   0 teo        (501) staff       (20)     1325 2024-05-06 16:31:42.724672 pynanovna-0.0.6/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)      668 2024-05-04 14:44:35.000000 pynanovna-0.0.6/README.md
--rw-r--r--   0 teo        (501) staff       (20)      637 2024-05-06 16:31:13.000000 pynanovna-0.0.6/pyproject.toml
--rw-r--r--   0 teo        (501) staff       (20)       38 2024-05-06 16:31:42.725646 pynanovna-0.0.6/setup.cfg
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.671632 pynanovna-0.0.6/src/
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.691628 pynanovna-0.0.6/src/pynanovna/
--rw-r--r--   0 teo        (501) staff       (20)    16095 2024-05-04 11:44:22.000000 pynanovna-0.0.6/src/pynanovna/Calibration.py
--rw-r--r--   0 teo        (501) staff       (20)     8952 2024-05-04 11:44:22.000000 pynanovna-0.0.6/src/pynanovna/CalibrationGuide.py
--rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.6/src/pynanovna/RFTools.py
--rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.6/src/pynanovna/SITools.py
--rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.6/src/pynanovna/Sweep.py
--rw-r--r--   0 teo        (501) staff       (20)    11095 2024-05-06 16:28:01.000000 pynanovna-0.0.6/src/pynanovna/SweepWorker.py
--rw-r--r--   0 teo        (501) staff       (20)     8824 2024-05-04 11:44:22.000000 pynanovna-0.0.6/src/pynanovna/Touchstone.py
--rw-r--r--   0 teo        (501) staff       (20)      101 2024-05-04 14:14:44.000000 pynanovna-0.0.6/src/pynanovna/__init__.py
--rw-r--r--   0 teo        (501) staff       (20)      653 2024-05-04 14:20:41.000000 pynanovna-0.0.6/src/pynanovna/example.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.719961 pynanovna-0.0.6/src/pynanovna/hardware/
--rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/AVNA.py
--rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/Hardware.py
--rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/JNCRadio_VNA_3G.py
--rw-r--r--   0 teo        (501) staff       (20)     4134 2024-05-06 16:27:53.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA.py
--rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_F.py
--rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_F_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_H.py
--rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_H4.py
--rw-r--r--   0 teo        (501) staff       (20)     9852 2024-05-06 15:57:18.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/SV4401A.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/SV6301A.py
--rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/Serial.py
--rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/TinySA.py
--rw-r--r--   0 teo        (501) staff       (20)     6490 2024-05-06 16:28:00.000000 pynanovna-0.0.6/src/pynanovna/hardware/VNA.py
--rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/Version.py
--rw-r--r--   0 teo        (501) staff       (20)    10177 2024-05-06 16:24:11.000000 pynanovna-0.0.6/src/pynanovna/pynanovna.py
--rw-r--r--   0 teo        (501) staff       (20)     3973 2024-05-04 14:02:01.000000 pynanovna-0.0.6/src/pynanovna/vis.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.722318 pynanovna-0.0.6/src/pynanovna.egg-info/
--rw-r--r--   0 teo        (501) staff       (20)     1325 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)     1033 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/SOURCES.txt
--rw-r--r--   0 teo        (501) staff       (20)        1 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/dependency_links.txt
--rw-r--r--   0 teo        (501) staff       (20)       60 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/requires.txt
--rw-r--r--   0 teo        (501) staff       (20)       10 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/top_level.txt
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-15 12:36:17.198414 pynanovna-0.0.7/
+-rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.7/LICENCE
+-rw-r--r--   0 teo        (501) staff       (20)     1325 2024-05-15 12:36:17.197723 pynanovna-0.0.7/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)      668 2024-05-04 14:44:35.000000 pynanovna-0.0.7/README.md
+-rw-r--r--   0 teo        (501) staff       (20)      637 2024-05-15 12:34:08.000000 pynanovna-0.0.7/pyproject.toml
+-rw-r--r--   0 teo        (501) staff       (20)       38 2024-05-15 12:36:17.198519 pynanovna-0.0.7/setup.cfg
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-15 12:36:17.176240 pynanovna-0.0.7/src/
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-15 12:36:17.182787 pynanovna-0.0.7/src/pynanovna/
+-rw-r--r--   0 teo        (501) staff       (20)    16095 2024-05-04 11:44:22.000000 pynanovna-0.0.7/src/pynanovna/Calibration.py
+-rw-r--r--   0 teo        (501) staff       (20)     8958 2024-05-13 15:58:37.000000 pynanovna-0.0.7/src/pynanovna/CalibrationGuide.py
+-rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.7/src/pynanovna/RFTools.py
+-rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.7/src/pynanovna/SITools.py
+-rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.7/src/pynanovna/Sweep.py
+-rw-r--r--   0 teo        (501) staff       (20)    11095 2024-05-06 16:28:01.000000 pynanovna-0.0.7/src/pynanovna/SweepWorker.py
+-rw-r--r--   0 teo        (501) staff       (20)     8824 2024-05-04 11:44:22.000000 pynanovna-0.0.7/src/pynanovna/Touchstone.py
+-rw-r--r--   0 teo        (501) staff       (20)      101 2024-05-04 14:14:44.000000 pynanovna-0.0.7/src/pynanovna/__init__.py
+-rw-r--r--   0 teo        (501) staff       (20)      653 2024-05-04 14:20:41.000000 pynanovna-0.0.7/src/pynanovna/example.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-15 12:36:17.196128 pynanovna-0.0.7/src/pynanovna/hardware/
+-rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/AVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/Hardware.py
+-rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/JNCRadio_VNA_3G.py
+-rw-r--r--   0 teo        (501) staff       (20)     4134 2024-05-06 16:27:53.000000 pynanovna-0.0.7/src/pynanovna/hardware/NanoVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/NanoVNA_F.py
+-rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/NanoVNA_F_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/NanoVNA_H.py
+-rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/NanoVNA_H4.py
+-rw-r--r--   0 teo        (501) staff       (20)     9852 2024-05-06 15:57:18.000000 pynanovna-0.0.7/src/pynanovna/hardware/NanoVNA_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/SV4401A.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/SV6301A.py
+-rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/Serial.py
+-rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/TinySA.py
+-rw-r--r--   0 teo        (501) staff       (20)     6490 2024-05-06 16:28:00.000000 pynanovna-0.0.7/src/pynanovna/hardware/VNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.7/src/pynanovna/hardware/Version.py
+-rw-r--r--   0 teo        (501) staff       (20)    10493 2024-05-15 12:34:52.000000 pynanovna-0.0.7/src/pynanovna/pynanovna.py
+-rw-r--r--   0 teo        (501) staff       (20)     4125 2024-05-15 12:34:52.000000 pynanovna-0.0.7/src/pynanovna/vis.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-15 12:36:17.196949 pynanovna-0.0.7/src/pynanovna.egg-info/
+-rw-r--r--   0 teo        (501) staff       (20)     1325 2024-05-15 12:36:17.000000 pynanovna-0.0.7/src/pynanovna.egg-info/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)     1033 2024-05-15 12:36:17.000000 pynanovna-0.0.7/src/pynanovna.egg-info/SOURCES.txt
+-rw-r--r--   0 teo        (501) staff       (20)        1 2024-05-15 12:36:17.000000 pynanovna-0.0.7/src/pynanovna.egg-info/dependency_links.txt
+-rw-r--r--   0 teo        (501) staff       (20)       60 2024-05-15 12:36:17.000000 pynanovna-0.0.7/src/pynanovna.egg-info/requires.txt
+-rw-r--r--   0 teo        (501) staff       (20)       10 2024-05-15 12:36:17.000000 pynanovna-0.0.7/src/pynanovna.egg-info/top_level.txt
```

### Comparing `pynanovna-0.0.6/LICENCE` & `pynanovna-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/PKG-INFO` & `pynanovna-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanovna
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to use a NanoVNA
 Author-email: Teo Bergkvist <bergkvist.teo@protonmail.com>
 Project-URL: Homepage, https://github.com/PICC-Group/pynanovna
 Project-URL: Issues, https://github.com/PICC-Group/pynanovna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pynanovna-0.0.6/README.md` & `pynanovna-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/pyproject.toml` & `pynanovna-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pynanovna"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name = "Teo Bergkvist", email = "bergkvist.teo@protonmail.com" },
 ]
 description = "A package to use a NanoVNA"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `pynanovna-0.0.6/src/pynanovna/Calibration.py` & `pynanovna-0.0.7/src/pynanovna/Calibration.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/CalibrationGuide.py` & `pynanovna-0.0.7/src/pynanovna/CalibrationGuide.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             return True
 
         if self.nextStep == 1:
             # Open
             self.cal_save("open")
             self.nextStep = 2
             response = input(
-                """Calibrate load.\nPlease connect the "load" standard to port 0 of the NanoVNA.\n\nPress Ok when you are ready to continue. (q to quit)."""
+                """Calibrate load.\nPlease connect the "load" standard to port 0 of the NanoVNA.\n\nPress enter when you are ready to continue. (q to quit)."""
             )
 
             if response.lower() == "q":
                 self.nextStep = -1
                 return False
             self.worker.run()
             return True
@@ -209,15 +209,15 @@
             return True
 
         if self.nextStep == 3:
             # Isolation
             self.cal_save("isolation")
             self.nextStep = 4
             response = input(
-                """Calibrate through.\nPlease connect the "through" standard between port 0 and port 1 of the NanoVNA.\n\nPress Ok when you are ready to continue. (q to quit)."""
+                """Calibrate through.\nPlease connect the "through" standard between port 0 and port 1 of the NanoVNA.\n\nPress enter when you are ready to continue. (q to quit)."""
             )
 
             if response.lower() == "q":
                 self.nextStep = -1
                 return False
             self.worker.run()
             return True
```

### Comparing `pynanovna-0.0.6/src/pynanovna/RFTools.py` & `pynanovna-0.0.7/src/pynanovna/RFTools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/SITools.py` & `pynanovna-0.0.7/src/pynanovna/SITools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/Sweep.py` & `pynanovna-0.0.7/src/pynanovna/Sweep.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/SweepWorker.py` & `pynanovna-0.0.7/src/pynanovna/SweepWorker.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/Touchstone.py` & `pynanovna-0.0.7/src/pynanovna/Touchstone.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/example.py` & `pynanovna-0.0.7/src/pynanovna/example.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/AVNA.py` & `pynanovna-0.0.7/src/pynanovna/hardware/AVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/Hardware.py` & `pynanovna-0.0.7/src/pynanovna/hardware/Hardware.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/JNCRadio_VNA_3G.py` & `pynanovna-0.0.7/src/pynanovna/hardware/JNCRadio_VNA_3G.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA.py` & `pynanovna-0.0.7/src/pynanovna/hardware/NanoVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_V2.py` & `pynanovna-0.0.7/src/pynanovna/hardware/NanoVNA_V2.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/SV4401A.py` & `pynanovna-0.0.7/src/pynanovna/hardware/SV4401A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/SV6301A.py` & `pynanovna-0.0.7/src/pynanovna/hardware/SV6301A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/Serial.py` & `pynanovna-0.0.7/src/pynanovna/hardware/Serial.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/TinySA.py` & `pynanovna-0.0.7/src/pynanovna/hardware/TinySA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/VNA.py` & `pynanovna-0.0.7/src/pynanovna/hardware/VNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/hardware/Version.py` & `pynanovna-0.0.7/src/pynanovna/hardware/Version.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.6/src/pynanovna/pynanovna.py` & `pynanovna-0.0.7/src/pynanovna/pynanovna.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,24 @@
             )
             if self.verbose:
                 print("VNA is connected: ", self.vna.connected())
                 print("Firmware: ", self.vna.readFirmware())
                 print("Features: ", self.vna.read_features())
                 print("Version", self.vna.name)
 
-    def calibrate(self, savefile=None, load_file=False):
+    def calibrate(
+        self,
+        load_file=False,
+        savefile=None,
+    ):
         """Run the calibration guide and calibrate the NanoVNA.
 
         Args:
-            savefile (path): Path to save the calibration. Defaults to None.
             load_file (bool, optional): Path to existing calibration. Defaults to False.
+            savefile (path): Path to save the calibration. Defaults to None.
         """
         if self.playback_mode:
             print("Cannot calibrate in playback mode. Connect NanoVNA and restart.")
             return
         if load_file:
             self.CalibrationGuide.loadCalibration(load_file)
             return
@@ -90,33 +94,35 @@
         if self.playback_mode:
             print("Cannot do a sweep in playback mode. Connect NanoVNA and restart.")
             return
         self.worker.sweep.set_mode("SINGLE")
         self.worker.run()
         return self._get_data()
 
-    def stream_data(self, data_file=False):
+    def stream_data(self, data_file=False, start_delay=2.0):
         """Creates a data stream from the continuous sweeping. (Or a previously recorded file.)
 
         Args:
             data_file (string): Path to a previously recorded csv file to stream from. Defaults to False.
+            start_delay (float): Time to wait for the stream to start before yielding values.
 
         Yields:
             list: Yields a list of data when new data is available.
         """
-        if not data_file:
-            self._stream_data()
-        sleep(2)
         try:
             if not data_file:
                 if self.playback_mode:
                     print(
                         "Cannot stream data from NanoVNA in playback mode. Connect NanoVNA and restart."
                     )
                     return
+
+                self._stream_data()
+                sleep(start_delay)
+
                 stream = self._access_data()
             else:
                 stream = self._csv_streamer(data_file)
 
             for data in stream:
                 yield data  # Yield each piece of data as it comes
 
@@ -155,24 +161,28 @@
                     if i != 0:
                         if sweepdivider in line:
                             if package != ([], []):
                                 yield package
                             package = ([], [])
                             continue
                         data_vals = [complex(val) for val in line.split(",")]
-                        package[0].append(Datapoint(
-                            data_vals[-1].real,
-                            data_vals[0].real,
-                            data_vals[0].imag,
-                        ))
-                        package[1].append(Datapoint(
-                            data_vals[-1].real,
-                            data_vals[1].real,
-                            data_vals[1].imag,
-                        ))
+                        package[0].append(
+                            Datapoint(
+                                data_vals[-1].real,
+                                data_vals[0].real,
+                                data_vals[0].imag,
+                            )
+                        )
+                        package[1].append(
+                            Datapoint(
+                                data_vals[-1].real,
+                                data_vals[1].real,
+                                data_vals[1].imag,
+                            )
+                        )
         except KeyboardInterrupt:
             return
         except Exception as e:
             print(e)
 
     def _access_data(self):
         """Fetches the data from the sweep worker as long as it is running a sweep.
@@ -254,15 +264,16 @@
 
         Raises:
             Exception: If the NanoVNA was not successfully disconnected.
         """
         if self.playback_mode:
             print("Cannot kill in playback mode. Connect NanoVNA and restart.")
             return
-        self._stop_worker()
+        if self.worker.running:
+            self._stop_worker()
         self.vna.disconnect()
         if self.vna.connected():
             raise Exception("The VNA was not successfully disconnected.")
         else:
             if self.verbose:
                 print("Disconnected VNA.")
             return
```

### Comparing `pynanovna-0.0.6/src/pynanovna/vis.py` & `pynanovna-0.0.7/src/pynanovna/vis.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,19 @@
 
                 fig.canvas.draw()
                 fig.canvas.flush_events()
                 plt.pause(0.01)
 
         except KeyboardInterrupt:
             return
-        
+
         except Exception as e:
             print("Error in plot: ", e)
 
+
 def polar(stream, normalize=False):
     plt.ion()
     fig, ax = plt.subplots(1, 2, subplot_kw=dict(polar=True))
     fig.tight_layout(pad=4.0)
 
     # Initialize lines for each subplot
     (line1,) = ax[0].plot([], [], label="S11")
@@ -85,16 +86,22 @@
                     ax[0].set_ylim(min(s11) * 10, max(s11) * 10)
                     ax[1].set_ylim(min(s21) * 10, max(s21) * 10)
 
                     if normalize:
                         first_s11, first_s21 = s11[0], s21[0]
                         first_phase1, first_phase2 = theta1[0], theta2[0]
 
-                        ax[0].set_ylim(min([gain - first_s11 for gain in s11]) * 10, max([gain - first_s11 for gain in s11]) * 10)
-                        ax[1].set_ylim(min([gain - first_s21 for gain in s21]) * 10, max([gain - first_s21 for gain in s21]) * 10)
+                        ax[0].set_ylim(
+                            min([gain - first_s11 for gain in s11]) * 10,
+                            max([gain - first_s11 for gain in s11]) * 10,
+                        )
+                        ax[1].set_ylim(
+                            min([gain - first_s21 for gain in s21]) * 10,
+                            max([gain - first_s21 for gain in s21]) * 10,
+                        )
 
                     first_data = False
 
                 if normalize:
                     s11 = [gain - first_s11 for gain in s11]
                     s21 = [gain - first_s21 for gain in s21]
                     theta1 = [(phase - first_phase1) % (2 * pi) for phase in theta1]
@@ -105,10 +112,10 @@
 
                 fig.canvas.draw()
                 fig.canvas.flush_events()
                 plt.pause(0.01)
 
         except KeyboardInterrupt:
             return
-        
+
         except Exception as e:
-            print("Error in plot: ", e)
+            print("Error in plot: ", e)
```

### Comparing `pynanovna-0.0.6/src/pynanovna.egg-info/PKG-INFO` & `pynanovna-0.0.7/src/pynanovna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanovna
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to use a NanoVNA
 Author-email: Teo Bergkvist <bergkvist.teo@protonmail.com>
 Project-URL: Homepage, https://github.com/PICC-Group/pynanovna
 Project-URL: Issues, https://github.com/PICC-Group/pynanovna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pynanovna-0.0.6/src/pynanovna.egg-info/SOURCES.txt` & `pynanovna-0.0.7/src/pynanovna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

