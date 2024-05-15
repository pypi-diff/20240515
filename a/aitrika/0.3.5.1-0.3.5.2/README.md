# Comparing `tmp/aitrika-0.3.5.1.tar.gz` & `tmp/aitrika-0.3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitrika-0.3.5.1.tar", max compression
+gzip compressed data, was "aitrika-0.3.5.2.tar", max compression
```

## Comparing `aitrika-0.3.5.1.tar` & `aitrika-0.3.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1071 2024-05-09 15:14:41.749522 aitrika-0.3.5.1/LICENSE
--rw-r--r--   0        0        0     2890 2024-05-15 10:05:48.277670 aitrika-0.3.5.1/README.md
--rw-r--r--   0        0        0        0 2024-05-07 13:24:47.559630 aitrika-0.3.5.1/aitrika/__init__.py
--rw-r--r--   0        0        0     3118 2024-05-15 09:54:25.368276 aitrika-0.3.5.1/aitrika/app.py
--rw-r--r--   0        0        0        0 2024-05-07 13:24:47.559630 aitrika-0.3.5.1/aitrika/data/__init__.py
--rw-r--r--   0        0        0   425626 2024-05-10 15:39:15.292099 aitrika-0.3.5.1/aitrika/data/breast_cancer_brca1_brca2.pdf
--rw-r--r--   0        0        0   391183 2024-05-11 15:05:45.745959 aitrika-0.3.5.1/aitrika/data/review_of_breast_cancer_pathological_image_processing.pdf
--rw-r--r--   0        0        0   759554 2024-05-09 07:47:33.183766 aitrika-0.3.5.1/aitrika/data/targets_of_neuroprotection_in_glaucoma.pdf
--rw-r--r--   0        0        0        0 2024-05-07 13:24:47.563630 aitrika-0.3.5.1/aitrika/engine/__init__.py
--rw-r--r--   0        0        0    13537 2024-05-15 13:38:30.188102 aitrika-0.3.5.1/aitrika/engine/aitrika.py
--rw-r--r--   0        0        0        0 2024-05-07 13:24:47.563630 aitrika-0.3.5.1/aitrika/llm/__init__.py
--rw-r--r--   0        0        0     2304 2024-05-14 09:57:30.044064 aitrika-0.3.5.1/aitrika/llm/anyscale.py
--rw-r--r--   0        0        0      312 2024-05-09 07:06:56.147899 aitrika-0.3.5.1/aitrika/llm/base_llm.py
--rw-r--r--   0        0        0     2209 2024-05-13 09:44:04.348729 aitrika-0.3.5.1/aitrika/llm/groq.py
--rw-r--r--   0        0        0     2373 2024-05-13 09:19:27.589208 aitrika-0.3.5.1/aitrika/llm/huggingface.py
--rw-r--r--   0        0        0     2128 2024-05-13 09:19:35.173144 aitrika-0.3.5.1/aitrika/llm/neutrino.py
--rw-r--r--   0        0        0     2034 2024-05-13 09:19:40.713098 aitrika-0.3.5.1/aitrika/llm/ollama.py
--rw-r--r--   0        0        0     2144 2024-05-13 09:19:45.745056 aitrika-0.3.5.1/aitrika/llm/openai.py
--rw-r--r--   0        0        0      960 2024-05-15 09:55:02.799893 aitrika-0.3.5.1/aitrika/main.py
--rw-r--r--   0        0        0        0 2024-05-07 13:24:47.563630 aitrika-0.3.5.1/aitrika/prompts/__init__.py
--rw-r--r--   0        0        0     1312 2024-05-15 09:47:28.804842 aitrika-0.3.5.1/aitrika/prompts/prompts.py
--rw-r--r--   0        0        0        0 2024-05-07 13:24:47.563630 aitrika-0.3.5.1/aitrika/utils/__init__.py
--rw-r--r--   0        0        0      461 2024-05-15 13:38:50.019621 aitrika-0.3.5.1/aitrika/utils/load_spacy_model.py
--rw-r--r--   0        0        0      429 2024-05-11 15:23:42.151746 aitrika-0.3.5.1/aitrika/utils/loader.py
--rw-r--r--   0        0        0      528 2024-05-10 17:00:49.451049 aitrika-0.3.5.1/aitrika/utils/text_parser.py
--rw-r--r--   0        0        0      836 2024-05-15 13:39:09.639274 aitrika-0.3.5.1/pyproject.toml
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 aitrika-0.3.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-09 15:14:41.749522 aitrika-0.3.5.2/LICENSE
+-rw-r--r--   0        0        0     2918 2024-05-15 13:46:12.918079 aitrika-0.3.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 13:24:47.559630 aitrika-0.3.5.2/aitrika/__init__.py
+-rw-r--r--   0        0        0     3118 2024-05-15 09:54:25.368276 aitrika-0.3.5.2/aitrika/app.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:24:47.559630 aitrika-0.3.5.2/aitrika/data/__init__.py
+-rw-r--r--   0        0        0   425626 2024-05-10 15:39:15.292099 aitrika-0.3.5.2/aitrika/data/breast_cancer_brca1_brca2.pdf
+-rw-r--r--   0        0        0   391183 2024-05-11 15:05:45.745959 aitrika-0.3.5.2/aitrika/data/review_of_breast_cancer_pathological_image_processing.pdf
+-rw-r--r--   0        0        0   759554 2024-05-09 07:47:33.183766 aitrika-0.3.5.2/aitrika/data/targets_of_neuroprotection_in_glaucoma.pdf
+-rw-r--r--   0        0        0        0 2024-05-07 13:24:47.563630 aitrika-0.3.5.2/aitrika/engine/__init__.py
+-rw-r--r--   0        0        0    13537 2024-05-15 13:38:30.188102 aitrika-0.3.5.2/aitrika/engine/aitrika.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:24:47.563630 aitrika-0.3.5.2/aitrika/llm/__init__.py
+-rw-r--r--   0        0        0     2304 2024-05-14 09:57:30.044064 aitrika-0.3.5.2/aitrika/llm/anyscale.py
+-rw-r--r--   0        0        0      312 2024-05-09 07:06:56.147899 aitrika-0.3.5.2/aitrika/llm/base_llm.py
+-rw-r--r--   0        0        0     2209 2024-05-13 09:44:04.348729 aitrika-0.3.5.2/aitrika/llm/groq.py
+-rw-r--r--   0        0        0     2373 2024-05-13 09:19:27.589208 aitrika-0.3.5.2/aitrika/llm/huggingface.py
+-rw-r--r--   0        0        0     2128 2024-05-13 09:19:35.173144 aitrika-0.3.5.2/aitrika/llm/neutrino.py
+-rw-r--r--   0        0        0     2034 2024-05-13 09:19:40.713098 aitrika-0.3.5.2/aitrika/llm/ollama.py
+-rw-r--r--   0        0        0     2144 2024-05-13 09:19:45.745056 aitrika-0.3.5.2/aitrika/llm/openai.py
+-rw-r--r--   0        0        0      960 2024-05-15 09:55:02.799893 aitrika-0.3.5.2/aitrika/main.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:24:47.563630 aitrika-0.3.5.2/aitrika/prompts/__init__.py
+-rw-r--r--   0        0        0     1312 2024-05-15 09:47:28.804842 aitrika-0.3.5.2/aitrika/prompts/prompts.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:24:47.563630 aitrika-0.3.5.2/aitrika/utils/__init__.py
+-rw-r--r--   0        0        0      452 2024-05-15 13:46:07.122136 aitrika-0.3.5.2/aitrika/utils/load_spacy_model.py
+-rw-r--r--   0        0        0      429 2024-05-11 15:23:42.151746 aitrika-0.3.5.2/aitrika/utils/loader.py
+-rw-r--r--   0        0        0      528 2024-05-10 17:00:49.451049 aitrika-0.3.5.2/aitrika/utils/text_parser.py
+-rw-r--r--   0        0        0      836 2024-05-15 13:46:38.873839 aitrika-0.3.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 aitrika-0.3.5.2/PKG-INFO
```

### Comparing `aitrika-0.3.5.1/LICENSE` & `aitrika-0.3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/README.md` & `aitrika-0.3.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,7 +126,8 @@
 
 AItrika is licensed under the MIT License. See the LICENSE file for more details.
 
 ## TODO
 
 - [ ] Create documentation
 - [ ] Add docstrings
+- [ ] Create Python package
```

### Comparing `aitrika-0.3.5.1/aitrika/app.py` & `aitrika-0.3.5.2/aitrika/app.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/data/breast_cancer_brca1_brca2.pdf` & `aitrika-0.3.5.2/aitrika/data/breast_cancer_brca1_brca2.pdf`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/data/review_of_breast_cancer_pathological_image_processing.pdf` & `aitrika-0.3.5.2/aitrika/data/review_of_breast_cancer_pathological_image_processing.pdf`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/data/targets_of_neuroprotection_in_glaucoma.pdf` & `aitrika-0.3.5.2/aitrika/data/targets_of_neuroprotection_in_glaucoma.pdf`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/engine/aitrika.py` & `aitrika-0.3.5.2/aitrika/engine/aitrika.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/llm/anyscale.py` & `aitrika-0.3.5.2/aitrika/llm/anyscale.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/llm/groq.py` & `aitrika-0.3.5.2/aitrika/llm/groq.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/llm/huggingface.py` & `aitrika-0.3.5.2/aitrika/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/llm/neutrino.py` & `aitrika-0.3.5.2/aitrika/llm/neutrino.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/llm/ollama.py` & `aitrika-0.3.5.2/aitrika/llm/ollama.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/llm/openai.py` & `aitrika-0.3.5.2/aitrika/llm/openai.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/main.py` & `aitrika-0.3.5.2/aitrika/main.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/prompts/prompts.py` & `aitrika-0.3.5.2/aitrika/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/aitrika/utils/text_parser.py` & `aitrika-0.3.5.2/aitrika/utils/text_parser.py`

 * *Files identical despite different names*

### Comparing `aitrika-0.3.5.1/pyproject.toml` & `aitrika-0.3.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aitrika"
-version = "0.3.5.1"
+version = "0.3.5.2"
 description = "Enhance your knowledge in medical research."
 authors = ["Danilo Palumbo"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `aitrika-0.3.5.1/PKG-INFO` & `aitrika-0.3.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitrika
-Version: 0.3.5.1
+Version: 0.3.5.2
 Summary: Enhance your knowledge in medical research.
 License: MIT
 Author: Danilo Palumbo
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -156,8 +156,9 @@
 
 AItrika is licensed under the MIT License. See the LICENSE file for more details.
 
 ## TODO
 
 - [ ] Create documentation
 - [ ] Add docstrings
+- [ ] Create Python package
```

