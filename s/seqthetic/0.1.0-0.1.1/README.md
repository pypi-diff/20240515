# Comparing `tmp/seqthetic-0.1.0.tar.gz` & `tmp/seqthetic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqthetic-0.1.0.tar", max compression
+gzip compressed data, was "seqthetic-0.1.1.tar", max compression
```

## Comparing `seqthetic-0.1.0.tar` & `seqthetic-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      740 2024-05-07 07:28:14.794309 seqthetic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    12058 2024-05-14 07:00:49.209241 seqthetic-0.1.0/readme.md
--rw-r--r--   0        0        0        0 2024-04-23 03:46:19.493282 seqthetic-0.1.0/seqthetic/__init__.py
--rw-r--r--   0        0        0     2902 2024-05-09 06:12:03.733437 seqthetic-0.1.0/seqthetic/dataset.py
--rw-r--r--   0        0        0      562 2024-05-14 04:17:11.407174 seqthetic-0.1.0/seqthetic/dependencies/__init__.py
--rw-r--r--   0        0        0      883 2024-05-14 03:57:53.546887 seqthetic-0.1.0/seqthetic/dependencies/adapter.py
--rw-r--r--   0        0        0     1795 2024-05-14 04:32:16.874428 seqthetic-0.1.0/seqthetic/dependencies/base.py
--rw-r--r--   0        0        0     2534 2024-05-08 02:35:11.698745 seqthetic-0.1.0/seqthetic/dependencies/fbm.py
--rw-r--r--   0        0        0     1882 2024-05-07 07:27:35.421846 seqthetic-0.1.0/seqthetic/dependencies/function.py
--rw-r--r--   0        0        0     1500 2024-05-07 07:27:35.425272 seqthetic-0.1.0/seqthetic/dependencies/random.py
--rw-r--r--   0        0        0     2798 2024-05-07 07:27:35.369313 seqthetic-0.1.0/seqthetic/mapping.py
--rw-r--r--   0        0        0     1305 2024-05-08 11:53:41.162062 seqthetic-0.1.0/seqthetic/range.py
--rw-r--r--   0        0        0     1199 2024-05-14 04:41:56.662366 seqthetic-0.1.0/seqthetic/seed.py
--rw-r--r--   0        0        0     4075 2024-05-09 06:40:31.603486 seqthetic-0.1.0/seqthetic/spec_variation.py
--rw-r--r--   0        0        0     4030 2024-05-14 04:37:34.418005 seqthetic-0.1.0/seqthetic/synthesis_spec.py
--rw-r--r--   0        0        0     1804 2024-05-07 07:27:35.389403 seqthetic-0.1.0/seqthetic/synthesizer.py
--rw-r--r--   0        0        0     1349 2024-05-09 06:38:18.422069 seqthetic-0.1.0/seqthetic/utils.py
--rw-r--r--   0        0        0        0 2024-05-07 12:03:34.624527 seqthetic-0.1.0/seqthetic/vary/__init__.py
--rw-r--r--   0        0        0      709 2024-05-09 04:33:48.215716 seqthetic-0.1.0/seqthetic/vary/compose_ops.py
--rw-r--r--   0        0        0     1475 2024-05-07 16:38:49.316467 seqthetic-0.1.0/seqthetic/vary/compute_ops.py
--rw-r--r--   0        0        0     1232 2024-05-08 12:19:45.887199 seqthetic-0.1.0/seqthetic/vary/domain_ops.py
--rw-r--r--   0        0        0     5426 2024-05-14 04:32:16.874428 seqthetic-0.1.0/seqthetic/vary/transform.py
--rw-r--r--   0        0        0      954 2024-05-08 03:02:01.961163 seqthetic-0.1.0/seqthetic/vary/variation.py
--rw-r--r--   0        0        0     4102 2024-05-14 04:41:06.866213 seqthetic-0.1.0/seqthetic/vary/variator.py
--rw-r--r--   0        0        0     4512 2024-05-07 07:42:37.614955 seqthetic-0.1.0/seqthetic/vocabulary.py
--rw-r--r--   0        0        0    12500 1970-01-01 00:00:00.000000 seqthetic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      740 2024-05-15 03:31:55.153019 seqthetic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12058 2024-05-14 07:00:49.209241 seqthetic-0.1.1/readme.md
+-rw-r--r--   0        0        0        0 2024-04-23 03:46:19.493282 seqthetic-0.1.1/seqthetic/__init__.py
+-rw-r--r--   0        0        0     2934 2024-05-15 01:08:34.241672 seqthetic-0.1.1/seqthetic/dataset.py
+-rw-r--r--   0        0        0      562 2024-05-14 04:17:11.407174 seqthetic-0.1.1/seqthetic/dependencies/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-14 03:57:53.546887 seqthetic-0.1.1/seqthetic/dependencies/adapter.py
+-rw-r--r--   0        0        0     1795 2024-05-14 04:32:16.874428 seqthetic-0.1.1/seqthetic/dependencies/base.py
+-rw-r--r--   0        0        0     2534 2024-05-08 02:35:11.698745 seqthetic-0.1.1/seqthetic/dependencies/fbm.py
+-rw-r--r--   0        0        0     1882 2024-05-07 07:27:35.421846 seqthetic-0.1.1/seqthetic/dependencies/function.py
+-rw-r--r--   0        0        0     1500 2024-05-07 07:27:35.425272 seqthetic-0.1.1/seqthetic/dependencies/random.py
+-rw-r--r--   0        0        0     2798 2024-05-07 07:27:35.369313 seqthetic-0.1.1/seqthetic/mapping.py
+-rw-r--r--   0        0        0     1305 2024-05-08 11:53:41.162062 seqthetic-0.1.1/seqthetic/range.py
+-rw-r--r--   0        0        0     1246 2024-05-15 02:19:29.918718 seqthetic-0.1.1/seqthetic/seed.py
+-rw-r--r--   0        0        0     4075 2024-05-09 06:40:31.603486 seqthetic-0.1.1/seqthetic/spec_variation.py
+-rw-r--r--   0        0        0     5704 2024-05-15 02:55:53.636248 seqthetic-0.1.1/seqthetic/synthesis_spec.py
+-rw-r--r--   0        0        0     3647 2024-05-15 02:51:58.490011 seqthetic-0.1.1/seqthetic/synthesizer.py
+-rw-r--r--   0        0        0     1349 2024-05-09 06:38:18.422069 seqthetic-0.1.1/seqthetic/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 12:03:34.624527 seqthetic-0.1.1/seqthetic/vary/__init__.py
+-rw-r--r--   0        0        0      709 2024-05-09 04:33:48.215716 seqthetic-0.1.1/seqthetic/vary/compose_ops.py
+-rw-r--r--   0        0        0     1475 2024-05-07 16:38:49.316467 seqthetic-0.1.1/seqthetic/vary/compute_ops.py
+-rw-r--r--   0        0        0     1232 2024-05-08 12:19:45.887199 seqthetic-0.1.1/seqthetic/vary/domain_ops.py
+-rw-r--r--   0        0        0     5426 2024-05-14 04:32:16.874428 seqthetic-0.1.1/seqthetic/vary/transform.py
+-rw-r--r--   0        0        0      954 2024-05-08 03:02:01.961163 seqthetic-0.1.1/seqthetic/vary/variation.py
+-rw-r--r--   0        0        0     4102 2024-05-14 04:41:06.866213 seqthetic-0.1.1/seqthetic/vary/variator.py
+-rw-r--r--   0        0        0     4526 2024-05-15 03:27:39.863802 seqthetic-0.1.1/seqthetic/vocabulary.py
+-rw-r--r--   0        0        0    12500 1970-01-01 00:00:00.000000 seqthetic-0.1.1/PKG-INFO
```

### Comparing `seqthetic-0.1.0/pyproject.toml` & `seqthetic-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqthetic"
-version = "0.1.0"
+version = "0.1.1"
 description = "Creates sequence data for pretraining and benchmarking sequence models"
 authors = ["Shom <shaomi_lin@126.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
```

### Comparing `seqthetic-0.1.0/readme.md` & `seqthetic-0.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/dataset.py` & `seqthetic-0.1.1/seqthetic/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 SavePath = namedtuple("SavePath", ["spec_path", "dataset_path"])
 
 
 class Dataset:
     df: pd.DataFrame
     spec: SynthesisSpec
-    columns = ["dependency", "sequence", "domain_id", "metadata"]
+    columns = ["dependency", "sequence", "domain_id", "split", "metadata"]
     dtype = {
         "dependency": object,
         "sequence": object,
+        "split": str,
         "domain_id": str,
         "metadata": object,
     }
 
     def __init__(self, spec: SynthesisSpec, df: pd.DataFrame):
         self.spec = spec
         self.df = df
```

### Comparing `seqthetic-0.1.0/seqthetic/dependencies/__init__.py` & `seqthetic-0.1.1/seqthetic/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/dependencies/adapter.py` & `seqthetic-0.1.1/seqthetic/dependencies/adapter.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/dependencies/base.py` & `seqthetic-0.1.1/seqthetic/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/dependencies/fbm.py` & `seqthetic-0.1.1/seqthetic/dependencies/fbm.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/dependencies/function.py` & `seqthetic-0.1.1/seqthetic/dependencies/function.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/dependencies/random.py` & `seqthetic-0.1.1/seqthetic/dependencies/random.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/mapping.py` & `seqthetic-0.1.1/seqthetic/mapping.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/range.py` & `seqthetic-0.1.1/seqthetic/range.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/seed.py` & `seqthetic-0.1.1/seqthetic/seed.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,7 +35,8 @@
         else:
             return np.random.default_rng(seed)
 
 
 class SpecSeed(BaseModel):
     vocabulary: Seed = Field(default_factory=Seed)
     domains: List[Seed]  = Field(default_factory=list)
+    split: Seed = Field(default_factory=Seed)
```

### Comparing `seqthetic-0.1.0/seqthetic/spec_variation.py` & `seqthetic-0.1.1/seqthetic/spec_variation.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/utils.py` & `seqthetic-0.1.1/seqthetic/utils.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/vary/compose_ops.py` & `seqthetic-0.1.1/seqthetic/vary/compose_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/vary/compute_ops.py` & `seqthetic-0.1.1/seqthetic/vary/compute_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/vary/domain_ops.py` & `seqthetic-0.1.1/seqthetic/vary/domain_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/vary/transform.py` & `seqthetic-0.1.1/seqthetic/vary/transform.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/vary/variation.py` & `seqthetic-0.1.1/seqthetic/vary/variation.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/vary/variator.py` & `seqthetic-0.1.1/seqthetic/vary/variator.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.0/seqthetic/vocabulary.py` & `seqthetic-0.1.1/seqthetic/vocabulary.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,23 @@
     def make_vocab_prob(self) -> VocabProb:
         pass
 
     def set_seed(self, seed: Seed):
         self.seed = seed
 
 
+# todo
 class CorpusVocabulary(BaseVocabulary):
     distribution: str = "corpus"
-    spec: Dict[int, float]
+    weight: Dict[int, float]
     corpus_name: str
 
     def make_vocab_prob(self) -> VocabProb:
         vocab_prob = VocabProb(
-            self.size, list(self.spec.keys()), list(self.spec.values())
+            self.size, list(self.weight.keys()), list(self.weight.values())
         )
         return vocab_prob
 
 
 class LogLinearVocabulary(BaseVocabulary):
     """todo"""
```

### Comparing `seqthetic-0.1.0/PKG-INFO` & `seqthetic-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqthetic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Creates sequence data for pretraining and benchmarking sequence models
 Author: Shom
 Author-email: shaomi_lin@126.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: flake8 (>=7.0.0,<8.0.0)
```

