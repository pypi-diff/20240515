# Comparing `tmp/dbopenapi-0.0.4.tar.gz` & `tmp/dbopenapi-0.0.5.tar.gz`

## Comparing `dbopenapi-0.0.4.tar` & `dbopenapi-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/dbopenapi.pyproj
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/src/dbopenapi/OpenApi.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/src/dbopenapi/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/src/dbopenapi/code_realtime_account.py
--rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/src/dbopenapi/tr_code_to_path.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/LICENSE
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dbopenapi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/dbopenapi.pyproj
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/src/dbopenapi/OpenApi.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/src/dbopenapi/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/src/dbopenapi/code_realtime_account.py
+-rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/src/dbopenapi/tr_code_to_path.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/PKG-INFO
```

### Comparing `dbopenapi-0.0.4/dbopenapi.pyproj` & `dbopenapi-0.0.5/dbopenapi.pyproj`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.4/src/dbopenapi/OpenApi.py` & `dbopenapi-0.0.5/src/dbopenapi/OpenApi.py`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.4/src/dbopenapi/tr_code_to_path.py` & `dbopenapi-0.0.5/src/dbopenapi/tr_code_to_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     "CFOHQ02500" : "/api/v1/trading/night-futureoption/inquiry/balance", # 선물옵션 잔고조회 (야간)
     
     # 국내선물옵션시세
     "FCODES" : "/api/v1/quote/kr-futureoption/inquiry/future-ticker", # 선물종목 조회
     "OCODES" : "/api/v1/quote/kr-futureoption/inquiry/option-ticker", # 옵션종목 조회
     "FPRICE" : "/api/v1/quote/kr-futureoption/inquiry/price", # 현재가조회 ...............
     "FHOGA" : "/api/v1/quote/kr-futureoption/inquiry/orderbook", # 호가조회 ...............
-    "DAYTRADE" : "/api/v1/quote/kr-futureoption/inquiry/daily-price", # 일별체결조회
-    "CONCLUSION" : "/api/v1/quote/kr-futureoption/inquiry/hour-price", # 시간대별체결조회
+    "FDAYTRADE" : "/api/v1/quote/kr-futureoption/inquiry/daily-price", # 일별체결조회 ...............
+    "FCONCLUSION" : "/api/v1/quote/kr-futureoption/inquiry/hour-price", # 시간대별체결조회 ...............
     
     # 국내선물옵션시세(실시간)
     "IF0" : "/websocket", # [실시간]선물옵션주문체결
     "F01" : "/websocket", # [실시간]지수선물호가
     "F00" : "/websocket", # [실시간]지수선물체결
     "F91" : "/websocket", # [실시간]미니지수선물호가
     "F90" : "/websocket", # [실시간]미니지수선물체결
```

### Comparing `dbopenapi-0.0.4/.gitignore` & `dbopenapi-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.4/LICENSE` & `dbopenapi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.4/README.md` & `dbopenapi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.4/pyproject.toml` & `dbopenapi-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dbopenapi"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="teranum", email="teranum@gmail.com" },
 ]
 description = "package for db openapi"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dbopenapi-0.0.4/PKG-INFO` & `dbopenapi-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbopenapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: package for db openapi
 Project-URL: Homepage, https://github.com/teranum/python-packages/tree/master/dbopenapi
 Project-URL: Issues, https://github.com/teranum/python-packages/issues
 Author-email: teranum <teranum@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

