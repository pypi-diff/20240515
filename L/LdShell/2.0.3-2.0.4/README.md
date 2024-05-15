# Comparing `tmp/LdShell-2.0.3.tar.gz` & `tmp/LdShell-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LdShell-2.0.3.tar", last modified: Sun May 12 02:02:40 2024, max compression
+gzip compressed data, was "LdShell-2.0.4.tar", last modified: Wed May 15 04:42:08 2024, max compression
```

## Comparing `LdShell-2.0.3.tar` & `LdShell-2.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 02:02:40.753208 LdShell-2.0.3/
--rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-2.0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-12 02:02:40.749641 LdShell-2.0.3/LdShell/
--rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-2.0.3/LdShell/__init__.py
--rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-2.0.3/LdShell/__version__.py
--rw-rw-rw-   0        0        0     8841 2024-05-12 01:56:40.000000 LdShell-2.0.3/LdShell/core.py
--rw-rw-rw-   0        0        0      250 2024-05-12 01:54:35.000000 LdShell-2.0.3/LdShell/test.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:02:40.752039 LdShell-2.0.3/LdShell.egg-info/
--rw-rw-rw-   0        0        0     3038 2024-05-12 02:02:40.000000 LdShell-2.0.3/LdShell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-12 02:02:40.000000 LdShell-2.0.3/LdShell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 02:02:40.000000 LdShell-2.0.3/LdShell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-12 02:02:40.000000 LdShell-2.0.3/LdShell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3038 2024-05-12 02:02:40.753208 LdShell-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-2.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 02:02:40.753208 LdShell-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3767 2024-05-12 01:59:58.000000 LdShell-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:42:08.855738 LdShell-2.0.4/
+-rw-rw-rw-   0        0        0     1060 2024-05-15 00:27:20.000000 LdShell-2.0.4/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-15 04:42:08.839826 LdShell-2.0.4/LdShell/
+-rw-rw-rw-   0        0        0       20 2024-05-15 00:27:20.000000 LdShell-2.0.4/LdShell/__init__.py
+-rw-rw-rw-   0        0        0      352 2024-05-15 00:27:20.000000 LdShell-2.0.4/LdShell/__version__.py
+-rw-rw-rw-   0        0        0     9095 2024-05-15 04:41:16.000000 LdShell-2.0.4/LdShell/core.py
+-rw-rw-rw-   0        0        0      250 2024-05-15 00:27:20.000000 LdShell-2.0.4/LdShell/test.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:42:08.855738 LdShell-2.0.4/LdShell.egg-info/
+-rw-rw-rw-   0        0        0     3038 2024-05-15 04:42:08.000000 LdShell-2.0.4/LdShell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-15 04:42:08.000000 LdShell-2.0.4/LdShell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 04:42:08.000000 LdShell-2.0.4/LdShell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 04:42:08.000000 LdShell-2.0.4/LdShell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2024-05-15 00:27:20.000000 LdShell-2.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3038 2024-05-15 04:42:08.855738 LdShell-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2338 2024-05-15 00:27:20.000000 LdShell-2.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 04:42:08.855738 LdShell-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3767 2024-05-15 04:41:51.000000 LdShell-2.0.4/setup.py
```

### Comparing `LdShell-2.0.3/LICENSE` & `LdShell-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LdShell-2.0.3/LdShell/core.py` & `LdShell-2.0.4/LdShell/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         child=15
         Tap=16
         Checked=17
         LongCLick=18
         ListText=19
         ListLocal=20
         ALL=21
+        Code=22
+        Count=23
 class InitLdPlayer :
      index=0
      _debug=False
      def __init__(self, index=None,debug=False):
           InitLdPlayer.index=index
           InitLdPlayer._debug=debug
     
@@ -189,14 +191,23 @@
     def Text(self):
         return self.InistrPost(LdType.text)
 
     # 下面定义了一个 ALL 方法
     def ALL(self):
         return self.InistrPost(LdType.ALL)
     
+    # 下面定义了一个 Code 方法
+    def Code(self):
+        return self.InistrPost(LdType.Code)
+    
+    # 下面定义了一个 Code 方法
+    def Count(self):
+        return self.InistrPost(LdType.Count)
+    
+
     # 下面定义了一个 ListText 方法
     def ListText(self):
         return self.InistrPost(LdType.ListText)
     
     # 下面定义了一个 ListLocal 方法
     def ListLocal(self):
         return self.InistrPost(LdType.ListLocal)
```

### Comparing `LdShell-2.0.3/LdShell.egg-info/PKG-INFO` & `LdShell-2.0.4/LdShell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 2.0.3
+Version: 2.0.4
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-2.0.3/PKG-INFO` & `LdShell-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 2.0.3
+Version: 2.0.4
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-2.0.3/README.md` & `LdShell-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `LdShell-2.0.3/setup.py` & `LdShell-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'LdShell'
 DESCRIPTION = 'My short description for my project.'
 URL="http://www.google.com/"
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.0.3'
+VERSION = '2.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

