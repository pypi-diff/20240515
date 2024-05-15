# Comparing `tmp/konoha-5.5.6.tar.gz` & `tmp/konoha-5.5.6a0.tar.gz`

## Comparing `konoha-5.5.6.tar` & `konoha-5.5.6a0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/py.typed
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/sentence_tokenizer.py
--rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/api/__init__.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/api/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/api/v1/__init__.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/api/v1/batch_tokenization.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/api/v1/tokenization.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/data/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/data/resource.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/data/token.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/character_tokenizer.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/janome_tokenizer.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/konoha_api_tokenizer.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/kytea_tokenizer.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/mecab_tokenizer.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/nagisa_tokenizer.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/sentencepiece_tokenizer.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/sudachi_tokenizer.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/tokenizer.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 konoha-5.5.6/src/konoha/word_tokenizers/whitespace_tokenizer.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 konoha-5.5.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 konoha-5.5.6/LICENSE
--rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 konoha-5.5.6/README.md
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 konoha-5.5.6/pyproject.toml
--rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 konoha-5.5.6/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/py.typed
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/sentence_tokenizer.py
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/__init__.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/v1/__init__.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/v1/batch_tokenization.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/v1/tokenization.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/data/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/data/resource.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/data/token.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/character_tokenizer.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/janome_tokenizer.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/konoha_api_tokenizer.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/kytea_tokenizer.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/mecab_tokenizer.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/nagisa_tokenizer.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/sentencepiece_tokenizer.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/sudachi_tokenizer.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/tokenizer.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 konoha-5.5.6a0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 konoha-5.5.6a0/LICENSE
+-rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 konoha-5.5.6a0/README.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 konoha-5.5.6a0/pyproject.toml
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 konoha-5.5.6a0/PKG-INFO
```

### Comparing `konoha-5.5.6/src/konoha/sentence_tokenizer.py` & `konoha-5.5.6a0/konoha/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/api/v1/batch_tokenization.py` & `konoha-5.5.6a0/konoha/api/v1/batch_tokenization.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/api/v1/tokenization.py` & `konoha-5.5.6a0/konoha/api/v1/tokenization.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/data/resource.py` & `konoha-5.5.6a0/konoha/data/resource.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/data/token.py` & `konoha-5.5.6a0/konoha/data/token.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizers/__init__.py` & `konoha-5.5.6a0/konoha/word_tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizers/janome_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/janome_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizers/kytea_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/kytea_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizers/mecab_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/mecab_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizers/nagisa_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/nagisa_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizers/sentencepiece_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizers/sudachi_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/sudachi_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/src/konoha/word_tokenizers/tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/LICENSE` & `konoha-5.5.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/README.md` & `konoha-5.5.6a0/README.md`

 * *Files identical despite different names*

### Comparing `konoha-5.5.6/pyproject.toml` & `konoha-5.5.6a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "konoha"
-version = "5.5.6"
+version = "5.5.6a"
 description = "Add your description here"
 authors = [{ name = "himkt", email = "himkt@klis.tsukuba.ac.jp" }]
 dependencies = [
     "requests<3.0.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
@@ -53,15 +53,20 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.sdist]
-only-include = ["src"]
+packages = ["src/konoha"]
+only-packages = true
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/konoha"]
+only-packages = true
 
 [[tool.mypy.overrides]]
 module = [
     "boto3",
     "janome.tokenizer",
     "nagisa",
     "natto",
```

### Comparing `konoha-5.5.6/PKG-INFO` & `konoha-5.5.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: konoha
-Version: 5.5.6
+Version: 5.5.6a0
 Summary: Add your description here
 Author-email: himkt <himkt@klis.tsukuba.ac.jp>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: requests<3.0.0
 Provides-Extra: all
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.3 Name: konoha Version: 5.5.6 Summary: Add your description
-here Author-email: himkt
+Metadata-Version: 2.3 Name: konoha Version: 5.5.6a0 Summary: Add your
+description here Author-email: himkt
 klis.tsukuba.ac.jp> License-Expression: MIT License-File: LICENSE Requires-
 Python: >=3.8 Requires-Dist: requests<3.0.0 Provides-Extra: all Requires-Dist:
 boto3~=1.34.0; extra == 'all' Requires-Dist: fastapi<1.0.0; extra == 'all'
 Requires-Dist: janome~=0.5.0; extra == 'all' Requires-Dist: kytea~=0.1.0; extra
 == 'all' Requires-Dist: nagisa~=0.2.10; extra == 'all' Requires-Dist: natto-
 py~=1.0.0; extra == 'all' Requires-Dist: sentencepiece~=0.1.85; extra == 'all'
 Requires-Dist: sudachidict-core==20230927; extra == 'all' Requires-Dist:
```

