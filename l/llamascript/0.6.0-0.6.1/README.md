# Comparing `tmp/llamascript-0.6.0.tar.gz` & `tmp/llamascript-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamascript-0.6.0.tar", last modified: Wed May 15 15:13:27 2024, max compression
+gzip compressed data, was "llamascript-0.6.1.tar", last modified: Wed May 15 15:22:58 2024, max compression
```

## Comparing `llamascript-0.6.0.tar` & `llamascript-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-15 15:13:27.148214 llamascript-0.6.0/
--rw-r--r--   0 lewis-family   (501) staff       (20)    11324 2024-04-30 20:50:05.000000 llamascript-0.6.0/LICENSE
--rw-r--r--   0 lewis-family   (501) staff       (20)     3084 2024-05-15 15:13:27.147089 llamascript-0.6.0/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)     2620 2024-05-15 14:46:22.000000 llamascript-0.6.0/README.md
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-15 15:13:27.142538 llamascript-0.6.0/llamascript/
--rw-r--r--   0 lewis-family   (501) staff       (20)       42 2024-05-15 14:56:58.000000 llamascript-0.6.0/llamascript/__init__.py
--rw-r--r--   0 lewis-family   (501) staff       (20)     7270 2024-05-15 15:08:50.000000 llamascript-0.6.0/llamascript/lang.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-15 15:13:27.146188 llamascript-0.6.0/llamascript.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)     3084 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      282 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       53 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/entry_points.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/requires.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       12 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/top_level.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-05-15 15:13:27.148423 llamascript-0.6.0/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)      947 2024-05-15 15:11:10.000000 llamascript-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:22:58.351679 llamascript-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-15 15:22:49.000000 llamascript-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-15 15:22:58.351679 llamascript-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-15 15:22:49.000000 llamascript-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:22:58.351679 llamascript-0.6.1/llamascript/
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-15 15:22:49.000000 llamascript-0.6.1/llamascript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:22:58.351679 llamascript-0.6.1/llamascript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:22:58.351679 llamascript-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-15 15:22:49.000000 llamascript-0.6.1/setup.py
```

### Comparing `llamascript-0.6.0/LICENSE` & `llamascript-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llamascript-0.6.0/PKG-INFO` & `llamascript-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.6.0
+Version: 0.6.1
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,15 +63,16 @@
 ```llamascript
 IGNORE
 USE llama3
 PROMPT Hello, how are you?
 CHAT
 ```
 
-***Note:*** ***For more examples see [here.](examples/)***
+> [!NOTE]\
+> For more examples see [here.](examples/)
 
 You can then run LlamaScript with the following command:
 
 ```bash
 llamascript
 ```
```

### Comparing `llamascript-0.6.0/README.md` & `llamascript-0.6.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 ```llamascript
 IGNORE
 USE llama3
 PROMPT Hello, how are you?
 CHAT
 ```
 
-***Note:*** ***For more examples see [here.](examples/)***
+> [!NOTE]\
+> For more examples see [here.](examples/)
 
 You can then run LlamaScript with the following command:
 
 ```bash
 llamascript
 ```
```

### Comparing `llamascript-0.6.0/llamascript/lang.py` & `llamascript-0.6.1/llamascript/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__version__ = "0.6.1"
+
 import asyncio
 import ollama
 import logging
 import sys
 import subprocess
 import os
```

### Comparing `llamascript-0.6.0/llamascript.egg-info/PKG-INFO` & `llamascript-0.6.1/llamascript.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.6.0
+Version: 0.6.1
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,15 +63,16 @@
 ```llamascript
 IGNORE
 USE llama3
 PROMPT Hello, how are you?
 CHAT
 ```
 
-***Note:*** ***For more examples see [here.](examples/)***
+> [!NOTE]\
+> For more examples see [here.](examples/)
 
 You can then run LlamaScript with the following command:
 
 ```bash
 llamascript
 ```
```

### Comparing `llamascript-0.6.0/setup.py` & `llamascript-0.6.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     entry_points={
         "console_scripts": [
-            "llamascript=llamascript.lang:run",
+            "llamascript=llamascript:run",
         ],
     },
 )
```

