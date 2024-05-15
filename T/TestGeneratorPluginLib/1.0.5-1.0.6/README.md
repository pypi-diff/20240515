# Comparing `tmp/TestGeneratorPluginLib-1.0.5.tar.gz` & `tmp/TestGeneratorPluginLib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.0.5.tar", last modified: Wed May 15 12:15:51 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.0.6.tar", last modified: Wed May 15 14:21:11 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.0.5.tar` & `TestGeneratorPluginLib-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:15:51.715334 TestGeneratorPluginLib-1.0.5/
--rw-rw-rw-   0        0        0     1090 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-15 12:15:51.715334 TestGeneratorPluginLib-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 12:15:51.715334 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      288 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0     1707 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0     1780 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_language.py
--rw-rw-rw-   0        0        0     1219 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0     3064 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     3344 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:15:51.715334 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-15 12:15:51.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-05-15 12:15:51.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:15:51.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-15 12:15:51.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-15 12:15:51.000000 TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 12:15:51.715334 TestGeneratorPluginLib-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-15 12:15:07.000000 TestGeneratorPluginLib-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/
+-rw-rw-rw-   0        0        0     1090 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      288 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1780 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0     3101 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     3344 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/setup.py
```

### Comparing `TestGeneratorPluginLib-1.0.5/LICENSE` & `TestGeneratorPluginLib-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.5/PKG-INFO` & `TestGeneratorPluginLib-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.5
+Version: 1.0.6
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_language.py` & `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_language.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
         os.makedirs(build_path)
         os.makedirs(os.path.dirname(dist_path), exist_ok=True)
 
         for el in self._directories:
             shutil.copytree(el, os.path.join(build_path, el))
         shutil.copy(argv[0], os.path.join(build_path, os.path.basename(argv[0])))
 
-        subprocess.run(['pip', 'install', self._requirements, '-t', os.path.join(build_path, '__packages__')])
+        if self._requirements:
+            subprocess.run(['pip', 'install', *self._requirements, '-t', os.path.join(build_path, '__packages__')])
 
         with open(os.path.join(build_path, '__plugin__.py'), 'w', encoding='utf-8') as f:
             f.write(f"""from TestGeneratorPluginLib._built_plugin import BuiltPlugin
 from {os.path.basename(argv[0][:-3])} import plugin
 
 __plugin__ = BuiltPlugin(plugin, '{sys.platform}')
 """)
```

### Comparing `TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.5/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.5
+Version: 1.0.6
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.5/setup.py` & `TestGeneratorPluginLib-1.0.6/setup.py`

 * *Files identical despite different names*

