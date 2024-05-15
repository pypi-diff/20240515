# Comparing `tmp/fazah-3.27.tar.gz` & `tmp/fazah-3.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazah-3.27.tar", last modified: Sat May 11 19:22:50 2024, max compression
+gzip compressed data, was "fazah-3.29.tar", last modified: Wed May 15 04:29:08 2024, max compression
```

## Comparing `fazah-3.27.tar` & `fazah-3.29.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-11 19:22:50.889044 fazah-3.27/
-drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-11 19:22:50.887585 fazah-3.27/Fazah/
--rw-r--r--   0 will       (501) staff       (20)       30 2024-05-11 19:19:48.000000 fazah-3.27/Fazah/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     1219 2024-05-11 19:19:43.000000 fazah-3.27/Fazah/fazahclass.py
--rw-r--r--   0 will       (501) staff       (20)      308 2024-05-11 19:22:50.888920 fazah-3.27/PKG-INFO
-drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-11 19:22:50.888462 fazah-3.27/fazah.egg-info/
--rw-r--r--   0 will       (501) staff       (20)      308 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)      232 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/SOURCES.txt
--rw-r--r--   0 will       (501) staff       (20)        1 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/dependency_links.txt
--rw-r--r--   0 will       (501) staff       (20)       27 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/requires.txt
--rw-r--r--   0 will       (501) staff       (20)        6 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/top_level.txt
--rw-r--r--   0 will       (501) staff       (20)       38 2024-05-11 19:22:50.889100 fazah-3.27/setup.cfg
--rw-r--r--   0 will       (501) staff       (20)      496 2024-05-11 19:22:26.000000 fazah-3.27/setup.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-11 19:22:50.888739 fazah-3.27/tests/
--rw-r--r--   0 will       (501) staff       (20)     1218 2024-05-03 22:27:31.000000 fazah-3.27/tests/test.openai.py
--rw-r--r--   0 will       (501) staff       (20)     1320 2024-05-11 19:21:49.000000 fazah-3.27/tests/test_gemini.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-15 04:29:08.891991 fazah-3.29/
+drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-15 04:29:08.888919 fazah-3.29/Fazah/
+-rw-r--r--   0 will       (501) staff       (20)       30 2024-05-11 19:19:48.000000 fazah-3.29/Fazah/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     1219 2024-05-15 04:19:23.000000 fazah-3.29/Fazah/fazahclass.py
+-rw-r--r--   0 will       (501) staff       (20)     4236 2024-05-15 04:29:08.891722 fazah-3.29/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)     4064 2024-05-15 04:17:15.000000 fazah-3.29/README.md
+drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-15 04:29:08.890571 fazah-3.29/fazah.egg-info/
+-rw-r--r--   0 will       (501) staff       (20)     4236 2024-05-15 04:29:08.000000 fazah-3.29/fazah.egg-info/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)      280 2024-05-15 04:29:08.000000 fazah-3.29/fazah.egg-info/SOURCES.txt
+-rw-r--r--   0 will       (501) staff       (20)        1 2024-05-15 04:29:08.000000 fazah-3.29/fazah.egg-info/dependency_links.txt
+-rw-r--r--   0 will       (501) staff       (20)       27 2024-05-15 04:29:08.000000 fazah-3.29/fazah.egg-info/requires.txt
+-rw-r--r--   0 will       (501) staff       (20)        6 2024-05-15 04:29:08.000000 fazah-3.29/fazah.egg-info/top_level.txt
+-rw-r--r--   0 will       (501) staff       (20)       38 2024-05-15 04:29:08.892044 fazah-3.29/setup.cfg
+-rw-r--r--   0 will       (501) staff       (20)      408 2024-05-15 04:20:29.000000 fazah-3.29/setup.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-15 04:29:08.891420 fazah-3.29/tests/
+-rw-r--r--   0 will       (501) staff       (20)     1218 2024-05-03 22:27:31.000000 fazah-3.29/tests/test.openai.py
+-rw-r--r--   0 will       (501) staff       (20)     1320 2024-05-15 04:06:07.000000 fazah-3.29/tests/test_gemini.py
```

### Comparing `fazah-3.27/Fazah/fazahclass.py` & `fazah-3.29/Fazah/fazahclass.py`

 * *Files identical despite different names*

### Comparing `fazah-3.27/tests/test.openai.py` & `fazah-3.29/tests/test.openai.py`

 * *Files identical despite different names*

### Comparing `fazah-3.27/tests/test_gemini.py` & `fazah-3.29/tests/test_gemini.py`

 * *Files identical despite different names*

