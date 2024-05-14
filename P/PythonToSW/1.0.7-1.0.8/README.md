# Comparing `tmp/PythonToSW-1.0.7.tar.gz` & `tmp/PythonToSW-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.0.7.tar", last modified: Tue May 14 18:07:36 2024, max compression
+gzip compressed data, was "PythonToSW-1.0.8.tar", last modified: Tue May 14 18:33:17 2024, max compression
```

## Comparing `PythonToSW-1.0.7.tar` & `PythonToSW-1.0.8.tar`

### file list

```diff
@@ -1,54 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.443158 PythonToSW-1.0.7/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       66 2024-05-14 18:04:45.000000 PythonToSW-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1731 2024-05-14 18:07:36.442412 PythonToSW-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.0.7/README.md
--rw-rw-rw-   0        0        0        5 2024-05-14 18:07:03.000000 PythonToSW-1.0.7/VERSION
--rw-rw-rw-   0        0        0       42 2024-05-14 18:07:36.443158 PythonToSW-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1967 2024-05-14 18:02:21.000000 PythonToSW-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.406413 PythonToSW-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.413160 PythonToSW-1.0.7/src/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.424918 PythonToSW-1.0.7/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.0.7/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.0.7/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    10866 2024-05-14 18:06:38.000000 PythonToSW-1.0.7/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.440919 PythonToSW-1.0.7/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.7/src/PythonToSW/executions/__toImport.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.0.7/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.7/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.441665 PythonToSW-1.0.7/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1731 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1614 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 18:33:17.829411 PythonToSW-1.0.8/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       66 2024-05-14 18:04:45.000000 PythonToSW-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1731 2024-05-14 18:33:17.827852 PythonToSW-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.0.8/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-14 18:33:11.000000 PythonToSW-1.0.8/VERSION
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:33:17.830159 PythonToSW-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1967 2024-05-14 18:02:21.000000 PythonToSW-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:33:17.768040 PythonToSW-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:33:17.777125 PythonToSW-1.0.8/src/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:33:17.802503 PythonToSW-1.0.8/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.0.8/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.0.8/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    10866 2024-05-14 18:06:38.000000 PythonToSW-1.0.8/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:33:17.826332 PythonToSW-1.0.8/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     3605 2024-05-14 18:30:32.000000 PythonToSW-1.0.8/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.8/src/PythonToSW/executions/__toImport.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getCharacterItem.py
+-rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getObjectData.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getVehicleComponents.py
+-rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.0.8/src/PythonToSW/executions/getVehicleData.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.0.8/src/PythonToSW/executions/setCharacterData.py
+-rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.0.8/src/PythonToSW/executions/setCharacterItem.py
+-rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.0.8/src/PythonToSW/executions/setCharacterTooltip.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.8/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.0.8/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.0.8/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.8/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:33:17.827335 PythonToSW-1.0.8/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1731 2024-05-14 18:33:17.000000 PythonToSW-1.0.8/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1938 2024-05-14 18:33:17.000000 PythonToSW-1.0.8/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:33:17.000000 PythonToSW-1.0.8/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-14 18:33:17.000000 PythonToSW-1.0.8/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 18:33:17.000000 PythonToSW-1.0.8/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.0.7/LICENSE` & `PythonToSW-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/PKG-INFO` & `PythonToSW-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.0.7/README.md` & `PythonToSW-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/setup.py` & `PythonToSW-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/__init__.py` & `PythonToSW-1.0.8/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/addon/script.lua` & `PythonToSW-1.0.8/src/PythonToSW/addon/script.lua`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/addon.py` & `PythonToSW-1.0.8/src/PythonToSW/addon.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/event.py` & `PythonToSW-1.0.8/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/exceptions.py` & `PythonToSW-1.0.8/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -78,24 +78,31 @@
 from .addMapLabel import AddMapLabel
 from .addMapLine import AddMapLine
 from .addMapObject import AddMapObject
 from .announce import Announce
 from .clearOilSpills import ClearOilSpills
 from .clearRadiation import ClearRadiation
 from .clearVehicles import ClearVehicles
+from .getCharacterItem import GetCharacterItem
+from .getObjectData import GetObjectData
 from .getPlayerCharacter import GetPlayerCharacter
 from .getPlayerPos import GetPlayerPos
 from .getPlayers import GetPlayers
 from .getSeasonalEvent import GetSeasonalEvent
 from .getUniqueID import GetUniqueID
+from .getVehicleComponents import GetVehicleComponents
+from .getVehicleData import GetVehicleData
 from .isAridDLC import IsAridDLC
 from .isSpaceDLC import IsSpaceDLC
 from .isWeaponsDLC import IsWeaponsDLC
 from .removeAdmin import RemoveAdmin
 from .removeAuth import RemoveAuth
 from .removeMapLabel import RemoveMapLabel
 from .removeMapLine import RemoveMapLine
 from .removeMapObject import RemoveMapObject
 from .removePopup import RemovePopup
+from .setCharacterData import SetCharacterData
+from .setCharacterItem import SetCharacterItem
+from .setCharacterTooltip import SetCharacterTooltip
 from .setOilSpill import SetOilSpill
 from .setPlayerPos import SetPlayerPos
 from .setPopup import SetPopup
```

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/__toImport.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/__toImport.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/announce.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.0.8/src/PythonToSW/executions/setPopup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 
 # ---- // Imports
 from . import BaseExecution
 from .. import matrix
 
 # ---- // Main
 class SetPopup(BaseExecution):
-    def __init__(self, peer_id: int, ui_id: int, visible: bool, text: str, pos: list, render_distance: int, vehicle_parent_id: int = 0, object_parent_id: int = 0):
+    def __init__(self, peer_id: int, ui_id: int, visible: bool, text: str, pos: list, renderDistance: int, vehicleParentID: int = 0, objectParentID: int = 0):
         super().__init__(
             functionName = "setPopup",
-            arguments = [peer_id, ui_id, "", visible, text, *matrix.getXYZ(pos), render_distance, vehicle_parent_id, object_parent_id]
+            arguments = [peer_id, ui_id, "", visible, text, *matrix.getXYZ(pos), renderDistance, vehicleParentID, objectParentID]
         )
```

### Comparing `PythonToSW-1.0.7/src/PythonToSW/helpers.py` & `PythonToSW-1.0.8/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW/matrix.py` & `PythonToSW-1.0.8/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.7/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.0.8/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.0.7/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.0.8/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,24 +23,31 @@
 src/PythonToSW/executions/addMapLabel.py
 src/PythonToSW/executions/addMapLine.py
 src/PythonToSW/executions/addMapObject.py
 src/PythonToSW/executions/announce.py
 src/PythonToSW/executions/clearOilSpills.py
 src/PythonToSW/executions/clearRadiation.py
 src/PythonToSW/executions/clearVehicles.py
+src/PythonToSW/executions/getCharacterItem.py
+src/PythonToSW/executions/getObjectData.py
 src/PythonToSW/executions/getPlayerCharacter.py
 src/PythonToSW/executions/getPlayerPos.py
 src/PythonToSW/executions/getPlayers.py
 src/PythonToSW/executions/getSeasonalEvent.py
 src/PythonToSW/executions/getUniqueID.py
+src/PythonToSW/executions/getVehicleComponents.py
+src/PythonToSW/executions/getVehicleData.py
 src/PythonToSW/executions/isAridDLC.py
 src/PythonToSW/executions/isSpaceDLC.py
 src/PythonToSW/executions/isWeaponsDLC.py
 src/PythonToSW/executions/removeAdmin.py
 src/PythonToSW/executions/removeAuth.py
 src/PythonToSW/executions/removeMapLabel.py
 src/PythonToSW/executions/removeMapLine.py
 src/PythonToSW/executions/removeMapObject.py
 src/PythonToSW/executions/removePopup.py
+src/PythonToSW/executions/setCharacterData.py
+src/PythonToSW/executions/setCharacterItem.py
+src/PythonToSW/executions/setCharacterTooltip.py
 src/PythonToSW/executions/setOilSpill.py
 src/PythonToSW/executions/setPlayerPos.py
 src/PythonToSW/executions/setPopup.py
```

