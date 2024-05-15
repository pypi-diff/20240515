# Comparing `tmp/saf_datasets-0.6.2.tar.gz` & `tmp/saf_datasets-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saf_datasets-0.6.2.tar", last modified: Fri May 10 05:53:32 2024, max compression
+gzip compressed data, was "saf_datasets-0.6.4.tar", last modified: Tue May 14 20:41:15 2024, max compression
```

## Comparing `saf_datasets-0.6.2.tar` & `saf_datasets-0.6.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.031966 saf_datasets-0.6.2/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 saf_datasets-0.6.2/LICENSE
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-10 05:53:32.031690 saf_datasets-0.6.2/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3491 2024-05-08 18:45:21.000000 saf_datasets-0.6.2/README.md
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      671 2024-05-09 14:05:21.000000 saf_datasets-0.6.2/pyproject.toml
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 14:09:52.000000 saf_datasets-0.6.2/requirements.txt
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.022665 saf_datasets-0.6.2/saf_datasets/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      366 2024-05-09 14:03:38.000000 saf_datasets-0.6.2/saf_datasets/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.025968 saf_datasets-0.6.2/saf_datasets/annotators/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       80 2024-04-22 11:09:48.000000 saf_datasets-0.6.2/saf_datasets/annotators/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1362 2024-05-08 15:57:27.000000 saf_datasets-0.6.2/saf_datasets/annotators/allennlp_srl.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      165 2023-11-29 15:12:10.000000 saf_datasets-0.6.2/saf_datasets/annotators/models.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1088 2024-05-08 16:03:49.000000 saf_datasets-0.6.2/saf_datasets/annotators/spacy.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     4742 2024-05-08 16:14:10.000000 saf_datasets-0.6.2/saf_datasets/annotators/transformer.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.029623 saf_datasets-0.6.2/saf_datasets/data_access/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-03-13 13:13:57.000000 saf_datasets-0.6.2/saf_datasets/data_access/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1941 2024-05-08 15:54:57.000000 saf_datasets-0.6.2/saf_datasets/data_access/allnli.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     5375 2024-05-08 15:28:33.000000 saf_datasets-0.6.2/saf_datasets/data_access/codwoe.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1907 2024-05-08 15:32:04.000000 saf_datasets-0.6.2/saf_datasets/data_access/cpae.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    12727 2024-05-08 14:56:10.000000 saf_datasets-0.6.2/saf_datasets/data_access/dataset.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     2922 2024-05-08 15:37:48.000000 saf_datasets-0.6.2/saf_datasets/data_access/entailmentbank.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2608 2024-05-08 17:18:08.000000 saf_datasets-0.6.2/saf_datasets/data_access/stsb.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     8793 2024-05-08 15:08:33.000000 saf_datasets-0.6.2/saf_datasets/data_access/wiktionary.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4059 2024-05-08 15:14:59.000000 saf_datasets-0.6.2/saf_datasets/data_access/wordnet_filtered.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.030711 saf_datasets-0.6.2/saf_datasets/wrappers/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-13 14:11:53.000000 saf_datasets-0.6.2/saf_datasets/wrappers/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      793 2024-05-08 15:45:05.000000 saf_datasets-0.6.2/saf_datasets/wrappers/hf.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2062 2024-05-08 15:51:39.000000 saf_datasets-0.6.2/saf_datasets/wrappers/torch.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.031332 saf_datasets-0.6.2/saf_datasets.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/PKG-INFO
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      873 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/SOURCES.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/dependency_links.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/requires.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       13 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-10 05:53:32.032025 saf_datasets-0.6.2/setup.cfg
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      815 2024-05-09 14:05:21.000000 saf_datasets-0.6.2/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:41:15.195810 saf_datasets-0.6.4/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 saf_datasets-0.6.4/LICENSE
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-14 20:41:15.195554 saf_datasets-0.6.4/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3491 2024-05-08 18:45:21.000000 saf_datasets-0.6.4/README.md
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      671 2024-05-14 20:38:15.000000 saf_datasets-0.6.4/pyproject.toml
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 14:09:52.000000 saf_datasets-0.6.4/requirements.txt
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:41:15.187841 saf_datasets-0.6.4/saf_datasets/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      366 2024-05-09 14:03:38.000000 saf_datasets-0.6.4/saf_datasets/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:41:15.190575 saf_datasets-0.6.4/saf_datasets/annotators/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       80 2024-04-22 11:09:48.000000 saf_datasets-0.6.4/saf_datasets/annotators/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1325 2024-05-14 14:26:13.000000 saf_datasets-0.6.4/saf_datasets/annotators/allennlp_srl.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      165 2023-11-29 15:12:10.000000 saf_datasets-0.6.4/saf_datasets/annotators/models.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1088 2024-05-08 16:03:49.000000 saf_datasets-0.6.4/saf_datasets/annotators/spacy.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     4882 2024-05-10 08:55:47.000000 saf_datasets-0.6.4/saf_datasets/annotators/transformer.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:41:15.193505 saf_datasets-0.6.4/saf_datasets/data_access/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-03-13 13:13:57.000000 saf_datasets-0.6.4/saf_datasets/data_access/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1941 2024-05-08 15:54:57.000000 saf_datasets-0.6.4/saf_datasets/data_access/allnli.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     5375 2024-05-08 15:28:33.000000 saf_datasets-0.6.4/saf_datasets/data_access/codwoe.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1907 2024-05-08 15:32:04.000000 saf_datasets-0.6.4/saf_datasets/data_access/cpae.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    12727 2024-05-08 14:56:10.000000 saf_datasets-0.6.4/saf_datasets/data_access/dataset.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     3921 2024-05-14 20:34:09.000000 saf_datasets-0.6.4/saf_datasets/data_access/entailmentbank.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2608 2024-05-08 17:18:08.000000 saf_datasets-0.6.4/saf_datasets/data_access/stsb.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     8793 2024-05-08 15:08:33.000000 saf_datasets-0.6.4/saf_datasets/data_access/wiktionary.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4048 2024-05-14 20:30:54.000000 saf_datasets-0.6.4/saf_datasets/data_access/wordnet_filtered.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:41:15.194691 saf_datasets-0.6.4/saf_datasets/wrappers/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-13 14:11:53.000000 saf_datasets-0.6.4/saf_datasets/wrappers/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      793 2024-05-08 15:45:05.000000 saf_datasets-0.6.4/saf_datasets/wrappers/hf.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2062 2024-05-08 15:51:39.000000 saf_datasets-0.6.4/saf_datasets/wrappers/torch.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:41:15.195238 saf_datasets-0.6.4/saf_datasets.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-14 20:41:15.000000 saf_datasets-0.6.4/saf_datasets.egg-info/PKG-INFO
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      873 2024-05-14 20:41:15.000000 saf_datasets-0.6.4/saf_datasets.egg-info/SOURCES.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-14 20:41:15.000000 saf_datasets-0.6.4/saf_datasets.egg-info/dependency_links.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-14 20:41:15.000000 saf_datasets-0.6.4/saf_datasets.egg-info/requires.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       13 2024-05-14 20:41:15.000000 saf_datasets-0.6.4/saf_datasets.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-14 20:41:15.195865 saf_datasets-0.6.4/setup.cfg
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      815 2024-05-14 20:38:09.000000 saf_datasets-0.6.4/setup.py
```

### Comparing `saf_datasets-0.6.2/LICENSE` & `saf_datasets-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/PKG-INFO` & `saf_datasets-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saf-datasets
-Version: 0.6.2
+Version: 0.6.4
 Summary: Data set loading and annotation facilities for the Simple Annotation Framework
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/saf_datasets
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/saf_datasets/issues
 Keywords: datasets,annotated,nlp
```

### Comparing `saf_datasets-0.6.2/README.md` & `saf_datasets-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/pyproject.toml` & `saf_datasets-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saf-datasets"
-version = "0.6.2"
+version = "0.6.4"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" }
 ]
 description = "Data set loading and annotation facilities for the Simple Annotation Framework"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `saf_datasets-0.6.2/saf_datasets/annotators/allennlp_srl.py` & `saf_datasets-0.6.4/saf_datasets/annotators/allennlp_srl.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from saf.annotators import Annotator
 
 
 class AllenSRLAnnotator(Annotator):
     """
     Annotator class for Semantic Role Labelling, based on the AllenNLP SRL model (Argument Structure)
     """
-    def __init__(self, annot_model: str = "en_core_web_sm"):
+    def __init__(self):
         super(AllenSRLAnnotator, self).__init__()
         self.annot_model = pretrained.load_predictor("structured-prediction-srl-bert")
 
     def annotate(self, sentences: Iterable[Sentence]):
         for sent in tqdm(sentences, desc="Annotating (AllenNLP SRL)"):
             annots = self.annot_model.predict(sent.surface)
             sent.tokens = [tok for tok in sent.tokens if (tok.surface.strip())]
```

### Comparing `saf_datasets-0.6.2/saf_datasets/annotators/spacy.py` & `saf_datasets-0.6.4/saf_datasets/annotators/spacy.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets/annotators/transformer.py` & `saf_datasets-0.6.4/saf_datasets/annotators/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 class TransformerAnnotator(Annotator):
     """
     Annotator class for general transformer-based annotation (token classification) models
 
     Args:
         annot_model (str): the path or identifier for a pretrained model checkpoint.
+        tag (str): the annotation tag to which the annotations will be stored (e.g., NER, SRL, DSR).
         labels (Dict[int, str]): valid labels and their corresponding values (ids).
         max_len (int): maximum sentence length.
         device (str): device (e.g., 'cpu', 'cuda') where the model will be stored and ran.
     """
-    def __init__(self, annot_model: str, labels: Dict[int, str] = None, max_len: int = 128, device: str = None):
+    def __init__(self, annot_model: str, tag: str, labels: Dict[int, str] = None, max_len: int = 128, device: str = None):
         super(TransformerAnnotator, self).__init__()
         if (not device):
             if (cuda.is_available()):
                 self.device = "cuda"
             else:
                 self.device = "cpu"
         else:
@@ -43,14 +44,15 @@
             annot_model = self.model_path.replace(".zip", "")
 
         self.annot_model = AutoModelForTokenClassification.from_pretrained(annot_model).to(self.device)
         self.annot_tokenizer = AutoTokenizer.from_pretrained(annot_model)
         self.annot_config = AutoConfig.from_pretrained(annot_model)
         self.ids_to_labels = labels if labels else self.annot_config.id2label
         self.max_len = max_len
+        self.tag = tag
 
     def annotate(self, sentences: Iterable[Sentence]):
         for sent in tqdm(sentences, desc="Annotating (Transformer)"):
             #tag each definition
             sentence = sent.surface
             inputs = self.annot_tokenizer(sentence.strip().split(),
                                           is_split_into_words=True,
@@ -80,11 +82,11 @@
             word_tags = [[word, label] for word, label in zip(sentence.split(), prediction)]
             #mapping back to the original tokens via string matching
             for i in range(len(sent.tokens)):
                 if sent.tokens[i].surface.isalnum():
                     for j in range(len(word_tags)):
                         if sent.tokens[i].surface in word_tags[j][0]:
                             word_tags[j][0] = word_tags[j][0].replace(sent.tokens[i].surface,"")
-                            sent.tokens[i].annotations["dsr"] = word_tags[j][1]
+                            sent.tokens[i].annotations[self.tag] = word_tags[j][1]
                             break
                 else:
-                    sent.tokens[i].annotations["dsr"] = "O"
+                    sent.tokens[i].annotations[self.tag] = "O"
```

### Comparing `saf_datasets-0.6.2/saf_datasets/data_access/allnli.py` & `saf_datasets-0.6.4/saf_datasets/data_access/allnli.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets/data_access/codwoe.py` & `saf_datasets-0.6.4/saf_datasets/data_access/codwoe.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets/data_access/cpae.py` & `saf_datasets-0.6.4/saf_datasets/data_access/cpae.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets/data_access/dataset.py` & `saf_datasets-0.6.4/saf_datasets/data_access/dataset.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets/data_access/entailmentbank.py` & `saf_datasets-0.6.4/saf_datasets/data_access/entailmentbank.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import os
+import pickle
 import jsonlines
+import gzip
 from zipfile import ZipFile
 from tqdm import tqdm
 from spacy.lang.en import English
 from saf import Sentence, Token
 from .dataset import SentenceDataSet, BASE_URL
 
 FILE_VERSION = "entailment_trees_emnlp2021_data_v3"
 PATH = "EntailmentBank/%s.zip" % FILE_VERSION
 URL = BASE_URL + "%s.zip" % FILE_VERSION
 
+ANNOT_RESOURCES = {
+    "pos+lemma+ctag+dep+srl#noproof": {
+        "path": "EntailmentBank/eb_spacy_srl_noproof.pickle.gz",
+        "url": BASE_URL + "eb_spacy_srl_noproof.pickle.gz"
+    }
+}
+
 
 class EntailmentBankDataSet(SentenceDataSet):
     """
     Wrapper for the EntailmentBank dataset: https://allenai.org/data/entailmentbank
 
     Context, hypothesis, question, answer and proof sentences for a single entry in the original dataset are split
     adjacently, and can be grouped by their 'id' annotation.
@@ -64,7 +73,28 @@
         Args:
             idx (int): index for the ith sentence in the dataset.
 
         :return: A single term decomposition (Sentence).
         """
         return self.data[idx]
 
+    @staticmethod
+    def from_resource(locator: str):
+        """
+        Downloaads a per-annotated resource available at the specified locator
+
+        Example:
+            >>> dataset = EntailmentBankDataSet.from_resource("pos+lemma+ctag+dep+srl#noproof")
+        """
+        dataset = None
+        if (locator in ANNOT_RESOURCES):
+            path = ANNOT_RESOURCES[locator]["path"]
+            url = ANNOT_RESOURCES[locator]["url"]
+            data_path = SentenceDataSet.download_resource(path, url)
+            dataset = EntailmentBankDataSet(url="")
+            with gzip.open(data_path, "rb") as resource_file:
+                dataset.data = pickle.load(resource_file)
+        else:
+            print(f"No resource found at locator: {locator}")
+
+        return dataset
+
```

### Comparing `saf_datasets-0.6.2/saf_datasets/data_access/stsb.py` & `saf_datasets-0.6.4/saf_datasets/data_access/stsb.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets/data_access/wiktionary.py` & `saf_datasets-0.6.4/saf_datasets/data_access/wiktionary.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets/data_access/wordnet_filtered.py` & `saf_datasets-0.6.4/saf_datasets/data_access/wordnet_filtered.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         Example:
             >>> dataset = WordNetFilteredDataSet.from_resource("pos+lemma+ctag+dep+dsr+srl")
         """
         dataset = None
         if (locator in ANNOT_RESOURCES):
             path = ANNOT_RESOURCES[locator]["path"]
             url = ANNOT_RESOURCES[locator]["url"]
-            data_path = WiktionaryDefinitionCorpus.download_resource(path, url)
+            data_path = SentenceDataSet.download_resource(path, url)
             with gzip.open(data_path, "rb") as resource_file:
                 dataset = pickle.load(resource_file)
         else:
             print(f"No resource found at locator: {locator}")
 
         return dataset
```

### Comparing `saf_datasets-0.6.2/saf_datasets/wrappers/hf.py` & `saf_datasets-0.6.4/saf_datasets/wrappers/hf.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets/wrappers/torch.py` & `saf_datasets-0.6.4/saf_datasets/wrappers/torch.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/saf_datasets.egg-info/PKG-INFO` & `saf_datasets-0.6.4/saf_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saf-datasets
-Version: 0.6.2
+Version: 0.6.4
 Summary: Data set loading and annotation facilities for the Simple Annotation Framework
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/saf_datasets
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/saf_datasets/issues
 Keywords: datasets,annotated,nlp
```

### Comparing `saf_datasets-0.6.2/saf_datasets.egg-info/SOURCES.txt` & `saf_datasets-0.6.4/saf_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.2/setup.py` & `saf_datasets-0.6.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = [str(x).strip() for x in all_reqs]
 
     return install_requires
 
 
 setup(
     name='saf_datasets',
-    version='0.6.2',
+    version='0.6.4',
     packages=['saf_datasets', 'saf_datasets.annotators', 'saf_datasets.data_access', 'saf_datasets.wrappers'],
     url='',
     author='Danilo S. Carvalho',
     author_email='danilo.carvalho@manchester.ac.uk',
     description='Data set loading and annotation facilities for the Simple Annotation Framework',
     install_requires=load_requirements()
 )
```

