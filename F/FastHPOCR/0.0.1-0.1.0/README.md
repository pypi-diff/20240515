# Comparing `tmp/FastHPOCR-0.0.1.tar.gz` & `tmp/FastHPOCR-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastHPOCR-0.0.1.tar", last modified: Mon Mar 18 02:28:17 2024, max compression
+gzip compressed data, was "FastHPOCR-0.1.0.tar", last modified: Wed May 15 13:43:38 2024, max compression
```

## Comparing `FastHPOCR-0.0.1.tar` & `FastHPOCR-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-03-18 02:28:17.045081 FastHPOCR-0.0.1/
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-03-18 02:28:17.038549 FastHPOCR-0.0.1/FastHPOCR/
--rw-r--r--   0 tudor      (501) staff       (20)     1254 2024-03-18 02:20:56.000000 FastHPOCR-0.0.1/FastHPOCR/HPOAnnotator.py
--rw-r--r--   0 tudor      (501) staff       (20)     3485 2024-03-18 02:18:32.000000 FastHPOCR-0.0.1/FastHPOCR/IndexHPO.py
--rw-r--r--   0 tudor      (501) staff       (20)     1898 2024-03-18 02:22:07.000000 FastHPOCR-0.0.1/FastHPOCR/README.md
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-03-18 01:56:25.000000 FastHPOCR-0.0.1/FastHPOCR/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-03-18 02:28:17.039928 FastHPOCR-0.0.1/FastHPOCR/cr/
--rw-r--r--   0 tudor      (501) staff       (20)     3621 2024-03-18 02:00:25.000000 FastHPOCR-0.0.1/FastHPOCR/cr/CRIndexKB.py
--rw-r--r--   0 tudor      (501) staff       (20)     1051 2024-02-21 03:39:40.000000 FastHPOCR-0.0.1/FastHPOCR/cr/CandidateMatcher.py
--rw-r--r--   0 tudor      (501) staff       (20)     2277 2024-03-18 02:00:22.000000 FastHPOCR-0.0.1/FastHPOCR/cr/FormatResults.py
--rw-r--r--   0 tudor      (501) staff       (20)     1734 2024-03-02 08:55:02.000000 FastHPOCR-0.0.1/FastHPOCR/cr/SequenceCache.py
--rw-r--r--   0 tudor      (501) staff       (20)     3499 2024-03-18 02:00:19.000000 FastHPOCR-0.0.1/FastHPOCR/cr/TextProcessor.py
--rw-r--r--   0 tudor      (501) staff       (20)     3875 2024-03-18 02:00:14.000000 FastHPOCR-0.0.1/FastHPOCR/cr/TextSplitter.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:40.000000 FastHPOCR-0.0.1/FastHPOCR/cr/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-03-18 02:28:17.040619 FastHPOCR-0.0.1/FastHPOCR/index/
--rw-r--r--   0 tudor      (501) staff       (20)     2323 2024-03-18 02:01:02.000000 FastHPOCR-0.0.1/FastHPOCR/index/IndexTerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     4102 2024-03-18 02:01:01.000000 FastHPOCR-0.0.1/FastHPOCR/index/LabelProcessor.py
--rw-r--r--   0 tudor      (501) staff       (20)     2183 2024-03-18 02:00:59.000000 FastHPOCR-0.0.1/FastHPOCR/index/PreprocessOntologyTerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     2556 2024-02-28 12:38:42.000000 FastHPOCR-0.0.1/FastHPOCR/index/SynonymExpader.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:32.000000 FastHPOCR-0.0.1/FastHPOCR/index/__init__.py
--rw-r--r--   0 tudor      (501) staff       (20)     1058 2024-03-18 01:51:44.000000 FastHPOCR-0.0.1/FastHPOCR/license.txt
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-03-18 02:28:17.040850 FastHPOCR-0.0.1/FastHPOCR/resources/
--rw-r--r--   0 tudor      (501) staff       (20)     1337 2024-02-28 10:39:58.000000 FastHPOCR-0.0.1/FastHPOCR/resources/base-synonyms
--rw-r--r--   0 tudor      (501) staff       (20)  6300038 2024-03-11 22:24:57.000000 FastHPOCR-0.0.1/FastHPOCR/resources/vocab.clusters.list
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-03-18 02:28:17.044823 FastHPOCR-0.0.1/FastHPOCR/util/
--rw-r--r--   0 tudor      (501) staff       (20)      828 2024-02-20 02:33:16.000000 FastHPOCR-0.0.1/FastHPOCR/util/AnnotationObject.py
--rw-r--r--   0 tudor      (501) staff       (20)     1123 2024-03-18 02:01:19.000000 FastHPOCR-0.0.1/FastHPOCR/util/AnnotationToken.py
--rw-r--r--   0 tudor      (501) staff       (20)     1395 2024-03-18 01:03:07.000000 FastHPOCR-0.0.1/FastHPOCR/util/CRConstants.py
--rw-r--r--   0 tudor      (501) staff       (20)     1159 2024-02-28 03:26:30.000000 FastHPOCR-0.0.1/FastHPOCR/util/ContentUtil.py
--rw-r--r--   0 tudor      (501) staff       (20)     4740 2024-03-18 02:01:14.000000 FastHPOCR-0.0.1/FastHPOCR/util/OntoReader.py
--rw-r--r--   0 tudor      (501) staff       (20)    42275 2024-03-02 08:55:57.000000 FastHPOCR-0.0.1/FastHPOCR/util/SequenceData.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:36:52.000000 FastHPOCR-0.0.1/FastHPOCR/util/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-03-18 02:28:17.039041 FastHPOCR-0.0.1/FastHPOCR.egg-info/
--rw-r--r--   0 tudor      (501) staff       (20)      206 2024-03-18 02:28:17.000000 FastHPOCR-0.0.1/FastHPOCR.egg-info/PKG-INFO
--rw-r--r--   0 tudor      (501) staff       (20)      914 2024-03-18 02:28:17.000000 FastHPOCR-0.0.1/FastHPOCR.egg-info/SOURCES.txt
--rw-r--r--   0 tudor      (501) staff       (20)        1 2024-03-18 02:28:17.000000 FastHPOCR-0.0.1/FastHPOCR.egg-info/dependency_links.txt
--rw-r--r--   0 tudor      (501) staff       (20)       10 2024-03-18 02:28:17.000000 FastHPOCR-0.0.1/FastHPOCR.egg-info/top_level.txt
--rw-r--r--   0 tudor      (501) staff       (20)      206 2024-03-18 02:28:17.044957 FastHPOCR-0.0.1/PKG-INFO
--rw-r--r--   0 tudor      (501) staff       (20)       38 2024-03-18 02:28:17.045123 FastHPOCR-0.0.1/setup.cfg
--rw-r--r--   0 tudor      (501) staff       (20)      447 2024-03-18 01:52:09.000000 FastHPOCR-0.0.1/setup.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.373817 FastHPOCR-0.1.0/
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.366516 FastHPOCR-0.1.0/FastHPOCR/
+-rw-r--r--   0 tudor      (501) staff       (20)     1295 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/HPOAnnotator.py
+-rw-r--r--   0 tudor      (501) staff       (20)     4837 2024-05-15 13:34:45.000000 FastHPOCR-0.1.0/FastHPOCR/IndexHPO.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3491 2024-05-15 11:09:02.000000 FastHPOCR-0.1.0/FastHPOCR/IndexORPHANET.py
+-rw-r--r--   0 tudor      (501) staff       (20)     4492 2024-05-15 11:09:14.000000 FastHPOCR-0.1.0/FastHPOCR/IndexSNOMED.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3507 2024-05-06 04:11:34.000000 FastHPOCR-0.1.0/FastHPOCR/README.md
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-03-18 01:56:25.000000 FastHPOCR-0.1.0/FastHPOCR/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.368003 FastHPOCR-0.1.0/FastHPOCR/cr/
+-rw-r--r--   0 tudor      (501) staff       (20)     3621 2024-05-15 11:06:19.000000 FastHPOCR-0.1.0/FastHPOCR/cr/CRIndexKB.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1051 2024-02-21 03:39:40.000000 FastHPOCR-0.1.0/FastHPOCR/cr/CandidateMatcher.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3642 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/cr/FormatResults.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1734 2024-03-02 08:55:02.000000 FastHPOCR-0.1.0/FastHPOCR/cr/SequenceCache.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3675 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/cr/TextProcessor.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3875 2024-05-15 11:06:36.000000 FastHPOCR-0.1.0/FastHPOCR/cr/TextSplitter.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:40.000000 FastHPOCR-0.1.0/FastHPOCR/cr/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.369438 FastHPOCR-0.1.0/FastHPOCR/index/
+-rw-r--r--   0 tudor      (501) staff       (20)     1353 2024-05-15 13:43:03.000000 FastHPOCR-0.1.0/FastHPOCR/index/HPOLabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2323 2024-05-15 11:06:42.000000 FastHPOCR-0.1.0/FastHPOCR/index/IndexTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3564 2024-05-15 13:24:33.000000 FastHPOCR-0.1.0/FastHPOCR/index/LabelProcessor.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1062 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/index/ORPHALabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2508 2024-05-15 13:24:25.000000 FastHPOCR-0.1.0/FastHPOCR/index/PreprocessHPOTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2157 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/index/PreprocessORPHATerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2135 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/index/PreprocessSNOMEDTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1703 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/index/SNOMEDLabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3036 2024-05-02 09:49:49.000000 FastHPOCR-0.1.0/FastHPOCR/index/SNOMEDParser.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2556 2024-02-28 12:38:42.000000 FastHPOCR-0.1.0/FastHPOCR/index/SynonymExpader.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:32.000000 FastHPOCR-0.1.0/FastHPOCR/index/__init__.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1058 2024-03-18 01:51:44.000000 FastHPOCR-0.1.0/FastHPOCR/license.txt
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.369680 FastHPOCR-0.1.0/FastHPOCR/resources/
+-rw-r--r--   0 tudor      (501) staff       (20)     1385 2024-05-13 14:33:20.000000 FastHPOCR-0.1.0/FastHPOCR/resources/base-synonyms
+-rw-r--r--   0 tudor      (501) staff       (20)  6300038 2024-05-14 04:27:52.000000 FastHPOCR-0.1.0/FastHPOCR/resources/vocab.clusters.list
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.373534 FastHPOCR-0.1.0/FastHPOCR/util/
+-rw-r--r--   0 tudor      (501) staff       (20)      828 2024-02-20 02:33:16.000000 FastHPOCR-0.1.0/FastHPOCR/util/AnnotationObject.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1123 2024-05-15 11:07:20.000000 FastHPOCR-0.1.0/FastHPOCR/util/AnnotationToken.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1511 2024-05-02 10:33:44.000000 FastHPOCR-0.1.0/FastHPOCR/util/CRConstants.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1196 2024-05-14 04:26:12.000000 FastHPOCR-0.1.0/FastHPOCR/util/ContentUtil.py
+-rw-r--r--   0 tudor      (501) staff       (20)     4740 2024-05-15 11:07:31.000000 FastHPOCR-0.1.0/FastHPOCR/util/OntoReader.py
+-rw-r--r--   0 tudor      (501) staff       (20)    42275 2024-03-02 08:55:57.000000 FastHPOCR-0.1.0/FastHPOCR/util/SequenceData.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:36:52.000000 FastHPOCR-0.1.0/FastHPOCR/util/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.367069 FastHPOCR-0.1.0/FastHPOCR.egg-info/
+-rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-15 13:43:38.000000 FastHPOCR-0.1.0/FastHPOCR.egg-info/PKG-INFO
+-rw-r--r--   0 tudor      (501) staff       (20)     1190 2024-05-15 13:43:38.000000 FastHPOCR-0.1.0/FastHPOCR.egg-info/SOURCES.txt
+-rw-r--r--   0 tudor      (501) staff       (20)        1 2024-05-15 13:43:38.000000 FastHPOCR-0.1.0/FastHPOCR.egg-info/dependency_links.txt
+-rw-r--r--   0 tudor      (501) staff       (20)       10 2024-05-15 13:43:38.000000 FastHPOCR-0.1.0/FastHPOCR.egg-info/top_level.txt
+-rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-15 13:43:38.373690 FastHPOCR-0.1.0/PKG-INFO
+-rw-r--r--   0 tudor      (501) staff       (20)       38 2024-05-15 13:43:38.373865 FastHPOCR-0.1.0/setup.cfg
+-rw-r--r--   0 tudor      (501) staff       (20)      447 2024-05-15 13:43:25.000000 FastHPOCR-0.1.0/setup.py
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/HPOAnnotator.py` & `FastHPOCR-0.1.0/FastHPOCR/HPOAnnotator.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 class HPOAnnotator:
     crIndexKB = None
 
     def __init__(self, crDataFile):
         self.crIndexKB = CRIndexKB()
         self.crIndexKB.load(crDataFile)
 
-    def annotate(self, text) -> [AnnotationObject]:
+    def annotate(self, text: str, longestMatch = False) -> [AnnotationObject]:
         textProcessor = TextProcessor(self.crIndexKB)
         textProcessor.process(text)
 
         candidateMatcher = CandidateMatcher(self.crIndexKB)
         candidateMatcher.matchCandidates(textProcessor.getCandidates())
 
-        result = FormatResults(text, self.crIndexKB, candidateMatcher.getMatches()).getResult()
+        result = FormatResults(text, self.crIndexKB, candidateMatcher.getMatches(), longestMatch).getResult()
         return result
 
     def printResults(self, annotationList):
         lines = []
         for annotationObject in annotationList:
             lines.append(annotationObject.toString())
         print('\n'.join(lines))
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/IndexHPO.py` & `FastHPOCR-0.1.0/FastHPOCR/IndexORPHANET.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import os
+import pkgutil
 import time
 from os.path import join
-import pkgutil
 
 from FastHPOCR.cr.CRIndexKB import CRIndexKB
 from FastHPOCR.index.IndexTerms import IndexTerms
-from FastHPOCR.index.PreprocessOntologyTerms import PreprocessOntologyTerms
+from FastHPOCR.index.PreprocessORPHATerms import PreprocessORPHATerms
 from FastHPOCR.index.SynonymExpader import SynonymExpader
-from FastHPOCR.util.CRConstants import HP_INDEX_FILE, BASE_CLUSTERS, KB_FILE_POS_KB, BASE_SYNONYMS
+from FastHPOCR.util.CRConstants import BASE_CLUSTERS, BASE_SYNONYMS, ORPHA_INDEX_FILE
 
 
-class IndexHPO:
+class IndexORPHANET:
     resFolder = None
-    hpoLocation = None
+    orphaDataFile = None
     outputFolder = None
     valid = False
 
     clusters = {}
     synClusters = {}
     crIndexKB = None
 
-    def __init__(self, hpoLocation: str, outputFolder: str):
+    def __init__(self, orphaDataFile: str, outputFolder: str):
         self.resFolder = 'resources'
-        self.hpoLocation = hpoLocation
+        self.orphaDataFile = orphaDataFile
         self.outputFolder = outputFolder
         self.valid = False
         self.crIndexKB = CRIndexKB()
 
     def index(self):
         start = time.time()
         self.checkPrerequisites()
         if not self.valid:
             return
 
         self.loadPrerequisites()
-        print(' - Preprocessing ontology terms ...')
-        preprocessOntologyTerms = PreprocessOntologyTerms(self.hpoLocation)
+        print(' - Preprocessing ORPHA terms ...')
+        preprocessOntologyTerms = PreprocessORPHATerms(self.orphaDataFile)
         processedTerms = preprocessOntologyTerms.getProcessedTerms()
 
-        print(' - Indexing ontology terms ...')
+        print(' - Indexing ORPHA terms ...')
         indexTerms = IndexTerms(processedTerms, self.clusters, self.crIndexKB)
         termsToIndex = indexTerms.getTermsToIndex()
         voidTokens = indexTerms.getVoidTokens()
 
         synonymExpader = SynonymExpader(termsToIndex, voidTokens, self.synClusters)
         termsToIndex = synonymExpader.getTermsToIndex()
 
         print(' - Serializing index ...')
         self.crIndexKB.setHPOIndex(termsToIndex)
-        self.crIndexKB.serialize(join(self.outputFolder, HP_INDEX_FILE), self.clusters)
+        self.crIndexKB.serialize(join(self.outputFolder, ORPHA_INDEX_FILE), self.clusters)
         end = time.time()
-        print(' - HPO index created in {}s'.format(round(end - start, 2)))
+        print(' - ORPHA index created in {}s'.format(round(end - start, 2)))
 
     def loadPrerequisites(self):
         self.loadClusterData()
         self.loadSynClusters()
 
     def loadClusterData(self):
         self.clusters = {}
@@ -82,16 +82,16 @@
                     token = token.strip()
                     clusterSet.append(self.clusters[token])
                 for token in tokens:
                     token = token.strip()
                     self.synClusters[self.clusters[token]] = clusterSet
 
     def checkPrerequisites(self):
-        if not os.path.isfile(self.hpoLocation):
-            print('ERROR: Ontology file provided [{}] does not exist!'.format(self.hpoLocation))
+        if not os.path.isfile(self.orphaDataFile):
+            print('ERROR: Orphanet JSON data file provided [{}] does not exist!'.format(self.orphaDataFile))
             self.valid = False
             return
         if not os.path.isdir(self.outputFolder):
             print('ERROR: Output folder provided [{}] does not exist!'.format(self.outputFolder))
             self.valid = False
             return
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/README.md` & `FastHPOCR-0.1.0/FastHPOCR/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,29 +6,63 @@
 * Understanding the target ontology - and hence processing the ontology terms appropriately for text mining
 More concretely, it uses a pre-built large collection of clusters of morphologically-equivalent tokens - to address lexical variability - and to reduce the boundary detection step to spans containing only tokens belonging to ontology concepts. Pre-processing the domain knowledge to create the collection of clusters was performed using OpenAI’s gpt-4.0 model and the resulting vocabulary contains 573,507 tokens, which leads to virtually no updates needed.
 
 **FastHPOCR** was built for speed:
 * Indexing a new ontology version takes ~3min
 * Performing concept recognition on plain text: ~5s for 10,000 publication abstracts
 
+## v2.0
+
+In v2.0, the library was expanded to include the ability to index SNOMED-CT branches and the ORPHANET terminology.
+The accuracy of performing concept recognition using these two vocabularies has not been assessed yet.
+
 ## Usage
 
-### Indexing step
+### Indexing HPO
 
 Use `IndexHPO` to create an index from an existing HPO version:
 ```python
     from FastHPOCR.IndexHPO import IndexHPO
 
     indexHPO = IndexHPO(<hpoFileLocation>, <outputFolder>)
     indexHPO.index()
 ```
 where
-* `hpoFileLocation` is the path to the `hp.obo` file targeted for indexing
-* `outputFolder` is the path where the resulting index will be deposited
+* `hpoFileLocation` - path to the `hp.obo` file targeted for indexing
+* `outputFolder` - path where the resulting index will be deposited
+
+### Indexing SNOMED
+
+Use `IndexSNOMED` to create an index from an existing SNOMED version using a given root concept:
+```python
+    from FastHPOCR.IndexSNOMED import IndexSNOMED
+
+    indexSNOMED = IndexSNOMED(<descriptionFile>, <relationsFile>, <rootConcept>, <outputFolder>)
+    indexSNOMED.index()
+```
+where
+* `descriptionFile` - path to the SNOMED description file targeted for indexing - e.g., `sct2_Description_Full-en_INT_20230630.txt`
+* `relationsFile` - path to the SNOMED relations file - e.g., `sct2_Relationship_Full_INT_20230630.txt`
+* `rootConcept` - concept to be used as root for the branch of SNOMED to be indexed - e.g., `SCTID:64572001` or `64572001` (*Disease*)
+* `outputFolder` - path where the resulting index will be deposited
+
+**NOTE:** this functionality is intentionally targeting a particular branch of the terminology and not the terminology in its entirety. Hence, providing a `rootConcept` is mandatory.
 
+### Indexing ORPHANET
+
+Use `IndexORPHANET` to create an index from an existing HPO version:
+```python
+    from FastHPOCR.IndexORPHANET import IndexORPHANET
+
+    indexORPHANET = IndexORPHANET(<orphaDataFile>, <outputFolder>)
+    indexORPHANET.index()
+```
+where
+* `orphaDataFile` - path to the unpacked JSON Orphanet data file (`en_product1.json`) containing the definitions of the disorders
+* `outputFolder` - path where the resulting index will be deposited
 
 ### Concept recognition step
 
 Use `HPOAnnotator`
 
 ```python
     from FastHPOCR.HPOAnnotator import HPOAnnotator
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/cr/CRIndexKB.py` & `FastHPOCR-0.1.0/FastHPOCR/cr/CRIndexKB.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/cr/CandidateMatcher.py` & `FastHPOCR-0.1.0/FastHPOCR/cr/CandidateMatcher.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/cr/SequenceCache.py` & `FastHPOCR-0.1.0/FastHPOCR/cr/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/cr/TextProcessor.py` & `FastHPOCR-0.1.0/FastHPOCR/cr/TextProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,18 @@
                     candidateSig = self.toClusterSig(current)
                     lst = []
                     if candidateSig in self.candidates:
                         lst = self.candidates[candidateSig]
                     lst.append(current)
                     self.candidates[candidateSig] = lst
 
-                    seqMap = SequenceData.SEQ_DATA[len(current)]
+                    size = len(current)
+                    if size > 20:
+                        size = 20
+                    seqMap = SequenceData.SEQ_DATA[size]
 
                     for size in seqMap:
                         if size != len(current):
                             seqOptions = seqMap[size]
                             for array in seqOptions:
                                 self.expandCandidates(current, array)
                     current = []
@@ -55,15 +58,18 @@
             candidateSig = self.toClusterSig(current)
             lst = []
             if candidateSig in self.candidates:
                 lst = self.candidates[candidateSig]
             lst.append(current)
             self.candidates[candidateSig] = lst
 
-            seqMap = SequenceData.SEQ_DATA[len(current)]
+            size = len(current)
+            if size > 20:
+                size = 20
+            seqMap = SequenceData.SEQ_DATA[size]
 
             for size in seqMap:
                 if size != len(current):
                     seqOptions = seqMap[size]
                     for array in seqOptions:
                         self.expandCandidates(current, array)
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/cr/TextSplitter.py` & `FastHPOCR-0.1.0/FastHPOCR/cr/TextSplitter.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/index/IndexTerms.py` & `FastHPOCR-0.1.0/FastHPOCR/index/IndexTerms.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/index/LabelProcessor.py` & `FastHPOCR-0.1.0/FastHPOCR/index/LabelProcessor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,43 @@
-from FastHPOCR.util.CRConstants import PHENOTYPIC_ABNORMALITY
-
-
 class LabelProcessor:
-    ontoReader = None
     terms = {}
     labels = {}
     dupLabels = {}
+    allow3LetterAcronyms = False
 
-    def __init__(self, ontoReader):
-        self.ontoReader = ontoReader
-        self.terms = {}
+    def __init__(self, terms, allow3LetterAcronyms=False):
+        self.terms = terms
+        self.allow3LetterAcronyms = allow3LetterAcronyms
         self.labels = {}
         self.dupLabels = {}
 
         print(' - Processing labels ...')
-        self.collectTerms()
         self.processBracketsInLabels()
         print(' - Collected {} terms.'.format(len(self.terms)))
         print(' - Found {} duplicated labels.'.format(len(self.dupLabels)))
         for label in self.dupLabels:
             print(' -- {} -> {}'.format(label, self.dupLabels[label]))
         self.processDuplicates()
 
-    def collectTerms(self):
-        for uri in self.ontoReader.terms:
-            if PHENOTYPIC_ABNORMALITY in self.ontoReader.allSuperClasses[uri]:
-                label = self.ontoReader.terms[uri]
-                syns = []
-                if uri in self.ontoReader.synonyms:
-                    for syn in self.ontoReader.synonyms[uri]:
-                        if len(syn) < 4 and syn.isupper():
-                            continue
-                        syns.append(syn)
-                self.terms[uri] = {
-                    'label': label,
-                    'syns': syns
-                }
-
     def processBracketsInLabels(self):
         for uri in self.terms:
             label = self.terms[uri]['label']
             syns = self.terms[uri]['syns']
 
             newSyns = []
             if '(' in label:
                 label = self.processBrackets(label)
             for syn in syns:
                 procced = self.processBrackets(syn, isSyn=True)
                 if procced:
-                    if len(syn) < 4 and syn.isupper():
+                    size = 4
+                    if self.allow3LetterAcronyms:
+                        size = 3
+
+                    if len(syn) < size:
                         continue
                     newSyns.append(syn)
 
             self.terms[uri] = {
                 'label': label,
                 'syns': newSyns
             }
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/index/PreprocessOntologyTerms.py` & `FastHPOCR-0.1.0/FastHPOCR/index/PreprocessORPHATerms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from FastHPOCR.index.LabelProcessor import LabelProcessor
+from FastHPOCR.index.ORPHALabelCollector import ORPHALabelCollector
 from FastHPOCR.util import ContentUtil
 from FastHPOCR.util.CRConstants import VB_BLACKLIST, POS_LIST
-from FastHPOCR.util.OntoReader import OntoReader
 
 
-class PreprocessOntologyTerms:
-    ontoReader = None
+class PreprocessORPHATerms:
     processedTerms = {}
     terms = {}
 
-    def __init__(self, ontologyFile):
-        self.ontoReader = OntoReader(ontologyFile)
+    def __init__(self, orphaDataFile):
         self.processedTerms = {}
 
-        labelProcessor = LabelProcessor(self.ontoReader)
+        labelProcessor = LabelProcessor(ORPHALabelCollector(orphaDataFile).getTerms())
         self.terms = labelProcessor.getProcessedTerms()
 
         self.filterTerms()
 
     def filterTerms(self):
         for uri in self.terms:
             label = self.terms[uri]['label']
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/index/SynonymExpader.py` & `FastHPOCR-0.1.0/FastHPOCR/index/SynonymExpader.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/license.txt` & `FastHPOCR-0.1.0/FastHPOCR/license.txt`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/resources/base-synonyms` & `FastHPOCR-0.1.0/FastHPOCR/resources/base-synonyms`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-involvement,deformity,mutilation, malformation, changes, characteristics, disorder, defect, disability, dysfunction, difficulty, deficit, disturbance, abnormality, anomaly, manifestation, disrupted, difficult, problem, complication, issue, finding, alteration, degradation
+involvement,deformity,mutilation, malformation, changes, characteristics, disorder, defect, disability, dysfunction, difficulty, deficit, disturbance, abnormality, anomaly, manifestation, disrupted, difficult, problem, complication, issue, finding, alteration, degradation, dysregulation
 neonatal, birth, infancy
 edema, swelling
 bifid,duplication
 cutaneous, skin
 keratocyst,cyst
 cancer,tumor,neuroma,neurinoma
 outburst, burst
@@ -25,17 +25,17 @@
 oral, mouth, buccal
 scleral, intrascleral
 opacities, cataract
 puppet, aspect, disposition
 fists, hands
 paresis, palsy
 digit, finger
-reduced, decreased
-enlarged, increased, raised, elevated
-motor, movement
+reduced, decreased, diminished, low
+enlarged, increased, raised, elevated, high
+motor, movement, mobility
 colobomata, colomba
 nose, nasal
 tooth, dental
 external, outer
 internal, inner
 patch, spot
 diminished, lack
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/resources/vocab.clusters.list` & `FastHPOCR-0.1.0/FastHPOCR/resources/vocab.clusters.list`

 * *Files 0% similar despite different names*

```diff
@@ -1277,16 +1277,15 @@
 aob,aobs
 aofmd,aofmded,aofmder,aofmdest,aofmding,aofmds
 aoi,aoied,aoier,aoiest,aoiing,aois,aous,aouses,aouss
 aoii,aoiied,aoiier,aoiiest,aoiiing,aoiis,aoius,aoiuses,aoiuss
 aoiii,aoiiied,aoiiier,aoiiiest,aoiiiing,aoiiis,aoiius,aoiiuses,aoiiuss
 aom,aoms
 aop,aops
-aorta,aortae,aortas
-aortic
+aorta,aortae,aortas,aortic,aortal,aortarctia
 aortici,aorticu,aorticued,aorticuing,aorticus,aorticused,aorticuser,aorticuses,aorticusest,aorticusing,aorticuss,aorticussed,aorticusser,aorticussest,aorticussing
 aorticopulmonary
 aorticorenal
 aortitides,aortitis
 aorto,aortoed,aortoer,aortoes,aortoest,aortoing,aortos
 aortopulmonary
 aosd
@@ -1777,16 +1776,15 @@
 aurocephalosyndactylied,aurocephalosyndactylier,aurocephalosyndactylies,aurocephalosyndactyliest,aurocephalosyndactyly,aurocephalosyndactylyed,aurocephalosyndactylyer,aurocephalosyndactylyest,aurocephalosyndactylying,aurocephalosyndactylys
 auscultation
 auscultatory
 ausem,ausemed,auseming,ausemmed,ausemming,ausems,ausemsed,ausemser,ausemses,ausemsest,ausemsing,ausemss
 austin,austins
 australian,australians
 australis
-autism,autisms
-autistic,autistics
+autism,autisms,autistic,autistics
 auto,autos
 autoagressia,autoagression,autoagressioned,autoagressioner,autoagressionest,autoagressioning,autoagressions
 autoamputation
 autoantibodies,autoantibody
 autoantigen,autoantigens
 autodesmosome,autodesmosomes
 autoerythrocyte,autoerythrocytes
@@ -2898,16 +2896,15 @@
 calcul
 calculi,calculus,calculuses
 caldag,caldaged,caldager,caldagest,caldagged,caldagger,caldaggest,caldagging,caldaging,caldags
 calderón,calderóned,calderóner,calderónest,calderóning,calderónned,calderónner,calderónnest,calderónning,calderóns
 calf,calve,calved,calves,calving
 caliber
 calibre
-caliceal
-calices,calix,calixes
+calices,calix,calixes,caliceal,calyceal
 caliciviridae
 caliectasis
 california
 californian,californians
 calja,caljae,caljaed,caljaer,caljaest,caljaing,caljas,caljon,caljons,caljum,caljums
 call,called,calling,calls
 calleja,callejas
@@ -4375,16 +4372,15 @@
 corectopia
 cori,coris
 corin
 corino,corinoed,corinoer,corinoes,corinoest,corinoing,corinos
 cork,corked,corking,corks
 cormane,cormaned,cormaneed,cormaneer,cormaneest,cormaneing,cormaner,cormanes,cormanest,cormaning
 cormie,cormieer,cormieest,cormier,cormiered,cormierer,cormierest,cormiering,cormiers,cormiest,cormy,cormyer,cormyest
-cornea,corneae,corneas,corneum
-corneal
+cornea,corneae,corneas,corneum,corneal
 cornelia,cornelias
 corneo,corneoed,corneoer,corneoest,corneoing,corneos
 corneocyte,corneocytes
 corneogoniodysgeneses,corneogoniodysgenesi,corneogoniodysgenesides,corneogoniodysgenesied,corneogoniodysgenesiing,corneogoniodysgenesis,corneogoniodysgenesised,corneogoniodysgenesiser,corneogoniodysgenesises,corneogoniodysgenesisest,corneogoniodysgenesising,corneogoniodysgenesiss,corneogoniodysgenesissed,corneogoniodysgenesisser,corneogoniodysgenesissest,corneogoniodysgenesissing
 corneoiridogoniodysgeneses,corneoiridogoniodysgenesi,corneoiridogoniodysgenesides,corneoiridogoniodysgenesied,corneoiridogoniodysgenesiing,corneoiridogoniodysgenesis,corneoiridogoniodysgenesised,corneoiridogoniodysgenesiser,corneoiridogoniodysgenesises,corneoiridogoniodysgenesisest,corneoiridogoniodysgenesising,corneoiridogoniodysgenesiss,corneoiridogoniodysgenesissed,corneoiridogoniodysgenesisser,corneoiridogoniodysgenesissest,corneoiridogoniodysgenesissing
 corneolenticular,corneolenticulared,corneolenticularer,corneolenticularest,corneolenticularing,corneolenticularred,corneolenticularrer,corneolenticularrest,corneolenticularring,corneolenticulars
 corneoretinal
@@ -5480,26 +5476,23 @@
 dilatation,dilatations,dilate,dilated,dilates,dilating,dilation,dilations
 dilatator,dilatators
 dilator,dilators
 dile,diled,dileed,dileer,dileest,dileing,diler,diles,dilest,diling,dille,dilled,dilleed,dilleing,dilles,dilling,dillinged,dillinger,dillingest,dillinging,dillings,dills,dillung
 dillies,dilly,dillys
 dillon,dillons
 dilo,diloed,diloes,diloing,dilos,dilosed,diloser,diloses,dilosest,dilosing,diloss,dilossed,dilosser,dilossest,dilossing
-dilute,diluted,dilutes,diluting
-dilution,dilutions
+dilute,diluted,dilutes,diluting,dilution,dilutions
 dim,dimmed,dimmer,dimmers,dimmest,dimming,dims
 dimelia
 dimension,dimensions
-dimer,dimers
-dimeric
+dimer,dimers,dimeric
 dimethylglycine
 diminish,diminished,diminishes,diminishing
 dimitri,dimitris
-dimorphic
-dimorphous
+dimorphic,dimorphous
 dimple,dimpled,dimples,dimpling
 din,dinned,dinning,dins
 dincsoy,dincsoyed,dincsoyer,dincsoyest,dincsoying,dincsoys,dincsoyyed,dincsoyyer,dincsoyyest,dincsoyying
 dingwall,dingwalls
 dinno,dinnoed,dinnoer,dinnoes,dinnoest,dinnoing,dinnos
 dioctophyme
 dioctophymiases,dioctophymiasi,dioctophymiasides,dioctophymiasied,dioctophymiasiing,dioctophymiasis,dioctophymiasised,dioctophymiasiser,dioctophymiasises,dioctophymiasisest,dioctophymiasising,dioctophymiasiss,dioctophymiasissed,dioctophymiasisser,dioctophymiasissest,dioctophymiasissing
@@ -9723,16 +9716,15 @@
 hypermelanotic
 hypermenorrhea
 hypermetabolism
 hypermethioninemia
 hypermethylation,hypermethylations
 hypermetric
 hypermetropia
-hypermobile
-hypermobilities,hypermobility
+hypermobile,hypermobilities,hypermobility
 hypermorphic
 hypermutation,hypermutations
 hypermyelinat,hypermyelinate,hypermyelinated,hypermyelinatedded,hypermyelinatedder,hypermyelinateddest,hypermyelinatedding,hypermyelinateded,hypermyelinateder,hypermyelinatedest,hypermyelinateding,hypermyelinateds,hypermyelinateed,hypermyelinateeded,hypermyelinateeding,hypermyelinateeds,hypermyelinateing,hypermyelinates,hypermyelinating,hypermyelinats,hypermyelinatted,hypermyelinatting
 hypermyelinatia,hypermyelination,hypermyelinationed,hypermyelinationer,hypermyelinationest,hypermyelinationing,hypermyelinations
 hypernasal
 hypernatraemia,hypernatraemias
 hypernatremia,hypernatremias
@@ -20225,18 +20217,15 @@
 stephan,stephaned,stephaner,stephanest,stephaning,stephanned,stephanner,stephannest,stephanning,stephans
 stephanion,stephanioned,stephanioner,stephanionest,stephanioning,stephanions
 steppage
 stercoraceous
 stercoral
 stereocilia,stereocilium
 stereopses,stereopsis
-stereotype,stereotyped,stereotypes,stereotyping
-stereotypic
-stereotypical
-stereotypies,stereotypy
+stereotype,stereotyped,stereotypes,stereotyping,stereotypic,stereotypical,stereotypies,stereotypy
 sterile,steriles
 sterilities,sterility
 stern,sterner,sternest,sterns
 sterna,sternum,sternums
 sternal
 sternales,sternalis
 sternberg,sternbergs
@@ -22876,16 +22865,15 @@
 wholly
 whoop,whooped,whooping,whoops
 whorl,whorled,whorling,whorls
 whr,whrs
 whrn,whrned,whrner,whrnest,whrning,whrns
 whsi,whsu,whsued,whsuing,whsus,whsused,whsuser,whsuses,whsusest,whsusing,whsuss,whsussed,whsusser,whsussest,whsussing
 whyte,whyted,whyteed,whyteer,whyteest,whyteing,whyter,whytes,whytest,whyting
-wide,widen,widened,widening,widens,wider,wides,widest
-widely
+wide,widen,widened,widening,widens,wider,wides,widest,widely
 widow,widows
 width,widths
 wieack,wieacke,wieackeer,wieackeest,wieacker,wieackered,wieackerer,wieackerest,wieackering,wieackerred,wieackerrer,wieackerrest,wieackerring,wieackers,wieackest
 wiedemann,wiedemanns
 wiedmann,wiedmanned,wiedmanner,wiedmannest,wiedmanning,wiedmanns
 wiethe,wiethes
 wilbrandt,wilbrandted,wilbrandter,wilbrandtest,wilbrandting,wilbrandts
@@ -35081,15 +35069,14 @@
 aonach
 aonema
 aonian
 aonite
 aorist
 aoristic,aorists
 aoristically
-aortal,aortarctia
 aortalgia
 aortectasia,aortectasis,aortectomy
 aortenbogen
 aortenruptur
 aortenstenose
 aortenstenosen
 aortica,aortico,aorticum,aortism
@@ -56974,15 +56961,15 @@
 calvous
 calvum,calvus
 calxes
 calybite
 calycanth,calycate
 calycanthaceae,calycanthaceous,calycanthin,calycanthine,calycanthus
 calycanthemous,calycanthemy
-calyceal,calycectasis,calycectomy
+calycectasis,calycectomy
 calyceraceae,calyceraceous
 calyciferous,calyciform
 calycifloral,calyciflorate,calyciflorous
 calycina,calycinal,calycine
 calycle,calycli
 calycled,calycles
 calycocarpum,calycoid,calycosum
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/util/AnnotationObject.py` & `FastHPOCR-0.1.0/FastHPOCR/util/AnnotationObject.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/util/AnnotationToken.py` & `FastHPOCR-0.1.0/FastHPOCR/util/AnnotationToken.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/util/CRConstants.py` & `FastHPOCR-0.1.0/FastHPOCR/util/CRConstants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 NULL = 'NULL'
 POS_CD = 'CD'
 POS_NN = 'NN'
 LABEL = 'LABEL'
 LAYPERSON = 'LAYPERSON'
 PHENOTYPIC_ABNORMALITY = 'HP:0000118'
+SCTID_PREFIX = 'SCTID:'
+ORPHA_PREFIX = 'ORPHA:'
 
 BASE_CLUSTERS = 'vocab.clusters.list'
 HP_INDEX_FILE = 'hp.index'
+SNOMED_INDEX_FILE = 'snomed.index'
+ORPHA_INDEX_FILE = 'orpha.index'
 KB_FILE_POS_KB = 'posKB.kb'
 BASE_SYNONYMS = 'base-synonyms'
 
 POS_FILTER = ['IN', 'DT', 'CC']
 
 POS_LIST_FULL = ['of',
             'the',
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/util/ContentUtil.py` & `FastHPOCR-0.1.0/FastHPOCR/util/ContentUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     return text
 
 
 def cleanToken(token):
     token = token.lower()
     token = token.replace('"', '')
     token = token.replace('\'', '')
+    token = token.replace('’', '')
     token = token.replace(',', '')
     token = token.replace('.', '')
     token = token.replace('>', '')
     token = token.replace('<', '')
     token = token.replace('%', '')
     token = token.replace(')', '')
     token = token.replace('(', '')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FastHPOCR-0.0.1/FastHPOCR/util/OntoReader.py` & `FastHPOCR-0.1.0/FastHPOCR/util/OntoReader.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.0.1/FastHPOCR/util/SequenceData.py` & `FastHPOCR-0.1.0/FastHPOCR/util/SequenceData.py`

 * *Files identical despite different names*

