# Comparing `tmp/zhlyr-4.7-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/zhlyr-4.8-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 348687 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:09 zhlyr-4.7.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:09 zhlyr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:09 zhlyr.libs/
--rwxrwxrwx  2.0 unx     4083 b- defN 24-May-15 19:09 zhlyr-4.7.dist-info/METADATA
--rwxrwxrwx  2.0 unx      152 b- defN 24-May-15 19:09 zhlyr-4.7.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        6 b- defN 24-May-15 19:09 zhlyr-4.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      691 b- defN 24-May-15 19:09 zhlyr-4.7.dist-info/RECORD
--rwxrwxrwx  2.0 unx   486116 b- defN 24-May-15 19:09 zhlyr/serialize.c
--rwxrwxrwx  2.0 unx     2179 b- defN 24-May-15 19:09 zhlyr/zhlyr.py
--rwxrwxrwx  2.0 unx     1847 b- defN 24-May-15 19:09 zhlyr/recosnize.py
--rwxrwxrwx  2.0 unx   650528 b- defN 24-May-15 19:09 zhlyr/serialize.cpython-312-x86_64-linux-gnu.so
--rwxrwxrwx  2.0 unx       92 b- defN 24-May-15 19:09 zhlyr/__init__.py
-12 files, 1145694 bytes uncompressed, 347229 bytes compressed:  69.7%
+Zip file size: 348702 bytes, number of entries: 12
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:32 zhlyr-4.8.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:32 zhlyr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:32 zhlyr.libs/
+-rwxrwxrwx  2.0 unx     4083 b- defN 24-May-15 19:32 zhlyr-4.8.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      152 b- defN 24-May-15 19:32 zhlyr-4.8.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        6 b- defN 24-May-15 19:32 zhlyr-4.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      691 b- defN 24-May-15 19:32 zhlyr-4.8.dist-info/RECORD
+-rwxrwxrwx  2.0 unx   486116 b- defN 24-May-15 19:32 zhlyr/serialize.c
+-rwxrwxrwx  2.0 unx     2179 b- defN 24-May-15 19:32 zhlyr/zhlyr.py
+-rwxrwxrwx  2.0 unx     1875 b- defN 24-May-15 19:32 zhlyr/recosnize.py
+-rwxrwxrwx  2.0 unx   650528 b- defN 24-May-15 19:32 zhlyr/serialize.cpython-312-x86_64-linux-gnu.so
+-rwxrwxrwx  2.0 unx       93 b- defN 24-May-15 19:32 zhlyr/__init__.py
+12 files, 1145723 bytes uncompressed, 347244 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,26 +1,26 @@
-Filename: zhlyr-4.7.dist-info/
+Filename: zhlyr-4.8.dist-info/
 Comment: 
 
 Filename: zhlyr/
 Comment: 
 
 Filename: zhlyr.libs/
 Comment: 
 
-Filename: zhlyr-4.7.dist-info/METADATA
+Filename: zhlyr-4.8.dist-info/METADATA
 Comment: 
 
-Filename: zhlyr-4.7.dist-info/WHEEL
+Filename: zhlyr-4.8.dist-info/WHEEL
 Comment: 
 
-Filename: zhlyr-4.7.dist-info/top_level.txt
+Filename: zhlyr-4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: zhlyr-4.7.dist-info/RECORD
+Filename: zhlyr-4.8.dist-info/RECORD
 Comment: 
 
 Filename: zhlyr/serialize.c
 Comment: 
 
 Filename: zhlyr/zhlyr.py
 Comment:
```

## zhlyr/recosnize.py

```diff
@@ -1,12 +1,12 @@
 from typing import Union, Optional
 from shazamio import Shazam as RecoSnizer
 import json , os , asyncio
 from pathlib import Path
-from serilize import Serializer
+from .serialize import Serializer
 RecoSnizer_ = RecoSnizer()
 class RecoSnize(RecoSnizer):
     '''
     :param `data`: `bytes` | `bytearray` or `str path` | `Path` object 
     to get info from it.
     :param `proxy`: `str` | `None` to set `proxy` for your `request`
     '''
@@ -35,15 +35,15 @@
     async def text(self):
         '''
         Returns a string of the recognizer.
         '''
         return str(await self.recognizer)
 
 
-
+Serializer({'hello':'hi'})
 # Example to use to RecoSnizer :
 
 # async def main():
 #     data_path = r'C:\Users\Mtsky\Downloads\Telegram Desktop\mzaf_17549133339911745381.plus.aac.ep (2).m4a'
 #     result = await RecoSnize(data_path).json()
 #     print(Serializer(result).track.title)
```

## zhlyr/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .recosnize import RecoSnize
 from .zhlyr import ZhLyr
-from .serilize import Serializer
+from .serialize import Serializer
```

## Comparing `zhlyr-4.7.dist-info/METADATA` & `zhlyr-4.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 4.7
+Version: 4.8
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
```

