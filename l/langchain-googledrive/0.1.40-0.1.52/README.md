# Comparing `tmp/langchain_googledrive-0.1.40.tar.gz` & `tmp/langchain_googledrive-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_googledrive-0.1.40.tar", max compression
+gzip compressed data, was "langchain_googledrive-0.1.52.tar", max compression
```

## Comparing `langchain_googledrive-0.1.40.tar` & `langchain_googledrive-0.1.52.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-09-29 15:31:57.756473 langchain_googledrive-0.1.40/LICENSE.txt
--rw-r--r--   0        0        0     1391 2024-03-12 07:53:57.458994 langchain_googledrive-0.1.40/README.md
--rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/__init__.py
--rw-r--r--   0        0        0       84 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/document_loaders/__init__.py
--rw-r--r--   0        0        0    13362 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.40/langchain_googledrive/document_loaders/google_drive.py
--rw-r--r--   0        0        0       90 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/retrievers/__init__.py
--rw-r--r--   0        0        0     2214 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.40/langchain_googledrive/retrievers/google_drive.py
--rw-r--r--   0        0        0       97 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/tools/google_drive/__init__.py
--rw-r--r--   0        0        0     1183 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.40/langchain_googledrive/tools/google_drive/tool.py
--rw-r--r--   0        0        0      109 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.40/langchain_googledrive/utilities/__init__.py
--rw-r--r--   0        0        0    77959 2024-04-08 10:52:09.662282 langchain_googledrive-0.1.40/langchain_googledrive/utilities/google_drive.py
--rw-r--r--   0        0        0     3399 2024-03-19 17:23:21.113431 langchain_googledrive-0.1.40/pyproject.toml
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 langchain_googledrive-0.1.40/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-29 15:31:57.756473 langchain_googledrive-0.1.52/LICENSE.txt
+-rw-r--r--   0        0        0     1391 2024-03-12 07:53:57.458994 langchain_googledrive-0.1.52/README.md
+-rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/__init__.py
+-rw-r--r--   0        0        0       84 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13362 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.52/langchain_googledrive/document_loaders/google_drive.py
+-rw-r--r--   0        0        0       90 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/retrievers/__init__.py
+-rw-r--r--   0        0        0     2214 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.52/langchain_googledrive/retrievers/google_drive.py
+-rw-r--r--   0        0        0       97 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/tools/google_drive/__init__.py
+-rw-r--r--   0        0        0     1183 2024-01-23 17:23:17.423814 langchain_googledrive-0.1.52/langchain_googledrive/tools/google_drive/tool.py
+-rw-r--r--   0        0        0      109 2023-09-05 14:03:36.513202 langchain_googledrive-0.1.52/langchain_googledrive/utilities/__init__.py
+-rw-r--r--   0        0        0    77982 2024-05-15 13:21:49.172506 langchain_googledrive-0.1.52/langchain_googledrive/utilities/google_drive.py
+-rw-r--r--   0        0        0     3399 2024-03-19 17:23:21.113431 langchain_googledrive-0.1.52/pyproject.toml
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 langchain_googledrive-0.1.52/PKG-INFO
```

### Comparing `langchain_googledrive-0.1.40/LICENSE.txt` & `langchain_googledrive-0.1.52/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.40/README.md` & `langchain_googledrive-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.40/langchain_googledrive/document_loaders/google_drive.py` & `langchain_googledrive-0.1.52/langchain_googledrive/document_loaders/google_drive.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.40/langchain_googledrive/retrievers/google_drive.py` & `langchain_googledrive-0.1.52/langchain_googledrive/retrievers/google_drive.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.40/langchain_googledrive/tools/google_drive/tool.py` & `langchain_googledrive-0.1.52/langchain_googledrive/tools/google_drive/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.40/langchain_googledrive/utilities/google_drive.py` & `langchain_googledrive-0.1.52/langchain_googledrive/utilities/google_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,15 +930,15 @@
                 return name
         except HttpError:
             # Sometime, it's impossible to get the file name of a folder.
             # It's because a shortcut reference an inaccessible file.
             return "inaccessible-folder"
 
     def _get_file_by_id(self, file_id: str, **kwargs: Any) -> Dict:
-        get_kwargs = {**self._kwargs, **kwargs, **{"fields": self.fields}}
+        get_kwargs = {**self._kwargs, **self._gdrive_kwargs, **kwargs, **{"fields": self.fields}}
         get_kwargs = {
             key: get_kwargs[key]
             for key in get_kwargs
             if key in GoogleDriveUtilities._gdrive_get_params
         }
         return self.files.get(fileId=file_id, **get_kwargs).execute()
```

### Comparing `langchain_googledrive-0.1.40/pyproject.toml` & `langchain_googledrive-0.1.52/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.1.40/PKG-INFO` & `langchain_googledrive-0.1.52/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-googledrive
-Version: 0.1.40
+Version: 0.1.52
 Summary: This is a temporary project while I wait for my langchain [pull-request](https://github.com/hwchase17/langchain/pull/5135) to be validated.
 Home-page: https://www.github.com/pprados/langchain-googledrive
 License: Apache 2.0
 Author: Philippe PRADOS
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

