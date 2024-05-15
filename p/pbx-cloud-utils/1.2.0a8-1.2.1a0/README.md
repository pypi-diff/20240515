# Comparing `tmp/pbx_cloud_utils-1.2.0a8-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.2.1a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7562 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 11:19 cloud_utils/__init__.py
--rw-r--r--  2.0 unx    12261 b- defN 24-Apr-22 11:06 cloud_utils/aio_storage.py
--rw-r--r--  2.0 unx       57 b- defN 24-Apr-22 11:06 cloud_utils/const.py
--rw-r--r--  2.0 unx      284 b- defN 24-Apr-02 10:50 cloud_utils/exceptions.py
--rw-r--r--  2.0 unx     9960 b- defN 24-Apr-22 11:06 cloud_utils/storage.py
--rw-r--r--  2.0 unx     1345 b- defN 24-Apr-18 13:35 cloud_utils/types.py
--rw-r--r--  2.0 unx      346 b- defN 24-Apr-02 10:50 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-22 11:19 pbx_cloud_utils-1.2.0a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 11:19 pbx_cloud_utils-1.2.0a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-22 11:19 pbx_cloud_utils-1.2.0a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      886 b- defN 24-Apr-22 11:19 pbx_cloud_utils-1.2.0a8.dist-info/RECORD
-11 files, 25567 bytes uncompressed, 6056 bytes compressed:  76.3%
+Zip file size: 7570 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 24-May-14 11:12 cloud_utils/__init__.py
+-rw-r--r--  2.0 unx    12094 b- defN 24-May-14 09:38 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx       57 b- defN 24-May-14 09:38 cloud_utils/const.py
+-rw-r--r--  2.0 unx      284 b- defN 24-May-14 09:38 cloud_utils/exceptions.py
+-rw-r--r--  2.0 unx     9960 b- defN 24-May-14 09:38 cloud_utils/storage.py
+-rw-r--r--  2.0 unx     1365 b- defN 24-May-14 09:38 cloud_utils/types.py
+-rw-r--r--  2.0 unx      346 b- defN 24-May-14 09:38 cloud_utils/utils.py
+-rw-r--r--  2.0 unx      324 b- defN 24-May-14 11:12 pbx_cloud_utils-1.2.1a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 11:12 pbx_cloud_utils-1.2.1a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-14 11:12 pbx_cloud_utils-1.2.1a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      886 b- defN 24-May-14 11:12 pbx_cloud_utils-1.2.1a0.dist-info/RECORD
+11 files, 25420 bytes uncompressed, 6064 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a8.dist-info/METADATA
+Filename: pbx_cloud_utils-1.2.1a0.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a8.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.2.1a0.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a8.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.2.1a0.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a8.dist-info/RECORD
+Filename: pbx_cloud_utils-1.2.1a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/aio_storage.py

```diff
@@ -1,14 +1,13 @@
 import datetime
 import os
 from abc import ABC, abstractmethod
 from io import BytesIO
 from typing import Any, Tuple
 
-from aiobotocore import config as s3_config
 from azure.storage.blob import BlobSasPermissions, generate_blob_sas
 from azure.storage.blob.aio import BlobClient, ContainerClient
 from google.cloud import storage as gcs_storage
 
 from cloud_utils.const import GOOGLE_BUCKET_API_URL
 from cloud_utils.types import (
     PbxACL,
@@ -21,15 +20,16 @@
     gcs_storage_class_map,
     s3_acl_map,
     s3_storage_class_map,
 )
 from cloud_utils.utils import get_account_key
 
 try:
-    import aiobotocore  # type: ignore
+    from aiobotocore import config as s3_config
+    from aiobotocore.session import get_session
 
     HAS_AIOBOTOCORE = True
 except ImportError:  # pragma: no cover
     HAS_AIOBOTOCORE = False
 
 
 class AsyncStorage(ABC):
@@ -88,28 +88,28 @@
 
     def __new__(cls, *args, **kwargs):
         if not HAS_AIOBOTOCORE:  # pragma: no cover
             raise ImportError("Required aiobotocore, please install aiobotocore>=1.4.0.")
         return super().__new__(cls)
 
     async def delete_object(self, key: str):
-        session = aiobotocore.session.get_session()
+        session = get_session()
         async with session.create_client("s3", self.region_name) as client:
             await client.delete_object(Bucket=self.bucket_name, Key=key)
 
     async def generate_presigned_url(
         self,
         key: str,
         size: str,
         content_md5: str,
         addressing_style: S3AddressingStyles = "path",
         **kwargs: Any,
     ) -> Tuple[str, dict]:
         headers = {"Content-Length": str(size), "Content-MD5": content_md5}
-        session = aiobotocore.session.get_session()
+        session = get_session()
         config = s3_config.AioConfig(s3={"addressing_style": addressing_style})
         async with session.create_client(
             "s3",
             region_name=self.region_name,
             config=config,
             **self.extra_kwargs,
         ) as client:
@@ -127,40 +127,40 @@
 
     async def change_storage_class(
         self,
         key: str,
         target_storage_class: PbxStorageClass,
         acl: PbxACL = PbxACL.PUBLIC_READ,
     ) -> None:
-        session = aiobotocore.session.get_session()
+        session = get_session()
         async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
                 MetadataDirective="COPY",
             )
 
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
-        session = aiobotocore.session.get_session()
+        session = get_session()
         async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=target_key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 MetadataDirective="COPY",
             )
 
     async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
-        session = aiobotocore.session.get_session()
+        session = get_session()
         async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             obj = await client.get_object(Bucket=self.bucket_name, Key=key)
             async with obj["Body"] as body_stream:
                 data = await body_stream.read()
             return BytesIO(data), {
                 "mimetype": obj.get("ContentType"),
                 "storage_class": obj.get("StorageClass", "STANDARD"),
@@ -170,15 +170,15 @@
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
     ) -> UploadObjectData:
-        session = aiobotocore.session.get_session()
+        session = get_session()
         async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             response = await client.put_object(
                 ACL=self.provider_acl_map[acl.name],
                 Body=content.getvalue(),
                 Bucket=self.bucket_name,
                 Key=key,
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
@@ -286,28 +286,28 @@
         self.bucket_client.blob(key).update_storage_class(
             self.provider_storage_class_map[target_storage_class.name]
         )
 
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
-        session = aiobotocore.session.get_session()
+        session = get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
             await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=target_key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 MetadataDirective="COPY",
             )
 
     async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
-        session = aiobotocore.session.get_session()
+        session = get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
             obj = await client.get_object(Bucket=self.bucket_name, Key=key)
             async with obj["Body"] as body_stream:
                 data = await body_stream.read()
             storage_class = obj["ResponseMetadata"]["HTTPHeaders"]["x-goog-storage-class"]
@@ -320,15 +320,15 @@
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
     ) -> UploadObjectData:
-        session = aiobotocore.session.get_session()
+        session = get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
             response = await client.put_object(
                 ACL=self.provider_acl_map[acl.name],
                 Body=content.getvalue(),
                 Bucket=self.bucket_name,
```

## cloud_utils/types.py

```diff
@@ -1,7 +1,8 @@
+# flake8: noqa A005
 from dataclasses import dataclass
 from enum import IntEnum
 from typing import Literal
 
 S3AddressingStyles = Literal["path", "virtual", "auto"]
```

## Comparing `pbx_cloud_utils-1.2.0a8.dist-info/RECORD` & `pbx_cloud_utils-1.2.1a0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cloud_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cloud_utils/aio_storage.py,sha256=erGxV_PZ4trq1zIZKgq_EGK47YCSc1EY9Dq_SlQQMrw,12261
+cloud_utils/aio_storage.py,sha256=hTMYwaK2Bx64vQVUj1PFKXg_649-sOIy3PQnSRpuifE,12094
 cloud_utils/const.py,sha256=I0vJw5LuVCMJZK3ajhM1v2O85cpxnnirDG-scWyxeRE,57
 cloud_utils/exceptions.py,sha256=4TFl0EqL8X2vEgs4xpNgev93bDMcawfVc9DAty7SAqw,284
 cloud_utils/storage.py,sha256=R2b2zyENuPgcodtSx67jetwG12BydFf_XV0QD05z8e8,9960
-cloud_utils/types.py,sha256=Z02LFpyt7JsD8fgbNUn5W8wzgrQJmESVhpVZrzMeaQM,1345
+cloud_utils/types.py,sha256=o98xCZ9mwhjvvm2-CmGkgcEVbdj8wbZxwIgKICr2E08,1365
 cloud_utils/utils.py,sha256=gi__PPdP5YKxehoe9Az5lhAgN11sFxk3YLmHM0cxm1I,346
-pbx_cloud_utils-1.2.0a8.dist-info/METADATA,sha256=z0fxOfiBSGDH8Eu9Y7tvd3TbV2g5F6f8gMD-KxctikY,324
-pbx_cloud_utils-1.2.0a8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pbx_cloud_utils-1.2.0a8.dist-info/top_level.txt,sha256=zcaARuOP8yoOZ9pwOjV7p4206IX9CFMTKA_QPvxCtvA,12
-pbx_cloud_utils-1.2.0a8.dist-info/RECORD,,
+pbx_cloud_utils-1.2.1a0.dist-info/METADATA,sha256=nFMt0GsaEPVVJW36DSJ9zOybORDUTDfv1Uidewh1ylA,324
+pbx_cloud_utils-1.2.1a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pbx_cloud_utils-1.2.1a0.dist-info/top_level.txt,sha256=zcaARuOP8yoOZ9pwOjV7p4206IX9CFMTKA_QPvxCtvA,12
+pbx_cloud_utils-1.2.1a0.dist-info/RECORD,,
```

