# Comparing `tmp/socketsecurity-0.0.50-py3-none-any.whl.zip` & `tmp/socketsecurity-0.0.51-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,17 @@
-Zip file size: 2702437 bytes, number of entries: 13
--rw-r--r--  2.0 unx    25977 b- defN 24-May-15 05:05 socketsecurity/core/__init__.py
+Zip file size: 2704431 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       49 b- defN 24-May-15 05:11 socketsecurity/__init__.py
+-rw-r--r--  2.0 unx     5457 b- defN 24-May-13 20:47 socketsecurity/socketcli.py
+-rw-r--r--  2.0 unx    25945 b- defN 24-May-15 05:12 socketsecurity/core/__init__.py
 -rw-r--r--  2.0 unx     8606 b- defN 24-May-13 22:21 socketsecurity/core/classes.py
 -rw-r--r--  2.0 unx      626 b- defN 24-Apr-29 13:52 socketsecurity/core/exceptions.py
 -rw-r--r--  2.0 unx    11251 b- defN 24-May-08 17:15 socketsecurity/core/github.py
 -rw-r--r--  2.0 unx    11208 b- defN 24-May-05 18:30 socketsecurity/core/glitlab.py
 -rw-r--r--  2.0 unx    67547 b- defN 24-May-05 17:36 socketsecurity/core/issues.py
 -rw-r--r--  2.0 unx 17442610 b- defN 24-May-06 19:45 socketsecurity/core/licenses.py
 -rw-r--r--  2.0 unx    11834 b- defN 24-May-08 17:02 socketsecurity/core/messages.py
--rw-r--r--  2.0 unx      771 b- defN 24-May-15 05:09 socketsecurity-0.0.50.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-15 05:09 socketsecurity-0.0.50.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 24-May-15 05:09 socketsecurity-0.0.50.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 24-May-15 05:09 socketsecurity-0.0.50.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1140 b- defN 24-May-15 05:09 socketsecurity-0.0.50.dist-info/RECORD
-13 files, 17581736 bytes uncompressed, 2700523 bytes compressed:  84.6%
+-rw-r--r--  2.0 unx      771 b- defN 24-May-15 05:12 socketsecurity-0.0.51.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 05:12 socketsecurity-0.0.51.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 24-May-15 05:12 socketsecurity-0.0.51.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 24-May-15 05:12 socketsecurity-0.0.51.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1305 b- defN 24-May-15 05:12 socketsecurity-0.0.51.dist-info/RECORD
+15 files, 17587375 bytes uncompressed, 2702259 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -1,7 +1,13 @@
+Filename: socketsecurity/__init__.py
+Comment: 
+
+Filename: socketsecurity/socketcli.py
+Comment: 
+
 Filename: socketsecurity/core/__init__.py
 Comment: 
 
 Filename: socketsecurity/core/classes.py
 Comment: 
 
 Filename: socketsecurity/core/exceptions.py
@@ -18,23 +24,23 @@
 
 Filename: socketsecurity/core/licenses.py
 Comment: 
 
 Filename: socketsecurity/core/messages.py
 Comment: 
 
-Filename: socketsecurity-0.0.50.dist-info/METADATA
+Filename: socketsecurity-0.0.51.dist-info/METADATA
 Comment: 
 
-Filename: socketsecurity-0.0.50.dist-info/WHEEL
+Filename: socketsecurity-0.0.51.dist-info/WHEEL
 Comment: 
 
-Filename: socketsecurity-0.0.50.dist-info/entry_points.txt
+Filename: socketsecurity-0.0.51.dist-info/entry_points.txt
 Comment: 
 
-Filename: socketsecurity-0.0.50.dist-info/top_level.txt
+Filename: socketsecurity-0.0.51.dist-info/top_level.txt
 Comment: 
 
-Filename: socketsecurity-0.0.50.dist-info/RECORD
+Filename: socketsecurity-0.0.51.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## socketsecurity/core/__init__.py

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.50'
+__version__ = '0.0.51'
 __all__ = [
     "Core",
     "log"
 ]
 
 
 global encoded_key
@@ -36,15 +36,14 @@
 timeout = 30
 full_scan_path = ""
 repository_path = ""
 all_issues = AllIssues()
 org_id = None
 org_slug = None
 all_new_alerts = False
-issue_file = "core/issues.json"
 security_policy = {}
 log = logging.getLogger("socketdev")
 log.addHandler(logging.NullHandler())
 
 
 def encode_key(token: str) -> None:
     """
```

## Comparing `socketsecurity-0.0.50.dist-info/METADATA` & `socketsecurity-0.0.51.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.50
+Version: 0.0.51
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `socketsecurity-0.0.50.dist-info/RECORD` & `socketsecurity-0.0.51.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-socketsecurity/core/__init__.py,sha256=KreBHydGNpQiv5mUWYiC02ms5yd4UqJb6yM0-SAj3fA,25977
+socketsecurity/__init__.py,sha256=VwFcI7y-q6P_5EDMwpCK21EirBfu5YizorB_DY0MAV0,49
+socketsecurity/socketcli.py,sha256=H4XEJXnT6du_u6pLvwOLcNV2B8K4A9r0UalEayRHQq4,5457
+socketsecurity/core/__init__.py,sha256=1gNLxoO93s5_vnKb4wl_velrehxkLvgm21337ZDY3LU,25945
 socketsecurity/core/classes.py,sha256=VlIzLOhG9Z5K-95ovblrCR9wDgGBs0N3mFSa6d9qbw8,8606
 socketsecurity/core/exceptions.py,sha256=C7q0D3KlnE3ff4FyTnlY9TxU3G-7xaRZcxpanUPvCzc,626
 socketsecurity/core/github.py,sha256=pvVE6l6qrJ18pw_1BtaPksVomchz1zDzJ09qSDFx5AU,11251
 socketsecurity/core/glitlab.py,sha256=SVfSDIbctTU5pOP_K_-YQAz8lIapZ3soFgkzdIKzajo,11208
 socketsecurity/core/issues.py,sha256=_AsYSTV-Fu4_o0fmxRV7JMZGQKyyaeN8mIvv64szwQ8,67547
 socketsecurity/core/licenses.py,sha256=VIpK01sRmKy_94ulojgWJHS2K8xo9YnW5KoJYhn8aaI,17442610
 socketsecurity/core/messages.py,sha256=O_1ik6vQKcajmio4IPT3saZYMzsuibsxx38Mw_WFFK0,11834
-socketsecurity-0.0.50.dist-info/METADATA,sha256=1x7vbEcccOfoLTC4WK6wa_iFTsLU-G1WDfaWTK16FOM,771
-socketsecurity-0.0.50.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-socketsecurity-0.0.50.dist-info/entry_points.txt,sha256=6RvItr40ejlapwQ9_dS5U5iuaBDvp8lIL2NZOn1xSPM,59
-socketsecurity-0.0.50.dist-info/top_level.txt,sha256=ukMzHpGy5wQ9XCd7OzP2Y2iBz3zd9mB7RtNzj5wf6c4,15
-socketsecurity-0.0.50.dist-info/RECORD,,
+socketsecurity-0.0.51.dist-info/METADATA,sha256=stgHunNLgu57bUmht5IeuS5uGAkGYdDttyX1mpdGm-g,771
+socketsecurity-0.0.51.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+socketsecurity-0.0.51.dist-info/entry_points.txt,sha256=6RvItr40ejlapwQ9_dS5U5iuaBDvp8lIL2NZOn1xSPM,59
+socketsecurity-0.0.51.dist-info/top_level.txt,sha256=ukMzHpGy5wQ9XCd7OzP2Y2iBz3zd9mB7RtNzj5wf6c4,15
+socketsecurity-0.0.51.dist-info/RECORD,,
```

