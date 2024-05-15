# Comparing `tmp/ansys-api-sherlock-0.1.27.tar.gz` & `tmp/ansys_api_sherlock-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-sherlock-0.1.27.tar", last modified: Tue Mar 26 08:27:37 2024, max compression
+gzip compressed data, was "ansys_api_sherlock-0.1.28.tar", last modified: Wed May 15 15:21:29 2024, max compression
```

## Comparing `ansys-api-sherlock-0.1.27.tar` & `ansys_api_sherlock-0.1.28.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:27:37.756671 ansys-api-sherlock-0.1.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-26 08:27:37.756671 ansys-api-sherlock-0.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 08:27:37.756671 ansys-api-sherlock-0.1.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:27:37.752671 ansys-api-sherlock-0.1.27/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:27:37.752671 ansys-api-sherlock-0.1.27/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:27:37.752671 ansys-api-sherlock-0.1.27/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:27:37.752671 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:27:37.756671 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockCommonService.proto
--rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockLayerService.proto
--rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockModelService.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockPartsService.proto
--rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockProjectService.proto
--rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-03-26 08:27:30.000000 ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockStackupService.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:27:37.756671 ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-26 08:27:37.000000 ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-26 08:27:37.000000 ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:27:37.000000 ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 08:27:37.000000 ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 08:27:37.000000 ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 08:27:37.000000 ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:21:29.852033 ansys_api_sherlock-0.1.28/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-15 15:21:29.852033 ansys_api_sherlock-0.1.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:21:29.852033 ansys_api_sherlock-0.1.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:21:29.844033 ansys_api_sherlock-0.1.28/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:21:29.844033 ansys_api_sherlock-0.1.28/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:21:29.844033 ansys_api_sherlock-0.1.28/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:21:29.848033 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:21:29.848033 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockCommonService.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockLayerService.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockModelService.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockPartsService.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockProjectService.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-05-15 15:21:21.000000 ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockStackupService.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:21:29.852033 ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-15 15:21:29.000000 ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-15 15:21:29.000000 ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:21:29.000000 ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 15:21:29.000000 ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 15:21:29.000000 ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 15:21:29.000000 ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/top_level.txt
```

### Comparing `ansys-api-sherlock-0.1.27/LICENSE` & `ansys_api_sherlock-0.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/PKG-INFO` & `ansys_api_sherlock-0.1.28/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.27
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 08:27:37 on 26 March 2024
+Version: 0.1.28
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 15:21:29 on 15 May 2024
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.27/README.md` & `ansys_api_sherlock-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/setup.py` & `ansys_api_sherlock-0.1.28/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto` & `ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockCommonService.proto` & `ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockCommonService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockLayerService.proto` & `ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockLayerService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto` & `ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockModelService.proto` & `ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockModelService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockPartsService.proto` & `ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockPartsService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockProjectService.proto` & `ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockProjectService.proto`

 * *Files 13% similar despite different names*

```diff
@@ -191,17 +191,17 @@
   repeated CCA ccas				= 2;	// CCA's assigned to the project.
 }
 
 /**
  * Request to add a project to Sherlock.
  */
 message AddProjectRequest {
-  string project          = 1;
-  string category         = 2;
-  string description      = 3;
+  string project          = 1; // Sherlock project name.
+  string category         = 2; // Project category.
+  string description      = 3; // Project description.
 }
 
 message CCA {
   string ccaName = 1; 									// Name of the circuit card.
   optional string description = 2; 						// Description of the circuit card.
   optional string defaultSolderType = 3; 				// Default solder type.
   optional double defaultStencilThickness = 4; 			// Default stencil thickness.
@@ -362,14 +362,30 @@
  * Request for importing a .zip project archive when Sherlock is in single project mode.
  */
  message ImportProjectZipSingleModeRequest {
   ImportProjectZipRequest projZipRequest   		= 1;  // Encapsulates project name, category and full path to project .zip archive. 
   string destFileDir							= 2;  // Directory in which the Sherlock project folder will be created. 
 }
 
+/**
+ * Request for exporting the designated Sherlock project as a .zip file.
+ */
+ message ExportProjectRequest {
+  string project				= 1; 	// Sherlock project name.
+  bool exportDesignFiles		= 2; 	// If true, export all design files assigned to the project.
+  bool exportResultFiles		= 3; 	// If true, export all analysis module results.
+  bool exportArchivedResults    = 4; 	// If true, export all archived result files.
+  bool exportUserFiles			= 5; 	// If true, export all user properties and custom data files.
+  bool exportLogFiles			= 6; 	// If true, export all Sherlock console and application logs.
+  bool exportSystemData 		= 7; 	// If true, export all system technical data.
+  string exportFileDirectory	= 8;	// Full path of the directory where the .zip file is to be exported.
+  string exportFileName			= 9; 	// Name of the zip file containing the project's exported data.
+  bool overwriteExistingFile 	= 10;   // If true, an existing file will be overwritten.
+}
+
 service SherlockProjectService {
   // Generates the project report and return it via streaming.
   rpc genReport(GenReportRequest) returns (stream GenReportResponse);
 
   // Generates the project CCA report and return it via streaming.
   rpc genCCAReport(GenCCAReportRequest) returns (stream GenCCAReportResponse);
   
@@ -407,8 +423,12 @@
   rpc addThermalMaps(AddThermalMapRequest) returns (AddThermalMapResponse);
 
   // Imports a zipped project archive -- multiple project mode.
   rpc importProjectZipArchive(ImportProjectZipRequest) returns (ReturnCode);
 
   // Imports a zipped project archive -- single project mode.
   rpc importProjectZipArchiveSingleMode(ImportProjectZipSingleModeRequest) returns (ReturnCode);
+
+  // Exports project to a zipped archive file.
+  rpc exportProject(ExportProjectRequest) returns (ReturnCode);
+
 }
```

### Comparing `ansys-api-sherlock-0.1.27/src/ansys/api/sherlock/v0/SherlockStackupService.proto` & `ansys_api_sherlock-0.1.28/src/ansys/api/sherlock/v0/SherlockStackupService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/PKG-INFO` & `ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.27
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 08:27:37 on 26 March 2024
+Version: 0.1.28
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 15:21:29 on 15 May 2024
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.27/src/ansys_api_sherlock.egg-info/SOURCES.txt` & `ansys_api_sherlock-0.1.28/src/ansys_api_sherlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

