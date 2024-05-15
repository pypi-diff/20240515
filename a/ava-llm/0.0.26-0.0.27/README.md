# Comparing `tmp/ava_llm-0.0.26.tar.gz` & `tmp/ava_llm-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ava_llm-0.0.26.tar", last modified: Tue May 14 08:47:43 2024, max compression
+gzip compressed data, was "ava_llm-0.0.27.tar", last modified: Wed May 15 14:42:15 2024, max compression
```

## Comparing `ava_llm-0.0.26.tar` & `ava_llm-0.0.27.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.476608 ava_llm-0.0.26/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1066 2024-05-13 18:36:13.000000 ava_llm-0.0.26/LICENSE
--rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-14 08:47:43.476608 ava_llm-0.0.26/PKG-INFO
--rwxr-xr-x   0 mihai     (1000) mihai     (1000)      173 2024-05-13 19:06:40.000000 ava_llm-0.0.26/README.md
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.473608 ava_llm-0.0.26/ava_llm/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2024-05-13 07:38:09.000000 ava_llm-0.0.26/ava_llm/__init__.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.474608 ava_llm-0.0.26/ava_llm/conversations/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       99 2024-05-13 07:36:36.000000 ava_llm-0.0.26/ava_llm/conversations/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1084 2024-05-13 18:37:34.000000 ava_llm-0.0.26/ava_llm/conversations/buffer.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1245 2024-05-13 18:37:36.000000 ava_llm-0.0.26/ava_llm/conversations/chat_history.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     2338 2024-05-13 18:37:32.000000 ava_llm-0.0.26/ava_llm/conversations/chat_memory.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      851 2024-05-12 14:25:17.000000 ava_llm-0.0.26/ava_llm/conversations/memory.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.475608 ava_llm-0.0.26/ava_llm/conversations/messages/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2024-05-13 07:36:57.000000 ava_llm-0.0.26/ava_llm/conversations/messages/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      185 2024-05-13 18:37:40.000000 ava_llm-0.0.26/ava_llm/conversations/messages/ai.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      390 2024-05-13 14:34:08.000000 ava_llm-0.0.26/ava_llm/conversations/messages/base.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      192 2024-05-13 18:37:38.000000 ava_llm-0.0.26/ava_llm/conversations/messages/human.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.475608 ava_llm-0.0.26/ava_llm/handlers/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       42 2024-05-13 07:37:15.000000 ava_llm-0.0.26/ava_llm/handlers/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3292 2024-05-14 07:45:24.000000 ava_llm-0.0.26/ava_llm/handlers/meta.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3345 2024-05-14 07:13:22.000000 ava_llm-0.0.26/ava_llm/handlers/openai.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.475608 ava_llm-0.0.26/ava_llm/language_models/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       19 2024-05-13 07:35:56.000000 ava_llm-0.0.26/ava_llm/language_models/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     4762 2024-05-14 08:46:15.000000 ava_llm-0.0.26/ava_llm/language_models/llm.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.475608 ava_llm-0.0.26/ava_llm/prompts/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       44 2024-05-13 07:37:37.000000 ava_llm-0.0.26/ava_llm/prompts/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      620 2024-05-10 11:43:12.000000 ava_llm-0.0.26/ava_llm/prompts/base.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      466 2024-05-13 18:37:41.000000 ava_llm-0.0.26/ava_llm/prompts/template.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.476608 ava_llm-0.0.26/ava_llm/utils/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       21 2024-05-13 07:38:00.000000 ava_llm-0.0.26/ava_llm/utils/__init__.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1438 2024-05-13 18:37:37.000000 ava_llm-0.0.26/ava_llm/utils/utils.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 08:47:43.476608 ava_llm-0.0.26/ava_llm.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-14 08:47:43.000000 ava_llm-0.0.26/ava_llm.egg-info/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)      809 2024-05-14 08:47:43.000000 ava_llm-0.0.26/ava_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-14 08:47:43.000000 ava_llm-0.0.26/ava_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       26 2024-05-14 08:47:43.000000 ava_llm-0.0.26/ava_llm.egg-info/requires.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        8 2024-05-14 08:47:43.000000 ava_llm-0.0.26/ava_llm.egg-info/top_level.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-14 08:47:43.476608 ava_llm-0.0.26/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)      476 2024-05-14 08:46:31.000000 ava_llm-0.0.26/setup.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.933242 ava_llm-0.0.27/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1066 2024-05-13 18:36:13.000000 ava_llm-0.0.27/LICENSE
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-15 14:42:15.933242 ava_llm-0.0.27/PKG-INFO
+-rwxr-xr-x   0 mihai     (1000) mihai     (1000)      173 2024-05-13 19:06:40.000000 ava_llm-0.0.27/README.md
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.930242 ava_llm-0.0.27/ava_llm/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2024-05-13 07:38:09.000000 ava_llm-0.0.27/ava_llm/__init__.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.931242 ava_llm-0.0.27/ava_llm/conversations/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       99 2024-05-13 07:36:36.000000 ava_llm-0.0.27/ava_llm/conversations/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1084 2024-05-13 18:37:34.000000 ava_llm-0.0.27/ava_llm/conversations/buffer.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1245 2024-05-13 18:37:36.000000 ava_llm-0.0.27/ava_llm/conversations/chat_history.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     2338 2024-05-13 18:37:32.000000 ava_llm-0.0.27/ava_llm/conversations/chat_memory.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      851 2024-05-12 14:25:17.000000 ava_llm-0.0.27/ava_llm/conversations/memory.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.931242 ava_llm-0.0.27/ava_llm/conversations/messages/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2024-05-13 07:36:57.000000 ava_llm-0.0.27/ava_llm/conversations/messages/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      185 2024-05-13 18:37:40.000000 ava_llm-0.0.27/ava_llm/conversations/messages/ai.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      439 2024-05-15 14:38:58.000000 ava_llm-0.0.27/ava_llm/conversations/messages/base.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      192 2024-05-13 18:37:38.000000 ava_llm-0.0.27/ava_llm/conversations/messages/human.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.931242 ava_llm-0.0.27/ava_llm/handlers/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       42 2024-05-13 07:37:15.000000 ava_llm-0.0.27/ava_llm/handlers/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3292 2024-05-14 07:45:24.000000 ava_llm-0.0.27/ava_llm/handlers/meta.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3345 2024-05-14 07:13:22.000000 ava_llm-0.0.27/ava_llm/handlers/openai.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.932242 ava_llm-0.0.27/ava_llm/language_models/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       19 2024-05-13 07:35:56.000000 ava_llm-0.0.27/ava_llm/language_models/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     4762 2024-05-14 08:46:15.000000 ava_llm-0.0.27/ava_llm/language_models/llm.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.932242 ava_llm-0.0.27/ava_llm/prompts/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       44 2024-05-13 07:37:37.000000 ava_llm-0.0.27/ava_llm/prompts/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      620 2024-05-10 11:43:12.000000 ava_llm-0.0.27/ava_llm/prompts/base.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      466 2024-05-13 18:37:41.000000 ava_llm-0.0.27/ava_llm/prompts/template.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.932242 ava_llm-0.0.27/ava_llm/utils/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       21 2024-05-13 07:38:00.000000 ava_llm-0.0.27/ava_llm/utils/__init__.py
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1438 2024-05-13 18:37:37.000000 ava_llm-0.0.27/ava_llm/utils/utils.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-15 14:42:15.932242 ava_llm-0.0.27/ava_llm.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      339 2024-05-15 14:42:15.000000 ava_llm-0.0.27/ava_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      809 2024-05-15 14:42:15.000000 ava_llm-0.0.27/ava_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-15 14:42:15.000000 ava_llm-0.0.27/ava_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       26 2024-05-15 14:42:15.000000 ava_llm-0.0.27/ava_llm.egg-info/requires.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        8 2024-05-15 14:42:15.000000 ava_llm-0.0.27/ava_llm.egg-info/top_level.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-15 14:42:15.933242 ava_llm-0.0.27/setup.cfg
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      476 2024-05-15 14:41:55.000000 ava_llm-0.0.27/setup.py
```

### Comparing `ava_llm-0.0.26/LICENSE` & `ava_llm-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/conversations/buffer.py` & `ava_llm-0.0.27/ava_llm/conversations/buffer.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/conversations/chat_history.py` & `ava_llm-0.0.27/ava_llm/conversations/chat_history.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/conversations/chat_memory.py` & `ava_llm-0.0.27/ava_llm/conversations/chat_memory.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/conversations/memory.py` & `ava_llm-0.0.27/ava_llm/conversations/memory.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/handlers/meta.py` & `ava_llm-0.0.27/ava_llm/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/handlers/openai.py` & `ava_llm-0.0.27/ava_llm/handlers/openai.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/language_models/llm.py` & `ava_llm-0.0.27/ava_llm/language_models/llm.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/prompts/base.py` & `ava_llm-0.0.27/ava_llm/prompts/base.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm/utils/utils.py` & `ava_llm-0.0.27/ava_llm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ava_llm-0.0.26/ava_llm.egg-info/SOURCES.txt` & `ava_llm-0.0.27/ava_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

