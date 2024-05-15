# Comparing `tmp/blues_lib-1.1.3.tar.gz` & `tmp/blues_lib-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.1.3.tar", last modified: Mon May 13 17:03:23 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.1.4.tar", last modified: Wed May 15 15:55:22 2024, max compression
```

## Comparing `blues_lib-1.1.3.tar` & `blues_lib-1.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.705390 blues_lib-1.1.3/
--rw-rw-rw-   0        0        0     1172 2024-05-13 17:03:23.705390 blues_lib-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      697 2024-05-12 15:38:25.000000 blues_lib-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.635805 blues_lib-1.1.3/blues_lib/
--rw-rw-rw-   0        0        0        0 2024-05-10 14:52:26.000000 blues_lib-1.1.3/blues_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.645758 blues_lib-1.1.3/blues_lib/sele/
--rw-rw-rw-   0        0        0      652 2024-05-12 04:42:19.000000 blues_lib-1.1.3/blues_lib/sele/BluesBrowser.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/sele/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.648605 blues_lib-1.1.3/blues_lib/sele/action/
--rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.1.3/blues_lib/sele/action/BluesDriverAction.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/sele/action/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.674516 blues_lib-1.1.3/blues_lib/sele/action/parts/
--rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesAlertAction.py
--rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesCookieAction.py
--rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesDocumentAction.py
--rw-rw-rw-   0        0        0     4408 2024-05-08 16:59:14.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesElementAction.py
--rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesEventAction.py
--rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesFormAction.py
--rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesFrameAction.py
--rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesJavaScriptAction.py
--rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesMoverAction.py
--rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesSelectAction.py
--rw-rw-rw-   0        0        0     3398 2024-05-12 15:25:06.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesWindowAction.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.680009 blues_lib-1.1.3/blues_lib/sele/browser/
--rw-rw-rw-   0        0        0     3862 2024-05-13 13:14:08.000000 blues_lib-1.1.3/blues_lib/sele/browser/BluesChrome.py
--rw-rw-rw-   0        0        0     3280 2024-05-13 13:12:42.000000 blues_lib-1.1.3/blues_lib/sele/browser/BluesDebugChrome.py
--rw-rw-rw-   0        0        0     4120 2024-05-12 15:25:06.000000 blues_lib-1.1.3/blues_lib/sele/browser/BluesProxyChrome.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/sele/browser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.685930 blues_lib-1.1.3/blues_lib/sql/
--rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.1.3/blues_lib/sql/BluesMySQLExecutor.py
--rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.1.3/blues_lib/sql/BluesSQLConvertor.py
--rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.1.3/blues_lib/sql/BluesSQLExecutor.py
--rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.1.3/blues_lib/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.703388 blues_lib-1.1.3/blues_lib/util/
--rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.1.3/blues_lib/util/BluesConsole.py
--rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.1.3/blues_lib/util/BluesDateTime.py
--rw-rw-rw-   0        0        0     5231 2024-05-13 17:00:25.000000 blues_lib-1.1.3/blues_lib/util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.1.3/blues_lib/util/BluesImager.py
--rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.1.3/blues_lib/util/BluesLogger.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.1.3/blues_lib/util/BluesMailer.py
--rw-rw-rw-   0        0        0     1744 2024-05-13 12:40:57.000000 blues_lib-1.1.3/blues_lib/util/BluesPowerShell.py
--rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.1.3/blues_lib/util/BluesType.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.642553 blues_lib-1.1.3/blues_lib.egg-info/
--rw-rw-rw-   0        0        0     1172 2024-05-13 17:03:23.000000 blues_lib-1.1.3/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2024-05-13 17:03:23.000000 blues_lib-1.1.3/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:03:23.000000 blues_lib-1.1.3/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-13 17:03:23.000000 blues_lib-1.1.3/blues_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-13 17:03:23.707686 blues_lib-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      575 2024-05-13 17:00:41.000000 blues_lib-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.207097 blues_lib-1.1.4/
+-rw-rw-rw-   0        0        0     1172 2024-05-15 15:55:22.207097 blues_lib-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2024-05-12 15:38:25.000000 blues_lib-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.145641 blues_lib-1.1.4/blues_lib/
+-rw-rw-rw-   0        0        0        0 2024-05-10 14:52:26.000000 blues_lib-1.1.4/blues_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.154756 blues_lib-1.1.4/blues_lib/sele/
+-rw-rw-rw-   0        0        0      652 2024-05-12 04:42:19.000000 blues_lib-1.1.4/blues_lib/sele/BluesBrowser.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.4/blues_lib/sele/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.156771 blues_lib-1.1.4/blues_lib/sele/action/
+-rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.1.4/blues_lib/sele/action/BluesDriverAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.4/blues_lib/sele/action/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.177768 blues_lib-1.1.4/blues_lib/sele/action/parts/
+-rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesAlertAction.py
+-rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesCookieAction.py
+-rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesDocumentAction.py
+-rw-rw-rw-   0        0        0     4476 2024-05-14 16:07:22.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesElementAction.py
+-rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesEventAction.py
+-rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesFormAction.py
+-rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesFrameAction.py
+-rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesJavaScriptAction.py
+-rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesMoverAction.py
+-rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesSelectAction.py
+-rw-rw-rw-   0        0        0     3398 2024-05-12 15:25:06.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/BluesWindowAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.4/blues_lib/sele/action/parts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.185190 blues_lib-1.1.4/blues_lib/sele/browser/
+-rw-rw-rw-   0        0        0     3862 2024-05-13 13:14:08.000000 blues_lib-1.1.4/blues_lib/sele/browser/BluesChrome.py
+-rw-rw-rw-   0        0        0     3280 2024-05-13 13:12:42.000000 blues_lib-1.1.4/blues_lib/sele/browser/BluesDebugChrome.py
+-rw-rw-rw-   0        0        0     4120 2024-05-12 15:25:06.000000 blues_lib-1.1.4/blues_lib/sele/browser/BluesProxyChrome.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.4/blues_lib/sele/browser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.190807 blues_lib-1.1.4/blues_lib/sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.1.4/blues_lib/sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.1.4/blues_lib/sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.1.4/blues_lib/sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.1.4/blues_lib/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.206077 blues_lib-1.1.4/blues_lib/util/
+-rw-rw-rw-   0        0        0     1494 2024-05-15 15:54:09.000000 blues_lib-1.1.4/blues_lib/util/BluesConsole.py
+-rw-rw-rw-   0        0        0      813 2024-05-15 15:47:32.000000 blues_lib-1.1.4/blues_lib/util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     5231 2024-05-13 17:00:25.000000 blues_lib-1.1.4/blues_lib/util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.1.4/blues_lib/util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.1.4/blues_lib/util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.1.4/blues_lib/util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1713 2024-05-14 16:40:53.000000 blues_lib-1.1.4/blues_lib/util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.1.4/blues_lib/util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.4/blues_lib/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:55:22.151720 blues_lib-1.1.4/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1172 2024-05-15 15:55:22.000000 blues_lib-1.1.4/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2024-05-15 15:55:22.000000 blues_lib-1.1.4/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:55:22.000000 blues_lib-1.1.4/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 15:55:22.000000 blues_lib-1.1.4/blues_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-15 15:55:22.208100 blues_lib-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      575 2024-05-15 15:55:18.000000 blues_lib-1.1.4/setup.py
```

### Comparing `blues_lib-1.1.3/PKG-INFO` & `blues_lib-1.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues_lib
-Version: 1.1.3
+Version: 1.1.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.1.3/README.md` & `blues_lib-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/BluesBrowser.py` & `blues_lib-1.1.4/blues_lib/sele/BluesBrowser.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/BluesDriverAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/BluesDriverAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesAlertAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesAlertAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesCookieAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesCookieAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesDocumentAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesDocumentAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesElementAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesElementAction.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,42 +77,42 @@
     @description : Determines whether the element exists
     @param {str} selector : css selector
     @returns {bool}
     '''
     eles = self.get_all(selector)
     return True if eles else False
 
-  def is_presence(self,selector):
-    return self.__get_status(selector,'presence')
+  def is_presence(self,selector,timeout=1):
+    return self.__get_status(selector,timeout,'presence')
 
-  def is_visibility(self,selector):
-    return self.__get_status(selector,'visibility')
+  def is_visibility(self,selector,timeout=1):
+    return self.__get_status(selector,timeout,'visibility')
 
-  def is_clickable(self,selector):
-    return self.__get_status(selector,'clickable')
+  def is_clickable(self,selector,timeout=1):
+    return self.__get_status(selector,timeout,'clickable')
   
   def is_enabled(self,selector):
     return self.get(selector).is_enabled()
 
   def is_displayed(self,selector):
     return self.get(selector).is_displayed()
 
   def is_selected(self,selector):
     return self.get(selector).is_selected()
 
   # === part last:  tool func === #
-  def __get_status(self,selector,wait_type):
+  def __get_status(self,selector,timeout,wait_type):
     '''
     @description : Determines whether the element exists
     @param {str} selector : css selector
     @param {str} wait_type
     @returns {bool}
     '''
     try:
-      self.wait(selector,1,wait_type)
+      self.wait(selector,timeout,wait_type)
       return True
     except Exception as e:
       return False
 
   def __get_wait_func(self,selector,wait_type='presence'):
     '''
     @description 获取条件判断函数
```

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesEventAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesEventAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesFormAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesFormAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesFrameAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesFrameAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesJavaScriptAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesJavaScriptAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesMoverAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesMoverAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesSelectAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesSelectAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesWindowAction.py` & `blues_lib-1.1.4/blues_lib/sele/action/parts/BluesWindowAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/browser/BluesChrome.py` & `blues_lib-1.1.4/blues_lib/sele/browser/BluesChrome.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/browser/BluesDebugChrome.py` & `blues_lib-1.1.4/blues_lib/sele/browser/BluesDebugChrome.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sele/browser/BluesProxyChrome.py` & `blues_lib-1.1.4/blues_lib/sele/browser/BluesProxyChrome.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sql/BluesMySQLExecutor.py` & `blues_lib-1.1.4/blues_lib/sql/BluesMySQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sql/BluesSQLConvertor.py` & `blues_lib-1.1.4/blues_lib/sql/BluesSQLConvertor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/sql/BluesSQLExecutor.py` & `blues_lib-1.1.4/blues_lib/sql/BluesSQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/util/BluesConsole.py` & `blues_lib-1.1.4/blues_lib/util/BluesConsole.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 class BluesConsole():
 
   COLORS = {
     'warn' : '\033[93m',
     'success' : '\033[92m',
     'info' : '\033[94m',
     'error' : '\033[91m',
-    'light' : '\033[95m',
+    'wait' : '\033[95m',
     'bold' : '\033[1m',
     'underline' : '\033[4m',
     'default' : '\033[0m',
   }
 
   @classmethod
-  def success(cls,value,label='sucess: '):
+  def success(cls,value,label='Sucess'):
     '''
     @description : print value with colorful prefix
     @param {any} value : any type of value
     @param {str} label :  the label in prefix
     '''
-    print(f"\n{cls.COLORS['success']}>>> {label}{cls.COLORS['default']}",value)
+    print(f"\n{cls.COLORS['success']}{label} >>> {cls.COLORS['default']}",value)
   
   @classmethod
-  def info(cls,value,label='info: '):
-    print(f"\n{cls.COLORS['info']}>>> {label}{cls.COLORS['default']}",value)
+  def info(cls,value,label='Info'):
+    print(f"\n{cls.COLORS['info']}{label} >>> {cls.COLORS['default']}",value)
   
   @classmethod
-  def warn(cls,value,label='warn: '):
-    print(f"\n{cls.COLORS['warn']}>>> {label}{cls.COLORS['default']}",value)
+  def warn(cls,value,label='Warn'):
+    print(f"\n{cls.COLORS['warn']}{label} >>> {cls.COLORS['default']}",value)
   
   @classmethod
-  def error(cls,value,label='error: '):
-    print(f"\n{cls.COLORS['error']}>>> {label}{cls.COLORS['default']}",value)
+  def error(cls,value,label='Error'):
+    print(f"\n{cls.COLORS['error']}{label} >>> {cls.COLORS['default']}",value)
   
   @classmethod
-  def light(cls,value,label='light: '):
-    print(f"\n{cls.COLORS['light']}>>> {label}{cls.COLORS['default']}",value)
+  def wait(cls,value,label='Wait'):
+    print(f"\n{cls.COLORS['wait']}{label} >>> {cls.COLORS['default']}",value)
   
   @classmethod
-  def bold(cls,value,label='bold: '):
-    print(f"\n{cls.COLORS['bold']}>>> {label}{cls.COLORS['default']}",value)
+  def bold(cls,value,label='Bold'):
+    print(f"\n{cls.COLORS['bold']}{label} >>> {cls.COLORS['default']}",value)
   
   @classmethod
-  def underline(cls,value,label='underline: '):
-    print(f"\n{cls.COLORS['underline']}>>> {label}{cls.COLORS['default']}",value)
+  def underline(cls,value,label='Underline'):
+    print(f"\n{cls.COLORS['underline']}{label} >>> {cls.COLORS['default']}",value)
   
   @classmethod
-  def print(cls,value,label='log: '):
-    print(f"\n>>> {label}",value)
+  def print(cls,value,label='Log'):
+    print(f"\n{label} >>> ",value)
```

### Comparing `blues_lib-1.1.3/blues_lib/util/BluesDateTime.py` & `blues_lib-1.1.4/blues_lib/util/BluesDateTime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from .BluesConsole import BluesConsole
 
 class BluesDateTime():
 
   spend = 0
 
   @classmethod
   def count_down(cls,payload):
@@ -16,15 +17,15 @@
 
     duration = payload.get('duration',10)
     interval = payload.get('interval',1)
     title = payload.get('title','coutdown')
     printable = payload.get('printable')
     
     if printable: 
-      print('===> %s : %s' % (title,duration-cls.spend))
+      BluesConsole.wait('%s : %s' % (title,duration-cls.spend))
 
     time.sleep(interval) 
     cls.spend+=interval
     if cls.spend < duration:
       cls.count_down(payload)
     else:
       cls.spend=0
```

### Comparing `blues_lib-1.1.3/blues_lib/util/BluesFiler.py` & `blues_lib-1.1.4/blues_lib/util/BluesFiler.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/util/BluesImager.py` & `blues_lib-1.1.4/blues_lib/util/BluesImager.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/util/BluesLogger.py` & `blues_lib-1.1.4/blues_lib/util/BluesLogger.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/util/BluesMailer.py` & `blues_lib-1.1.4/blues_lib/util/BluesMailer.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/blues_lib/util/BluesPowerShell.py` & `blues_lib-1.1.4/blues_lib/util/BluesPowerShell.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     @param {str}  args : the multi exe executor's arguments, split by space
      - '--arg1 --arg2 --arg3'
     '''
     args_list = ''
     if args:
       args_list = '-ArgumentList \'%s\''  % args
     ps_script = 'Start-Process -FilePath \'%s\' %s' % (file_path,args_list)
-    print('===>ps',ps_script)
     return cls.execute(ps_script )
 
   @classmethod
   def get_env_value(cls,name):
     '''
     @description : get env variable's value
     @param {str} name : varibale's name
```

### Comparing `blues_lib-1.1.3/blues_lib.egg-info/PKG-INFO` & `blues_lib-1.1.4/blues_lib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues-lib
-Version: 1.1.3
+Version: 1.1.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.1.3/blues_lib.egg-info/SOURCES.txt` & `blues_lib-1.1.4/blues_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.3/setup.py` & `blues_lib-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
   name="blues_lib", # package name
-  version="1.1.3", # package version
+  version="1.1.4", # package version
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
   packages=find_packages(), # package module
   # add from requirement.txt,本地测试注释所有包，不能从镜像立即安装
   install_requires=[
     #'Pillow>=10.3.0',
     #'Requests>=2.31.0',
```

