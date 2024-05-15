# Comparing `tmp/utils_ai_nuuuwan-1.0.2.tar.gz` & `tmp/utils_ai_nuuuwan-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_ai_nuuuwan-1.0.2.tar", last modified: Wed May 15 06:45:33 2024, max compression
+gzip compressed data, was "utils_ai_nuuuwan-1.0.3.tar", last modified: Wed May 15 07:24:41 2024, max compression
```

## Comparing `utils_ai_nuuuwan-1.0.2.tar` & `utils_ai_nuuuwan-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.704371 utils_ai_nuuuwan-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.704371 utils_ai_nuuuwan-1.0.2/src/utils_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.704371 utils_ai_nuuuwan-1.0.2/src/utils_ai/apps/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/apps/ChatApp.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.704371 utils_ai_nuuuwan-1.0.2/src/utils_ai/core/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/core/ChatRole.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/core/Message.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/GenericAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/GenericAIImage.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/GenericAIText.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/MistralAIProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/OpenAIProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/ProviderFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 06:45:09.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:33.708371 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 06:45:33.000000 utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:41.420702 utils_ai_nuuuwan-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 07:24:41.420702 utils_ai_nuuuwan-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:24:41.420702 utils_ai_nuuuwan-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:41.416702 utils_ai_nuuuwan-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:41.416702 utils_ai_nuuuwan-1.0.3/src/utils_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:41.416702 utils_ai_nuuuwan-1.0.3/src/utils_ai/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/apps/ChatApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:41.416702 utils_ai_nuuuwan-1.0.3/src/utils_ai/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/core/ChatRole.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/core/Message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:41.420702 utils_ai_nuuuwan-1.0.3/src/utils_ai/generic_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/generic_ai/GenericAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/generic_ai/GenericAIImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/generic_ai/GenericAIText.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/generic_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:41.420702 utils_ai_nuuuwan-1.0.3/src/utils_ai/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/providers/MistralAIProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/providers/OpenAIProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/providers/ProviderFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 07:24:13.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:41.420702 utils_ai_nuuuwan-1.0.3/src/utils_ai_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 07:24:41.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 07:24:41.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:24:41.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 07:24:41.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 07:24:41.000000 utils_ai_nuuuwan-1.0.3/src/utils_ai_nuuuwan.egg-info/top_level.txt
```

### Comparing `utils_ai_nuuuwan-1.0.2/LICENSE` & `utils_ai_nuuuwan-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.2/PKG-INFO` & `utils_ai_nuuuwan-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_ai-nuuuwan
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utilities with AI support
 Home-page: https://github.com/nuuuwan/utils_ai
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_ai_nuuuwan-1.0.2/setup.py` & `utils_ai_nuuuwan-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils_ai'
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 DESCRIPTION = "Utilities with AI support"
 INSTALL_REQUIRES = [
     'utils_base-nuuuwan',
     'utils_www-nuuuwan',
     'openai',
     'mistralai',
 ]
```

### Comparing `utils_ai_nuuuwan-1.0.2/src/utils_ai/apps/ChatApp.py` & `utils_ai_nuuuwan-1.0.3/src/utils_ai/apps/ChatApp.py`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/GenericAIImage.py` & `utils_ai_nuuuwan-1.0.3/src/utils_ai/generic_ai/GenericAIImage.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from utils_base import Log, Hash
 from utils_www import WWW
 
 log = Log('GenericAIImage')
 
 
 class GenericAIImage:
-    DIR_DESKTOP = os.environ['DIR_DESKTOP'] 
+    DIR_DESKTOP = os.environ.get('DIR_DESKTOP') 
     def get_image_url(self, prompt: str) -> str:
         raise NotImplementedError
 
     def draw(self, prompt: str):
         h = Hash.md5(prompt)[:8]
         image_path = os.path.join(GenericAIImage.DIR_DESKTOP, f'{h}.png')
         if os.path.exists(image_path):
```

### Comparing `utils_ai_nuuuwan-1.0.2/src/utils_ai/generic_ai/GenericAIText.py` & `utils_ai_nuuuwan-1.0.3/src/utils_ai/generic_ai/GenericAIText.py`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/MistralAIProvider.py` & `utils_ai_nuuuwan-1.0.3/src/utils_ai/providers/MistralAIProvider.py`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/OpenAIProvider.py` & `utils_ai_nuuuwan-1.0.3/src/utils_ai/providers/OpenAIProvider.py`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.2/src/utils_ai/providers/ProviderFactory.py` & `utils_ai_nuuuwan-1.0.3/src/utils_ai/providers/ProviderFactory.py`

 * *Files identical despite different names*

### Comparing `utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/PKG-INFO` & `utils_ai_nuuuwan-1.0.3/src/utils_ai_nuuuwan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_ai-nuuuwan
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utilities with AI support
 Home-page: https://github.com/nuuuwan/utils_ai
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_ai_nuuuwan-1.0.2/src/utils_ai_nuuuwan.egg-info/SOURCES.txt` & `utils_ai_nuuuwan-1.0.3/src/utils_ai_nuuuwan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

