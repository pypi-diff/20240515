# Comparing `tmp/cleanse_speech-0.1.1.tar.gz` & `tmp/cleanse_speech-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanse_speech-0.1.1.tar", last modified: Tue May 14 17:31:04 2024, max compression
+gzip compressed data, was "cleanse_speech-0.1.2.tar", last modified: Wed May 15 00:52:46 2024, max compression
```

## Comparing `cleanse_speech-0.1.1.tar` & `cleanse_speech-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1065 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/LICENSE
--rwxr-xr-x   0        0        0       94 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/NOTICE.MD
--rwxr-xr-x   0        0        0      992 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/README.md
--rw-r--r--   0        0        0      556 2024-05-14 17:31:04.676538 cleanse_speech-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      100 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/src/cleanse_speech/__init__.py
--rw-r--r--   0        0        0     2957 2024-05-14 17:30:52.460575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_advertisement.bin
--rw-r--r--   0        0        0     9075 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_general.bin
--rw-r--r--   0        0        0    92572 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_netease.bin
--rw-r--r--   0        0        0     5134 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_politics.bin
--rw-r--r--   0        0        0     4224 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_pornographic.bin
--rw-r--r--   0        0        0     1002 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/bookshelf.py
--rw-r--r--   0        0        0     7087 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/src/cleanse_speech/dlfa.py
--rwxr-xr-x   0        0        0        0 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      665 2024-05-14 17:30:52.464575 cleanse_speech-0.1.1/tests/test_dfa.py
--rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 cleanse_speech-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1065 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0       94 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/NOTICE.MD
+-rwxr-xr-x   0        0        0     1522 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/README.md
+-rw-r--r--   0        0        0      556 2024-05-15 00:52:46.510141 cleanse_speech-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/src/cleanse_speech/__init__.py
+-rw-r--r--   0        0        0     2956 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_advertisement.bin
+-rw-r--r--   0        0        0     9075 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_general.bin
+-rw-r--r--   0        0        0    92572 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_netease.bin
+-rw-r--r--   0        0        0     5134 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_politics.bin
+-rw-r--r--   0        0        0     4224 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_pornographic.bin
+-rw-r--r--   0        0        0     1002 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/src/cleanse_speech/bookshelf.py
+-rw-r--r--   0        0        0     7095 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/src/cleanse_speech/dlfa.py
+-rwxr-xr-x   0        0        0        0 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-15 00:52:26.041947 cleanse_speech-0.1.2/tests/test_dfa.py
+-rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 cleanse_speech-0.1.2/PKG-INFO
```

### Comparing `cleanse_speech-0.1.1/LICENSE` & `cleanse_speech-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.1/pyproject.toml` & `cleanse_speech-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cleanse-speech"
-version = "0.1.1"
+version = "0.1.2"
 description = "An intelligent Python library designed to detect and filter offensive language, ensuring respectful and constructive communication in any digital space."
 authors = [
     { name = "llmkira", email = "me@dianas.cyou" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_advertisement.bin` & `cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_advertisement.bin`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -170,8 +170,8 @@
 56ef5b6u5L+hCg==
 56efd3gK
 5Luj5LuYCg==
 5aSn6YeP5pS2Cg==
 5Y2W5pSv5LuY5a6dCg==
 5LiK5Y+35ZmoCg==
 5Luj5Y+RCg==
-5byV5rWB
+5byV5rWB
```

### Comparing `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_general.bin` & `cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_general.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_netease.bin` & `cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_netease.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_politics.bin` & `cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_politics.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.1/src/cleanse_speech/bin/cn_pornographic.bin` & `cleanse_speech-0.1.2/src/cleanse_speech/bin/cn_pornographic.bin`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.1/src/cleanse_speech/bookshelf.py` & `cleanse_speech-0.1.2/src/cleanse_speech/bookshelf.py`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.1/src/cleanse_speech/dlfa.py` & `cleanse_speech-0.1.2/src/cleanse_speech/dlfa.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         else:
             words = words_resource
         for word in words:
             word = word.strip()
             if word:
                 try:
                     decoded_word = base64.b64decode(word).decode('utf-8')
-                    word_to_add = decoded_word
+                    word_to_add = decoded_word.strip()
                 except (Exception, UnicodeDecodeError):
                     word_to_add = word
                 if word_to_add not in self.ban_words_set:
                     self.ban_words_set.add(word_to_add)
                     self.ban_words_list.append(word_to_add)
         self.build_ban_words_dict(self.ban_words_list)
```

### Comparing `cleanse_speech-0.1.1/tests/test_dfa.py` & `cleanse_speech-0.1.2/tests/test_dfa.py`

 * *Files identical despite different names*

### Comparing `cleanse_speech-0.1.1/PKG-INFO` & `cleanse_speech-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1
-Name: cleanse-speech
-Version: 0.1.1
-Summary: An intelligent Python library designed to detect and filter offensive language, ensuring respectful and constructive communication in any digital space.
-Author-Email: llmkira <me@dianas.cyou>
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # cleanse-speech 🚀
 
 [![PyPI version](https://badge.fury.io/py/cleanse_speech.svg)](https://badge.fury.io/py/cleanse_speech)
 [![Downloads](https://pepy.tech/badge/cleanse_speech)](https://pepy.tech/project/cleanse_speech)
 [![Downloads](https://pepy.tech/badge/cleanse_speech/month)](https://pepy.tech/project/cleanse_speech)
 
-Python🐍 3.9+ support. 
+Python🐍 3.9+ support.
+
+A library for cleansing sensitive words in speech.
 
+> [!NOTE]
+> This library is designed with the intent to promote a harmonious online environment by identifying and
+> addressing offensive language. It is **not** intended to enforce strict censorship or infringe upon free speech. Our
+> goal is to foster respectful communication and ensure that all users feel safe and included in online communities. By
+> using this library, developers can help create spaces where open dialogue is encouraged while maintaining a level of
+> decency and mutual respect.
 
+## Installation
 
 ```shell
 pip install cleanse-speech
 ```
 
 ## Usage
 
 ```python
+import io
+
 from cleanse_speech import DLFA
+from cleanse_speech import SpamShelf
 
 if __name__ == '__main__':
     dfa = DLFA(words_resource=[
         ['你好'],
         io.BytesIO(b'sensitive'),
+        SpamShelf.CN.ADVERTISEMENT,
     ])
     print(dfa.contains_illegal('This is a 你好 word.'))
     print(dfa.censor_all('This is a 你好 word.'))
     print(dfa.extract_illegal_words('This is a 你好 word.'))
     dfa.update_words(['sensitive', 'word', 'new'])
-    print(dfa.contains_illegal('This is a new sensitive word.'))
-    print(dfa.censor_all('This is a new sensitive word.'))
     print(dfa.extract_illegal_words('This is a new sensitive word.'))
 ```
```

