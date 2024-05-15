# Comparing `tmp/exasol_bucketfs-0.8.0.tar.gz` & `tmp/exasol_bucketfs-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_bucketfs-0.8.0.tar", max compression
+gzip compressed data, was "exasol_bucketfs-0.9.0.tar", max compression
```

## Comparing `exasol_bucketfs-0.8.0.tar` & `exasol_bucketfs-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1063 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/LICENSE
--rw-r--r--   0        0        0     1710 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/README.rst
--rw-r--r--   0        0        0    12369 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol/bucketfs/__init__.py
--rw-r--r--   0        0        0      235 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol/bucketfs/version.py
--rw-r--r--   0        0        0      470 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/__init__.py
--rw-r--r--   0        0        0     2510 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/abstract_bucketfs_location.py
--rw-r--r--   0        0        0      767 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucket_config.py
--rw-r--r--   0        0        0     1031 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_config.py
--rw-r--r--   0        0        0     1287 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_connection_config.py
--rw-r--r--   0        0        0     3132 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_factory.py
--rw-r--r--   0        0        0     5226 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_location.py
--rw-r--r--   0        0        0     5863 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_utils.py
--rw-r--r--   0        0        0     1097 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/buckets.py
--rw-r--r--   0        0        0      852 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/delete.py
--rw-r--r--   0        0        0     3446 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/download.py
--rw-r--r--   0        0        0     2067 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/github_release_file_bucketfs_uploader.py
--rw-r--r--   0        0        0     1628 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/list_files.py
--rw-r--r--   0        0        0     3388 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/load_file_from_local_fs.py
--rw-r--r--   0        0        0     4777 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/localfs_mock_bucketfs_location.py
--rw-r--r--   0        0        0     1440 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/release_link_extractor.py
--rw-r--r--   0        0        0     3993 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/upload.py
--rw-r--r--   0        0        0      235 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/version.py
--rw-r--r--   0        0        0     1436 2023-03-21 14:22:38.873715 exasol_bucketfs-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 exasol_bucketfs-0.8.0/setup.py
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 exasol_bucketfs-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-02-16 11:25:23.746302 exasol_bucketfs-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1710 2024-02-16 11:25:23.746302 exasol_bucketfs-0.9.0/README.rst
+-rw-r--r--   0        0        0    13335 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol/bucketfs/__init__.py
+-rw-r--r--   0        0        0      404 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol/bucketfs/version.py
+-rw-r--r--   0        0        0      470 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/__init__.py
+-rw-r--r--   0        0        0     2510 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/abstract_bucketfs_location.py
+-rw-r--r--   0        0        0      756 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucket_config.py
+-rw-r--r--   0        0        0     1020 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_config.py
+-rw-r--r--   0        0        0     1276 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_connection_config.py
+-rw-r--r--   0        0        0     3132 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_factory.py
+-rw-r--r--   0        0        0     5226 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_location.py
+-rw-r--r--   0        0        0     5808 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_utils.py
+-rw-r--r--   0        0        0     1097 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/buckets.py
+-rw-r--r--   0        0        0      852 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/delete.py
+-rw-r--r--   0        0        0     3446 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/download.py
+-rw-r--r--   0        0        0     2067 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/github_release_file_bucketfs_uploader.py
+-rw-r--r--   0        0        0     1628 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/list_files.py
+-rw-r--r--   0        0        0     3388 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/load_file_from_local_fs.py
+-rw-r--r--   0        0        0     4777 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/localfs_mock_bucketfs_location.py
+-rw-r--r--   0        0        0     1440 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/release_link_extractor.py
+-rw-r--r--   0        0        0     3993 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/upload.py
+-rw-r--r--   0        0        0      235 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/version.py
+-rw-r--r--   0        0        0     1398 2024-02-16 11:25:23.750302 exasol_bucketfs-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2548 1970-01-01 00:00:00.000000 exasol_bucketfs-0.9.0/setup.py
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 exasol_bucketfs-0.9.0/PKG-INFO
```

### Comparing `exasol_bucketfs-0.8.0/LICENSE` & `exasol_bucketfs-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/README.rst` & `exasol_bucketfs-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol/bucketfs/__init__.py` & `exasol_bucketfs-0.9.0/exasol/bucketfs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
         HTTPIE:
           $  http --auth w:write --auth-type basic --download GET http://127.0.0.1:6666/default/myfile.txt
 
         CURL:
           $ curl -u "w:write" --output myfile.txt  http://127.0.0.1:6666/default/myfile.txt
 """
+from __future__ import annotations
+
 import hashlib
 from collections import defaultdict
 from pathlib import Path
 from typing import (
     BinaryIO,
     ByteString,
     Iterable,
@@ -111,33 +113,45 @@
 class Service:
     """Provides a simple to use api to access a bucketfs service.
 
     Attributes:
         buckets: lists all available buckets.
     """
 
-    def __init__(self, url: str, credentials: Mapping[str, Mapping[str, str]] = None):
+    def __init__(
+        self,
+        url: str,
+        credentials: Mapping[str, Mapping[str, str]] = None,
+        verify: bool | str = True,
+    ):
         """Create a new Service instance.
 
         Args:
-            url: of the bucketfs service, e.g. `http(s)://127.0.0.1:2580`.
-            credentials: a mapping containing credentials (username and password) for buckets.
+            url:
+                Url of the bucketfs service, e.g. `http(s)://127.0.0.1:2580`.
+            credentials:
+                A mapping containing credentials (username and password) for buckets.
                 E.g. {"bucket1": { "username": "foo", "password": "bar" }}
+            verify:
+                Either a boolean, in which case it controls whether we verify
+                the server's TLS certificate, or a string, in which case it must be a path
+                to a CA bundle to use. Defaults to ``True``.
         """
         self._url = _parse_service_url(url)
         self._authenticator = defaultdict(
             lambda: {"username": "r", "password": "read"},
             credentials if credentials is not None else {},
         )
+        self._verify = verify
 
     @property
-    def buckets(self) -> MutableMapping[str, "Bucket"]:
+    def buckets(self) -> MutableMapping[str, Bucket]:
         """List all available buckets."""
         url = _build_url(service_url=self._url)
-        response = requests.get(url)
+        response = requests.get(url, verify=self._verify)
         try:
             response.raise_for_status()
         except HTTPError as ex:
             raise BucketFsError(
                 f"Couldn't list of all buckets from: {self._url}"
             ) from ex
 
@@ -151,36 +165,52 @@
             )
             for name in buckets
         }
 
     def __str__(self) -> str:
         return f"Service<{self._url}>"
 
-    def __iter__(self) -> Iterator["Bucket"]:
+    def __iter__(self) -> Iterator[Bucket]:
         yield from self.buckets
 
-    def __getitem__(self, item: str) -> "Bucket":
+    def __getitem__(self, item: str) -> Bucket:
         return self.buckets[item]
 
 
 class Bucket:
-    def __init__(self, name: str, service: str, username: str, password: str):
+    def __init__(
+        self,
+        name: str,
+        service: str,
+        username: str,
+        password: str,
+        verify: bool | str = True,
+    ):
         """
         Create a new bucket instance.
 
         Args:
-            name: of the bucket.
-            service: url where this bucket is hosted on.
-            username: used for authentication.
-            password: used for authentication.
+            name:
+                Name of the bucket.
+            service:
+                Url where this bucket is hosted on.
+            username:
+                Username used for authentication.
+            password:
+                Password used for authentication.
+            verify:
+                Either a boolean, in which case it controls whether we verify
+                the server's TLS certificate, or a string, in which case it must be a path
+                to a CA bundle to use. Defaults to ``True``.
         """
         self._name = name
         self._service = _parse_service_url(service)
         self._username = username
         self._password = password
+        self._verify = verify
 
     def __str__(self):
         return f"Bucket<{self.name} | on: {self._service}>"
 
     @property
     def name(self) -> str:
         return self._name
@@ -188,38 +218,38 @@
     @property
     def _auth(self) -> HTTPBasicAuth:
         return HTTPBasicAuth(username=self._username, password=self._password)
 
     @property
     def files(self) -> Iterable[str]:
         url = _build_url(service_url=self._service, bucket=self.name)
-        response = requests.get(url, auth=self._auth)
+        response = requests.get(url, auth=self._auth, verify=self._verify)
         try:
             response.raise_for_status()
         except HTTPError as ex:
             raise BucketFsError(
                 f"Couldn't retrieve file list form bucket: {self.name}"
             ) from ex
         return {line for line in _lines(response)}
 
     def __iter__(self) -> Iterator[str]:
         yield from self.files
 
     def upload(
-        self, path: str, data: Union[ByteString, BinaryIO, Iterable[ByteString]]
+        self, path: str, data: ByteString | BinaryIO | Iterable[ByteString]
     ) -> None:
         """
         Uploads a file onto this bucket
 
         Args:
             path: in the bucket the file shall be associated with.
             data: raw content of the file.
         """
         url = _build_url(service_url=self._service, bucket=self.name, path=path)
-        response = requests.put(url, data=data, auth=self._auth)
+        response = requests.put(url, data=data, auth=self._auth, verify=self._verify)
         try:
             response.raise_for_status()
         except HTTPError as ex:
             raise BucketFsError(f"Couldn't upload file: {path}") from ex
 
     def delete(self, path) -> None:
         """
@@ -228,15 +258,15 @@
         Args:
             path: points to the file which shall be deleted.
 
         Raises:
             A BucketFsError if the operation couldn't be executed successfully.
         """
         url = _build_url(service_url=self._service, bucket=self.name, path=path)
-        response = requests.delete(url, auth=self._auth)
+        response = requests.delete(url, auth=self._auth, verify=self._verify)
         try:
             response.raise_for_status()
         except HTTPError as ex:
             raise BucketFsError(f"Couldn't delete: {path}") from ex
 
     def download(self, path: str, chunk_size: int = 8192) -> Iterable[ByteString]:
         """
@@ -246,15 +276,17 @@
             path: which shall be downloaded.
             chunk_size: which shall be used for downloading.
 
         Returns:
             An iterable of binary chunks representing the downloaded file.
         """
         url = _build_url(service_url=self._service, bucket=self.name, path=path)
-        with requests.get(url, stream=True, auth=self._auth) as response:
+        with requests.get(
+            url, stream=True, auth=self._auth, verify=self._verify
+        ) as response:
             try:
                 response.raise_for_status()
             except HTTPError as ex:
                 raise BucketFsError(f"Couldn't download: {path}") from ex
 
             yield from response.iter_content(chunk_size=chunk_size)
 
@@ -292,15 +324,15 @@
     def chunk_size(self, value: int) -> None:
         self._chunk_size = value
 
     def __iter__(self) -> Iterable[str]:
         yield from self._bucket.files
 
     def __setitem__(
-        self, key: str, value: Union[ByteString, BinaryIO, Iterable[ByteString]]
+        self, key: str, value: ByteString | BinaryIO | Iterable[ByteString]
     ) -> None:
         """
         Uploads a file onto this bucket.
 
         See also Bucket:upload
         """
         self._bucket.upload(path=key, data=value)
@@ -321,15 +353,15 @@
         """
         return self._bucket.download(item, self._chunk_size)
 
     def __str__(self):
         return f"MappedBucket<{self._bucket}>"
 
 
-def _chunk_as_bytes(chunk: Union[int, ByteString]) -> ByteString:
+def _chunk_as_bytes(chunk: int | ByteString) -> ByteString:
     """
     In some scenarios python converts single bytes to integers:
     >>> chunks = [type(chunk) for chunk in b"abc"]
     >>> chunks
     ... [<class 'int'>, <class 'int'>, <class 'int'>]
     in order to cope with this transparently this wrapper can be used.
     """
@@ -369,15 +401,15 @@
 
     Return:
         A string representation of the converted bytes.
     """
     return _bytes(chunks).decode(encoding)
 
 
-def as_file(chunks: Iterable[ByteString], filename: Union[str, Path]) -> Path:
+def as_file(chunks: Iterable[ByteString], filename: str | Path) -> Path:
     """
     Transforms a set of byte chunks into a string.
 
     Args:
         chunks: which shall be written to file.
         filename: for the file which is to be created.
```

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/abstract_bucketfs_location.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/abstract_bucketfs_location.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucket_config.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucket_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class BucketConfig:
     """
     The BucketConfig contains all required information about a BucketFS
     to access it either via HTTP[S] or in the file system inside of UDFs.
     """
 
-    @typechecked(always=True)
+    @typechecked()
     def __init__(self, bucket_name: str, bucketfs_config: BucketFSConfig):
         if bucket_name == "":
             raise ValueError("Bucket name can't be an empty string")
         self._bucket_name = bucket_name
         self._bucketfs_config = bucketfs_config
 
     @property
```

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_config.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     The BucketFSConfig contains all required information
     to access it either via HTTP[S] or in the file system inside of UDFs.
     The BucketFSConnectionConfig is here by optional,
     because in UDF we sometimes don't want to use HTTP[S].
     """
 
-    @typechecked(always=True)
+    @typechecked()
     def __init__(
         self,
         bucketfs_name: str,
         connection_config: Union[BucketFSConnectionConfig, None] = None,
     ):
         self._connection_config = connection_config
         if bucketfs_name == "":
```

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_connection_config.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_connection_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class BucketFSConnectionConfig:
     """
     The BucketFSConnectionConfig contains all necessary information
     to connect to the BucketFS Server via HTTP[s]
     """
 
-    @typechecked(always=True)
+    @typechecked()
     def __init__(
         self, host: str, port: int, user: str, pwd: str, is_https: bool = False
     ):
         self._is_https = is_https
         if host == "":
             raise ValueError("Host can't be an empty string")
         self._host = host
```

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_factory.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_factory.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_location.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_location.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/bucketfs_utils.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/bucketfs_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,28 +31,28 @@
 ) -> PurePosixPath:
     path_in_bucket = PurePosixPath(path_in_bucket)
     if path_in_bucket.is_absolute():
         path_in_bucket = path_in_bucket.relative_to(PurePosixPath("/"))
     return path_in_bucket
 
 
-@typechecked(always=True)
+@typechecked()
 def generate_bucketfs_udf_path(bucketfs_config: BucketFSConfig) -> PurePosixPath:
     """
     This function generates the path where UDFs can access the content of a
     BucketFS in their file system
 
     :param bucketfs_config: Config of the BucketFS, the BucketFSConnectionConfig in the BucketFSConfig can be None
     :return: Path of the given BucketFS in the file system of the UDFs
     """
     path = PurePosixPath("/buckets/", bucketfs_config.bucketfs_name)
     return path
 
 
-@typechecked(always=True)
+@typechecked()
 def generate_bucket_udf_path(
     bucket_config: BucketConfig, path_in_bucket: Union[None, str, PurePosixPath]
 ) -> PurePosixPath:
     """
     This function generates the path where UDFs can access the content of a
     bucket or the given path in a bucket in their file system
 
@@ -68,15 +68,15 @@
         path_in_bucket = correct_path_in_bucket_for_archives(path_in_bucket)
     else:
         path_in_bucket = ""
     path = PurePosixPath(path, path_in_bucket)
     return path
 
 
-@typechecked(always=True)
+@typechecked()
 def generate_bucketfs_http_url(
     bucketfs_config: BucketFSConfig, with_credentials: bool = False
 ) -> urllib.parse.ParseResult:
     """
     This function generates an HTTP[s] url for the given BucketFSConfig
     with or without basic authentication  (a template: http[s]://user:password@host:port)
 
@@ -103,15 +103,15 @@
         f"{protocol}://{credentials}"
         f"{encoded_host}:{bucketfs_config.connection_config.port}"
     )
     urlparse = urllib.parse.urlparse(url)
     return urlparse
 
 
-@typechecked(always=True)
+@typechecked()
 def generate_bucket_http_url(
     bucket_config: BucketConfig,
     path_in_bucket: Union[None, str, PurePosixPath],
     with_credentials: bool = False,
 ) -> urllib.parse.ParseResult:
     """
     This function generates an HTTP[s] url for the given bucket or the path in the bucket
@@ -132,15 +132,15 @@
         for part in PurePosixPath(bucket_config.bucket_name, path_in_bucket).parts
     )
     url = urllib.parse.urljoin(url.geturl(), encoded_bucket_and_path_in_bucket)
     urlparse = urllib.parse.urlparse(url)
     return urlparse
 
 
-@typechecked(always=True)
+@typechecked()
 def create_auth_object(bucket_config: BucketConfig) -> HTTPBasicAuth:
     if bucket_config.bucketfs_config.connection_config is None:
         raise TypeError(
             "bucket_config.bucketfs_config.connection_config "
             "can't be None for this operation"
         )
     auth = HTTPBasicAuth(
```

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/buckets.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/buckets.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/delete.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/delete.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/download.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/download.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/github_release_file_bucketfs_uploader.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/github_release_file_bucketfs_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/list_files.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/list_files.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/load_file_from_local_fs.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/load_file_from_local_fs.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/localfs_mock_bucketfs_location.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/localfs_mock_bucketfs_location.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/release_link_extractor.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/release_link_extractor.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/exasol_bucketfs_utils_python/upload.py` & `exasol_bucketfs-0.9.0/exasol_bucketfs_utils_python/upload.py`

 * *Files identical despite different names*

### Comparing `exasol_bucketfs-0.8.0/pyproject.toml` & `exasol_bucketfs-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "exasol-bucketfs"
 packages  = [
     {include = "exasol"},
     {include = "exasol_bucketfs_utils_python"}
 ]
-version = "0.8.0"
+version = "0.9.0"
 description = "BucketFS utilities for the Python programming language"
 
 license = "MIT"
 
 authors = [
     "Torsten Kilias <torsten.kilias@exasol.com>",
     "Nicola Coretti <nicola.coretti@exasol.com>",
@@ -22,27 +22,28 @@
 
 keywords = ['exasol', 'bucketfs']
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = ">=2.24.0"
 joblib=">=1.0.1"
-typeguard = "^2.11.1"
+typeguard = "4.0.0"
 
 
 [tool.poetry.dev-dependencies]
 pyexasol = "^0.24.0"
 dill = "^0.3.4"
-exasol-udf-mock-python = { git = "https://github.com/exasol/udf-mock-python.git", branch = "main" }
+exasol-udf-mock-python = "^0.1.0"
 toml = ">=0.10.2"
 
 [tool.poetry.group.dev.dependencies]
 sphinx-copybutton = "^0.5.0"
 myst-parser = "^0.18.1"
 exasol-toolbox = ">=0.3.0"
+pytest-localserver = "^0.8.1"
 
 [tool.coverage.run]
 source = [
     "exasol",
 ]
 
 [tool.coverage.report]
```

### Comparing `exasol_bucketfs-0.8.0/setup.py` & `exasol_bucketfs-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['exasol', 'exasol.bucketfs', 'exasol_bucketfs_utils_python']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['joblib>=1.0.1', 'requests>=2.24.0', 'typeguard>=2.11.1,<3.0.0']
+['joblib>=1.0.1', 'requests>=2.24.0', 'typeguard==4.0.0']
 
 setup_kwargs = {
     'name': 'exasol-bucketfs',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'BucketFS utilities for the Python programming language',
     'long_description': 'Exasol Bucketfs\n###############\n\n.. image:: https://img.shields.io/pypi/v/exasol-bucketfs\n     :target: https://pypi.org/project/exasol-bucketfs/\n     :alt: PyPI Version\n\n.. image:: https://img.shields.io/pypi/pyversions/exasol-bucketfs\n    :target: https://pypi.org/project/sexasol-bucketfs\n    :alt: PyPI - Python Version\n\n.. image:: https://img.shields.io/badge/exasol-7.1.9%20%7C%207.0.18-green\n    :target: https://www.exasol.com/\n    :alt: Exasol - Supported Version(s)\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: Formatter - Black\n\n.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg\n    :target: https://pycqa.github.io/isort/\n    :alt: Formatter - Isort\n\n.. image:: https://img.shields.io/pypi/l/exasol-bucketfs\n     :target: https://opensource.org/licenses/MIT\n     :alt: License\n\n.. image:: https://img.shields.io/github/last-commit/exasol/bucketfs-python\n     :target: https://pypi.org/project/exasol-bucketfs/\n     :alt: Last Commit\n\n\nExasol Bucketfs is a python library to interact with Exasol `Bucketfs-Service(s) <https://docs.exasol.com/db/latest/database_concepts/bucketfs/bucketfs.htm>`_.\n\n🚀 Features\n------------\n\n* List all buckets of a bucketfs service\n* List all files in a bucket\n* Download files from bucketfs\n* Upload files to bucketfs\n* Delete files from bucketfs\n* Pythonic API\n\n🔌️ Prerequisites\n-----------------\n\n- `Python <https://www.python.org/>`_ >= 3.8\n\n💾 Installation\n----------------\n\n.. code-block:: shell\n\n    pip install exasol-bucketfs\n\n📚 Documentation\n----------------\n\nThe latest documentation can be found `here <https://exasol.github.io/bucketfs-python/>`_.\n\n',
     'author': 'Torsten Kilias',
     'author_email': 'torsten.kilias@exasol.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/exasol/bucketfs-python',
```

### Comparing `exasol_bucketfs-0.8.0/PKG-INFO` & `exasol_bucketfs-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exasol-bucketfs
-Version: 0.8.0
+Version: 0.9.0
 Summary: BucketFS utilities for the Python programming language
 Home-page: https://github.com/exasol/bucketfs-python
 License: MIT
 Keywords: exasol,bucketfs
 Author: Torsten Kilias
 Author-email: torsten.kilias@exasol.com
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: joblib (>=1.0.1)
 Requires-Dist: requests (>=2.24.0)
-Requires-Dist: typeguard (>=2.11.1,<3.0.0)
+Requires-Dist: typeguard (==4.0.0)
 Project-URL: Repository, https://github.com/exasol/bucketfs-python
 Description-Content-Type: text/x-rst
 
 Exasol Bucketfs
 ###############
 
 .. image:: https://img.shields.io/pypi/v/exasol-bucketfs
```

