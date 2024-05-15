# Comparing `tmp/osparc_filecomms-1.0.3-py2.py3-none-any.whl.zip` & `tmp/osparc_filecomms-1.0.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5371 bytes, number of entries: 8
--rw-r--r--  2.0 unx      217 b- defN 24-Apr-26 10:10 osparc_filecomms/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 24-Apr-26 10:11 osparc_filecomms/_version.py
--rw-r--r--  2.0 unx     6553 b- defN 24-Apr-26 10:10 osparc_filecomms/handshakers.py
--rw-r--r--  2.0 unx      678 b- defN 24-Apr-26 10:11 osparc_filecomms-1.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3081 b- defN 24-Apr-26 10:11 osparc_filecomms-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-26 10:11 osparc_filecomms-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-26 10:11 osparc_filecomms-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      691 b- defN 24-Apr-26 10:11 osparc_filecomms-1.0.3.dist-info/RECORD
-8 files, 11758 bytes uncompressed, 4151 bytes compressed:  64.7%
+Zip file size: 5372 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      217 b- defN 24-May-15 10:48 osparc_filecomms/__init__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-May-15 10:48 osparc_filecomms/_version.py
+-rw-r--r--  2.0 unx     6554 b- defN 24-May-15 10:48 osparc_filecomms/handshakers.py
+-rw-r--r--  2.0 unx      678 b- defN 24-May-15 10:48 osparc_filecomms-1.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3081 b- defN 24-May-15 10:48 osparc_filecomms-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-15 10:48 osparc_filecomms-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-May-15 10:48 osparc_filecomms-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      691 b- defN 24-May-15 10:48 osparc_filecomms-1.0.4.dist-info/RECORD
+8 files, 11759 bytes uncompressed, 4152 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: osparc_filecomms/_version.py
 Comment: 
 
 Filename: osparc_filecomms/handshakers.py
 Comment: 
 
-Filename: osparc_filecomms-1.0.3.dist-info/LICENSE.txt
+Filename: osparc_filecomms-1.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: osparc_filecomms-1.0.3.dist-info/METADATA
+Filename: osparc_filecomms-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: osparc_filecomms-1.0.3.dist-info/WHEEL
+Filename: osparc_filecomms-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: osparc_filecomms-1.0.3.dist-info/top_level.txt
+Filename: osparc_filecomms-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: osparc_filecomms-1.0.3.dist-info/RECORD
+Filename: osparc_filecomms-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## osparc_filecomms/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '1.0.3'
-__version_tuple__ = version_tuple = (1, 0, 3)
+__version__ = version = '1.0.4'
+__version_tuple__ = version_tuple = (1, 0, 4)
```

## osparc_filecomms/handshakers.py

```diff
@@ -60,15 +60,15 @@
 
         self.last_write = path, content
 
     def retry_last_write(self):
         if self.last_write is not None:
             path, content = self.last_write
             self.write_filecontent(path, content)
-            logger.info(f"Retried writingfile content to {path}")
+            logger.info(f"Retried writing file content to {path}")
 
     def shake_initiator(self):
         """Shake hand by initiator"""
 
         handshake_out = {
             "command": "register",
             "uuid": self.self_uuid,
```

## Comparing `osparc_filecomms-1.0.3.dist-info/LICENSE.txt` & `osparc_filecomms-1.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `osparc_filecomms-1.0.3.dist-info/METADATA` & `osparc_filecomms-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osparc_filecomms
-Version: 1.0.3
+Version: 1.0.4
 Summary: oSparc file communications
 Author: Werner Van Geit @ IT'IS Zurich
 License: Copyright (C) IT'IS Foundation - All Rights Reserved
         
         Written by Werner Van Geit <vangeit at itis.swiss>, 2023
         
         Unless required by applicable law or agreed to in writing,
```

## Comparing `osparc_filecomms-1.0.3.dist-info/RECORD` & `osparc_filecomms-1.0.4.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 osparc_filecomms/__init__.py,sha256=RaYgQTzgQT-5M6hF9TsXf8ZR_o4MN5JZeGidHDaOpX0,217
-osparc_filecomms/_version.py,sha256=vs6W4yrsz3i8OMGT2jlW8NQDmpo9yxVa6jtyzIhHvWw,411
-osparc_filecomms/handshakers.py,sha256=YXNeZhROaKJGot5b_QNgCTzGYJIiNekCNORiEzB3uOY,6553
-osparc_filecomms-1.0.3.dist-info/LICENSE.txt,sha256=G37dm51umRlw_tAWPHkBbh2CS6aSj5-LRq3cu7ke3FI,678
-osparc_filecomms-1.0.3.dist-info/METADATA,sha256=Aln9yNJheuhRA5sBqkhfRRf_NwTYYxa9QBT1XGp5Ud8,3081
-osparc_filecomms-1.0.3.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-osparc_filecomms-1.0.3.dist-info/top_level.txt,sha256=s_RGt5qLbQnDwc2uMVPkae7VeyqfQgvomsENuCPisLc,17
-osparc_filecomms-1.0.3.dist-info/RECORD,,
+osparc_filecomms/_version.py,sha256=9acUHRb1fq-uv5dr49LlEh189daKw4-SeypW5NxDolA,411
+osparc_filecomms/handshakers.py,sha256=NylTKDvtlifI3E9bEveGIGOSCVCZgY1HMc2PSS37ZwI,6554
+osparc_filecomms-1.0.4.dist-info/LICENSE.txt,sha256=G37dm51umRlw_tAWPHkBbh2CS6aSj5-LRq3cu7ke3FI,678
+osparc_filecomms-1.0.4.dist-info/METADATA,sha256=ymCd6xuz4-RMjVQfdfcuDe2MElbfVkty6VrZu7D_99s,3081
+osparc_filecomms-1.0.4.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+osparc_filecomms-1.0.4.dist-info/top_level.txt,sha256=s_RGt5qLbQnDwc2uMVPkae7VeyqfQgvomsENuCPisLc,17
+osparc_filecomms-1.0.4.dist-info/RECORD,,
```

