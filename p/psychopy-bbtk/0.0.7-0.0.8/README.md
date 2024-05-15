# Comparing `tmp/psychopy_bbtk-0.0.7.tar.gz` & `tmp/psychopy_bbtk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy_bbtk-0.0.7.tar", last modified: Thu May  9 18:44:18 2024, max compression
+gzip compressed data, was "psychopy_bbtk-0.0.8.tar", last modified: Wed May 15 16:32:31 2024, max compression
```

## Comparing `psychopy_bbtk-0.0.7.tar` & `psychopy_bbtk-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/docs_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/docs_src/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/docs_src/generatePages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/psychopy_bbtk/
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/psychopy_bbtk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/psychopy_bbtk/components/
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/psychopy_bbtk/components/tpad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/psychopy_bbtk/forcePad.py
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/psychopy_bbtk/tpad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/tests/test_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/tests/test_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/tests/test_coder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/tests/test_coder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/tests/test_coder/test_running_via_liaison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.196690 psychopy_bbtk-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-15 16:32:31.196690 psychopy_bbtk-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/docs_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/docs_src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/docs_src/generatePages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/psychopy_bbtk/
+-rw-r--r--   0 runner    (1001) docker     (127)    19359 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/psychopy_bbtk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/psychopy_bbtk/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/psychopy_bbtk/components/tpad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/psychopy_bbtk/forcePad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/psychopy_bbtk/tpad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:32:31.196690 psychopy_bbtk-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/tests/test_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/tests/test_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/tests/test_coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/tests/test_coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/tests/test_coder/test_running_via_liaison.py
```

### Comparing `psychopy_bbtk-0.0.7/LICENSE` & `psychopy_bbtk-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.7/PKG-INFO` & `psychopy_bbtk-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-bbtk
-Version: 0.0.7
+Version: 0.0.8
 Summary: Extension package for adding support for BlackBoxToolkit devices to PsychoPy.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/psychopy/psychopy-bbtk
 Project-URL: changelog, https://github.com/psychopy/psychopy-bbtk/blob/main/CHANGELOG.txt
 Project-URL: documentation, https://pages.github.com/psychopy/psychopy-bbtk
 Project-URL: repository, https://github.com/psychopy/psychopy-bbtk
```

### Comparing `psychopy_bbtk-0.0.7/README.md` & `psychopy_bbtk-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.7/docs_src/conf.py` & `psychopy_bbtk-0.0.8/docs_src/conf.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.7/docs_src/generatePages.py` & `psychopy_bbtk-0.0.8/docs_src/generatePages.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.7/psychopy_bbtk/__init__.py` & `psychopy_bbtk-0.0.8/psychopy_bbtk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,27 @@
 """
 
 # Part of the PsychoPy library
 # Copyright (C) 2002-2018 Jonathan Peirce (C) 2019-2022 Open Science Tools Ltd.
 # Distributed under the terms of the GNU General Public License (GPL).
 
 import time
+import importlib.metadata
 from psychopy import logging
 from psychopy.hardware import serialdevice
 
+
+# get version from pyproject.toml
+try:
+    __version__ = importlib.metadata.version("psychopy-bbtk")
+except importlib.metadata.PackageNotFoundError:
+    # fallback version to "0.dev"
+    __version__ = "0.dev"
+
+
 evtChannels = {
     0: "Key4",
     1: "Key3",
     2: "Key2",
     3: "Key1",
     4: "Opto4",
     5: "Opto3",
```

### Comparing `psychopy_bbtk-0.0.7/psychopy_bbtk/components/tpad.py` & `psychopy_bbtk-0.0.8/psychopy_bbtk/components/tpad.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.7/psychopy_bbtk/forcePad.py` & `psychopy_bbtk-0.0.8/psychopy_bbtk/forcePad.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.7/psychopy_bbtk/tpad.py` & `psychopy_bbtk-0.0.8/psychopy_bbtk/tpad.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     '0': "Button 2",
     '[': "Opto 1",
     ']': "Opto 2",
 }
 
 # define format for messages
 messageFormat = (
-    r"([{channels}]) ([{states}]) ([{buttons}]) (\d\d*)"
+    r"([{channels}]) ([{states}]) ([{buttons}]) (\d\d*)\r\n"
 ).format(
     channels="".join(re.escape(key) for key in channelCodes),
     states="".join(re.escape(key) for key in stateCodes),
     buttons="".join(re.escape(key) for key in buttonCodes)
 )
 
 
@@ -281,38 +281,40 @@
 
         return devices
 
     def resetTimer(self, clock=logging.defaultClock):
         self.parent.resetTimer(clock=clock)
 
 
-class TPadVoicekey:
+class TPadVoiceKey:
     def __init__(self, *args, **kwargs):
         pass
 
 
 class TPad(sd.SerialDevice):
     def __init__(
             self, port=None, baudrate=115200,
             byteSize=8, stopBits=1,
             parity="N",  # 'N'one, 'E'ven, 'O'dd, 'M'ask,
-            eol=b"\n",
+            eol=b"\r\n",
             maxAttempts=1, pauseDuration=1/1000,
             checkAwake=True
     ):
         # get port if not given
         if port is None:
             port = self._detectComPort()[0]
         # initial value for last timer reset
         self._lastTimerReset = logging.defaultClock._timeAtLastReset
         # dict of responses by timestamp
         self.messages = {}
         # indicator that a message dispatch is currently in progress (prevents threaded 
         # dispatch loops from tripping over one another)
         self._dispatchInProgress = False
+        # attribute to store last line in case of splicing
+        self._lastLine = ""
         # nodes
         self.nodes = []
         # attribute to keep track of mode state
         self._mode = None
         self._modeLock = False
         # initialise serial
         sd.SerialDevice.__init__(
@@ -383,17 +385,26 @@
     def dispatchMessages(self):
         # do nothing if there's already a dispatch in progress
         if self._dispatchInProgress:
             return
         # mark that a dispatch has begun
         self._dispatchInProgress = True
         # get data from box
-        self.pause()
-        data = self.getResponse(length=2)
-        self.pause()
+        data = self.getResponse(length=-1, timeout=1/10000)
+        # handle line splicing
+        if data:
+            # split into lines
+            data = data.splitlines(keepends=True)
+            # prepend last unfinished line to first line of this dispatch
+            data[0] = self._lastLine + data[0]
+            # if last line wasn't finished, store it for next dispatch
+            if not data[-1].endswith("\r\n"):
+                self._lastLine = data.pop(-1)
+            else:
+                self._lastLine = ""
         # parse lines
         for line in data:
             if re.match(messageFormat, line):
                 # if line fits format, split into attributes
                 device, state, channel, time = splitTPadMessage(line)
                 # integerise number
                 channel = int(channel)
```

### Comparing `psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/PKG-INFO` & `psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-bbtk
-Version: 0.0.7
+Version: 0.0.8
 Summary: Extension package for adding support for BlackBoxToolkit devices to PsychoPy.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/psychopy/psychopy-bbtk
 Project-URL: changelog, https://github.com/psychopy/psychopy-bbtk/blob/main/CHANGELOG.txt
 Project-URL: documentation, https://pages.github.com/psychopy/psychopy-bbtk
 Project-URL: repository, https://github.com/psychopy/psychopy-bbtk
```

### Comparing `psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/SOURCES.txt` & `psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.7/pyproject.toml` & `psychopy_bbtk-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psychopy-bbtk"
-version = "0.0.7"
+version = "0.0.8"
 description = "Extension package for adding support for BlackBoxToolkit devices to PsychoPy."
 readme = "README.md"
 requires-python = ">= 3.7"
 license = {text = "GNU General Public License v3 (GPLv3)"}
 authors = [
   { name = "Jon Peirce", email = "jon@opensceincetools.org" },
   { name = "Matthew Cutone", email = "mcutone@opensceincetools.org" },
```

### Comparing `psychopy_bbtk-0.0.7/tests/test_coder/test_running_via_liaison.py` & `psychopy_bbtk-0.0.8/tests/test_coder/test_running_via_liaison.py`

 * *Files identical despite different names*

