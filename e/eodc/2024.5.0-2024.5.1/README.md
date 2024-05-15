# Comparing `tmp/eodc-2024.5.0.tar.gz` & `tmp/eodc-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2024.5.0.tar", max compression
+gzip compressed data, was "eodc-2024.5.1.tar", max compression
```

## Comparing `eodc-2024.5.0.tar` & `eodc-2024.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      676 2024-05-13 13:27:29.542054 eodc-2024.5.0/README.md
--rw-r--r--   0        0        0      195 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/__init__.py
--rw-r--r--   0        0        0     1794 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/auth.py
--rw-r--r--   0        0        0     1311 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/dask.py
--rw-r--r--   0        0        0    13711 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/faas.py
--rw-r--r--   0        0        0     1183 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/settings.py
--rw-r--r--   0        0        0     2240 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/storage.py
--rw-r--r--   0        0        0        0 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/__init__.py
--rwxr-xr-x   0        0        0    15080 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/app.py
--rw-r--r--   0        0        0      261 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/assets/app.css
--rw-r--r--   0        0        0     2539 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/cards.py
--rw-r--r--   0        0        0     8522 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/navbar.py
--rw-r--r--   0        0        0     2867 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/utils.py
--rw-r--r--   0        0        0    32787 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/workspace.py
--rw-r--r--   0        0        0     1890 2024-05-13 13:27:29.546054 eodc-2024.5.0/pyproject.toml
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.5.0/PKG-INFO
+-rw-r--r--   0        0        0      676 2024-05-15 12:52:22.455075 eodc-2024.5.1/README.md
+-rw-r--r--   0        0        0      195 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/__init__.py
+-rw-r--r--   0        0        0     1794 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/auth.py
+-rw-r--r--   0        0        0     1311 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/dask.py
+-rw-r--r--   0        0        0    13711 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/faas.py
+-rw-r--r--   0        0        0     1183 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/settings.py
+-rw-r--r--   0        0        0     2240 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/storage.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/visualisation/vessel_detection/__init__.py
+-rwxr-xr-x   0        0        0    15080 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/visualisation/vessel_detection/app.py
+-rw-r--r--   0        0        0      261 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/visualisation/vessel_detection/assets/app.css
+-rw-r--r--   0        0        0     2539 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/visualisation/vessel_detection/cards.py
+-rw-r--r--   0        0        0     8522 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/visualisation/vessel_detection/navbar.py
+-rw-r--r--   0        0        0     2867 2024-05-15 12:52:22.455075 eodc-2024.5.1/eodc/visualisation/vessel_detection/utils.py
+-rw-r--r--   0        0        0    33301 2024-05-15 12:52:22.459075 eodc-2024.5.1/eodc/workspace.py
+-rw-r--r--   0        0        0     1890 2024-05-15 12:52:22.459075 eodc-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.5.1/PKG-INFO
```

### Comparing `eodc-2024.5.0/README.md` & `eodc-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/auth.py` & `eodc-2024.5.1/eodc/auth.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/dask.py` & `eodc-2024.5.1/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/faas.py` & `eodc-2024.5.1/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/settings.py` & `eodc-2024.5.1/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/storage.py` & `eodc-2024.5.1/eodc/storage.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/visualisation/vessel_detection/app.py` & `eodc-2024.5.1/eodc/visualisation/vessel_detection/app.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/visualisation/vessel_detection/cards.py` & `eodc-2024.5.1/eodc/visualisation/vessel_detection/cards.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/visualisation/vessel_detection/navbar.py` & `eodc-2024.5.1/eodc/visualisation/vessel_detection/navbar.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/visualisation/vessel_detection/utils.py` & `eodc-2024.5.1/eodc/visualisation/vessel_detection/utils.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.0/eodc/workspace.py` & `eodc-2024.5.1/eodc/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     underlying storage system, so that the EODC API can be used with
     different providers.
 
     It also implements the DefaultStacIO interface, which allows it to
     be used with the pystac library.
     """
 
+    storage_type: StorageType
+
     @staticmethod
     def create_adapter(
         tenant_url: str = None,  # Can be ignored for Azure
         storage_type: StorageType = StorageType.MINIO,
         parameters: dict[str, Any] = {},
     ) -> Self:
         if storage_type == StorageType.MINIO:
@@ -65,14 +67,18 @@
                 access_key=parameters["access_key"],
                 secret_key=parameters["secret_key"],
             )
         else:
             return None
 
     @abstractmethod
+    def get_credentials(self) -> dict[str, Any]:
+        pass
+
+    @abstractmethod
     def create_user_workspace(
         self, workspace_name: str, user_name: str, **kwargs
     ) -> None:
         pass
 
     @abstractmethod
     def delete_user_workspace(self, workspace_name: str):
@@ -242,14 +248,16 @@
         self,
         url: str,
         access_key: SecretStr,
         secret_key: SecretStr,
         mc_bin_path: Any = None,
         alias: str = "MINIO_EODC",
     ):
+        self.storage_type = StorageType.MINIO
+
         self.alias = alias
 
         self.minio_client = Minio(
             url,
             access_key=access_key.get_secret_value(),
             secret_key=secret_key.get_secret_value(),
             secure=True,
@@ -457,14 +465,15 @@
     as objects.
     """
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self
 
     def __init__(self, url: str, access_key: SecretStr, secret_key: SecretStr):
+        self.storage_type = StorageType.CEPH
         self.access_key = access_key
         self.secret_key = secret_key
         self.url = url
         self.s3_client = boto3.client(
             "s3",
             aws_access_key_id=access_key.get_secret_value(),
             aws_secret_access_key=secret_key.get_secret_value(),
@@ -480,15 +489,15 @@
 
         handlers_to_unregister = handlers.prefix_search("before-parameter-build.s3")
         handler_to_unregister = handlers_to_unregister[0]
         self.s3_client.meta.events._emitter.unregister(
             "before-parameter-build.s3", handler_to_unregister
         )
 
-    def get_s3_credentials(self):
+    def get_credentials(self):
         return {
             "url": self.url,
             "access_key": self.access_key.get_secret_value(),
             "secret_key": self.secret_key.get_secret_value(),
         }
 
     def register_user(self, user_name: str) -> dict[str, str]:
@@ -592,26 +601,35 @@
 
 class AzureAdapter(WorkspaceAdapter):
     """
     This Adapter implements the Azure API for the Workspaces API.
 
     Workspaces are implemented as containers, and files are implemented
     as blobs.
+
+    File Paths are just blobnames seperated by forward slashes '/'
     """
 
     blob_service_client: BlobServiceClient
 
+    connection_string: SecretStr
+
     def __init__(
         self,
         connection_string: SecretStr,
     ):
+        self.storage_type = StorageType.AZURE
+        self.connection_string = connection_string
         self.blob_service_client = BlobServiceClient.from_connection_string(
             conn_str=connection_string.get_secret_value()
         )
 
+    def get_credentials(self):
+        return {"connection_string": self.connection_string.get_secret_value()}
+
     def create_user_workspace(self, workspace_name: str, user_name: str, **kwargs):
         self.blob_service_client.create_container(workspace_name)
 
     def delete_user_workspace(self, workspace_name: str):
         self.blob_service_client.delete_container(workspace_name)
 
     def get_fsspec(self, workspace_name: str):
```

### Comparing `eodc-2024.5.0/pyproject.toml` & `eodc-2024.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eodc"
 
-version = "2024.5.0"
+version = "2024.5.1"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>", "Christoph Reimer <christoph.reimer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2024.5.0/PKG-INFO` & `eodc-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

