# Comparing `tmp/almgroad-0.0.4-py3-none-any.whl.zip` & `tmp/almgroad-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2820 bytes, number of entries: 7
+Zip file size: 2825 bytes, number of entries: 7
 -rw-rw----  2.0 unx       55 b- defN 24-May-15 03:30 almgroad/__init__.py
 -rw-rw----  2.0 unx      128 b- defN 24-May-15 03:17 almgroad/chat.py
--rw-rw----  2.0 unx     1064 b- defN 24-May-15 04:47 almgroad/infoinsta.py
--rw-rw----  2.0 unx     1434 b- defN 24-May-15 04:49 almgroad-0.0.4.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-15 04:49 almgroad-0.0.4.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-15 04:49 almgroad-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      526 b- defN 24-May-15 04:49 almgroad-0.0.4.dist-info/RECORD
-7 files, 3308 bytes uncompressed, 1888 bytes compressed:  42.9%
+-rw-rw----  2.0 unx     1071 b- defN 24-May-15 04:51 almgroad/infoinsta.py
+-rw-rw----  2.0 unx     1434 b- defN 24-May-15 04:52 almgroad-0.0.5.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-15 04:52 almgroad-0.0.5.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-15 04:52 almgroad-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      526 b- defN 24-May-15 04:52 almgroad-0.0.5.dist-info/RECORD
+7 files, 3315 bytes uncompressed, 1893 bytes compressed:  42.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: almgroad/chat.py
 Comment: 
 
 Filename: almgroad/infoinsta.py
 Comment: 
 
-Filename: almgroad-0.0.4.dist-info/METADATA
+Filename: almgroad-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.4.dist-info/WHEEL
+Filename: almgroad-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.4.dist-info/top_level.txt
+Filename: almgroad-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.0.4.dist-info/RECORD
+Filename: almgroad-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/infoinsta.py

```diff
@@ -3,15 +3,15 @@
 
 def Info_Insta(user_name):
     url = f"https://www.instagram.com/api/v1/users/web_profile_info/?username={user_name}"
     headers = {
         "X-Ig-App-Id": "1217981644879628",
     }
     try:
-        req = requests.get(url ,headers=headers)
+        req = requests.get(url ,headers=headers).json()
         bio = req["data"]["user"]["biography"]
         followers = req["data"]["user"]["edge_followed_by"]["count"]
         following = req["data"]["user"]["edge_follow"]["count"]
         fullname = req["data"]["user"]["full_name"]
         idd =  req["data"]["user"]["id"]
         username = req["data"]["user"]["username"]
         infoo = {
```

## Comparing `almgroad-0.0.4.dist-info/METADATA` & `almgroad-0.0.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

