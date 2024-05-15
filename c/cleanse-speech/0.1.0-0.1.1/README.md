# Comparing `tmp/cleanse_speech-0.1.0.tar.gz` & `tmp/cleanse_speech-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanse_speech-0.1.0.tar", last modified: Tue May 14 17:18:45 2024, max compression
+gzip compressed data, was "cleanse_speech-0.1.1.tar", last modified: Tue May 14 17:31:04 2024, max compression
```

## Comparing `cleanse_speech-0.1.0.tar` & `cleanse_speech-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rwxr-xr-x   0        0        0     1065 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/LICENSE
--rwxr-xr-x   0        0        0       94 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/NOTICE.MD
--rwxr-xr-x   0        0        0      992 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/README.md
--rw-r--r--   0        0        0      556 2024-05-14 17:18:45.783217 cleanse_speech-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       98 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/src/cleanse-speech/__init__.py
--rw-r--r--   0        0        0     2957 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_advertisement.bin
--rw-r--r--   0        0        0     9075 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_general.bin
--rw-r--r--   0        0        0    92572 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_netease.bin
--rw-r--r--   0        0        0     5134 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_politics.bin
--rw-r--r--   0        0        0     4224 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_pornographic.bin
--rw-r--r--   0        0        0     1002 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/src/cleanse-speech/bookshelf.py
--rw-r--r--   0        0        0     7087 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/src/cleanse-speech/dlfa.py
--rwxr-xr-x   0        0        0        3 2024-05-14 17:18:33.795215 cleanse_speech-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 cleanse_speech-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1065 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0       94 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/NOTICE.MD
+-rwxr-xr-x   0        0        0      992 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/README.md
+-rw-r--r--   0        0        0      556 2024-05-14 17:31:04.676538 cleanse_speech-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/src/cleanse_speech/__init__.py
+-rw-r--r--   0        0        0     2957 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_advertisement.bin
+-rw-r--r--   0        0        0     9075 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_general.bin
+-rw-r--r--   0        0        0    92572 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_netease.bin
+-rw-r--r--   0        0        0     5134 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_politics.bin
+-rw-r--r--   0        0        0     4224 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_pornographic.bin
+-rw-r--r--   0        0        0     1002 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bookshelf.py
+-rw-r--r--   0        0        0     7087 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/dlfa.py
+-rwxr-xr-x   0        0        0        0 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/tests/test_dfa.py
+-rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 cleanse_speech-0.1.1/PKG-INFO
```

### Comparing `cleanse_speech-0.1.0/LICENSE` & `cleanse_speech-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.0/README.md` & `cleanse_speech-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+Metadata-Version: 2.1
+Name: cleanse-speech
+Version: 0.1.1
+Summary: An intelligent Python library designed to detect and filter offensive language, ensuring respectful and constructive communication in any digital space.
+Author-Email: llmkira <me@dianas.cyou>
+License: MIT
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # cleanse-speech 🚀
 
-[![PyPI version](https://badge.fury.io/py/cleanse-speech.svg)](https://badge.fury.io/py/cleanse-speech)
-[![Downloads](https://pepy.tech/badge/cleanse-speech)](https://pepy.tech/project/cleanse-speech)
-[![Downloads](https://pepy.tech/badge/cleanse-speech/month)](https://pepy.tech/project/cleanse-speech)
+[![PyPI version](https://badge.fury.io/py/cleanse_speech.svg)](https://badge.fury.io/py/cleanse_speech)
+[![Downloads](https://pepy.tech/badge/cleanse_speech)](https://pepy.tech/project/cleanse_speech)
+[![Downloads](https://pepy.tech/badge/cleanse_speech/month)](https://pepy.tech/project/cleanse_speech)
 
 Python🐍 3.9+ support. 
 
 
 
 ```shell
 pip install cleanse-speech
```

### Comparing `cleanse_speech-0.1.0/pyproject.toml` & `cleanse_speech-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cleanse-speech"
-version = "0.1.0"
+version = "0.1.1"
 description = "An intelligent Python library designed to detect and filter offensive language, ensuring respectful and constructive communication in any digital space."
 authors = [
     { name = "llmkira", email = "me@dianas.cyou" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_advertisement.bin` & `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_advertisement.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_general.bin` & `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_general.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_netease.bin` & `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_netease.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_politics.bin` & `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_politics.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.0/src/cleanse-speech/bin/cn_pornographic.bin` & `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_pornographic.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.0/src/cleanse-speech/bookshelf.py` & `cleanse_speech-0.1.1/src/cleanse_speech/bookshelf.py`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.0/src/cleanse-speech/dlfa.py` & `cleanse_speech-0.1.1/src/cleanse_speech/dlfa.py`

 * *Files identical despite different names*

