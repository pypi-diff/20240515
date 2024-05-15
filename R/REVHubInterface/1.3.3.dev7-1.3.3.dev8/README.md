# Comparing `tmp/revhubinterface-1.3.3.dev7.tar.gz` & `tmp/revhubinterface-1.3.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.3.dev7.tar", last modified: Tue May 14 18:44:00 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.3.dev8.tar", last modified: Wed May 15 02:33:59 2024, max compression
```

## Comparing `revhubinterface-1.3.3.dev7.tar` & `revhubinterface-1.3.3.dev8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:44:00.893881 revhubinterface-1.3.3.dev7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:44:00.885881 revhubinterface-1.3.3.dev7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:44:00.889881 revhubinterface-1.3.3.dev7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 18:44:00.893881 revhubinterface-1.3.3.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:44:00.893881 revhubinterface-1.3.3.dev7/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:44:00.893881 revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 18:44:00.000000 revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-14 18:44:00.000000 revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:44:00.000000 revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 18:44:00.000000 revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 18:44:00.000000 revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 18:44:00.000000 revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:44:00.893881 revhubinterface-1.3.3.dev7/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/flatpak/flatpak-pip-generator
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 18:43:56.000000 revhubinterface-1.3.3.dev7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:44:00.893881 revhubinterface-1.3.3.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.898804 revhubinterface-1.3.3.dev8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.890804 revhubinterface-1.3.3.dev8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.890804 revhubinterface-1.3.3.dev8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-15 02:33:59.898804 revhubinterface-1.3.3.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.894804 revhubinterface-1.3.3.dev8/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.894804 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.894804 revhubinterface-1.3.3.dev8/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 02:33:59.898804 revhubinterface-1.3.3.dev8/setup.cfg
```

### Comparing `revhubinterface-1.3.3.dev7/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.3.dev8/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/.github/workflows/python-publish.yml` & `revhubinterface-1.3.3.dev8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/LICENSE.txt` & `revhubinterface-1.3.3.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/PKG-INFO` & `revhubinterface-1.3.3.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev7
+Version: 1.3.3.dev8
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev7/README.md` & `revhubinterface-1.3.3.dev8/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVADC.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVModule.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVServo.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface/__main__.py` & `revhubinterface-1.3.3.dev8/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev7
+Version: 1.3.3.dev8
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/REVHubInterface.spec` & `revhubinterface-1.3.3.dev8/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.3.dev8/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.3.dev8/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/flatpak/python3-requirements.json` & `revhubinterface-1.3.3.dev8/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.metainfo.xml`

 * *Files 3% similar despite different names*

#### Comparing `revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.metainfo.xml`

```diff
@@ -24,14 +24,18 @@
     <category>Development</category>
     <category>Science</category>
     <category>Education</category>
     <category>Robotics</category>
     <category>Monitor</category>
     <category>Electronics</category>
   </categories>
+  <branding>
+    <color type="primary" scheme-preference="light">#f05a28</color>
+    <color type="primary" scheme-preference="dark">#f05a28</color>
+  </branding>
   <screenshots>
     <screenshot type="default">
       <caption>Controlling motors</caption>
       <image type="source" width="1382" height="1590">https://unofficialrevport.org/revhubinterface/motorcontrol.png</image>
     </screenshot>
     <screenshot>
       <caption>Controlling servos</caption>
```

### Comparing `revhubinterface-1.3.3.dev7/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev7/pyproject.toml` & `revhubinterface-1.3.3.dev8/pyproject.toml`

 * *Files identical despite different names*

