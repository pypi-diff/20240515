# Comparing `tmp/blues_lib-1.1.6.tar.gz` & `tmp/blues_lib-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.1.6.tar", last modified: Wed May 15 16:56:50 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.1.7.tar", last modified: Wed May 15 17:02:18 2024, max compression
```

## Comparing `blues_lib-1.1.6.tar` & `blues_lib-1.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.441381 blues_lib-1.1.6/
--rw-rw-rw-   0        0        0     1172 2024-05-15 16:56:50.441381 blues_lib-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      697 2024-05-12 15:38:25.000000 blues_lib-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.385865 blues_lib-1.1.6/blues_lib/
--rw-rw-rw-   0        0        0        0 2024-05-10 14:52:26.000000 blues_lib-1.1.6/blues_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.392613 blues_lib-1.1.6/blues_lib/sele/
--rw-rw-rw-   0        0        0      652 2024-05-12 04:42:19.000000 blues_lib-1.1.6/blues_lib/sele/BluesBrowser.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.6/blues_lib/sele/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.395419 blues_lib-1.1.6/blues_lib/sele/action/
--rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.1.6/blues_lib/sele/action/BluesDriverAction.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.6/blues_lib/sele/action/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.415562 blues_lib-1.1.6/blues_lib/sele/action/parts/
--rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesAlertAction.py
--rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesCookieAction.py
--rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesDocumentAction.py
--rw-rw-rw-   0        0        0     4476 2024-05-14 16:07:22.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesElementAction.py
--rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesEventAction.py
--rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesFormAction.py
--rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesFrameAction.py
--rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesJavaScriptAction.py
--rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesMoverAction.py
--rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesSelectAction.py
--rw-rw-rw-   0        0        0     3398 2024-05-12 15:25:06.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/BluesWindowAction.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.6/blues_lib/sele/action/parts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.421590 blues_lib-1.1.6/blues_lib/sele/browser/
--rw-rw-rw-   0        0        0     3941 2024-05-15 16:56:35.000000 blues_lib-1.1.6/blues_lib/sele/browser/BluesChrome.py
--rw-rw-rw-   0        0        0     3280 2024-05-13 13:12:42.000000 blues_lib-1.1.6/blues_lib/sele/browser/BluesDebugChrome.py
--rw-rw-rw-   0        0        0     4120 2024-05-12 15:25:06.000000 blues_lib-1.1.6/blues_lib/sele/browser/BluesProxyChrome.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.6/blues_lib/sele/browser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.426397 blues_lib-1.1.6/blues_lib/sql/
--rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.1.6/blues_lib/sql/BluesMySQLExecutor.py
--rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.1.6/blues_lib/sql/BluesSQLConvertor.py
--rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.1.6/blues_lib/sql/BluesSQLExecutor.py
--rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.1.6/blues_lib/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.440382 blues_lib-1.1.6/blues_lib/util/
--rw-rw-rw-   0        0        0     1494 2024-05-15 15:54:09.000000 blues_lib-1.1.6/blues_lib/util/BluesConsole.py
--rw-rw-rw-   0        0        0      813 2024-05-15 15:47:32.000000 blues_lib-1.1.6/blues_lib/util/BluesDateTime.py
--rw-rw-rw-   0        0        0     5231 2024-05-13 17:00:25.000000 blues_lib-1.1.6/blues_lib/util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.1.6/blues_lib/util/BluesImager.py
--rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.1.6/blues_lib/util/BluesLogger.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.1.6/blues_lib/util/BluesMailer.py
--rw-rw-rw-   0        0        0     1713 2024-05-14 16:40:53.000000 blues_lib-1.1.6/blues_lib/util/BluesPowerShell.py
--rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.1.6/blues_lib/util/BluesType.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.6/blues_lib/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:56:50.390093 blues_lib-1.1.6/blues_lib.egg-info/
--rw-rw-rw-   0        0        0     1172 2024-05-15 16:56:50.000000 blues_lib-1.1.6/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2024-05-15 16:56:50.000000 blues_lib-1.1.6/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:56:50.000000 blues_lib-1.1.6/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-15 16:56:50.000000 blues_lib-1.1.6/blues_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-15 16:56:50.443333 blues_lib-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      575 2024-05-15 16:56:43.000000 blues_lib-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.599597 blues_lib-1.1.7/
+-rw-rw-rw-   0        0        0     1172 2024-05-15 17:02:18.599597 blues_lib-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2024-05-12 15:38:25.000000 blues_lib-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.549821 blues_lib-1.1.7/blues_lib/
+-rw-rw-rw-   0        0        0        0 2024-05-10 14:52:26.000000 blues_lib-1.1.7/blues_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.557078 blues_lib-1.1.7/blues_lib/sele/
+-rw-rw-rw-   0        0        0      652 2024-05-12 04:42:19.000000 blues_lib-1.1.7/blues_lib/sele/BluesBrowser.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.7/blues_lib/sele/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.559620 blues_lib-1.1.7/blues_lib/sele/action/
+-rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.1.7/blues_lib/sele/action/BluesDriverAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.7/blues_lib/sele/action/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.579567 blues_lib-1.1.7/blues_lib/sele/action/parts/
+-rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesAlertAction.py
+-rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesCookieAction.py
+-rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesDocumentAction.py
+-rw-rw-rw-   0        0        0     4476 2024-05-14 16:07:22.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesElementAction.py
+-rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesEventAction.py
+-rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesFormAction.py
+-rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesFrameAction.py
+-rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesJavaScriptAction.py
+-rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesMoverAction.py
+-rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesSelectAction.py
+-rw-rw-rw-   0        0        0     3398 2024-05-12 15:25:06.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/BluesWindowAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.7/blues_lib/sele/action/parts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.583383 blues_lib-1.1.7/blues_lib/sele/browser/
+-rw-rw-rw-   0        0        0     3942 2024-05-15 16:59:19.000000 blues_lib-1.1.7/blues_lib/sele/browser/BluesChrome.py
+-rw-rw-rw-   0        0        0     3280 2024-05-13 13:12:42.000000 blues_lib-1.1.7/blues_lib/sele/browser/BluesDebugChrome.py
+-rw-rw-rw-   0        0        0     4120 2024-05-12 15:25:06.000000 blues_lib-1.1.7/blues_lib/sele/browser/BluesProxyChrome.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.7/blues_lib/sele/browser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.587677 blues_lib-1.1.7/blues_lib/sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.1.7/blues_lib/sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.1.7/blues_lib/sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.1.7/blues_lib/sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.1.7/blues_lib/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.599597 blues_lib-1.1.7/blues_lib/util/
+-rw-rw-rw-   0        0        0     1494 2024-05-15 15:54:09.000000 blues_lib-1.1.7/blues_lib/util/BluesConsole.py
+-rw-rw-rw-   0        0        0      813 2024-05-15 15:47:32.000000 blues_lib-1.1.7/blues_lib/util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     5231 2024-05-13 17:00:25.000000 blues_lib-1.1.7/blues_lib/util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.1.7/blues_lib/util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.1.7/blues_lib/util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.1.7/blues_lib/util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1713 2024-05-14 16:40:53.000000 blues_lib-1.1.7/blues_lib/util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.1.7/blues_lib/util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.7/blues_lib/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:02:18.554983 blues_lib-1.1.7/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1172 2024-05-15 17:02:18.000000 blues_lib-1.1.7/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2024-05-15 17:02:18.000000 blues_lib-1.1.7/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:02:18.000000 blues_lib-1.1.7/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 17:02:18.000000 blues_lib-1.1.7/blues_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-15 17:02:18.601100 blues_lib-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      575 2024-05-15 17:02:01.000000 blues_lib-1.1.7/setup.py
```

### Comparing `blues_lib-1.1.6/PKG-INFO` & `blues_lib-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues_lib
-Version: 1.1.6
+Version: 1.1.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.1.6/README.md` & `blues_lib-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/BluesBrowser.py` & `blues_lib-1.1.7/blues_lib/sele/BluesBrowser.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/BluesDriverAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/BluesDriverAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesAlertAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesAlertAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesCookieAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesCookieAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesDocumentAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesDocumentAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesElementAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesElementAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesEventAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesEventAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesFormAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesFormAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesFrameAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesFrameAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesJavaScriptAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesJavaScriptAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesMoverAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesMoverAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesSelectAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesSelectAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/action/parts/BluesWindowAction.py` & `blues_lib-1.1.7/blues_lib/sele/action/parts/BluesWindowAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/browser/BluesChrome.py` & `blues_lib-1.1.7/blues_lib/sele/browser/BluesChrome.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     '--ignore-certificate-errors':'',
     '--disable-infobars':'',
     '--hide-crash-restore-bubble':'',
     '--disable-popup-blocking':'',
     #'--disable-extensions-api':'', # 禁用此项，会导致debug模式下也无法存储登录信息
     '--disable-application-install-prompt':'',
     '--no-first-run':'', 
-    '--disable-first-run-ui':'', # 可以屏蔽首次执行设置
+    #'--disable-first-run-ui':'', # 可以屏蔽首次执行设置
   }
 
   EXPERIMENTAL_OPTIONS = {
     'detach':True,
     'prefs' : {
       # 0 - Default, 1 - Allow, 2 - Block
       "profile.default_content_setting_values.notification": 2,
```

### Comparing `blues_lib-1.1.6/blues_lib/sele/browser/BluesDebugChrome.py` & `blues_lib-1.1.7/blues_lib/sele/browser/BluesDebugChrome.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sele/browser/BluesProxyChrome.py` & `blues_lib-1.1.7/blues_lib/sele/browser/BluesProxyChrome.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sql/BluesMySQLExecutor.py` & `blues_lib-1.1.7/blues_lib/sql/BluesMySQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sql/BluesSQLConvertor.py` & `blues_lib-1.1.7/blues_lib/sql/BluesSQLConvertor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/sql/BluesSQLExecutor.py` & `blues_lib-1.1.7/blues_lib/sql/BluesSQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/util/BluesConsole.py` & `blues_lib-1.1.7/blues_lib/util/BluesConsole.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/util/BluesDateTime.py` & `blues_lib-1.1.7/blues_lib/util/BluesDateTime.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/util/BluesFiler.py` & `blues_lib-1.1.7/blues_lib/util/BluesFiler.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/util/BluesImager.py` & `blues_lib-1.1.7/blues_lib/util/BluesImager.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/util/BluesLogger.py` & `blues_lib-1.1.7/blues_lib/util/BluesLogger.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/util/BluesMailer.py` & `blues_lib-1.1.7/blues_lib/util/BluesMailer.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib/util/BluesPowerShell.py` & `blues_lib-1.1.7/blues_lib/util/BluesPowerShell.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/blues_lib.egg-info/PKG-INFO` & `blues_lib-1.1.7/blues_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues-lib
-Version: 1.1.6
+Version: 1.1.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.1.6/blues_lib.egg-info/SOURCES.txt` & `blues_lib-1.1.7/blues_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.6/setup.py` & `blues_lib-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
   name="blues_lib", # package name
-  version="1.1.6", # package version
+  version="1.1.7", # package version
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
   packages=find_packages(), # package module
   # add from requirement.txt,本地测试注释所有包，不能从镜像立即安装
   install_requires=[
     #'Pillow>=10.3.0',
     #'Requests>=2.31.0',
```

