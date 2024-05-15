# Comparing `tmp/pypantera-0.0.1.tar.gz` & `tmp/pypantera-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypantera-0.0.1.tar", last modified: Thu Apr  4 13:09:25 2024, max compression
+gzip compressed data, was "pypantera-1.0.0.tar", last modified: Wed May 15 15:37:10 2024, max compression
```

## Comparing `pypantera-0.0.1.tar` & `pypantera-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,33 @@
-drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-04-04 13:09:25.185325 pypantera-0.0.1/
--rw-rw-r--   0 kdf       (1000) kdf       (1000)    35149 2024-04-04 07:28:43.000000 pypantera-0.0.1/LICENSE
--rw-rw-r--   0 kdf       (1000) kdf       (1000)     1845 2024-04-04 13:09:25.185325 pypantera-0.0.1/PKG-INFO
--rw-rw-r--   0 kdf       (1000) kdf       (1000)     1356 2024-04-04 13:03:18.000000 pypantera-0.0.1/README.md
-drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-04-04 13:09:25.177325 pypantera-0.0.1/pypantera/
--rw-rw-r--   0 kdf       (1000) kdf       (1000)       29 2024-04-04 13:04:59.000000 pypantera-0.0.1/pypantera/__init__.py
--rw-rw-r--   0 kdf       (1000) kdf       (1000)      110 2024-04-04 13:04:49.000000 pypantera-0.0.1/pypantera/main.py
-drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-04-04 13:09:25.185325 pypantera-0.0.1/pypantera.egg-info/
--rw-rw-r--   0 kdf       (1000) kdf       (1000)     1845 2024-04-04 13:09:25.000000 pypantera-0.0.1/pypantera.egg-info/PKG-INFO
--rw-rw-r--   0 kdf       (1000) kdf       (1000)      230 2024-04-04 13:09:25.000000 pypantera-0.0.1/pypantera.egg-info/SOURCES.txt
--rw-rw-r--   0 kdf       (1000) kdf       (1000)        1 2024-04-04 13:09:25.000000 pypantera-0.0.1/pypantera.egg-info/dependency_links.txt
--rw-rw-r--   0 kdf       (1000) kdf       (1000)       19 2024-04-04 13:09:25.000000 pypantera-0.0.1/pypantera.egg-info/requires.txt
--rw-rw-r--   0 kdf       (1000) kdf       (1000)       10 2024-04-04 13:09:25.000000 pypantera-0.0.1/pypantera.egg-info/top_level.txt
--rw-rw-r--   0 kdf       (1000) kdf       (1000)       38 2024-04-04 13:09:25.185325 pypantera-0.0.1/setup.cfg
--rw-rw-r--   0 kdf       (1000) kdf       (1000)      976 2024-04-04 13:07:45.000000 pypantera-0.0.1/setup.py
+drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:37:10.438193 pypantera-1.0.0/
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)    35149 2024-05-15 15:16:58.000000 pypantera-1.0.0/LICENSE
+-rw-r--r--   0 kdf       (1000) kdf       (1000)    15395 2024-05-15 15:37:10.438193 pypantera-1.0.0/PKG-INFO
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)    11120 2024-05-15 15:16:58.000000 pypantera-1.0.0/README.md
+drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:37:10.437193 pypantera-1.0.0/pypantera/
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/__init__.py
+drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:37:10.438193 pypantera-1.0.0/pypantera/pypantera.egg-info/
+-rw-r--r--   0 kdf       (1000) kdf       (1000)    15395 2024-05-15 15:37:10.000000 pypantera-1.0.0/pypantera/pypantera.egg-info/PKG-INFO
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     1045 2024-05-15 15:37:10.000000 pypantera-1.0.0/pypantera/pypantera.egg-info/SOURCES.txt
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)        1 2024-05-15 15:37:10.000000 pypantera-1.0.0/pypantera/pypantera.egg-info/dependency_links.txt
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     1716 2024-05-15 15:37:10.000000 pypantera-1.0.0/pypantera/pypantera.egg-info/requires.txt
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)       13 2024-05-15 15:37:10.000000 pypantera-1.0.0/pypantera/pypantera.egg-info/top_level.txt
+drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:37:10.437193 pypantera-1.0.0/pypantera/src/
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     3794 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/AbstractTextObfuscationDPMechanism.py
+drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:37:10.437193 pypantera-1.0.0/pypantera/src/EmbeddingPerturbationMechanism/
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     2873 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/EmbeddingPerturbationMechanism/AbstractEmbeddingPerturbationMechanism.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/EmbeddingPerturbationMechanism/__init__.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     5290 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/EmbeddingPerturbationMechanism/cmp.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     6418 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/EmbeddingPerturbationMechanism/mahalanobis.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)    10171 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/EmbeddingPerturbationMechanism/vickrey.py
+drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:37:10.437193 pypantera-1.0.0/pypantera/src/SamplingPerturbationMechanism/
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     1829 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/SamplingPerturbationMechanism/AbstractSamplingPerturbationMechanism.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/SamplingPerturbationMechanism/__init__.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     6361 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/SamplingPerturbationMechanism/custext.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     3965 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/SamplingPerturbationMechanism/santext.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     7316 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/SamplingPerturbationMechanism/tem.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/__init__.py
+drwxrwxr-x   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:37:10.438193 pypantera-1.0.0/pypantera/src/utils/
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)        0 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/utils/__init__.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     8038 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/utils/helper.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     1649 2024-05-15 15:16:58.000000 pypantera-1.0.0/pypantera/src/utils/vocab.py
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)       38 2024-05-15 15:37:10.438193 pypantera-1.0.0/setup.cfg
+-rw-rw-r--   0 kdf       (1000) kdf       (1000)     8120 2024-05-15 15:37:06.000000 pypantera-1.0.0/setup.py
```

### Comparing `pypantera-0.0.1/LICENSE` & `pypantera-1.0.0/LICENSE`

 * *Files identical despite different names*

