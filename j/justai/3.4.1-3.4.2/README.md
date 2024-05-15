# Comparing `tmp/justai-3.4.1.tar.gz` & `tmp/justai-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justai-3.4.1.tar", last modified: Tue May  7 11:14:38 2024, max compression
+gzip compressed data, was "justai-3.4.2.tar", last modified: Wed May 15 18:34:58 2024, max compression
```

## Comparing `justai-3.4.1.tar` & `justai-3.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 11:14:38.783425 justai-3.4.1/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.4.1/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.4.1/MANIFEST.in
--rw-r--r--   0 hp         (501) staff       (20)     6472 2024-05-07 11:14:38.783233 justai-3.4.1/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     4082 2024-05-07 11:14:37.000000 justai-3.4.1/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 11:14:38.776677 justai-3.4.1/justai/
--rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.4.1/justai/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 11:14:38.777977 justai-3.4.1/justai/agent/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.4.1/justai/agent/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     6234 2024-05-07 08:29:10.000000 justai-3.4.1/justai/agent/agent.py
--rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.4.1/justai/agent/message.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 11:14:38.778560 justai-3.4.1/justai/interactive/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.4.1/justai/interactive/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.4.1/justai/interactive/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.4.1/justai/interactive/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 11:14:38.779856 justai-3.4.1/justai/models/
--rw-r--r--   0 hp         (501) staff       (20)     4055 2024-05-07 08:44:49.000000 justai-3.4.1/justai/models/anthropic_models.py
--rw-r--r--   0 hp         (501) staff       (20)     2465 2024-05-02 08:28:02.000000 justai-3.4.1/justai/models/gguf_models.py
--rw-r--r--   0 hp         (501) staff       (20)     1009 2024-05-07 08:29:10.000000 justai-3.4.1/justai/models/model.py
--rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.4.1/justai/models/modelfactory.py
--rw-r--r--   0 hp         (501) staff       (20)     6242 2024-05-07 08:33:08.000000 justai-3.4.1/justai/models/openai_models.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 11:14:38.781040 justai-3.4.1/justai/tools/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.4.1/justai/tools/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.4.1/justai/tools/cache.py
--rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.4.1/justai/tools/display.py
--rw-r--r--   0 hp         (501) staff       (20)     3479 2024-04-29 12:34:52.000000 justai-3.4.1/justai/tools/log.py
--rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.4.1/justai/tools/prompts.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 11:14:38.782276 justai-3.4.1/justai/translator/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.4.1/justai/translator/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.4.1/justai/translator/languages.py
--rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.4.1/justai/translator/prompts.toml
--rw-r--r--   0 hp         (501) staff       (20)    16685 2024-05-05 14:41:25.000000 justai-3.4.1/justai/translator/translator.py
--rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.4.1/justai/translator/xliff.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-07 11:14:38.782690 justai-3.4.1/justai.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     6472 2024-05-07 11:14:38.000000 justai-3.4.1/justai.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      785 2024-05-07 11:14:38.000000 justai-3.4.1/justai.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2024-05-07 11:14:38.000000 justai-3.4.1/justai.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      155 2024-05-07 11:14:38.000000 justai-3.4.1/justai.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        7 2024-05-07 11:14:38.000000 justai-3.4.1/justai.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)      910 2024-05-07 11:14:37.000000 justai-3.4.1/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2024-05-07 11:14:38.783463 justai-3.4.1/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-15 18:34:58.263155 justai-3.4.2/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.4.2/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.4.2/MANIFEST.in
+-rw-r--r--   0 hp         (501) staff       (20)     6472 2024-05-15 18:34:58.262951 justai-3.4.2/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     4082 2024-05-15 18:34:56.000000 justai-3.4.2/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-15 18:34:58.255728 justai-3.4.2/justai/
+-rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.4.2/justai/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-15 18:34:58.257154 justai-3.4.2/justai/agent/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.4.2/justai/agent/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     6234 2024-05-07 08:29:10.000000 justai-3.4.2/justai/agent/agent.py
+-rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.4.2/justai/agent/message.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-15 18:34:58.257845 justai-3.4.2/justai/interactive/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.4.2/justai/interactive/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.4.2/justai/interactive/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.4.2/justai/interactive/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-15 18:34:58.259309 justai-3.4.2/justai/models/
+-rw-r--r--   0 hp         (501) staff       (20)     4055 2024-05-07 08:44:49.000000 justai-3.4.2/justai/models/anthropic_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     2465 2024-05-02 08:28:02.000000 justai-3.4.2/justai/models/gguf_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     1009 2024-05-07 08:29:10.000000 justai-3.4.2/justai/models/model.py
+-rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.4.2/justai/models/modelfactory.py
+-rw-r--r--   0 hp         (501) staff       (20)     6242 2024-05-07 08:33:08.000000 justai-3.4.2/justai/models/openai_models.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-15 18:34:58.260603 justai-3.4.2/justai/tools/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.4.2/justai/tools/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.4.2/justai/tools/cache.py
+-rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.4.2/justai/tools/display.py
+-rw-r--r--   0 hp         (501) staff       (20)     3479 2024-04-29 12:34:52.000000 justai-3.4.2/justai/tools/log.py
+-rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.4.2/justai/tools/prompts.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-15 18:34:58.261914 justai-3.4.2/justai/translator/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.4.2/justai/translator/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.4.2/justai/translator/languages.py
+-rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.4.2/justai/translator/prompts.toml
+-rw-r--r--   0 hp         (501) staff       (20)    16740 2024-05-15 18:33:00.000000 justai-3.4.2/justai/translator/translator.py
+-rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.4.2/justai/translator/xliff.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-15 18:34:58.262335 justai-3.4.2/justai.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     6472 2024-05-15 18:34:58.000000 justai-3.4.2/justai.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      785 2024-05-15 18:34:58.000000 justai-3.4.2/justai.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2024-05-15 18:34:58.000000 justai-3.4.2/justai.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      155 2024-05-15 18:34:58.000000 justai-3.4.2/justai.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        7 2024-05-15 18:34:58.000000 justai-3.4.2/justai.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)      910 2024-05-15 18:34:56.000000 justai-3.4.2/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2024-05-15 18:34:58.263193 justai-3.4.2/setup.cfg
```

### Comparing `justai-3.4.1/LICENSE` & `justai-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/PKG-INFO` & `justai-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.4.1
+Version: 3.4.2
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -55,15 +55,15 @@
 Requires-Dist: llama-cpp-python; extra == "llama"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.4.1
+Current version: 3.4.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.4.1/README.md` & `justai-3.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.4.1
+Current version: 3.4.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.4.1/justai/__init__.py` & `justai-3.4.2/justai/__init__.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/agent/agent.py` & `justai-3.4.2/justai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/agent/message.py` & `justai-3.4.2/justai/agent/message.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/interactive/commands.py` & `justai-3.4.2/justai/interactive/commands.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/interactive/repl.py` & `justai-3.4.2/justai/interactive/repl.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/models/anthropic_models.py` & `justai-3.4.2/justai/models/anthropic_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/models/gguf_models.py` & `justai-3.4.2/justai/models/gguf_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/models/model.py` & `justai-3.4.2/justai/models/model.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/models/modelfactory.py` & `justai-3.4.2/justai/models/modelfactory.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/models/openai_models.py` & `justai-3.4.2/justai/models/openai_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/tools/cache.py` & `justai-3.4.2/justai/tools/cache.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/tools/display.py` & `justai-3.4.2/justai/tools/display.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/tools/log.py` & `justai-3.4.2/justai/tools/log.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/tools/prompts.py` & `justai-3.4.2/justai/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/translator/languages.py` & `justai-3.4.2/justai/translator/languages.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/translator/prompts.toml` & `justai-3.4.2/justai/translator/prompts.toml`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai/translator/translator.py` & `justai-3.4.2/justai/translator/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,14 +304,17 @@
         key = self.get_key(source)
         self.cache[key] = translation
 
     def __contains__(self, source):
         key = self.get_key(source)
         return key in self.cache
 
+    def __len__(self):
+        return len(self.cache)
+
     def update(self, translation_dict):
         for source, translation in translation_dict.items():
             self.set(source, translation)
 
     def save(self):
         with open(self.file, 'wb') as f:
             pickle.dump(self.cache, f)
```

### Comparing `justai-3.4.1/justai/translator/xliff.py` & `justai-3.4.2/justai/translator/xliff.py`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/justai.egg-info/PKG-INFO` & `justai-3.4.2/justai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.4.1
+Version: 3.4.2
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -55,15 +55,15 @@
 Requires-Dist: llama-cpp-python; extra == "llama"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.4.1
+Current version: 3.4.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.4.1/justai.egg-info/SOURCES.txt` & `justai-3.4.2/justai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `justai-3.4.1/pyproject.toml` & `justai-3.4.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=69", "wheel>=0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "justai"
-version = "3.4.1"
+version = "3.4.2"
 description = "Makes working with OpenAI's GPT API and other LLM's super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

