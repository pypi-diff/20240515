# Comparing `tmp/almgroad-0.0.3-py3-none-any.whl.zip` & `tmp/almgroad-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2860 bytes, number of entries: 7
+Zip file size: 2820 bytes, number of entries: 7
 -rw-rw----  2.0 unx       55 b- defN 24-May-15 03:30 almgroad/__init__.py
 -rw-rw----  2.0 unx      128 b- defN 24-May-15 03:17 almgroad/chat.py
--rw-rw----  2.0 unx     1136 b- defN 24-May-15 04:20 almgroad/infoinsta.py
--rw-rw----  2.0 unx     1434 b- defN 24-May-15 04:23 almgroad-0.0.3.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-15 04:23 almgroad-0.0.3.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-15 04:23 almgroad-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      526 b- defN 24-May-15 04:23 almgroad-0.0.3.dist-info/RECORD
-7 files, 3380 bytes uncompressed, 1928 bytes compressed:  43.0%
+-rw-rw----  2.0 unx     1064 b- defN 24-May-15 04:47 almgroad/infoinsta.py
+-rw-rw----  2.0 unx     1434 b- defN 24-May-15 04:49 almgroad-0.0.4.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-15 04:49 almgroad-0.0.4.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-15 04:49 almgroad-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      526 b- defN 24-May-15 04:49 almgroad-0.0.4.dist-info/RECORD
+7 files, 3308 bytes uncompressed, 1888 bytes compressed:  42.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: almgroad/chat.py
 Comment: 
 
 Filename: almgroad/infoinsta.py
 Comment: 
 
-Filename: almgroad-0.0.3.dist-info/METADATA
+Filename: almgroad-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.3.dist-info/WHEEL
+Filename: almgroad-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.3.dist-info/top_level.txt
+Filename: almgroad-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.0.3.dist-info/RECORD
+Filename: almgroad-0.0.4.dist-info/RECORD
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
-        req = requests.get(url ,headers=headers).json()
+        req = requests.get(url ,headers=headers)
         bio = req["data"]["user"]["biography"]
         followers = req["data"]["user"]["edge_followed_by"]["count"]
         following = req["data"]["user"]["edge_follow"]["count"]
         fullname = req["data"]["user"]["full_name"]
         idd =  req["data"]["user"]["id"]
         username = req["data"]["user"]["username"]
         infoo = {
@@ -22,13 +22,13 @@
                 "FOLLOWING": following,
                 "BIO": bio,
                 "ID": idd,
                 "programmer": "ibrahim : telegram @B_xxBx"
             }
         }
         
-        infoo_json = json.dumps(infoo, indent=2, ensure_ascii=False)
-        return infoo_json
+        
+        return infoo
                 
     except Exception as e:
         return f"حدث خطأ :{e}"
```

## Comparing `almgroad-0.0.3.dist-info/METADATA` & `almgroad-0.0.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `almgroad-0.0.3.dist-info/RECORD` & `almgroad-0.0.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 almgroad/__init__.py,sha256=zoMF5LnI35a-tr86tp-UCgfcgFqVNHl_aXZB9Eh_UF8,55
 almgroad/chat.py,sha256=hUyCJzd5TaS-x1Y92c9Q5hCFMVnpKKg-nSvysy_KN30,128
-almgroad/infoinsta.py,sha256=WtBKkZNO87MEPDA3yiM8iya7PLi_wXLLkR2FpCk63k4,1136
-almgroad-0.0.3.dist-info/METADATA,sha256=FAdFgiA7Ve10XOPDwRoVEQ1IX9va5LBli6FExgP6vbQ,1434
-almgroad-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-almgroad-0.0.3.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
-almgroad-0.0.3.dist-info/RECORD,,
+almgroad/infoinsta.py,sha256=-py7cSz2WpBQUM5y7G8H0NxwVObMFAhMQgk566kuQ70,1064
+almgroad-0.0.4.dist-info/METADATA,sha256=IWp_D1qBjHWgfENDszmd4ZREfqkxGF4DJZUYl0YbU-g,1434
+almgroad-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+almgroad-0.0.4.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
+almgroad-0.0.4.dist-info/RECORD,,
```

