# Comparing `tmp/diffpass-0.1.0.tar.gz` & `tmp/diffpass-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffpass-0.1.0.tar", last modified: Fri May 10 11:24:25 2024, max compression
+gzip compressed data, was "diffpass-0.1.1.tar", last modified: Tue May 14 15:58:57 2024, max compression
```

## Comparing `diffpass-0.1.0.tar` & `diffpass-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-10 11:24:25.479231 diffpass-0.1.0/
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    11337 2023-08-31 17:21:49.000000 diffpass-0.1.0/LICENSE
--rw-rw-r--   0 lupo      (1001) lupo      (1001)      111 2023-08-31 17:21:49.000000 diffpass-0.1.0/MANIFEST.in
--rw-r--r--   0 lupo      (1001) lupo      (1001)    10887 2024-05-10 11:24:25.479231 diffpass-0.1.0/PKG-INFO
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     9745 2024-05-10 09:39:56.000000 diffpass-0.1.0/README.md
-drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-10 11:24:25.475231 diffpass-0.1.0/diffpass/
--rw-rw-r--   0 lupo      (1001) lupo      (1001)       22 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/__init__.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    26907 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/_modidx.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    26072 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/base.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     3660 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/constants.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    10162 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/data_utils.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     1700 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/entropy_ops.py
--rw-r--r--   0 lupo      (1001) lupo      (1001)     5360 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/gumbel_sinkhorn_ops.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     2263 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/ipa_utils.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    23338 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/model.py
--rw-r--r--   0 lupo      (1001) lupo      (1001)     1291 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/msa_parsing.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     4621 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/sequence_similarity_ops.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    17749 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/train.py
-drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-10 11:24:25.475231 diffpass-0.1.0/diffpass.egg-info/
--rw-r--r--   0 lupo      (1001) lupo      (1001)    10887 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/PKG-INFO
--rw-rw-r--   0 lupo      (1001) lupo      (1001)      553 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/SOURCES.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)        1 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/dependency_links.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)       38 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/entry_points.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)        1 2024-02-19 12:44:53.000000 diffpass-0.1.0/diffpass.egg-info/not-zip-safe
--rw-rw-r--   0 lupo      (1001) lupo      (1001)       89 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/requires.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)        9 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/top_level.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     1009 2024-05-10 11:22:19.000000 diffpass-0.1.0/settings.ini
--rw-rw-r--   0 lupo      (1001) lupo      (1001)       38 2024-05-10 11:24:25.479231 diffpass-0.1.0/setup.cfg
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     2596 2023-08-31 17:21:49.000000 diffpass-0.1.0/setup.py
+drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-14 15:58:57.756825 diffpass-0.1.1/
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    11337 2023-08-31 17:21:49.000000 diffpass-0.1.1/LICENSE
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)      111 2023-08-31 17:21:49.000000 diffpass-0.1.1/MANIFEST.in
+-rw-r--r--   0 lupo      (1001) lupo      (1001)    10637 2024-05-14 15:58:57.756825 diffpass-0.1.1/PKG-INFO
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     9495 2024-05-14 12:50:47.000000 diffpass-0.1.1/README.md
+drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-14 15:58:57.756825 diffpass-0.1.1/diffpass/
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)       22 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/__init__.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    26907 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/_modidx.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    27651 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/base.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     3660 2024-05-14 15:54:25.000000 diffpass-0.1.1/diffpass/constants.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    10162 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/data_utils.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     1700 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/entropy_ops.py
+-rw-r--r--   0 lupo      (1001) lupo      (1001)     5360 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/gumbel_sinkhorn_ops.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     2263 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/ipa_utils.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    24218 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/model.py
+-rw-r--r--   0 lupo      (1001) lupo      (1001)     1291 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/msa_parsing.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     4621 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/sequence_similarity_ops.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    17749 2024-05-14 15:54:26.000000 diffpass-0.1.1/diffpass/train.py
+drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-14 15:58:57.756825 diffpass-0.1.1/diffpass.egg-info/
+-rw-r--r--   0 lupo      (1001) lupo      (1001)    10637 2024-05-14 15:58:57.000000 diffpass-0.1.1/diffpass.egg-info/PKG-INFO
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)      553 2024-05-14 15:58:57.000000 diffpass-0.1.1/diffpass.egg-info/SOURCES.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)        1 2024-05-14 15:58:57.000000 diffpass-0.1.1/diffpass.egg-info/dependency_links.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)       38 2024-05-14 15:58:57.000000 diffpass-0.1.1/diffpass.egg-info/entry_points.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)        1 2024-02-19 12:44:53.000000 diffpass-0.1.1/diffpass.egg-info/not-zip-safe
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)       89 2024-05-14 15:58:57.000000 diffpass-0.1.1/diffpass.egg-info/requires.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)        9 2024-05-14 15:58:57.000000 diffpass-0.1.1/diffpass.egg-info/top_level.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     1009 2024-05-14 15:58:43.000000 diffpass-0.1.1/settings.ini
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)       38 2024-05-14 15:58:57.756825 diffpass-0.1.1/setup.cfg
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     2596 2023-08-31 17:21:49.000000 diffpass-0.1.1/setup.py
```

### Comparing `diffpass-0.1.0/LICENSE` & `diffpass-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/PKG-INFO` & `diffpass-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffpass
-Version: 0.1.0
+Version: 0.1.1
 Summary: Differentiable Pairing using Soft Scores
 Home-page: https://github.com/Bitbol-Lab/DiffPaSS
 Author: Umberto Lupo and Damiano Sgarbossa
 Author-email: umberto.lupo@epfl.ch, damiano.sgarbossa@epfl.ch
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -45,15 +45,15 @@
 
 A typical example of the problem DiffPaSS is designed to solve is the
 following: given two multiple sequence alignments (MSAs) A and B,
 containing interacting biological sequences, find the optimal one-to-one
 pairing between the sequences in A and B.
 
 <figure>
-<img src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/MSA_pairing_problem.svg" alt="MSA pairing problem" />
+<img src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/MSA_pairing_problem.svg" width="640" height="201.6" alt="MSA pairing problem" />
 <figcaption>
 Pairing problem for two multiple sequence alignments, where pairings are
 restricted to be within the same species
 </figcaption>
 </figure>
 
 To find an optimal pairing, we can maximize the average mutual
@@ -113,15 +113,15 @@
 
 4.  A notion of “robust pairs” that can be used to identify pairs that
     are consistently found throughout a DiffPaSS bootstrap. These pairs
     can be used as ground truths in another DiffPaSS run, giving rise to
     the DiffPaSS-Iterative Pairing Algorithm (DiffPaSS-IPA).
 
 <figure>
-<video src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/DiffPaSS_bootstrap.mp4" width="432" height="243" controls>
+<video src="https://github.com/Bitbol-Lab/DiffPaSS/assets/46537483/e411fe8c-2fed-4723-a25c-ff69a1abccec" width="640" height="360" controls>
 </video>
 <figcaption>
 The DiffPaSS bootstrap technique and robust pairs
 </figcaption>
 </figure>
 
 ## Installation
@@ -158,17 +158,17 @@
 First, parse your multiple sequence alignments (MSAs) in FASTA format
 into a list of tuples `(header, sequence)` using
 [`read_msa`](https://Bitbol-Lab.github.io/DiffPaSS/msa_parsing.html#read_msa).
 
 ``` python
 from diffpass.msa_parsing import read_msa
 
-# Parse and one-hot encode the MSAs
-msa_data_A = read_msa("path/to/msa_A.fasta")
-msa_data_B = read_msa("path/to/msa_B.fasta")
+# Parse the MSAs into lists of tuples (header, sequence)
+msa_A = read_msa("path/to/msa_A.fasta")
+msa_B = read_msa("path/to/msa_B.fasta")
 ```
 
 We assume that the MSAs contain species information in the headers,
 which will be used to restrict the pairings to be within the same
 species (more generally, “groups”). We need a simple function to extract
 the species information from the headers. For instance, if the headers
 are in the format `>sequence_id|species_name|...`, we can use:
@@ -179,72 +179,77 @@
 ```
 
 This function will be used to group the sequences by species:
 
 ``` python
 from diffpass.data_utils import create_groupwise_seq_records
 
-msa_data_A_species_by_species = create_groupwise_seq_records(msa_data_A, species_name_func)
-msa_data_B_species_by_species = create_groupwise_seq_records(msa_data_B, species_name_func)
+msa_A_by_sp = create_groupwise_seq_records(msa_A, species_name_func)
+msa_B_by_sp = create_groupwise_seq_records(msa_B, species_name_func)
 ```
 
 If one of the MSAs contains sequences from species not present in the
 other MSA, we can remove these species from both MSAs:
 
 ``` python
 from diffpass.data_utils import remove_groups_not_in_both
 
-msa_data_A_species_by_species, msa_data_B_species_by_species = remove_groups_not_in_both(
-    msa_data_A_species_by_species, msa_data_B_species_by_species
+msa_A_by_sp, msa_B_by_sp = remove_groups_not_in_both(
+    msa_A_by_sp, msa_B_by_sp
 )
 ```
 
 If there are species with different numbers of sequences in the two
 MSAs, we can add dummy sequences to the smaller species to make the
 number of sequences equal. For example, we can add dummy sequences
 consisting entirely of gap symbols:
 
 ``` python
 from diffpass.data_utils import pad_msas_with_dummy_sequences
 
-msa_data_A_species_by_species_padded, msa_data_B_species_by_species_padded = pad_msas_with_dummy_sequences(
-    msa_data_A_species_by_species, msa_data_B_species_by_species
+msa_A_by_sp_pad, msa_B_by_sp_pad = pad_msas_with_dummy_sequences(
+    msa_A_by_sp, msa_B_by_sp
 )
 
-species = list(msa_data_A_species_by_species_padded.keys())
-species_sizes = list(map(len, msa_data_A_species_by_species_padded.values()))
+species = list(msa_A_by_sp_pad.keys())
+species_sizes = list(map(len, msa_A_by_sp_pad.values()))
 ```
 
 Next, one-hot encode the MSAs using the
 [`one_hot_encode_msa`](https://Bitbol-Lab.github.io/DiffPaSS/data_utils.html#one_hot_encode_msa)
 function.
 
 ``` python
 from diffpass.data_utils import one_hot_encode_msa
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
 # Unpack the padded MSAs into a list of records
-msa_data_A_for_pairing = [record for records_this_species in msa_data_A_species_by_species_padded.values() for record in records_this_species]
-msa_data_B_for_pairing = [record for records_this_species in msa_data_B_species_by_species_padded.values() for record in records_this_species]
+msa_A_for_pairing = [
+    rec for recs_this_sp in msa_A_by_sp_pad.values() for rec in recs_this_sp
+]
+msa_B_for_pairing = [
+    rec for recs_this_sp in msa_B_by_sp_pad.values() for rec in recs_this_sp
+]
 
 # One-hot encode the MSAs and load them to a device
-msa_A_oh = one_hot_encode_msa(msa_data_A_for_pairing, device=device)
-msa_B_oh = one_hot_encode_msa(msa_data_B_for_pairing, device=device)
+msa_A_oh = one_hot_encode_msa(msa_A_for_pairing, device=device)
+msa_B_oh = one_hot_encode_msa(msa_B_for_pairing, device=device)
 ```
 
 ### Pairing optimization
 
 Finally, we can instantiate an
 [`InformationPairing`](https://Bitbol-Lab.github.io/DiffPaSS/train.html#informationpairing)
 object and optimize the mutual information between the paired MSAs using
-the DiffPaSS bootstrap algorithm. The results are stored in a
+the DiffPaSS bootstrapped optimization algorithm. The results are stored
+in a
 [`DiffPaSSResults`](https://Bitbol-Lab.github.io/DiffPaSS/base.html#diffpassresults)
-container. The lists of (hard) losses and permutations found can be
-accessed as attributes of the container.
+container. The lists of (hard) losses and permutations found during the
+optimization can be accessed as attributes of the container.
 
 ``` python
 from diffpass.train import InformationPairing
 
 information_pairing = InformationPairing(group_sizes=species_sizes).to(device)
 bootstrap_results = information_pairing.fit_bootstrap(x, y)
```

### Comparing `diffpass-0.1.0/README.md` & `diffpass-0.1.1/diffpass.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: diffpass
+Version: 0.1.1
+Summary: Differentiable Pairing using Soft Scores
+Home-page: https://github.com/Bitbol-Lab/DiffPaSS
+Author: Umberto Lupo and Damiano Sgarbossa
+Author-email: umberto.lupo@epfl.ch, damiano.sgarbossa@epfl.ch
+License: Apache Software License 2.0
+Keywords: nbdev jupyter notebook python
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: biopython
+Requires-Dist: tqdm
+Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+
 # DiffPaSS – Differentiable Pairing using Soft Scores
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Overview
 
 DiffPaSS is a family of high-performance and scalable PyTorch modules
@@ -12,15 +45,15 @@
 
 A typical example of the problem DiffPaSS is designed to solve is the
 following: given two multiple sequence alignments (MSAs) A and B,
 containing interacting biological sequences, find the optimal one-to-one
 pairing between the sequences in A and B.
 
 <figure>
-<img src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/MSA_pairing_problem.svg" alt="MSA pairing problem" />
+<img src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/MSA_pairing_problem.svg" width="640" height="201.6" alt="MSA pairing problem" />
 <figcaption>
 Pairing problem for two multiple sequence alignments, where pairings are
 restricted to be within the same species
 </figcaption>
 </figure>
 
 To find an optimal pairing, we can maximize the average mutual
@@ -80,15 +113,15 @@
 
 4.  A notion of “robust pairs” that can be used to identify pairs that
     are consistently found throughout a DiffPaSS bootstrap. These pairs
     can be used as ground truths in another DiffPaSS run, giving rise to
     the DiffPaSS-Iterative Pairing Algorithm (DiffPaSS-IPA).
 
 <figure>
-<video src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/DiffPaSS_bootstrap.mp4" width="432" height="243" controls>
+<video src="https://github.com/Bitbol-Lab/DiffPaSS/assets/46537483/e411fe8c-2fed-4723-a25c-ff69a1abccec" width="640" height="360" controls>
 </video>
 <figcaption>
 The DiffPaSS bootstrap technique and robust pairs
 </figcaption>
 </figure>
 
 ## Installation
@@ -125,17 +158,17 @@
 First, parse your multiple sequence alignments (MSAs) in FASTA format
 into a list of tuples `(header, sequence)` using
 [`read_msa`](https://Bitbol-Lab.github.io/DiffPaSS/msa_parsing.html#read_msa).
 
 ``` python
 from diffpass.msa_parsing import read_msa
 
-# Parse and one-hot encode the MSAs
-msa_data_A = read_msa("path/to/msa_A.fasta")
-msa_data_B = read_msa("path/to/msa_B.fasta")
+# Parse the MSAs into lists of tuples (header, sequence)
+msa_A = read_msa("path/to/msa_A.fasta")
+msa_B = read_msa("path/to/msa_B.fasta")
 ```
 
 We assume that the MSAs contain species information in the headers,
 which will be used to restrict the pairings to be within the same
 species (more generally, “groups”). We need a simple function to extract
 the species information from the headers. For instance, if the headers
 are in the format `>sequence_id|species_name|...`, we can use:
@@ -146,72 +179,77 @@
 ```
 
 This function will be used to group the sequences by species:
 
 ``` python
 from diffpass.data_utils import create_groupwise_seq_records
 
-msa_data_A_species_by_species = create_groupwise_seq_records(msa_data_A, species_name_func)
-msa_data_B_species_by_species = create_groupwise_seq_records(msa_data_B, species_name_func)
+msa_A_by_sp = create_groupwise_seq_records(msa_A, species_name_func)
+msa_B_by_sp = create_groupwise_seq_records(msa_B, species_name_func)
 ```
 
 If one of the MSAs contains sequences from species not present in the
 other MSA, we can remove these species from both MSAs:
 
 ``` python
 from diffpass.data_utils import remove_groups_not_in_both
 
-msa_data_A_species_by_species, msa_data_B_species_by_species = remove_groups_not_in_both(
-    msa_data_A_species_by_species, msa_data_B_species_by_species
+msa_A_by_sp, msa_B_by_sp = remove_groups_not_in_both(
+    msa_A_by_sp, msa_B_by_sp
 )
 ```
 
 If there are species with different numbers of sequences in the two
 MSAs, we can add dummy sequences to the smaller species to make the
 number of sequences equal. For example, we can add dummy sequences
 consisting entirely of gap symbols:
 
 ``` python
 from diffpass.data_utils import pad_msas_with_dummy_sequences
 
-msa_data_A_species_by_species_padded, msa_data_B_species_by_species_padded = pad_msas_with_dummy_sequences(
-    msa_data_A_species_by_species, msa_data_B_species_by_species
+msa_A_by_sp_pad, msa_B_by_sp_pad = pad_msas_with_dummy_sequences(
+    msa_A_by_sp, msa_B_by_sp
 )
 
-species = list(msa_data_A_species_by_species_padded.keys())
-species_sizes = list(map(len, msa_data_A_species_by_species_padded.values()))
+species = list(msa_A_by_sp_pad.keys())
+species_sizes = list(map(len, msa_A_by_sp_pad.values()))
 ```
 
 Next, one-hot encode the MSAs using the
 [`one_hot_encode_msa`](https://Bitbol-Lab.github.io/DiffPaSS/data_utils.html#one_hot_encode_msa)
 function.
 
 ``` python
 from diffpass.data_utils import one_hot_encode_msa
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
 # Unpack the padded MSAs into a list of records
-msa_data_A_for_pairing = [record for records_this_species in msa_data_A_species_by_species_padded.values() for record in records_this_species]
-msa_data_B_for_pairing = [record for records_this_species in msa_data_B_species_by_species_padded.values() for record in records_this_species]
+msa_A_for_pairing = [
+    rec for recs_this_sp in msa_A_by_sp_pad.values() for rec in recs_this_sp
+]
+msa_B_for_pairing = [
+    rec for recs_this_sp in msa_B_by_sp_pad.values() for rec in recs_this_sp
+]
 
 # One-hot encode the MSAs and load them to a device
-msa_A_oh = one_hot_encode_msa(msa_data_A_for_pairing, device=device)
-msa_B_oh = one_hot_encode_msa(msa_data_B_for_pairing, device=device)
+msa_A_oh = one_hot_encode_msa(msa_A_for_pairing, device=device)
+msa_B_oh = one_hot_encode_msa(msa_B_for_pairing, device=device)
 ```
 
 ### Pairing optimization
 
 Finally, we can instantiate an
 [`InformationPairing`](https://Bitbol-Lab.github.io/DiffPaSS/train.html#informationpairing)
 object and optimize the mutual information between the paired MSAs using
-the DiffPaSS bootstrap algorithm. The results are stored in a
+the DiffPaSS bootstrapped optimization algorithm. The results are stored
+in a
 [`DiffPaSSResults`](https://Bitbol-Lab.github.io/DiffPaSS/base.html#diffpassresults)
-container. The lists of (hard) losses and permutations found can be
-accessed as attributes of the container.
+container. The lists of (hard) losses and permutations found during the
+optimization can be accessed as attributes of the container.
 
 ``` python
 from diffpass.train import InformationPairing
 
 information_pairing = InformationPairing(group_sizes=species_sizes).to(device)
 bootstrap_results = information_pairing.fit_bootstrap(x, y)
```

### Comparing `diffpass-0.1.0/diffpass/_modidx.py` & `diffpass-0.1.1/diffpass/_modidx.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass/base.py` & `diffpass-0.1.1/diffpass/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __all__ = ['INGROUP_IDX_DTYPE', 'BootstrapList', 'GradientDescentList', 'GroupByGroupList', 'IndexPair', 'IndexPairsInGroup',
            'IndexPairsInGroups', 'dccn', 'make_pbar', 'DiffPaSSResults', 'DiffPaSSModel']
 
 # %% ../nbs/base.ipynb 4
 # Stdlib imports
 from copy import deepcopy
 from typing import Optional, Any, Sequence, Union
-from dataclasses import fields, dataclass
+from dataclasses import fields, dataclass, replace
 
 # Progress bars
 from tqdm import tqdm
 
 # NumPy
 import numpy as np
 
@@ -72,22 +72,22 @@
     # Hard permutations
     hard_perms: Union[
         GradientDescentList[GroupByGroupList[np.ndarray]],
         BootstrapList[GradientDescentList[GroupByGroupList[np.ndarray]]],
     ]
     # Hard losses
     hard_losses: Union[
-        GradientDescentList[GroupByGroupList[np.ndarray]],
-        BootstrapList[GradientDescentList[GroupByGroupList[np.ndarray]]],
+        GradientDescentList[GroupByGroupList[float]],
+        BootstrapList[GradientDescentList[GroupByGroupList[float]]],
     ]
     # Soft losses
     soft_losses: Optional[
         Union[
-            GradientDescentList[GroupByGroupList[np.ndarray]],
-            BootstrapList[GradientDescentList[GroupByGroupList[np.ndarray]]],
+            GradientDescentList[GroupByGroupList[float]],
+            BootstrapList[GradientDescentList[GroupByGroupList[float]]],
         ]
     ]
 
 
 class DiffPaSSModel(Module):
     """Base class for DiffPaSS models."""
 
@@ -314,15 +314,15 @@
             loss = out["loss"]
             results.hard_perms.append(
                 [
                     dccn(perms_this_group).argmax(axis=-1).astype(INGROUP_IDX_DTYPE)
                     for perms_this_group in perms
                 ]
             )
-            results.hard_losses.append(dccn(loss))
+            results.hard_losses.append(loss.item())
 
     def _soft_pass(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         *,
         results: DiffPaSSResults,
@@ -334,18 +334,15 @@
         perms = out["perms"]
         loss = out["loss"]
         if record_soft_perms:
             results.soft_perms.append(
                 [dccn(perms_this_group) for perms_this_group in perms]
             )
         if record_soft_losses:
-            results.soft_losses.append(dccn(loss))
-
-        # Compute total loss
-        loss = loss.sum()
+            results.soft_losses.append(loss.item())
 
         return loss
 
     def _record_current_log_alphas(self, results: DiffPaSSResults) -> None:
         results.log_alphas.append(
             [dccn(log_alpha) for log_alpha in self.permutation.log_alphas]
         )
@@ -513,14 +510,15 @@
         y: torch.Tensor,  # The target object (MSA or adjacency matrix of graphs), that the objects represented by `x` should be paired with. Not acted upon by soft/hard permutations
         *,
         n_start: int = 1,  # Number of fixed pairings to choose among the pairs not already fixed by `self.fixed_pairings`, using the results of the first call to `fit`
         n_end: Optional[
             int
         ] = None,  # If ``None``, the bootstrap will end when all pairs are fixed. Otherwise, the bootstrap will end when `n_end` pairs are fixed
         step_size: int = 1,  # Difference between the number of fixed pairings chosen at consecutive bootstrap iterations
+        n_repeats: int = 1,  # At each bootstrap iteration, `n_repeats` runs will be performed, and the run with the lowest loss will be chosen
         show_pbar: bool = True,  # If ``True``, show progress bar. Default: ``True``
         single_fit_cfg: Optional[
             dict
         ] = None,  # If not ``None``, configuration dictionary for gradient optimization in each bootstrap iteration (call to `fit`). See `fit` for details
     ) -> (
         DiffPaSSResults
     ):  # `DiffPaSSResults` container for fit results. All attributes are lists indexed by bootstrap iteration, containing lists indexed by gradient descent iteration as per `fit`
@@ -585,66 +583,95 @@
         # fixed matchings)
         pbar = list(range(n_start, n_end, step_size))
         pbar = tqdm(pbar) if show_pbar else pbar
         n_iters_with_optimization = int(can_optimize)
         for N in pbar:
             latest_hard_perms = results.hard_perms[-1]
             mapped_idxs = offsets + np.concatenate(latest_hard_perms)
-            rand_fixed_idxs = np.random.permutation(nonfixed_idxs)[:N]
-            rand_fixed_idxs = np.sort(rand_fixed_idxs)
-            rand_mapped_idxs = mapped_idxs[rand_fixed_idxs]
-            rand_group_idxs = group_idxs[rand_fixed_idxs]
-            rand_fixed_rel_idxs = rand_fixed_idxs - offsets[rand_fixed_idxs]
-            rand_mapped_rel_idxs = rand_mapped_idxs - offsets[rand_mapped_idxs]
-
-            # Update fixed matchings
-            fixed_pairings = [[] for _ in range(n_groups)]
-            for rand_group_idx, mapped_rel_idx, fixed_rel_idx in zip(
-                rand_group_idxs, rand_mapped_rel_idxs, rand_fixed_rel_idxs
-            ):
-                pair = (mapped_rel_idx, fixed_rel_idx)
-                fixed_pairings[rand_group_idx].append(pair)
-            fixed_pairings = [
-                initial_fixed_pairings[k] + fixed_pairings[k] for k in range(n_groups)
-            ]
-            self.permutation.init_fixed_pairings_and_log_alphas(
-                fixed_pairings, device=x.device
-            )
 
+            results_this_iter = self._init_results(
+                record_log_alphas=single_fit_cfg["record_log_alphas"],
+                record_soft_perms=single_fit_cfg["record_soft_perms"],
+                record_soft_losses=single_fit_cfg["record_soft_losses"],
+            )
             field_to_length_so_far = {
                 field_name: len(getattr(results, field_name))
                 for field_name in available_fields
             }
-            can_optimize = self._fit(x, y, results=results, **single_fit_cfg)
+            for _ in range(n_repeats):
+                rand_fixed_idxs = np.random.permutation(nonfixed_idxs)[:N]
+                rand_fixed_idxs = np.sort(rand_fixed_idxs)
+                rand_mapped_idxs = mapped_idxs[rand_fixed_idxs]
+                rand_group_idxs = group_idxs[rand_fixed_idxs]
+                rand_fixed_rel_idxs = rand_fixed_idxs - offsets[rand_fixed_idxs]
+                rand_mapped_rel_idxs = rand_mapped_idxs - offsets[rand_mapped_idxs]
+
+                # Update fixed matchings
+                fixed_pairings = [[] for _ in range(n_groups)]
+                for rand_group_idx, mapped_rel_idx, fixed_rel_idx in zip(
+                    rand_group_idxs, rand_mapped_rel_idxs, rand_fixed_rel_idxs
+                ):
+                    pair = (mapped_rel_idx, fixed_rel_idx)
+                    fixed_pairings[rand_group_idx].append(pair)
+                fixed_pairings = [
+                    initial_fixed_pairings[k] + fixed_pairings[k]
+                    for k in range(n_groups)
+                ]
+                self.permutation.init_fixed_pairings_and_log_alphas(
+                    fixed_pairings, device=x.device
+                )
+
+                can_optimize = self._fit(
+                    x, y, results=results_this_iter, **single_fit_cfg
+                )
+                if not can_optimize:
+                    slice_to_append = slice(-1, None)
+                    break
             if can_optimize:
                 n_iters_with_optimization += 1
-            else:
+                # Select run with lowest loss
+                reshaped_hard_losses_this_repeat = np.asarray(
+                    results_this_iter.hard_losses
+                ).reshape(n_repeats, -1)
+                size_each_repeat = reshaped_hard_losses_this_repeat.shape[1]
+                min_loss_idx = np.argmin(reshaped_hard_losses_this_repeat[:, -1])
+                slice_to_append = slice(
+                    min_loss_idx * size_each_repeat,
+                    (min_loss_idx + 1) * size_each_repeat,
+                )
+            [
+                getattr(results, field_name).extend(
+                    getattr(results_this_iter, field_name)[slice_to_append]
+                )
+                for field_name in available_fields
+            ]
+            if not can_optimize:
                 break
 
         # Reshape results according to number of iterations performed
+        reshaped_fields = {}
         for field_name in available_fields:
             results_this_field = getattr(results, field_name)
             n_optimized_results_this_field = (
                 len(results_this_field)
                 if can_optimize
                 else field_to_length_so_far[field_name]
             )
+            n_unoptimized_results_this_field = (
+                len(results_this_field) - n_optimized_results_this_field
+            )
 
             assert not n_optimized_results_this_field % n_iters_with_optimization
             n_in_each_optimized_iter = (
                 n_optimized_results_this_field // n_iters_with_optimization
             )
-            setattr(
-                results,
-                field_name,
-                [
-                    results_this_field[
-                        j
-                        * n_in_each_optimized_iter : (j + 1)
-                        * n_in_each_optimized_iter
-                    ]
-                    for j in range(n_iters_with_optimization)
+            reshaped_fields[field_name] = [
+                results_this_field[
+                    j * n_in_each_optimized_iter : (j + 1) * n_in_each_optimized_iter
                 ]
-                + [results_this_field[n_optimized_results_this_field:]],
+                for j in range(n_iters_with_optimization)
+            ] + [results_this_field[n_optimized_results_this_field:]] * bool(
+                n_unoptimized_results_this_field
             )
+        results = replace(results, **reshaped_fields)
 
         return results
```

### Comparing `diffpass-0.1.0/diffpass/constants.py` & `diffpass-0.1.1/diffpass/constants.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass/data_utils.py` & `diffpass-0.1.1/diffpass/data_utils.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass/entropy_ops.py` & `diffpass-0.1.1/diffpass/entropy_ops.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass/gumbel_sinkhorn_ops.py` & `diffpass-0.1.1/diffpass/gumbel_sinkhorn_ops.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass/ipa_utils.py` & `diffpass-0.1.1/diffpass/ipa_utils.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass/model.py` & `diffpass-0.1.1/diffpass/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 # %% ../nbs/model.ipynb 8
 class GeneralizedPermutation(Module):
     """Generalized permutation layer implementing both soft and hard permutations."""
 
     def __init__(
         self,
         *,
-        group_sizes: Iterable[int],
+        group_sizes: Sequence[int],
         fixed_pairings: Optional[IndexPairsInGroups] = None,
         tau: float = 1.0,
         n_iter: int = 1,
         noise: bool = False,
         noise_factor: float = 1.0,
         noise_std: bool = False,
         mode: Literal["soft", "hard"] = "soft",
@@ -252,15 +252,15 @@
         return list(mats)
 
 
 class MatrixApply(Module):
     """Apply matrices to chunks of a tensor of shape (n_samples, length, alphabet_size)
     and collate the results."""
 
-    def __init__(self, group_sizes: Iterable[int]) -> None:
+    def __init__(self, group_sizes: Sequence[int]) -> None:
         super().__init__()
         self.group_sizes = tuple(s for s in group_sizes)
         self._group_slices = _consecutive_slices_from_sizes(self.group_sizes)
 
     def forward(self, x: torch.Tensor, *, mats: Sequence[torch.Tensor]) -> torch.Tensor:
         out = torch.full_like(x, torch.nan)
         for mats_this_group, sl in zip(mats, self._group_slices):
@@ -271,15 +271,15 @@
         return out
 
 
 class PermutationConjugate(Module):
     """Conjugate blocks of a square 2D tensor of shape (n_samples, n_samples) by
     permutation matrices."""
 
-    def __init__(self, group_sizes: Iterable[int]) -> None:
+    def __init__(self, group_sizes: Sequence[int]) -> None:
         super().__init__()
         self.group_sizes = tuple(s for s in group_sizes)
         self._group_slices = _consecutive_slices_from_sizes(self.group_sizes)
 
     def forward(self, x: torch.Tensor, *, mats: Sequence[torch.Tensor]) -> torch.Tensor:
         out1 = torch.full_like(x, torch.nan)
         out2 = torch.full_like(x, torch.nan)
@@ -362,15 +362,15 @@
     similarities can be restricted to within groups.
     Differentiable operations are used to compute the similarities, which can be
     either dot products or an L^p distance function."""
 
     def __init__(
         self,
         *,
-        group_sizes: Optional[Iterable[int]] = None,
+        group_sizes: Optional[Sequence[int]] = None,
         use_dot: bool = True,
         p: Optional[float] = None,
     ) -> None:
         super().__init__()
         self.group_sizes = (
             tuple(s for s in group_sizes) if group_sizes is not None else None
         )
@@ -411,15 +411,15 @@
     similarities can be restricted to within groups.
     Differentiable operations are used to compute the similarities, which can be
     either dot products or an L^p distance function."""
 
     def __init__(
         self,
         *,
-        group_sizes: Optional[Iterable[int]] = None,
+        group_sizes: Optional[Sequence[int]] = None,
         use_dot: bool = True,
         p: Optional[float] = None,
         use_scoredist: bool = False,
         aa_to_int: Optional[dict[str, int]] = None,
         gaps_as_stars: bool = True,
     ) -> None:
         super().__init__()
@@ -481,15 +481,15 @@
     temperature parameter `tau`. In both cases, the main diagonal in the similarity
     matrix is excluded by setting its entries to minus infinity."""
 
     def __init__(
         self,
         *,
         reciprocal: bool = True,
-        group_sizes: Optional[Iterable[int]],
+        group_sizes: Optional[Sequence[int]],
         tau: float = 0.1,
         mode: Literal["soft", "hard"] = "soft",
     ) -> None:
         super().__init__()
         self.reciprocal = reciprocal
         self.group_sizes = (
             tuple(s for s in group_sizes) if group_sizes is not None else None
@@ -538,21 +538,26 @@
 
 # %% ../nbs/model.ipynb 25
 class InterGroupSimilarityLoss(Module):
     """Compute a loss that compares similarity matrices restricted to inter-group
     relationships.
 
     Similarity matrices are expected to be square and symmetric. The loss is computed
-    by comparing the (unrolled and concatenated) upper triangular blocks containing
-    inter-group similarities."""
+    by comparing the (flattened and concatenated) blocks containing inter-group
+    similarities."""
 
     def __init__(
         self,
         *,
-        group_sizes: Iterable[int],
+        # Number of entries in each group (e.g. species). Groups are assumed to be
+        # contiguous in the input similarity matrices
+        group_sizes: Sequence[int],
+        # If not ``None``, custom callable to compute the differentiable score between
+        # the flattened and concatenated inter-group blocks of the similarity matrices.
+        # Default: dot product
         score_fn: Union[callable, None] = None,
     ) -> None:
         super().__init__()
         self.group_sizes = tuple(s for s in group_sizes)
         self.score_fn = (
             partial(torch.tensordot, dims=1) if score_fn is None else score_fn
         )
@@ -584,42 +589,51 @@
 
 
 class IntraGroupSimilarityLoss(Module):
     """Compute a loss that compares similarity matrices restricted to intra-group
     relationships.
 
     Similarity matrices are expected to be square and symmetric. Their diagonal
-    elements are ignored.
-    If `group_sizes` is provided, the loss is computed by comparing the (unrolled
-    and concatenated) upper triangular blocks containing intra-group similarities.
+    elements are ignored if `exclude_diagonal` is set to ``True``.
+    If `group_sizes` is provided, the loss is computed by comparing the flattened
+    and concatenated upper triangular blocks containing intra-group similarities.
     Otherwise, the loss is computed by comparing the upper triangular part of the
-    full similarity matrices, excluding the main diagonal."""
+    full similarity matrices."""
 
     def __init__(
         self,
         *,
-        group_sizes: Optional[Iterable[int]] = None,
+        # Number of entries in each group (e.g. species). Groups are assumed to be
+        # contiguous in the input similarity matrices
+        group_sizes: Optional[Sequence[int]] = None,
+        # If not ``None``, custom callable to compute the differentiable score between
+        # the flattened and concatenated intra-group blocks of the similarity matrices
+        # Default: dot product
         score_fn: Union[callable, None] = None,
+        # If ``True``, exclude the diagonal elements from the computation
+        exclude_diagonal: bool = True,
     ) -> None:
         super().__init__()
         self.group_sizes = (
             tuple(s for s in group_sizes) if group_sizes is not None else None
         )
         self.score_fn = (
             partial(torch.tensordot, dims=1) if score_fn is None else score_fn
         )
+        self.exclude_diagonal = exclude_diagonal
 
         if self.group_sizes is not None:
             # Boolean mask for the main diagonal blocks corresponding to groups
             diag_blocks_mask = torch.block_diag(
                 *[torch.ones((s, s), dtype=torch.bool) for s in self.group_sizes]
             )
-            # Extract the upper triangular part, excluding the main diagonal
+            # Extract the upper triangular part
             self.register_buffer(
-                "_upper_diag_blocks_mask", torch.triu(diag_blocks_mask, diagonal=1)
+                "_upper_diag_blocks_mask",
+                torch.triu(diag_blocks_mask, diagonal=int(self.exclude_diagonal)),
             )
         else:
             self._upper_diag_blocks_mask = None
 
     def forward(
         self,
         similarities_x: torch.Tensor,
@@ -634,15 +648,15 @@
             mask = torch.triu(
                 torch.ones(
                     similarities_x.shape[-2:],
                     dtype=torch.bool,
                     layout=similarities_x.layout,
                     device=similarities_x.device,
                 ),
-                diagonal=1,
+                diagonal=int(self.exclude_diagonal),
             )
         else:
             mask = self._upper_diag_blocks_mask
 
         scores = self.score_fn(similarities_x[..., mask], similarities_y[..., mask])
         loss = -scores
```

### Comparing `diffpass-0.1.0/diffpass/msa_parsing.py` & `diffpass-0.1.1/diffpass/msa_parsing.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass/sequence_similarity_ops.py` & `diffpass-0.1.1/diffpass/sequence_similarity_ops.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass/train.py` & `diffpass-0.1.1/diffpass/train.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/diffpass.egg-info/PKG-INFO` & `diffpass-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: diffpass
-Version: 0.1.0
-Summary: Differentiable Pairing using Soft Scores
-Home-page: https://github.com/Bitbol-Lab/DiffPaSS
-Author: Umberto Lupo and Damiano Sgarbossa
-Author-email: umberto.lupo@epfl.ch, damiano.sgarbossa@epfl.ch
-License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: biopython
-Requires-Dist: tqdm
-Requires-Dist: pandas
-Provides-Extra: dev
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: jupyter; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-
 # DiffPaSS – Differentiable Pairing using Soft Scores
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Overview
 
 DiffPaSS is a family of high-performance and scalable PyTorch modules
@@ -45,15 +12,15 @@
 
 A typical example of the problem DiffPaSS is designed to solve is the
 following: given two multiple sequence alignments (MSAs) A and B,
 containing interacting biological sequences, find the optimal one-to-one
 pairing between the sequences in A and B.
 
 <figure>
-<img src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/MSA_pairing_problem.svg" alt="MSA pairing problem" />
+<img src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/MSA_pairing_problem.svg" width="640" height="201.6" alt="MSA pairing problem" />
 <figcaption>
 Pairing problem for two multiple sequence alignments, where pairings are
 restricted to be within the same species
 </figcaption>
 </figure>
 
 To find an optimal pairing, we can maximize the average mutual
@@ -113,15 +80,15 @@
 
 4.  A notion of “robust pairs” that can be used to identify pairs that
     are consistently found throughout a DiffPaSS bootstrap. These pairs
     can be used as ground truths in another DiffPaSS run, giving rise to
     the DiffPaSS-Iterative Pairing Algorithm (DiffPaSS-IPA).
 
 <figure>
-<video src="https://raw.githubusercontent.com/Bitbol-Lab/DiffPaSS/main/media/DiffPaSS_bootstrap.mp4" width="432" height="243" controls>
+<video src="https://github.com/Bitbol-Lab/DiffPaSS/assets/46537483/e411fe8c-2fed-4723-a25c-ff69a1abccec" width="640" height="360" controls>
 </video>
 <figcaption>
 The DiffPaSS bootstrap technique and robust pairs
 </figcaption>
 </figure>
 
 ## Installation
@@ -158,17 +125,17 @@
 First, parse your multiple sequence alignments (MSAs) in FASTA format
 into a list of tuples `(header, sequence)` using
 [`read_msa`](https://Bitbol-Lab.github.io/DiffPaSS/msa_parsing.html#read_msa).
 
 ``` python
 from diffpass.msa_parsing import read_msa
 
-# Parse and one-hot encode the MSAs
-msa_data_A = read_msa("path/to/msa_A.fasta")
-msa_data_B = read_msa("path/to/msa_B.fasta")
+# Parse the MSAs into lists of tuples (header, sequence)
+msa_A = read_msa("path/to/msa_A.fasta")
+msa_B = read_msa("path/to/msa_B.fasta")
 ```
 
 We assume that the MSAs contain species information in the headers,
 which will be used to restrict the pairings to be within the same
 species (more generally, “groups”). We need a simple function to extract
 the species information from the headers. For instance, if the headers
 are in the format `>sequence_id|species_name|...`, we can use:
@@ -179,72 +146,77 @@
 ```
 
 This function will be used to group the sequences by species:
 
 ``` python
 from diffpass.data_utils import create_groupwise_seq_records
 
-msa_data_A_species_by_species = create_groupwise_seq_records(msa_data_A, species_name_func)
-msa_data_B_species_by_species = create_groupwise_seq_records(msa_data_B, species_name_func)
+msa_A_by_sp = create_groupwise_seq_records(msa_A, species_name_func)
+msa_B_by_sp = create_groupwise_seq_records(msa_B, species_name_func)
 ```
 
 If one of the MSAs contains sequences from species not present in the
 other MSA, we can remove these species from both MSAs:
 
 ``` python
 from diffpass.data_utils import remove_groups_not_in_both
 
-msa_data_A_species_by_species, msa_data_B_species_by_species = remove_groups_not_in_both(
-    msa_data_A_species_by_species, msa_data_B_species_by_species
+msa_A_by_sp, msa_B_by_sp = remove_groups_not_in_both(
+    msa_A_by_sp, msa_B_by_sp
 )
 ```
 
 If there are species with different numbers of sequences in the two
 MSAs, we can add dummy sequences to the smaller species to make the
 number of sequences equal. For example, we can add dummy sequences
 consisting entirely of gap symbols:
 
 ``` python
 from diffpass.data_utils import pad_msas_with_dummy_sequences
 
-msa_data_A_species_by_species_padded, msa_data_B_species_by_species_padded = pad_msas_with_dummy_sequences(
-    msa_data_A_species_by_species, msa_data_B_species_by_species
+msa_A_by_sp_pad, msa_B_by_sp_pad = pad_msas_with_dummy_sequences(
+    msa_A_by_sp, msa_B_by_sp
 )
 
-species = list(msa_data_A_species_by_species_padded.keys())
-species_sizes = list(map(len, msa_data_A_species_by_species_padded.values()))
+species = list(msa_A_by_sp_pad.keys())
+species_sizes = list(map(len, msa_A_by_sp_pad.values()))
 ```
 
 Next, one-hot encode the MSAs using the
 [`one_hot_encode_msa`](https://Bitbol-Lab.github.io/DiffPaSS/data_utils.html#one_hot_encode_msa)
 function.
 
 ``` python
 from diffpass.data_utils import one_hot_encode_msa
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
 # Unpack the padded MSAs into a list of records
-msa_data_A_for_pairing = [record for records_this_species in msa_data_A_species_by_species_padded.values() for record in records_this_species]
-msa_data_B_for_pairing = [record for records_this_species in msa_data_B_species_by_species_padded.values() for record in records_this_species]
+msa_A_for_pairing = [
+    rec for recs_this_sp in msa_A_by_sp_pad.values() for rec in recs_this_sp
+]
+msa_B_for_pairing = [
+    rec for recs_this_sp in msa_B_by_sp_pad.values() for rec in recs_this_sp
+]
 
 # One-hot encode the MSAs and load them to a device
-msa_A_oh = one_hot_encode_msa(msa_data_A_for_pairing, device=device)
-msa_B_oh = one_hot_encode_msa(msa_data_B_for_pairing, device=device)
+msa_A_oh = one_hot_encode_msa(msa_A_for_pairing, device=device)
+msa_B_oh = one_hot_encode_msa(msa_B_for_pairing, device=device)
 ```
 
 ### Pairing optimization
 
 Finally, we can instantiate an
 [`InformationPairing`](https://Bitbol-Lab.github.io/DiffPaSS/train.html#informationpairing)
 object and optimize the mutual information between the paired MSAs using
-the DiffPaSS bootstrap algorithm. The results are stored in a
+the DiffPaSS bootstrapped optimization algorithm. The results are stored
+in a
 [`DiffPaSSResults`](https://Bitbol-Lab.github.io/DiffPaSS/base.html#diffpassresults)
-container. The lists of (hard) losses and permutations found can be
-accessed as attributes of the container.
+container. The lists of (hard) losses and permutations found during the
+optimization can be accessed as attributes of the container.
 
 ``` python
 from diffpass.train import InformationPairing
 
 information_pairing = InformationPairing(group_sizes=species_sizes).to(device)
 bootstrap_results = information_pairing.fit_bootstrap(x, y)
```

### Comparing `diffpass-0.1.0/diffpass.egg-info/SOURCES.txt` & `diffpass-0.1.1/diffpass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffpass-0.1.0/settings.ini` & `diffpass-0.1.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = DiffPaSS
 lib_name = diffpass
-version = 0.1.0
+version = 0.1.1
 min_python = 3.7
 license = apache2
 black_formatting = True
 doc_path = _docs
 lib_path = diffpass
 nbs_path = nbs
 recursive = True
```

### Comparing `diffpass-0.1.0/setup.py` & `diffpass-0.1.1/setup.py`

 * *Files identical despite different names*

