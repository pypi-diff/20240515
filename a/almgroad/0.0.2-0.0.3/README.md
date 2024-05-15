# Comparing `tmp/almgroad-0.0.2-py3-none-any.whl.zip` & `tmp/almgroad-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2823 bytes, number of entries: 7
+Zip file size: 2860 bytes, number of entries: 7
 -rw-rw----  2.0 unx       55 b- defN 24-May-15 03:30 almgroad/__init__.py
 -rw-rw----  2.0 unx      128 b- defN 24-May-15 03:17 almgroad/chat.py
--rw-rw----  2.0 unx      937 b- defN 24-May-14 19:17 almgroad/infoinsta.py
--rw-rw----  2.0 unx     1410 b- defN 24-May-15 03:32 almgroad-0.0.2.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-15 03:32 almgroad-0.0.2.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-15 03:32 almgroad-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 24-May-15 03:32 almgroad-0.0.2.dist-info/RECORD
-7 files, 3156 bytes uncompressed, 1891 bytes compressed:  40.1%
+-rw-rw----  2.0 unx     1136 b- defN 24-May-15 04:20 almgroad/infoinsta.py
+-rw-rw----  2.0 unx     1434 b- defN 24-May-15 04:23 almgroad-0.0.3.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-15 04:23 almgroad-0.0.3.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-15 04:23 almgroad-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      526 b- defN 24-May-15 04:23 almgroad-0.0.3.dist-info/RECORD
+7 files, 3380 bytes uncompressed, 1928 bytes compressed:  43.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: almgroad/chat.py
 Comment: 
 
 Filename: almgroad/infoinsta.py
 Comment: 
 
-Filename: almgroad-0.0.2.dist-info/METADATA
+Filename: almgroad-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.2.dist-info/WHEEL
+Filename: almgroad-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.2.dist-info/top_level.txt
+Filename: almgroad-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.0.2.dist-info/RECORD
+Filename: almgroad-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/infoinsta.py

```diff
@@ -1,31 +1,34 @@
 import requests 
+import json
+
 def Info_Insta(user_name):
-	url = f"https://www.instagram.com/api/v1/users/web_profile_info/?username={user_name}"
-	headers = {
-	    "X-Ig-App-Id": "1217981644879628",
-	}
-	try:
-	    req = requests.get(url ,headers=headers).json()
-	    bio = req["data"]["user"]["biography"]
-	    followers = req["data"]["user"]["edge_followed_by"]["count"]
-	    following = req["data"]["user"]["edge_follow"]["count"]
-	    fullname = req["data"]["user"]["full_name"]
-	    idd =  req["data"]["user"]["id"]
-	    username = req["data"]["user"]["username"]
-	    z=requests.get(f'https://o7aa.pythonanywhere.com/?id={idd}').json()
-	    date=z['date']
-	    infoo = f"""
-    \r     ( ACCOUNT INSTAGRAM )
-    
-	USERNAME : {username}
-	FULL NAME : {fullname}
-	FOLLOWERS : {followers}
-	FOLLOWING : {following}
-	BIO : {bio}
-	ID : {idd}
-	DATE : {date}
-	programmer : ibrahim : telegram @B_xxBx"""
-	    return infoo
-	except Exception as e:
-		return e
-	
+    url = f"https://www.instagram.com/api/v1/users/web_profile_info/?username={user_name}"
+    headers = {
+        "X-Ig-App-Id": "1217981644879628",
+    }
+    try:
+        req = requests.get(url ,headers=headers).json()
+        bio = req["data"]["user"]["biography"]
+        followers = req["data"]["user"]["edge_followed_by"]["count"]
+        following = req["data"]["user"]["edge_follow"]["count"]
+        fullname = req["data"]["user"]["full_name"]
+        idd =  req["data"]["user"]["id"]
+        username = req["data"]["user"]["username"]
+        infoo = {
+            "ACCOUNT INSTAGRAM": {
+                "USERNAME": username,
+                "FULL NAME": fullname,
+                "FOLLOWERS": followers,
+                "FOLLOWING": following,
+                "BIO": bio,
+                "ID": idd,
+                "programmer": "ibrahim : telegram @B_xxBx"
+            }
+        }
+        
+        infoo_json = json.dumps(infoo, indent=2, ensure_ascii=False)
+        return infoo_json
+                
+    except Exception as e:
+        return f"حدث خطأ :{e}"
+
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `almgroad-0.0.2.dist-info/METADATA` & `almgroad-0.0.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 
 python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps example-package-YOUR-USERNAME-HEREhttps://pypi.org/project/almgroad0770a/import requests
 import telebot
 from time import sleep 
 import threading 
 id = ايدي الحساب او القناة او المجموعة 
 bot = telebot.TeleBot("توكن_البوت")
```

