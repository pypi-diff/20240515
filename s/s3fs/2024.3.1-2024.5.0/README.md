# Comparing `tmp/s3fs-2024.3.1.tar.gz` & `tmp/s3fs-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3fs-2024.3.1.tar", last modified: Mon Mar 18 19:43:31 2024, max compression
+gzip compressed data, was "s3fs-2024.5.0.tar", last modified: Wed May 15 15:05:41 2024, max compression
```

## Comparing `s3fs-2024.3.1.tar` & `s3fs-2024.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:43:31.673912 s3fs-2024.3.1/
--rw-r--r--   0 mdurant    (502) staff       (20)     1505 2022-09-18 01:28:11.000000 s3fs-2024.3.1/LICENSE.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      225 2022-09-18 01:28:11.000000 s3fs-2024.3.1/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1590 2024-03-18 19:43:31.673818 s3fs-2024.3.1/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      620 2022-09-18 01:28:11.000000 s3fs-2024.3.1/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:43:31.664103 s3fs-2024.3.1/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:43:31.667891 s3fs-2024.3.1/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      906 2023-02-23 19:42:13.000000 s3fs-2024.3.1/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     5780 2024-03-18 19:42:51.000000 s3fs-2024.3.1/docs/source/changelog.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      151 2022-09-18 01:28:11.000000 s3fs-2024.3.1/docs/source/development.rst
--rw-r--r--   0 mdurant    (502) staff       (20)    11569 2023-07-27 13:28:45.000000 s3fs-2024.3.1/docs/source/index.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      530 2022-09-18 01:28:11.000000 s3fs-2024.3.1/docs/source/install.rst
--rw-r--r--   0 mdurant    (502) staff       (20)       71 2024-03-18 19:42:51.000000 s3fs-2024.3.1/requirements.txt
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:43:31.669661 s3fs-2024.3.1/s3fs/
--rw-r--r--   0 mdurant    (502) staff       (20)      160 2023-10-21 17:49:51.000000 s3fs-2024.3.1/s3fs/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2024-03-18 19:43:31.674336 s3fs-2024.3.1/s3fs/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)    88056 2024-03-18 19:36:35.000000 s3fs-2024.3.1/s3fs/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7779 2022-09-18 01:28:11.000000 s3fs-2024.3.1/s3fs/errors.py
--rw-r--r--   0 mdurant    (502) staff       (20)      237 2022-09-18 01:28:11.000000 s3fs-2024.3.1/s3fs/mapping.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:43:31.671748 s3fs-2024.3.1/s3fs/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:11.000000 s3fs-2024.3.1/s3fs/tests/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:43:31.672504 s3fs-2024.3.1/s3fs/tests/derived/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2023-06-05 15:35:23.000000 s3fs-2024.3.1/s3fs/tests/derived/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3603 2023-09-03 17:35:34.000000 s3fs-2024.3.1/s3fs/tests/derived/s3fs_fixtures.py
--rw-r--r--   0 mdurant    (502) staff       (20)      314 2023-06-05 15:35:23.000000 s3fs-2024.3.1/s3fs/tests/derived/s3fs_test.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2859 2023-12-05 14:14:44.000000 s3fs-2024.3.1/s3fs/tests/test_mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)    84078 2024-03-18 19:36:35.000000 s3fs-2024.3.1/s3fs/tests/test_s3fs.py
--rw-r--r--   0 mdurant    (502) staff       (20)      370 2022-09-18 01:28:11.000000 s3fs-2024.3.1/s3fs/tests/test_utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5246 2023-12-05 14:14:44.000000 s3fs-2024.3.1/s3fs/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:43:31.673278 s3fs-2024.3.1/s3fs.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     1590 2024-03-18 19:43:31.000000 s3fs-2024.3.1/s3fs.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      660 2024-03-18 19:43:31.000000 s3fs-2024.3.1/s3fs.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-03-18 19:43:31.000000 s3fs-2024.3.1/s3fs.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-19 15:15:30.000000 s3fs-2024.3.1/s3fs.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      156 2024-03-18 19:43:31.000000 s3fs-2024.3.1/s3fs.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        5 2024-03-18 19:43:31.000000 s3fs-2024.3.1/s3fs.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      438 2024-03-18 19:43:31.674206 s3fs-2024.3.1/setup.cfg
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1365 2023-02-23 19:42:13.000000 s3fs-2024.3.1/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    86854 2023-10-21 17:54:10.000000 s3fs-2024.3.1/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-15 15:05:41.487941 s3fs-2024.5.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1505 2022-09-18 01:28:11.000000 s3fs-2024.5.0/LICENSE.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      225 2022-09-18 01:28:11.000000 s3fs-2024.5.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1592 2024-05-15 15:05:41.487813 s3fs-2024.5.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      620 2022-09-18 01:28:11.000000 s3fs-2024.5.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-15 15:05:41.475087 s3fs-2024.5.0/docs/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-15 15:05:41.479251 s3fs-2024.5.0/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      906 2023-02-23 19:42:13.000000 s3fs-2024.5.0/docs/source/api.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     5913 2024-05-15 15:05:03.000000 s3fs-2024.5.0/docs/source/changelog.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      151 2022-09-18 01:28:11.000000 s3fs-2024.5.0/docs/source/development.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)    11569 2023-07-27 13:28:45.000000 s3fs-2024.5.0/docs/source/index.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      530 2022-09-18 01:28:11.000000 s3fs-2024.5.0/docs/source/install.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)       73 2024-05-15 15:05:03.000000 s3fs-2024.5.0/requirements.txt
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-15 15:05:41.481705 s3fs-2024.5.0/s3fs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      160 2023-10-21 17:49:51.000000 s3fs-2024.5.0/s3fs/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2024-05-15 15:05:41.488560 s3fs-2024.5.0/s3fs/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    88183 2024-03-26 17:43:39.000000 s3fs-2024.5.0/s3fs/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7779 2022-09-18 01:28:11.000000 s3fs-2024.5.0/s3fs/errors.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      237 2022-09-18 01:28:11.000000 s3fs-2024.5.0/s3fs/mapping.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-15 15:05:41.485775 s3fs-2024.5.0/s3fs/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:11.000000 s3fs-2024.5.0/s3fs/tests/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-15 15:05:41.486622 s3fs-2024.5.0/s3fs/tests/derived/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2023-06-05 15:35:23.000000 s3fs-2024.5.0/s3fs/tests/derived/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3603 2023-09-03 17:35:34.000000 s3fs-2024.5.0/s3fs/tests/derived/s3fs_fixtures.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      314 2023-06-05 15:35:23.000000 s3fs-2024.5.0/s3fs/tests/derived/s3fs_test.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2859 2023-12-05 14:14:44.000000 s3fs-2024.5.0/s3fs/tests/test_mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    84078 2024-03-18 19:36:35.000000 s3fs-2024.5.0/s3fs/tests/test_s3fs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      370 2022-09-18 01:28:11.000000 s3fs-2024.5.0/s3fs/tests/test_utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5246 2023-12-05 14:14:44.000000 s3fs-2024.5.0/s3fs/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-15 15:05:41.487157 s3fs-2024.5.0/s3fs.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1592 2024-05-15 15:05:41.000000 s3fs-2024.5.0/s3fs.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      660 2024-05-15 15:05:41.000000 s3fs-2024.5.0/s3fs.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-05-15 15:05:41.000000 s3fs-2024.5.0/s3fs.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-19 15:15:30.000000 s3fs-2024.5.0/s3fs.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      158 2024-05-15 15:05:41.000000 s3fs-2024.5.0/s3fs.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        5 2024-05-15 15:05:41.000000 s3fs-2024.5.0/s3fs.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2024-05-15 15:05:41.488332 s3fs-2024.5.0/setup.cfg
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1365 2023-02-23 19:42:13.000000 s3fs-2024.5.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    86854 2023-10-21 17:54:10.000000 s3fs-2024.5.0/versioneer.py
```

### Comparing `s3fs-2024.3.1/LICENSE.txt` & `s3fs-2024.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/PKG-INFO` & `s3fs-2024.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3fs
-Version: 2024.3.1
+Version: 2024.5.0
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >= 3.8
 License-File: LICENSE.txt
 Requires-Dist: aiobotocore<3.0.0,>=2.5.4
-Requires-Dist: fsspec==2024.3.1
+Requires-Dist: fsspec==2024.5.0.*
 Requires-Dist: aiohttp!=4.0.0a0,!=4.0.0a1
 Provides-Extra: awscli
 Requires-Dist: aiobotocore[awscli]<3.0.0,>=2.5.4; extra == "awscli"
 Provides-Extra: boto3
 Requires-Dist: aiobotocore[boto3]<3.0.0,>=2.5.4; extra == "boto3"
 
 s3fs
```

### Comparing `s3fs-2024.3.1/README.rst` & `s3fs-2024.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/docs/source/api.rst` & `s3fs-2024.5.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/docs/source/changelog.rst` & `s3fs-2024.5.0/docs/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2024.5.0
+--------
+
+- widen fsspec req version (#869)
+- _bulk_delete must return list (#866)
+- retry on "reduce request rate" (#865)
+
 2024.3.1
 --------
 
 - accept kwargs in get_file (#863)
 
 2024.3.0
 --------
```

### Comparing `s3fs-2024.3.1/docs/source/index.rst` & `s3fs-2024.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/docs/source/install.rst` & `s3fs-2024.5.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/s3fs/core.py` & `s3fs-2024.5.0/s3fs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,18 +114,21 @@
         except S3_RETRYABLE_ERRORS as e:
             err = e
             logger.debug("Retryable error: %s", e)
             await asyncio.sleep(min(1.7**i * 0.1, 15))
         except ClientError as e:
             logger.debug("Client error (maybe retryable): %s", e)
             err = e
+            wait_time = min(1.7**i * 0.1, 15)
             if "SlowDown" in str(e):
-                await asyncio.sleep(min(1.7**i * 0.1, 15))
+                await asyncio.sleep(wait_time)
+            elif "reduce your request rate" in str(e):
+                await asyncio.sleep(wait_time)
             elif "XAmzContentSHA256Mismatch" in str(e):
-                await asyncio.sleep(min(1.7**i * 0.1, 15))
+                await asyncio.sleep(wait_time)
             else:
                 break
         except Exception as e:
             logger.debug("Nonretryable error: %s", e)
             err = e
             break
 
@@ -1947,15 +1950,15 @@
         Parameters
         ----------
         pathlist : list(str)
             The keys to remove, must all be in the same bucket.
             Must have 0 < len <= 1000
         """
         if not pathlist:
-            return
+            return []
         buckets = {self.split_path(path)[0] for path in pathlist}
         if len(buckets) > 1:
             raise ValueError("Bulk delete files should refer to only one bucket")
         bucket = buckets.pop()
         if len(pathlist) > 1000:
             raise ValueError("Max number of files to delete in one call is 1000")
         delete_keys = {
```

### Comparing `s3fs-2024.3.1/s3fs/errors.py` & `s3fs-2024.5.0/s3fs/errors.py`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/s3fs/tests/derived/s3fs_fixtures.py` & `s3fs-2024.5.0/s3fs/tests/derived/s3fs_fixtures.py`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/s3fs/tests/test_mapping.py` & `s3fs-2024.5.0/s3fs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/s3fs/tests/test_s3fs.py` & `s3fs-2024.5.0/s3fs/tests/test_s3fs.py`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/s3fs/utils.py` & `s3fs-2024.5.0/s3fs/utils.py`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/s3fs.egg-info/PKG-INFO` & `s3fs-2024.5.0/s3fs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3fs
-Version: 2024.3.1
+Version: 2024.5.0
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >= 3.8
 License-File: LICENSE.txt
 Requires-Dist: aiobotocore<3.0.0,>=2.5.4
-Requires-Dist: fsspec==2024.3.1
+Requires-Dist: fsspec==2024.5.0.*
 Requires-Dist: aiohttp!=4.0.0a0,!=4.0.0a1
 Provides-Extra: awscli
 Requires-Dist: aiobotocore[awscli]<3.0.0,>=2.5.4; extra == "awscli"
 Provides-Extra: boto3
 Requires-Dist: aiobotocore[boto3]<3.0.0,>=2.5.4; extra == "boto3"
 
 s3fs
```

### Comparing `s3fs-2024.3.1/s3fs.egg-info/SOURCES.txt` & `s3fs-2024.5.0/s3fs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/setup.py` & `s3fs-2024.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `s3fs-2024.3.1/versioneer.py` & `s3fs-2024.5.0/versioneer.py`

 * *Files identical despite different names*

