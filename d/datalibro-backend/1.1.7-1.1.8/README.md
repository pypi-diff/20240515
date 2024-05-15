# Comparing `tmp/datalibro_backend-1.1.7.tar.gz` & `tmp/datalibro_backend-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_backend-1.1.7.tar", last modified: Mon May 13 10:16:03 2024, max compression
+gzip compressed data, was "datalibro_backend-1.1.8.tar", last modified: Wed May 15 06:18:36 2024, max compression
```

## Comparing `datalibro_backend-1.1.7.tar` & `datalibro_backend-1.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-13 10:16:03.036903 datalibro_backend-1.1.7/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.7/LICENSE.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-13 10:16:03.036621 datalibro_backend-1.1.7/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.7/README.md
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-13 10:16:03.035350 datalibro_backend-1.1.7/datalibro_backend/
--rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.7/datalibro_backend/__init__.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    15448 2024-05-13 10:15:45.000000 datalibro_backend-1.1.7/datalibro_backend/quality_check.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    12823 2024-05-13 09:15:55.000000 datalibro_backend-1.1.7/datalibro_backend/read_file.py
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-13 10:16:03.036393 datalibro_backend-1.1.7/datalibro_backend.egg-info/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-13 10:16:02.000000 datalibro_backend-1.1.7/datalibro_backend.egg-info/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-13 10:16:03.000000 datalibro_backend-1.1.7/datalibro_backend.egg-info/SOURCES.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-13 10:16:02.000000 datalibro_backend-1.1.7/datalibro_backend.egg-info/dependency_links.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-13 10:16:02.000000 datalibro_backend-1.1.7/datalibro_backend.egg-info/top_level.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-13 10:16:03.037007 datalibro_backend-1.1.7/setup.cfg
--rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-13 10:15:54.000000 datalibro_backend-1.1.7/setup.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-15 06:18:36.011304 datalibro_backend-1.1.8/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.8/LICENSE.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-15 06:18:36.011019 datalibro_backend-1.1.8/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.8/README.md
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-15 06:18:36.009971 datalibro_backend-1.1.8/datalibro_backend/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.8/datalibro_backend/__init__.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    15448 2024-05-13 10:15:45.000000 datalibro_backend-1.1.8/datalibro_backend/quality_check.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    12946 2024-05-15 06:17:37.000000 datalibro_backend-1.1.8/datalibro_backend/read_file.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-15 06:18:36.010802 datalibro_backend-1.1.8/datalibro_backend.egg-info/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-15 06:18:35.000000 datalibro_backend-1.1.8/datalibro_backend.egg-info/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-15 06:18:35.000000 datalibro_backend-1.1.8/datalibro_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-15 06:18:35.000000 datalibro_backend-1.1.8/datalibro_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-15 06:18:35.000000 datalibro_backend-1.1.8/datalibro_backend.egg-info/top_level.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-15 06:18:36.011361 datalibro_backend-1.1.8/setup.cfg
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-15 06:18:09.000000 datalibro_backend-1.1.8/setup.py
```

### Comparing `datalibro_backend-1.1.7/LICENSE.txt` & `datalibro_backend-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.7/PKG-INFO` & `datalibro_backend-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro_backend
-Version: 1.1.7
+Version: 1.1.8
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.7/README.md` & `datalibro_backend-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.7/datalibro_backend/quality_check.py` & `datalibro_backend-1.1.8/datalibro_backend/quality_check.py`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.7/datalibro_backend/read_file.py` & `datalibro_backend-1.1.8/datalibro_backend/read_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     }
     }
     response = requests.delete(url, headers=headers, json=data)
     if response.status_code == 200:
         print("Spreadsheet cleared successfully.")
     else:
         print("Failed to clear spreadsheet:", response.text)
-def upload_data_to_feishu(table, spreadsheet_token,sheet_id,defualt_start_index = 'A1'):
+def upload_data_to_feishu(table, spreadsheet_token,sheet_id,defualt_start_index = 'A1',delete_first='Yes',startIndex=1):
     app_id = 'cli_a5eeb3ad3837100b'
     app_secret = 'ftLZbDJOzDxSx0xiigALNev1tgHTvR4V'
     # Obtain an access token
     auth_url = "https://open.feishu.cn/open-apis/auth/v3/app_access_token/internal/"
     headers = {
         "Content-Type": "application/json"
     }
@@ -331,15 +331,18 @@
         "valueRange": {
             "range": f"{sheet_id}!{defualt_start_index}:T{len(value)+1}",
             "values": value
   
         }
     }
     try:
-        clear_fs_spreadsheet(access_token,spreadsheet_token,sheet_id,endIndex=len(value))
+        if delete_first == 'Yes':
+            clear_fs_spreadsheet(access_token,spreadsheet_token,sheet_id,startIndex=startIndex,endIndex=len(value))
+        else:
+            pass
         
     except:
         return f"{traceback.format_exc()}"
     response = requests.post(url, json=body, headers=headers)
     if response.status_code == 200:
         return "Data uploaded successfully."
     else:
```

### Comparing `datalibro_backend-1.1.7/datalibro_backend.egg-info/PKG-INFO` & `datalibro_backend-1.1.8/datalibro_backend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro-backend
-Version: 1.1.7
+Version: 1.1.8
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.7/setup.py` & `datalibro_backend-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="datalibro_backend",
-  version="1.1.7",
+  version="1.1.8",
   author="lucy",
   author_email="lucy@petlibro.com",
   description="A small package for your backend service",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/DesignLibro/datalibro_backend",
   packages=setuptools.find_packages(),
```

