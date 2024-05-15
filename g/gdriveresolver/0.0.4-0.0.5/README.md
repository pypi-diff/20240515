# Comparing `tmp/gdriveresolver-0.0.4.tar.gz` & `tmp/gdriveresolver-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdriveresolver-0.0.4.tar", last modified: Tue May 14 21:09:11 2024, max compression
+gzip compressed data, was "gdriveresolver-0.0.5.tar", last modified: Tue May 14 21:12:46 2024, max compression
```

## Comparing `gdriveresolver-0.0.4.tar` & `gdriveresolver-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:09:11.527958 gdriveresolver-0.0.4/
--rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.4/LICENSE
--rw-r--r--   0 harman     (501) staff       (20)     1603 2024-05-14 21:09:11.527799 gdriveresolver-0.0.4/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      992 2024-05-14 20:57:44.000000 gdriveresolver-0.0.4/README.md
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:09:11.527071 gdriveresolver-0.0.4/gdriveresolver/
--rw-r--r--   0 harman     (501) staff       (20)       42 2024-05-14 19:54:16.000000 gdriveresolver-0.0.4/gdriveresolver/__init__.py
--rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.4/gdriveresolver/exceptions.py
--rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-14 18:17:17.000000 gdriveresolver-0.0.4/gdriveresolver/model.py
--rw-r--r--   0 harman     (501) staff       (20)      850 2024-05-14 21:06:12.000000 gdriveresolver-0.0.4/gdriveresolver/resolver.py
--rw-r--r--   0 harman     (501) staff       (20)     2805 2024-05-14 19:26:42.000000 gdriveresolver-0.0.4/gdriveresolver/system_operations.py
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:09:11.527575 gdriveresolver-0.0.4/gdriveresolver.egg-info/
--rw-r--r--   0 harman     (501) staff       (20)     1603 2024-05-14 21:09:11.000000 gdriveresolver-0.0.4/gdriveresolver.egg-info/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      327 2024-05-14 21:09:11.000000 gdriveresolver-0.0.4/gdriveresolver.egg-info/SOURCES.txt
--rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-14 21:09:11.000000 gdriveresolver-0.0.4/gdriveresolver.egg-info/dependency_links.txt
--rw-r--r--   0 harman     (501) staff       (20)       15 2024-05-14 21:09:11.000000 gdriveresolver-0.0.4/gdriveresolver.egg-info/top_level.txt
--rw-r--r--   0 harman     (501) staff       (20)      683 2024-05-14 21:09:04.000000 gdriveresolver-0.0.4/pyproject.toml
--rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-14 21:09:11.527994 gdriveresolver-0.0.4/setup.cfg
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:12:46.576372 gdriveresolver-0.0.5/
+-rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.5/LICENSE
+-rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-14 21:12:46.576218 gdriveresolver-0.0.5/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      972 2024-05-14 21:11:01.000000 gdriveresolver-0.0.5/README.md
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:12:46.575278 gdriveresolver-0.0.5/gdriveresolver/
+-rw-r--r--   0 harman     (501) staff       (20)       37 2024-05-14 21:11:01.000000 gdriveresolver-0.0.5/gdriveresolver/__init__.py
+-rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.5/gdriveresolver/exceptions.py
+-rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-14 18:17:17.000000 gdriveresolver-0.0.5/gdriveresolver/model.py
+-rw-r--r--   0 harman     (501) staff       (20)      863 2024-05-14 21:12:27.000000 gdriveresolver-0.0.5/gdriveresolver/resolver.py
+-rw-r--r--   0 harman     (501) staff       (20)     2805 2024-05-14 19:26:42.000000 gdriveresolver-0.0.5/gdriveresolver/system_operations.py
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:12:46.576057 gdriveresolver-0.0.5/gdriveresolver.egg-info/
+-rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-14 21:12:46.000000 gdriveresolver-0.0.5/gdriveresolver.egg-info/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      327 2024-05-14 21:12:46.000000 gdriveresolver-0.0.5/gdriveresolver.egg-info/SOURCES.txt
+-rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-14 21:12:46.000000 gdriveresolver-0.0.5/gdriveresolver.egg-info/dependency_links.txt
+-rw-r--r--   0 harman     (501) staff       (20)       15 2024-05-14 21:12:46.000000 gdriveresolver-0.0.5/gdriveresolver.egg-info/top_level.txt
+-rw-r--r--   0 harman     (501) staff       (20)      683 2024-05-14 21:11:01.000000 gdriveresolver-0.0.5/pyproject.toml
+-rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-14 21:12:46.576405 gdriveresolver-0.0.5/setup.cfg
```

### Comparing `gdriveresolver-0.0.4/LICENSE` & `gdriveresolver-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.4/PKG-INFO` & `gdriveresolver-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,25 +16,25 @@
 Different systems may mount Google Drive to different locations. 
 This package automatically finds the mounted Google Drive directory so that it can resolve Google Drive relative
 paths to absolute system paths.
 
 Example Usage:
 
 ```python
-from gdriveresolver import GoogleDriveResolver
+from gdriveresolver import GDriveResolver
 
-gdrive_resolver = GoogleDriveResolver()
+gdrive_resolver = GDriveResolver()
 absolute_path: str = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
 ```
 
 ## Troubleshooting
 If GoogleDriveResolver cannot resolve your Google Drive path, it may not be searching at a sufficient depth.
 You can increase the depth by passing the `max_depth` parameter to the constructor.
 
 ```python
-from gdriveresolver import GoogleDriveResolver
+from gdriveresolver import GDriveResolver
 
-absolute_path = GoogleDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
+absolute_path = GDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
 print(absolute_path)
 ```
 If it still cannot resolve your path, please ensure that your Google Drive is mounted, accessible,
 and that it is called "Google Drive" or "GoogleDrive" in your system.
```

### Comparing `gdriveresolver-0.0.4/README.md` & `gdriveresolver-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 Different systems may mount Google Drive to different locations. 
 This package automatically finds the mounted Google Drive directory so that it can resolve Google Drive relative
 paths to absolute system paths.
 
 Example Usage:
 
 ```python
-from gdriveresolver import GoogleDriveResolver
+from gdriveresolver import GDriveResolver
 
-gdrive_resolver = GoogleDriveResolver()
+gdrive_resolver = GDriveResolver()
 absolute_path: str = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
 ```
 
 ## Troubleshooting
 If GoogleDriveResolver cannot resolve your Google Drive path, it may not be searching at a sufficient depth.
 You can increase the depth by passing the `max_depth` parameter to the constructor.
 
 ```python
-from gdriveresolver import GoogleDriveResolver
+from gdriveresolver import GDriveResolver
 
-absolute_path = GoogleDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
+absolute_path = GDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
 print(absolute_path)
 ```
 If it still cannot resolve your path, please ensure that your Google Drive is mounted, accessible,
 and that it is called "Google Drive" or "GoogleDrive" in your system.
```

### Comparing `gdriveresolver-0.0.4/gdriveresolver/model.py` & `gdriveresolver-0.0.5/gdriveresolver/model.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.4/gdriveresolver/resolver.py` & `gdriveresolver-0.0.5/gdriveresolver/resolver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from pathlib import Path
 from typing import Optional
 
 from .system_operations import get_operating_system, locate_google_drive
 
 
-class GoogleDriveResolver:
+class GDriveResolver:
     def __init__(self, max_depth: int = 6, max_workers: int = 5):
         self.os_type = get_operating_system()
         self.drive_path = locate_google_drive(self.os_type, max_depth, max_workers)
 
-    def resolve(self, relative_path: str) -> Optional[Path]:
+    def resolve(self, relative_path: str) -> Optional[str]:
         """
         Resolve the absolute path of a file given its relative path in Google Drive.
 
         Parameters:
             relative_path (str): The relative path within Google Drive.
 
         Returns:
             Optional[Path]: The absolute path if found, else None.
         """
         absolute_path = self.drive_path / self.os_type.sanitize_path(relative_path)
-        return absolute_path if absolute_path.exists() else None
+        if absolute_path:
+            return str(absolute_path)
+        return None
```

### Comparing `gdriveresolver-0.0.4/gdriveresolver/system_operations.py` & `gdriveresolver-0.0.5/gdriveresolver/system_operations.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.4/gdriveresolver.egg-info/PKG-INFO` & `gdriveresolver-0.0.5/gdriveresolver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,25 +16,25 @@
 Different systems may mount Google Drive to different locations. 
 This package automatically finds the mounted Google Drive directory so that it can resolve Google Drive relative
 paths to absolute system paths.
 
 Example Usage:
 
 ```python
-from gdriveresolver import GoogleDriveResolver
+from gdriveresolver import GDriveResolver
 
-gdrive_resolver = GoogleDriveResolver()
+gdrive_resolver = GDriveResolver()
 absolute_path: str = gdrive_resolver.resolve('my/path/in/google/drive/myfile.txt')
 ```
 
 ## Troubleshooting
 If GoogleDriveResolver cannot resolve your Google Drive path, it may not be searching at a sufficient depth.
 You can increase the depth by passing the `max_depth` parameter to the constructor.
 
 ```python
-from gdriveresolver import GoogleDriveResolver
+from gdriveresolver import GDriveResolver
 
-absolute_path = GoogleDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
+absolute_path = GDriveResolver(max_depth=10).resolve('my/path/in/google/drive/myfile.txt')
 print(absolute_path)
 ```
 If it still cannot resolve your path, please ensure that your Google Drive is mounted, accessible,
 and that it is called "Google Drive" or "GoogleDrive" in your system.
```

### Comparing `gdriveresolver-0.0.4/pyproject.toml` & `gdriveresolver-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gdriveresolver"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="C Harman", email="charman@netrias.com" },
 ]
 description = "A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

