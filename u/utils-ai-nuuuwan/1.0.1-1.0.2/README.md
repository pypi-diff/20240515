# Comparing `tmp/utils_ai_nuuuwan-1.0.1.tar.gz` & `tmp/utils_ai_nuuuwan-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_ai_nuuuwan-1.0.1.tar", last modified: Wed May 15 05:20:41 2024, max compression
+gzip compressed data, was "utils_ai_nuuuwan-1.0.2.tar", last modified: Wed May 15 06:45:33 2024, max compression
```

## Comparing `utils_ai_nuuuwan-1.0.1.tar` & `utils_ai_nuuuwan-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/src/utils_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/src/utils_ai/core/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/core/ChatRole.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/core/Message.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/src/utils_ai/generic_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/generic_ai/GenericAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/generic_ai/GenericAIImage.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/generic_ai/GenericAIText.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/generic_ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/src/utils_ai/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/providers/MistralAIProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/providers/OpenAIProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/providers/ProviderFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 05:18:40.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:20:41.982375 utils_ai_nuuuwan-1.0.1/src/utils_ai_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-15 05:20:41.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-15 05:20:41.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 05:20:41.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 05:20:41.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 05:20:41.000000 utils_ai_nuuuwan-1.0.1/src/utils_ai_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.704371 utils_ai_nuuuwan-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.704371 utils_ai_nuuuwan-1.0.2/src/utils_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.704371 utils_ai_nuuuwan-1.0.2/src/utils_ai/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/apps/ChatApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.704371 utils_ai_nuuuwan-1.0.2/src/utils_ai/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/core/ChatRole.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/core/Message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/GenericAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/GenericAIImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/GenericAIText.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/MistralAIProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/OpenAIProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/ProviderFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/top_level.txt
```

### Comparing `utils_ai_nuuuwan-1.0.1/LICENSE` & `utils_ai_nuuuwan-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.1/PKG-INFO` & `utils_ai_nuuuwan-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: utils_ai-nuuuwan
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities with AI support
 Home-page: https://github.com/nuuuwan/utils_ai
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: utils_base-nuuuwan
 Requires-Dist: utils_www-nuuuwan
 Requires-Dist: openai
-Requires-Dist: mistral
+Requires-Dist: mistralai
```

### Comparing `utils_ai_nuuuwan-1.0.1/setup.py` & `utils_ai_nuuuwan-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils_ai'
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "Utilities with AI support"
 INSTALL_REQUIRES = [
     'utils_base-nuuuwan',
     'utils_www-nuuuwan',
     'openai',
-    'mistral',
+    'mistralai',
 ]
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
     description=DESCRIPTION,
```

### Comparing `utils_ai_nuuuwan-1.0.1/src/utils_ai/providers/MistralAIProvider.py` & `utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/MistralAIProvider.py`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.1/src/utils_ai/providers/OpenAIProvider.py` & `utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/OpenAIProvider.py`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.1/src/utils_ai/providers/ProviderFactory.py` & `utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/ProviderFactory.py`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.1/src/utils_ai_nuuuwan.egg-info/PKG-INFO` & `utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: utils_ai-nuuuwan
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities with AI support
 Home-page: https://github.com/nuuuwan/utils_ai
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: utils_base-nuuuwan
 Requires-Dist: utils_www-nuuuwan
 Requires-Dist: openai
-Requires-Dist: mistral
+Requires-Dist: mistralai
```

### Comparing `utils_ai_nuuuwan-1.0.1/src/utils_ai_nuuuwan.egg-info/SOURCES.txt` & `utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 README.md
 setup.py
 src/utils_ai/__init__.py
+src/utils_ai/apps/ChatApp.py
+src/utils_ai/apps/__init__.py
 src/utils_ai/core/ChatRole.py
 src/utils_ai/core/Message.py
 src/utils_ai/core/__init__.py
 src/utils_ai/generic_ai/GenericAI.py
 src/utils_ai/generic_ai/GenericAIImage.py
 src/utils_ai/generic_ai/GenericAIText.py
 src/utils_ai/generic_ai/__init__.py
```

