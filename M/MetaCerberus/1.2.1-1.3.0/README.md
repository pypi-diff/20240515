# Comparing `tmp/MetaCerberus-1.2.1.tar.gz` & `tmp/metacerberus-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetaCerberus-1.2.1.tar", last modified: Wed Feb 14 03:48:49 2024, max compression
+gzip compressed data, was "metacerberus-1.3.0.tar", last modified: Wed May 15 19:31:44 2024, max compression
```

## Comparing `MetaCerberus-1.2.1.tar` & `metacerberus-1.3.0.tar`

### file list

```diff
@@ -1,113 +1,81 @@
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.368000 MetaCerberus-1.2.1/
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1507 2022-05-26 03:57:57.000000 MetaCerberus-1.2.1/LICENSE.txt
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.368000 MetaCerberus-1.2.1/MetaCerberus.egg-info/
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    16159 2024-02-14 03:48:49.000000 MetaCerberus-1.2.1/MetaCerberus.egg-info/PKG-INFO
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     3478 2024-02-14 03:48:49.000000 MetaCerberus-1.2.1/MetaCerberus.egg-info/SOURCES.txt
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)        1 2024-02-14 03:48:49.000000 MetaCerberus-1.2.1/MetaCerberus.egg-info/dependency_links.txt
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       94 2024-02-14 03:48:49.000000 MetaCerberus-1.2.1/MetaCerberus.egg-info/requires.txt
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       14 2024-02-14 03:48:49.000000 MetaCerberus-1.2.1/MetaCerberus.egg-info/top_level.txt
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    16159 2024-02-14 03:48:49.368000 MetaCerberus-1.2.1/PKG-INFO
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    15059 2024-01-31 19:41:21.000000 MetaCerberus-1.2.1/README.md
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.348000 MetaCerberus-1.2.1/bin/
--rwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)    42648 2024-02-14 03:33:57.000000 MetaCerberus-1.2.1/bin/metacerberus.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    11085 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/bin/pathview-metacerberus.R
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      879 2022-04-15 16:33:42.000000 MetaCerberus-1.2.1/bin/ray-slurm-metacerberus.sh
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.352000 MetaCerberus-1.2.1/lib/
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5129 2022-04-15 16:46:41.000000 MetaCerberus-1.2.1/lib/Chunker.py
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.352000 MetaCerberus-1.2.1/lib/FGS/
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)  2219806 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/FGS/FragGeneScanRS-Darwin.tar.gz
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)  3102361 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/FGS/FragGeneScanRS-Linux.tar.gz
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.356000 MetaCerberus-1.2.1/lib/PHANOTATE/
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       49 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/.gitattributes
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      794 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/.gitignore
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       85 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/.gitmodules
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2391 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/CHANGELOG.md
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      349 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/CITATION.md
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    35141 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/LICENSE
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      145 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/MANIFEST.in
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2443 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/README.md
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)        6 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/VERSION
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.356000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    58429 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/Phannotate Gene Length Statistics.ipynb
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     3506 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/README.md
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     4078 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/RunningSearches.md
--rwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)     1705 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/count_hits_per_orf.pl
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      132 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/counts_type.tsv.gz
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    84454 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/lastal_counts.ipynb
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      132 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/phanotate_all_orf_positions.txt.gz
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      130 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/Validation/phanotate_v_nr_lens.json.gz
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.356000 MetaCerberus-1.2.1/lib/PHANOTATE/include/
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1141 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/include/LICENSE
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    69484 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/include/uthash.h
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      661 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/setup.cfg
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.356000 MetaCerberus-1.2.1/lib/PHANOTATE/src/
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     5356 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/src/phanotate_connect.c
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.360000 MetaCerberus-1.2.1/lib/PHANOTATE/tests/
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)   171388 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/tests/NC_000866.1.fasta
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    49207 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/tests/NC_001416.1.fasta
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2527 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/tests/phiX174.faa
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     5501 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/tests/phiX174.fasta
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1867 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/tests/phiX174.fasta.gz
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     7636 2023-11-30 17:08:15.000000 MetaCerberus-1.2.1/lib/PHANOTATE/tests/phiX174.gbk
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)        0 2022-04-15 16:46:41.000000 MetaCerberus-1.2.1/lib/__init__.py
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.360000 MetaCerberus-1.2.1/lib/__pycache__/
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      142 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1224 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_decon.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2295 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_formatFasta.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2211 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_genecall.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2046 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_hmm.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1070 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_merge.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      992 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_metastats.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     4355 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_parser.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1855 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_prostats.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1665 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_qc.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    12803 2022-04-16 18:27:02.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_report.cpython-39.pyc
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      604 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_setup.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2168 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_trim.cpython-39.pyc
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5568 2022-04-16 18:27:01.000000 MetaCerberus-1.2.1/lib/__pycache__/metacerberus_visual.cpython-39.pyc
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.360000 MetaCerberus-1.2.1/lib/dependency_files/
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     4127 2022-04-15 16:46:41.000000 MetaCerberus-1.2.1/lib/dependency_files/PacBio_quality-control.fna
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    25304 2022-04-15 16:46:41.000000 MetaCerberus-1.2.1/lib/dependency_files/adapters.fna
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    49167 2022-04-15 16:46:41.000000 MetaCerberus-1.2.1/lib/dependency_files/lambda-phage.fna
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5527 2022-04-15 16:46:41.000000 MetaCerberus-1.2.1/lib/dependency_files/phix174_ill.ref.fna
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      121 2022-04-15 16:46:41.000000 MetaCerberus-1.2.1/lib/dependency_files/readme.md
-drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-02-14 03:48:49.364000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:41.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/454_10
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/454_30
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/454_5
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1197 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/complete
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   121095 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/gene
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1302 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/illumina_1
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1294 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/illumina_10
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1298 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/illumina_5
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5175 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/noncoding
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     8670 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/pwm
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)       63 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/readme.md
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   121095 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/rgene
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1294 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/sanger_10
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1298 2022-04-15 16:46:42.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/sanger_5
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:43.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/start
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:44.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/start1
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:44.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/stop
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:45.000000 MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/stop1
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1596 2022-04-15 16:46:45.000000 MetaCerberus-1.2.1/lib/metacerberus.config
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1238 2024-01-31 15:23:42.000000 MetaCerberus-1.2.1/lib/metacerberus_decon.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     3093 2024-01-31 15:23:42.000000 MetaCerberus-1.2.1/lib/metacerberus_formatFasta.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     4380 2024-01-31 15:23:42.000000 MetaCerberus-1.2.1/lib/metacerberus_genecall.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     5232 2024-01-31 15:23:42.000000 MetaCerberus-1.2.1/lib/metacerberus_hmm.py
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   163125 2022-04-16 18:29:53.000000 MetaCerberus-1.2.1/lib/metacerberus_logo.jpg
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1102 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/metacerberus_merge.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      827 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/metacerberus_metastats.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     7924 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/metacerberus_parser.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     5402 2024-01-31 15:23:42.000000 MetaCerberus-1.2.1/lib/metacerberus_prostats.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1529 2024-01-31 15:23:42.000000 MetaCerberus-1.2.1/lib/metacerberus_qc.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    16685 2024-01-31 15:23:42.000000 MetaCerberus-1.2.1/lib/metacerberus_report.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     4886 2023-08-29 23:32:40.000000 MetaCerberus-1.2.1/lib/metacerberus_setup.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2580 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/metacerberus_trim.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     7833 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/metacerberus_visual.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     5986 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/metacereberus_parser_wPl.py
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     9394 2023-07-17 20:24:51.000000 MetaCerberus-1.2.1/lib/metacereberus_visual_wPL.py
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  3512600 2022-04-15 16:46:47.000000 MetaCerberus-1.2.1/lib/plotly-2.0.0.min.js
--rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     7661 2022-04-15 16:46:48.000000 MetaCerberus-1.2.1/lib/style.css
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       38 2024-02-14 03:48:49.368000 MetaCerberus-1.2.1/setup.cfg
--rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2336 2024-02-14 03:46:15.000000 MetaCerberus-1.2.1/setup.py
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.964172 metacerberus-1.3.0/
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1507 2022-05-26 03:57:57.000000 metacerberus-1.3.0/LICENSE.txt
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.964172 metacerberus-1.3.0/MetaCerberus.egg-info/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    27851 2024-05-15 19:31:44.000000 metacerberus-1.3.0/MetaCerberus.egg-info/PKG-INFO
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2481 2024-05-15 19:31:44.000000 metacerberus-1.3.0/MetaCerberus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)        1 2024-05-15 19:31:44.000000 metacerberus-1.3.0/MetaCerberus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       87 2024-05-15 19:31:44.000000 metacerberus-1.3.0/MetaCerberus.egg-info/requires.txt
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       14 2024-05-15 19:31:44.000000 metacerberus-1.3.0/MetaCerberus.egg-info/top_level.txt
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    27851 2024-05-15 19:31:44.964172 metacerberus-1.3.0/PKG-INFO
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    26760 2024-05-15 19:09:25.000000 metacerberus-1.3.0/README.md
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.948172 metacerberus-1.3.0/bin/
+-rwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)    47334 2024-05-15 19:08:38.000000 metacerberus-1.3.0/bin/metacerberus.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    11085 2023-07-17 20:24:51.000000 metacerberus-1.3.0/bin/pathview-metacerberus.R
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      879 2022-04-15 16:33:42.000000 metacerberus-1.3.0/bin/ray-slurm-metacerberus.sh
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.952172 metacerberus-1.3.0/lib/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5129 2022-04-15 16:46:41.000000 metacerberus-1.3.0/lib/Chunker.py
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.952172 metacerberus-1.3.0/lib/DB/
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1498 2024-05-06 21:09:59.000000 metacerberus-1.3.0/lib/DB/databases.tsv
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.952172 metacerberus-1.3.0/lib/FGS/
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)  2219806 2023-07-17 20:24:51.000000 metacerberus-1.3.0/lib/FGS/FragGeneScanRS-Darwin.tar.gz
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)  3102361 2023-07-17 20:24:51.000000 metacerberus-1.3.0/lib/FGS/FragGeneScanRS-Linux.tar.gz
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)        0 2022-04-15 16:46:41.000000 metacerberus-1.3.0/lib/__init__.py
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.956172 metacerberus-1.3.0/lib/__pycache__/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      142 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1224 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_decon.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2295 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_formatFasta.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2211 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_genecall.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2046 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_hmm.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1070 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_merge.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      992 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_metastats.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     4355 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_parser.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1855 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_prostats.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1665 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_qc.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    12803 2022-04-16 18:27:02.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_report.cpython-39.pyc
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      604 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_setup.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2168 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_trim.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5568 2022-04-16 18:27:01.000000 metacerberus-1.3.0/lib/__pycache__/metacerberus_visual.cpython-39.pyc
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.960172 metacerberus-1.3.0/lib/dependency_files/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     4127 2022-04-15 16:46:41.000000 metacerberus-1.3.0/lib/dependency_files/PacBio_quality-control.fna
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    25304 2022-04-15 16:46:41.000000 metacerberus-1.3.0/lib/dependency_files/adapters.fna
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    49167 2022-04-15 16:46:41.000000 metacerberus-1.3.0/lib/dependency_files/lambda-phage.fna
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5527 2022-04-15 16:46:41.000000 metacerberus-1.3.0/lib/dependency_files/phix174_ill.ref.fna
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      121 2022-04-15 16:46:41.000000 metacerberus-1.3.0/lib/dependency_files/readme.md
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2024-05-15 19:31:44.964172 metacerberus-1.3.0/lib/fraggenescanplus_dependences/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:41.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/454_10
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/454_30
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/454_5
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1197 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/complete
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   121095 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/gene
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1302 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/illumina_1
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1294 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/illumina_10
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1298 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/illumina_5
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5175 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/noncoding
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     8670 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/pwm
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)       63 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/readme.md
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   121095 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/rgene
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1294 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/sanger_10
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1298 2022-04-15 16:46:42.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/sanger_5
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:43.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/start
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:44.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/start1
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:44.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/stop
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:45.000000 metacerberus-1.3.0/lib/fraggenescanplus_dependences/stop1
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1596 2022-04-15 16:46:45.000000 metacerberus-1.3.0/lib/metacerberus.config
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1238 2024-01-31 15:23:42.000000 metacerberus-1.3.0/lib/metacerberus_decon.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     3093 2024-01-31 15:23:42.000000 metacerberus-1.3.0/lib/metacerberus_formatFasta.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     4654 2024-05-15 16:24:14.000000 metacerberus-1.3.0/lib/metacerberus_genecall.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     5095 2024-05-15 16:24:14.000000 metacerberus-1.3.0/lib/metacerberus_hmm.py
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   163125 2022-04-16 18:29:53.000000 metacerberus-1.3.0/lib/metacerberus_logo.jpg
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1806 2024-05-15 16:24:14.000000 metacerberus-1.3.0/lib/metacerberus_merge.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      827 2023-07-17 20:24:51.000000 metacerberus-1.3.0/lib/metacerberus_metastats.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    10541 2024-05-15 16:24:14.000000 metacerberus-1.3.0/lib/metacerberus_parser.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     8016 2024-05-15 16:24:14.000000 metacerberus-1.3.0/lib/metacerberus_prostats.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1529 2024-01-31 15:23:42.000000 metacerberus-1.3.0/lib/metacerberus_qc.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    22476 2024-05-15 16:24:14.000000 metacerberus-1.3.0/lib/metacerberus_report.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     6050 2024-05-15 16:24:14.000000 metacerberus-1.3.0/lib/metacerberus_setup.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2580 2024-03-20 19:24:25.000000 metacerberus-1.3.0/lib/metacerberus_trim.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     7833 2023-07-17 20:24:51.000000 metacerberus-1.3.0/lib/metacerberus_visual.py
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  3512600 2022-04-15 16:46:47.000000 metacerberus-1.3.0/lib/plotly-2.0.0.min.js
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     7661 2022-04-15 16:46:48.000000 metacerberus-1.3.0/lib/style.css
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       38 2024-05-15 19:31:44.964172 metacerberus-1.3.0/setup.cfg
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2336 2024-05-15 17:20:35.000000 metacerberus-1.3.0/setup.py
```

### Comparing `MetaCerberus-1.2.1/LICENSE.txt` & `metacerberus-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/bin/metacerberus.py` & `metacerberus-1.3.0/bin/metacerberus.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """metacerberus.py: Versatile Functional Ontology Assignments for Metagenomes
 
 Uses Hidden Markov Model (HMM) searching with environmental focus of shotgun metaomics data.
 """
 
 
-__version__     = "1.2.1"
+__version__     = "1.3.0"
+__date__        = "March 2024"
 __author__      = "Jose L. Figueroa III, Richard A. White III"
-__copyright__   = "Copyright 2023"
-__date__        = "February 2024"
+__copyright__   = "Copyright 2022-2024"
 
 def warn(*args, **kwargs):
     pass
 import warnings
 warnings.warn = warn
 
 import sys
@@ -40,22 +40,24 @@
     metacerberus_genecall, metacerberus_hmm, metacerberus_parser,
     metacerberus_prostats, metacerberus_visual, metacerberus_report, Chunker
 )
 
 
 ##### Global Variables #####
 
+DEBUG = True
+
 # known file extensions
 FILES_FASTQ = ['.fastq', '.fq']#, '.fastq.gz', '.fq.gz']
 FILES_FASTA = [".fasta", ".fa", ".fna", ".ffn"]
 FILES_AMINO = [".faa"]
 
 # External file paths
-pathDB = pkg.resource_filename("meta_cerberus", "DB")
-pathFGS = pkg.resource_filename("meta_cerberus", "FGS")
+PATHDB = pkg.resource_filename("meta_cerberus", "DB")
+PATHFGS = pkg.resource_filename("meta_cerberus", "FGS")
 
 # qc sequence default locations (for decontamination)
 QC_SEQ = {
     "adapters": pkg.resource_filename("meta_cerberus", "dependency_files/adapters.fna"),
     "illumina": pkg.resource_filename("meta_cerberus", "dependency_files/phix174_ill.ref.fna"),
     "lambda": pkg.resource_filename("meta_cerberus", "dependency_files/lambda-phage.fna"),
     "pacbio": pkg.resource_filename("meta_cerberus", "dependency_files/PacBio_quality-control.fna")
@@ -72,26 +74,14 @@
     'EXE_PRODIGAL': 'prodigal',
     'EXE_PRODIGAL-GV': 'prodigal-gv',
     'EXE_PHANOTATE' : 'phanotate.py',
     'EXE_HMMSEARCH' : 'hmmsearch',
     'EXE_COUNT_ASSEMBLY': 'countAssembly.py'
     }
 
-# Databases
-DB_HMM = dict(
-    KOFam_all=Path(pathDB, 'KOFam_all.hmm.gz'),
-    KOFam_prokaryote=Path(pathDB, 'KOFam_prokaryote.hmm.gz'),
-    KOFam_eukaryote=Path(pathDB, 'KOFam_eukaryote.hmm.gz'),
-    COG=Path(pathDB, 'COG-noIter.hmm.gz'),
-    CAZy=Path(pathDB, 'CAZy.hmm.gz'),
-    PHROG=Path(pathDB, 'PHROG.hmm.gz'),
-    VOG=Path(pathDB, 'VOG.hmm.gz'),
-    ALL="KOFam_all, CAZy, COG, VOG, PHROG",
-    )
-
 # step names
 STEP = {
     1:"step_01-loadFiles",
     2:"step_02-QC",
     3:"step_03-trim",
     4:"step_04-decontaminate",    
     5:"step_05-format",
@@ -113,131 +103,207 @@
         print(host, funcName, time, path, file=outTime, sep='\t')
     return
 
 
 ## Ray Worker Threads ##
 @ray.remote
 def rayWorkerThread(func, key, dir_log, params:list):
+    '''Worker thread for Ray
+
+    Parameters:
+        func: The name of the function to call
+        key (str): The key name for the value being processed
+        dir_log (str): Path to the folder of the logfile
+        params**: A list of parameters to send to the called function
+
+    Returns:
+        key, ret, function_name
+    '''
     start = time.time()
     ret = func(*params)
     end = str(datetime.timedelta(seconds=time.time()-start))
     logTime(dir_log, socket.gethostname(), func.__name__, key, end)
     return key, ret, func.__name__
 
 
 ## MAIN
 def main():
     ## Parse the command line
     parser = argparse.ArgumentParser(add_help=False)
     parser.set_defaults()
+
+    # Setup options
+    setup = parser.add_argument_group('''Setup arguments''')
+    setup_grp = setup.add_mutually_exclusive_group(required=False)
+    setup_grp.add_argument('--setup', action="store_true", help="Setup additional dependencies [False]")
+    setup_grp.add_argument('--update', action="store_true", help="Update downloaded databases [False]")
+    setup_grp.add_argument('--list-db', action="store_true", help="List available and downloaded databases [False]")
+    setup.add_argument('--download', nargs='*', default=None, help="Downloads selected HMMs. Use the option --list-db for a list of available databases, default is to download all available databases")
+    setup_grp.add_argument('--uninstall', action="store_true", help="Remove downloaded databases and FragGeneScan+ [False]")
+
     # At least one of these options are required
-    required = parser.add_argument_group('''Required arguments
+    input = parser.add_argument_group(f'''Input files
 At least one sequence is required.
-<accepted formats {.fastq .fasta .faa .fna .ffn}>
+    accepted formats: [{', '.join(FILES_FASTQ + FILES_FASTA + FILES_AMINO)}]
 Example:
 > metacerberus.py --prodigal file1.fasta
 > metacerberus.py --config file.config
-*Note: If a sequence is given in .fastq format, one of --nanopore, --illumina, or --pacbio is required.''')
-    required.add_argument('-c', '--config', help = 'Path to config file, command line takes priority', is_config_file=True)
-    required.add_argument('--prodigal', action='append', default=[], help='Prokaryote nucleotide sequence (includes microbes, bacteriophage)')
-    required.add_argument('--fraggenescan', action='append', default=[], help='Eukaryote nucleotide sequence (includes other viruses, works all around for everything)')
-    required.add_argument('--super', action='append', default=[], help='Run sequence in both --prodigal and --fraggenescan modes')
-    required.add_argument('--prodigalgv', action='append', default=[], help='Giant virus nucleotide sequence')
-    required.add_argument('--phanotate', action='append', default=[], help='Phage sequence')
-    required.add_argument('--protein', '--amino', action='append', default=[], help='Protein Amino Acid sequence')
-    required.add_argument('--rollup', action='append', default=[], help='Rolled up annotations from HMMER')
+*Note: If a sequence is given in [{', '.join(FILES_FASTQ)}] format, one of --nanopore, --illumina, or --pacbio is required.''')
+    input.add_argument('-c', '--config', help = 'Path to config file, command line takes priority', is_config_file=True)
+    input.add_argument('--prodigal', nargs='+', default=[], help='Prokaryote nucleotide sequence (includes microbes, bacteriophage)')
+    input.add_argument('--fraggenescan', nargs='+', default=[], help='Eukaryote nucleotide sequence (includes other viruses, works all around for everything)')
+    input.add_argument('--super', nargs='+', default=[], help='Run sequence in both --prodigal and --fraggenescan modes')
+    input.add_argument('--prodigalgv', nargs='+', default=[], help='Giant virus nucleotide sequence')
+    input.add_argument('--phanotate', nargs='+', default=[], help='Phage sequence')
+    input.add_argument('--protein', '--amino', nargs='+', default=[], help='Protein Amino Acid sequence')
+    input.add_argument('--hmmer-tsv', nargs='+', default=[], help='Annotations tsv file from HMMER (experimental)')
+    input.add_argument('--class', type=str, default='', help='path to a tsv file which has class information for the samples. If this file is included scripts will be included to run Pathview in R')
     # Raw-read identification
-    readtype = parser.add_mutually_exclusive_group(required=False)
+    readtype = input.add_mutually_exclusive_group(required=False)
     readtype.add_argument('--illumina', action="store_true", help="Specifies that the given FASTQ files are from Illumina")
     readtype.add_argument('--nanopore', action="store_true", help="Specifies that the given FASTQ files are from Nanopore")
     readtype.add_argument('--pacbio', action="store_true", help="Specifies that the given FASTQ files are from PacBio")
+
+    # Output options
+    output = parser.add_argument_group(f'''Output options''')
+    output.add_argument('--dir-out', "--dir_out", type=str, default='./results-metacerberus', help='path to output directory, defaults to "results-metacerberus" in current directory. [./results-metacerberus]')
+    output.add_argument('--replace', action="store_true", help="Flag to replace existing files. [False]")
+    output.add_argument('--keep', action="store_true", help="Flag to keep temporary files. [False]")
+    output.add_argument('--tmpdir', type=str, default="", help='temp directory for RAY (experimental) [system tmp dir]')
+
+    # Database options
+    database = parser.add_argument_group(f'''Database options''')
+    database.add_argument('--hmm', nargs='+', default=['KOFam_all'], help="A list of databases for HMMER. Use the option --list-db for a list of available databases [KOFam_all]")
+    database.add_argument("--db-path", type=str, default=PATHDB, help="Path to folder of databases [Default: under the library path of MetaCerberus]")
+
     # optional flags
     optional = parser.add_argument_group('optional arguments')
-    optional.add_argument('--setup', action="store_true", help="Set this flag to ensure dependencies are setup [False]")
-    optional.add_argument('--uninstall', action="store_true", help="Set this flag to remove downloaded databases and FragGeneScan+ [False]")
-    optional.add_argument('--dir_out', type=str, default='./results-metacerberus', help='path to output directory, creates "pipeline" folder. Defaults to current directory. [./results-metacerberus]')
     optional.add_argument('--meta', action="store_true", help="Metagenomic nucleotide sequences (for prodigal) [False]")
     optional.add_argument('--scaffolds', action="store_true", help="Sequences are treated as scaffolds [False]")
     optional.add_argument('--minscore', type=float, default=60, help="Score cutoff for parsing HMMER results [60]")
     optional.add_argument('--evalue', type=float, default=1e-09, help="E-value cutoff for parsing HMMER results [1e-09]")
-    optional.add_argument('--skip_decon', action="store_true", help="Skip decontamination step. [False]")
-    optional.add_argument('--skip_pca', action="store_true", help="Skip PCA. [False]")
+    optional.add_argument('--skip-decon', action="store_true", help="Skip decontamination step. [False]")
+    optional.add_argument('--skip-pca', action="store_true", help="Skip PCA. [False]")
     optional.add_argument('--cpus', type=int, help="Number of CPUs to use per task. System will try to detect available CPUs if not specified [Auto Detect]")
     optional.add_argument('--chunker', type=int, default=0, help="Split files into smaller chunks, in Megabytes [Disabled by default]")
     optional.add_argument('--grouped', action="store_true", help="Group multiple fasta files into a single file before processing. When used with chunker can improve speed")
-    optional.add_argument('--replace', action="store_true", help="Flag to replace existing files. [False]")
-    optional.add_argument('--keep', action="store_true", help="Flag to keep temporary files. [False]")
-    optional.add_argument('--hmm', type=str, default='KOFam_all', help="Specify a coma seperated list of databases for HMMER. Use quotes around the list, or avoid spaces. (KOFam_all, KOFam_eukaryote, KOFam_prokaryote, COG, CAZy, PHROG, COG) [KOFam_all]")
-    optional.add_argument('--class', type=str, default='', help='path to a tsv file which has class information for the samples. If this file is included scripts will be included to run Pathview in R')
-    optional.add_argument('--slurm_nodes', type=str, default="", help=argparse.SUPPRESS)# help='list of node hostnames from SLURM, i.e. $SLURM_JOB_NODELIST.')
-    optional.add_argument('--slurm_single', action="store_true", help=argparse.SUPPRESS)# help='Force single node use, do not connect to host')
-    optional.add_argument('--tmpdir', type=str, default="", help='temp directory for RAY [system tmp dir]')
+    optional.add_argument('--slurm-nodes', type=str, default="", help=argparse.SUPPRESS)# help='list of node hostnames from SLURM, i.e. $SLURM_JOB_NODELIST.')
+    optional.add_argument('--slurm-single', action="store_true", help=argparse.SUPPRESS)# help='Force single node use, do not connect to host')
     optional.add_argument('--version', '-v', action='version',
                         version=f'MetaCerberus: \n version: {__version__} {__date__}',
                         help='show the version number and exit')
     optional.add_argument("-h", "--help", action="help", help="show this help message and exit")
     # Hidden from help, expected to load from config file
     dependencies = parser.add_argument_group()
     for key in DEPENDENCIES:
         dependencies.add_argument(f"--{key}", help=argparse.SUPPRESS)
     dependencies.add_argument('--adapters', type=str, default=QC_SEQ['adapters'], help="FASTA File containing adapter sequences for trimming")
     dependencies.add_argument('--qc_seq', type=str, default="default", help="FASTA File containing control sequences for decontamination")
 
     args = parser.parse_args()
 
     if args.uninstall:
-        metacerberus_setup.Remove(pathDB, pathFGS)
-
+        metacerberus_setup.remove(args.db_path, PATHFGS)
+        return 0
+    if args.list_db:
+        downloaded,to_download,urls,hmm_version = metacerberus_setup.list_db(args.db_path)
+        if downloaded:
+            print("HMM Databases already downloaded:")
+            for name,filelist in downloaded.items():
+                print(name, hmm_version[name], sep='\t')
+                #for filepath in filelist:
+                #    print('', filepath, sep='\t')
+        else:
+            print("No HMM databases are currently downloaded at:", args.db_path)
+        if to_download:
+            print("Available HMM databases to download:")
+            for name,filelist in to_download.items():
+                print(name, hmm_version[name], sep='\t')
+                #for filepath in filelist:
+                #    print('', filepath, sep='\t')
+        else:
+            print("All available HMM databases already downloaded at:", args.db_path)
+        return 0
     if args.setup:
-        metacerberus_setup.FGS(pathFGS)
-        metacerberus_setup.Download(pathDB)
-
-    if args.setup or args.uninstall:
+        print("Setting up FragGeneScanRS")
+        metacerberus_setup.FGS(PATHFGS)
+        return 0
+    if args.download is not None:
+        metacerberus_setup.download(args.db_path, args.download)
+        return 0
+    if args.update:
+        metacerberus_setup.update(args.db_path)
         return 0
 
+    # HMM Databases
+    DB_HMM = dict()
+    if Path(PATHDB, "databases.tsv").exists():
+        with Path(PATHDB, "databases.tsv").open() as reader:
+            header = reader.readline().split()
+            for line in reader:
+                name,filename,urlpath,date = line.split()
+                if ".hmm" in Path(filename).suffixes:
+                    if name == "KOFam":
+                        name = Path(filename).with_suffix('').stem
+                        if name == "KOFam_all" and "ALL" in args.hmm:
+                            args.hmm += [name]
+                    elif "ALL" in args.hmm:
+                        args.hmm += [name]
+                    DB_HMM[name] = Path(args.db_path, filename)
 
-    # TODO: Add Custom HMM DB
     dbHMM = dict()
-    if args.hmm.upper() == "ALL":
-        args.hmm = DB_HMM['ALL']
-    for i,hmm in enumerate([x.strip() for x in args.hmm.split(',')], 1):
-        print(f"HMM: '{hmm}'")
+    for hmm in [x.strip(',') for x in set(args.hmm)]:
         if hmm in DB_HMM:
             if DB_HMM[hmm].exists():
-                dbHMM[hmm] = DB_HMM[hmm]
+                if Path(DB_HMM[hmm]).name.startswith("KOFam"):
+                    dbHMM[f"{hmm}_KEGG"] = DB_HMM[hmm]
+                    dbHMM[f"{hmm}_FOAM"] = DB_HMM[hmm]
+                else:
+                    dbHMM[hmm] = DB_HMM[hmm]
             else:
                 print(f"ERROR: Cannot use '{hmm}', please download it using 'metacerberus.py --setup")
         else:
-            print(f"ERROR: Cannot use '{hmm}', custom databases not supported yet. Please use one of:", *list(DB_HMM.keys()))
+            dbpath = Path(hmm)
+            while Path(hmm).suffixes:
+                hmm = Path(hmm).with_suffix('')
+            if dbpath.exists() and hmm.with_suffix('.tsv').exists():
+                dbname = Path(dbpath).with_suffix('').stem
+                dbHMM[dbname] = dbpath
+                print("Loading custom HMM:", dbname, dbpath)
+            else:
+                print("Unable to load custom database")
     if not len(dbHMM):
         print("ERROR: No HMM DB Loaded")
         return 1
 
-    print("\nStarting MetaCerberus Pipeline\n")
+    print(f"\nStarting MetaCerberus v{__version__} Pipeline\n")
+    print("Using HMMs:")
+    for k,v in dbHMM.items():
+        print(k,v)
 
     # Merge related arguments
     if args.super:
         args.prodigal += args.super
         args.fraggenescan += args.super
 
     # Check if required flags are set
-    if not any([args.prodigal, args.fraggenescan, args.prodigalgv, args.phanotate, args.protein, args.rollup]):
+    if not any([args.prodigal, args.fraggenescan, args.prodigalgv, args.phanotate, args.protein, args.hmmer_tsv]):
         parser.error('At least one sequence must be declared either in the command line or through the config file')
     if args.chunker < 0:
         args.chunker = 0
     if args.grouped and args.chunker == 0:
         args.chunker = 1
 
     # Initialize Config Dictionary
     config = {}
     config['STEP'] = STEP
-    config['PATHDB'] = pathDB
+    config['PATHDB'] = PATHDB
 
     # Get FGS+ Folder from Library Path
-    config['EXE_FGS'] = os.path.join(pathFGS, DEPENDENCIES["EXE_FGS"])
+    config['EXE_FGS'] = os.path.join(PATHFGS, DEPENDENCIES["EXE_FGS"])
 
     # load all args into config
     for arg,value in args.__dict__.items():
         if value is not None:
             arg = arg.upper()
             if type(value) is str and os.path.isfile(value):
                 value = os.path.abspath(os.path.expanduser(value))
@@ -286,31 +352,33 @@
     #TODO: Fix this, does not set up slurm script
     #if config['SLURM_NODES']:
     #    metacerberus_setup.slurm(config['SLURM_NODES'])
     
     # Get CPU Count
     if 'CPUS' not in config:
         config['CPUS'] = psutil.cpu_count()
-    
+
     if args.slurm_single:
         # Force single node
-        ray.init(num_cpus=config['CPUS'], log_to_driver=False)
+        ray.init(num_cpus=config['CPUS'], log_to_driver=DEBUG)
         print("Started RAY single node")
         config['CLUSTER'] = False
     else:
         try:
-            ray.init(address='auto', log_to_driver=False)
+            ray.init(address='auto', log_to_driver=DEBUG)
             print("Started RAY on cluster")
             config['CLUSTER'] = True
         except:
-            ray.init(num_cpus=config['CPUS'], log_to_driver=False)
+            ray.init(num_cpus=config['CPUS'], log_to_driver=DEBUG)
             print("Started RAY single node")
             config['CLUSTER'] = False
     print(f"Running RAY on {len(ray.nodes())} node(s)")
     print(f"Using {config['CPUS']} CPUs per node")
+    temp_dir = Path(ray.nodes()[0]['ObjectStoreSocketName']).parent.parent
+    print("Ray temporary directory:", temp_dir)
 
 
     startTime = time.time()
     # Step 1 - Load Input Files
     print("\nSTEP 1: Loading sequence files:")
     fastq = {}
     fasta = {}
@@ -397,30 +465,31 @@
         elif os.path.isdir(item):
             for file in os.listdir(item):
                 ext = os.path.splitext(file)[1]
                 if ext in FILES_FASTQ + FILES_FASTA:
                     args.phanotate.append(os.path.join(item, file))
         else:
             print(f'{item} is not a valid sequence')
-    # Load Rollup input
-    for item in args.rollup:
+    # Load HMMER input
+    for item in args.hmmer_tsv:
         item = os.path.abspath(os.path.expanduser(item))
         if os.path.isfile(item):
             name, ext = os.path.splitext(os.path.basename(item))
             if ext in ['.tsv']:
                 rollup['rollup_'+name] = item
         else:
             print(f'{item} is not a valid sequence')
     
     print(f"Processing {len(fastq)} fastq sequences")
     print(f"Processing {len(fasta)} fasta sequences")
     print(f"Processing {len(amino)} protein sequences")
     print(f"Processing {len(rollup)} rollup files")
 
     if len(fastq) > 0:
+        config['META'] = True
         if not any([args.illumina, args.nanopore, args.pacbio]):
             parser.error('A .fastq file was given, but no flag specified as to the type.\nPlease use one of --illumina, --nanopore, or --pacbio')
         else:
             if args.illumina:
                 config['QC_SEQ'] = QC_SEQ["illumina"]
             if args.nanopore:
                 config['QC_SEQ'] = QC_SEQ["lambda"]
@@ -439,24 +508,25 @@
         #    pipeline.append(rayWorkerThread.remote(metacerberus_qc.checkQuality, key, config['DIR_OUT'], [value, config, f"{STEP[2]}/{key}"]))
         print("\nSTEP 3: Trimming fastq files")
         # Merge Paired End Reads
         fastqPaired = dict()
         for ext in FILES_FASTQ:
             fastqPaired.update( {k:v for k,v in fastq.items() if "R1"+ext in v and v.replace("R1"+ext, "R2"+ext) in fastq.values() } )
         for key,value in fastqPaired.items():
-            print("PAIRED:", key, value)
             reverse = fastq.pop(key.replace("R1", "R2"))
-            fastq.pop(key)
+            forward = fastq.pop(key)
             key = key.removesuffix("R1").rstrip('-_')
-            print(key)
-            fastq[key] = metacerberus_merge.mergePairedEnd([value,reverse], config, f"{STEP[3]}/{key}/merged")
+            #TODO: quick fix, improve for Ray
+            r1,r2 = metacerberus_trim.trimPairedRead([key, [value,reverse]], config, Path(STEP[3], key))
+            value = metacerberus_merge.mergePairedEnd([r1,r2], config, f"{STEP[3]}/{key}/merged")
+            pipeline += [ray.put([key, value, 'trimSingleRead'])]
         del fastqPaired # memory cleanup
         # Trim
         for key,value in fastq.items():
-            print("Trimming:", key, value)
+            print("TRIM:", key, value)
             pipeline.append(rayWorkerThread.remote(metacerberus_trim.trimSingleRead, key, config['DIR_OUT'], [[key, value], config, Path(STEP[3], key)]))
 
     # Step 5 Contig Entry Point
     # Only do this if a fasta file was given, not if fastq
     if fasta:# and "scaffold" in config:
         print("\nSTEP 5a: Removing N's from contig files")
         for key,value in fasta.items():
@@ -465,36 +535,43 @@
 
     # Step 8 Protein Entry Point
     jobsORF = 0
     if amino:
         set_add(step_curr, 8, "STEP 8: HMMER Search")
         for key,value in amino.items():
             pipeline += [ray.put([key, value, 'findORF_'])]
-            jobsORF += 1
+            for hmm in dbHMM:
+                jobsORF += 1
 
     # Step 9 Rollup Entry Point
     hmm_tsv = dict()
+    hmm_tsvs = dict()
     if rollup:
         set_add(step_curr, 8.5, "STEP 8: Filtering rollup file(s)")
         for key,value in rollup.items():
             amino[key] = None
-            tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, "filtered.tsv")
-            pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, key, config['DIR_OUT'], [value, tsv_filtered, config['PATHDB']]))
+            for hmm in dbHMM:
+                tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, "filtered.tsv")
+                pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, f"{hmm}/{key}", config['DIR_OUT'], [value, tsv_filtered, dbHMM[hmm]]))
 
     NStats = dict()
     readStats = dict()
     report_path = os.path.join(config['DIR_OUT'], STEP[10])
+    final_path = Path(config['DIR_OUT'], "final")
 
     groupIndex = dict()
     amino_queue = dict()
-    jobs_per_node = int(-(config["CPUS"] // -4))
     dictChunks = dict()
-    dictFiltered = dict()
+    countFiltered = dict()
     hmmRollup = {}
     hmmCounts = {}
+    if config['CLUSTER']:
+        jobs_per_node = 4/config['CPUS']
+    else:
+        jobs_per_node = 4
     while pipeline:
         ready,pipeline = ray.wait(pipeline, timeout=1)
         if not ready:
             continue
         key,value,func = ray.get(ready[0])
 
         if func == "checkQuality":
@@ -575,78 +652,36 @@
                 if jobsORF > 0:
                     continue #Continue until all ORFs are done
                 value = outfile
                 key = "grouped"
             set_add(step_curr, 8, "STEP 8: HMMER Search")
             if value: # TODO: Put this check at top of "findORF_" block
                 amino[key] = value
-                if not config['CLUSTER']:
-                    if config['CHUNKER'] > 0:
-                        chunks = Chunker.Chunker(amino[key], os.path.join(config['DIR_OUT'], 'chunks', key), f"{config['CHUNKER']}M", '>')
-                        for hmm in dbHMM.items():
-                            chunkCount = 1
-                            for chunk in chunks.files:
-                                key_chunk = f'chunk-{hmm[0]}-{chunkCount}-{len(chunks.files)}_{key}'
-                                key_name = f'chunk-{chunkCount}-{len(chunks.files)}_{key}'
-                                chunkCount += 1
-                                pipeline.append(rayWorkerThread.options(num_cpus=4).remote(metacerberus_hmm.searchHMM, [key_chunk], config['DIR_OUT'],
-                                                                                        [{key_name:chunk}, config, Path(STEP[8], key), hmm, 4]))
-                    else:
-                        outfile = Path(config['DIR_OUT'], STEP[8], key, f'{key}.tsv')
-                        if config['REPLACE'] or not outfile.exists(): #TODO: Possible bug, will always be true
-                            for hmm in dbHMM.items():
-                                hmm_key = f"{hmm[0]}-{key}"
-                                pipeline.append(rayWorkerThread.options(num_cpus=4).remote(metacerberus_hmm.searchHMM, [hmm_key], config['DIR_OUT'],
-                                                                        [{key:value}, config, Path(STEP[8]), hmm, 4]))
-                        else:
-                            #TODO: distinguish filtered tsv per hmm
-                            tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, "filtered.tsv")
-                            set_add(step_curr, 8.1, "STEP 8: Filtering HMMER results")
-                            pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, key, config['DIR_OUT'], [tsv_out, tsv_filtered, config['PATHDB']]))
-
-                    continue
                 if config['CHUNKER'] > 0:
                     chunks = Chunker.Chunker(amino[key], os.path.join(config['DIR_OUT'], 'chunks', key), f"{config['CHUNKER']}M", '>')
-                    jobsORF -= 1
                     for hmm in dbHMM.items():
                         chunkCount = 1
                         for chunk in chunks.files:
-                            amino_queue[f'chunk-{hmm[0]}-{chunkCount}-{len(chunks.files)}_{key}'] = chunk
+                            key_chunk = f'chunk-{hmm[0]}-{chunkCount}-{len(chunks.files)}_{key}'
+                            key_name = f'chunk-{chunkCount}-{len(chunks.files)}_{key}'
                             chunkCount += 1
-                            # submit searchHMM jobs
-                            if len(amino_queue) >= jobs_per_node:
-                                pipeline.append(rayWorkerThread.remote(metacerberus_hmm.searchHMM, list(amino_queue.keys()), config['DIR_OUT'],
-                                                                    [amino_queue, config, Path(STEP[8]), hmm]))
-                                amino_queue = dict()
-                    if len(amino_queue) > 0:
-                        # Leftover chunks in queue not submited yet
-                        pipeline.append(rayWorkerThread.remote(metacerberus_hmm.searchHMM, list(amino_queue.keys()), config['DIR_OUT'],
-                                                                [amino_queue, config, Path(STEP[8]), hmm]))
-                        amino_queue = dict()
+                            pipeline.append(rayWorkerThread.options(num_cpus=jobs_per_node).remote(metacerberus_hmm.searchHMM, [key_chunk], config['DIR_OUT'],
+                                                                                    [{key_name:chunk}, config, Path(STEP[8], key), hmm, 4]))
                 else:
-                    jobsORF -= 1
-                    for hmm in dbHMM.items():
-                        #hmm_key = f"{hmm[0]}-{key}"
-                        amino_queue[key] = value
-                        if len(amino_queue) >= jobs_per_node:
-                            print("Sending to HMMER:")
-                            amino_names = list()
-                            for k,v in amino_queue.items():
-                                amino_names += [f"{hmm[0]}-{key}"]
-                                print(k, v)
-                                print(amino_names)
-                            pipeline.append(rayWorkerThread.remote(metacerberus_hmm.searchHMM, amino_names, config['DIR_OUT'],
-                                                                    [amino_queue, config, Path(STEP[8]), hmm]))
-                            amino_queue = dict()
-                # submit remaining searchHMM jobs
-                if len(amino_queue) >= jobs_per_node and jobsORF == 0:
-                    print("DEBUG: Remaining amino queue", amino_queue)
-                    pipeline.append(rayWorkerThread.remote(metacerberus_hmm.searchHMM, list(amino_queue.keys()), config['DIR_OUT'],
-                                                            [amino_queue, config, Path(STEP[8]), hmm]))
-                    amino_queue = dict()
+                    outfile = Path(config['DIR_OUT'], STEP[8], key, f'{key}.tsv')
+                    if config['REPLACE'] or not outfile.exists(): #TODO: Possible bug, will always be true
+                        for hmm in dbHMM.items():
+                            hmm_key = f"{hmm[0]}/{key}"
+                            pipeline.append(rayWorkerThread.options(num_cpus=jobs_per_node).remote(metacerberus_hmm.searchHMM, [hmm_key], config['DIR_OUT'],
+                                                                    [{key:value}, config, Path(STEP[8]), hmm, 4]))
+                    else:
+                        #TODO: distinguish filtered tsv per hmm
+                        tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, "filtered.tsv")
+                        set_add(step_curr, 8.1, "STEP 8: Filtering HMMER results")
+                        pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, key, config['DIR_OUT'], [tsv_out, tsv_filtered, dbHMM[hmm]]))
         if func.startswith('searchHMM'):
             keys = key
             for key,tsv_file in zip(keys,value):
                 match = re.search(r"^chunk-([A-Za-z_]+)-(\d+)-(\d+)_(.+)", key)
                 if match: # Matches if the keys are part of chunks
                     hmm,i,l,key = match.groups()
                     hmm_key = f"{hmm}-{key}"
@@ -669,108 +704,172 @@
                                 dictChunks[hmm_key].remove(item)
                                 if not config['KEEP']:
                                     os.remove(item)
                             set_add(step_curr, 8.1, "STEP 8: Filtering HMMER results")
                             for k in key_set:
                                 tsv_out = Path(config['DIR_OUT'], STEP[8], k, f"{hmm}-{k}.tsv")
                                 tsv_filtered = Path(config['DIR_OUT'], STEP[8], k, f"filtered-{hmm}.tsv")
-                                pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, k, config['DIR_OUT'], [tsv_out, tsv_filtered, config['PATHDB']]))
+                                pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, f"{hmm}/{k}", config['DIR_OUT'], [tsv_out, tsv_filtered, dbHMM[hmm]]))
                             # FINISH SPLITTING GROUP
                             continue
                         # Not grouped
-                        tsv_out = Path(config['DIR_OUT'], STEP[8], key, f"{hmm_key}.tsv")
+                        tsv_out = Path(config['DIR_OUT'], STEP[8], key, f"{hmm}-{key}.tsv")
                         tsv_out.parent.mkdir(parents=True, exist_ok=True)
                         with tsv_out.open('w') as writer:
                             for item in sorted(dictChunks[hmm_key]):
                                 writer.write(open(item).read())
                                 dictChunks[hmm_key].remove(item)
                                 if not config['KEEP']:
                                     os.remove(item)
                         tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, f"filtered-{hmm}.tsv")
                         set_add(step_curr, 8.1, "STEP 8: Filtering HMMER results")
-                        pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, key, config['DIR_OUT'], [tsv_out, tsv_filtered, config['PATHDB']]))
+                        pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, f"{hmm}/{key}", config['DIR_OUT'], [tsv_out, tsv_filtered, dbHMM[hmm]]))
                 else:
                 # Not chunked file
-                    key:str
-                    hmm_key = key
-                    hmm,key = key.split(sep='-', maxsplit=1)
-                    tsv_out = Path(config['DIR_OUT'], STEP[8], key, f"{hmm_key}.tsv")
+                    hmm,key = key.split(sep='/', maxsplit=1)
+                    tsv_out = Path(config['DIR_OUT'], STEP[8], key, f"{hmm}-{key}.tsv")
                     with tsv_out.open('w') as writer:
                         writer.write(open(tsv_file).read())
                     if not config['KEEP']:
                             os.remove(tsv_file)
                     set_add(step_curr, 8.1, "STEP 8: Filtering HMMER results")
                     tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, f"filtered-{hmm}.tsv")
-                    pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, key, config['DIR_OUT'], [tsv_out, tsv_filtered, config['PATHDB']]))
+                    pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, f"{hmm}/{key}", config['DIR_OUT'], [tsv_out, tsv_filtered, dbHMM[hmm]]))
         if func.startswith('filterHMM'):
+            hmm,key = key.split('/')
+            set_add(step_curr, 9, "STEP 9: Parse HMMER results")
+            pipeline.append(rayWorkerThread.remote(metacerberus_parser.parseHmmer, key, config['DIR_OUT'], [value, config, f"{STEP[9]}/{key}", hmm, dbHMM[hmm]]))
+            
             tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, "filtered.tsv")
-            if key not in dictFiltered:
-                dictFiltered[key] = 0
+            if key not in hmm_tsvs:
+                hmm_tsvs[key] = dict()
                 with tsv_filtered.open('w') as writer:
-                    print("target", "query", "e-value", "score", "length", "start", "end", sep='\t', file=writer)
-            dictFiltered[key] += 1
-            with tsv_filtered.open('a') as writer:
-                writer.write(open(value).read())
-            if dictFiltered[key] == len(dbHMM):
+                    print("target", "query", "e-value", "score", "length", "start", "end", "hmmDB", sep='\t', file=writer)
+            if hmm not in hmm_tsvs[key]:
+                hmm_tsvs[key][hmm] = value
+            with tsv_filtered.open('a') as writer, open(value) as reader:
+                reader.readline() # Skip header
+                for line in reader:
+                    print(*line.rstrip('\n').split('\t'), hmm, sep='\t', file=writer)
+            if len(hmm_tsvs[key]) == len(dbHMM):
+                # old method
                 hmm_tsv[key] = tsv_filtered
-                set_add(step_curr, 9, "STEP 9: Parse HMMER results")
-                pipeline.append(rayWorkerThread.remote(metacerberus_parser.parseHmmer, key, config['DIR_OUT'], [tsv_filtered, config, f"{STEP[9]}/{key}"]))
+                outfile = Path(config['DIR_OUT'], STEP[9], key, f"top_5-{key}.tsv")
+                pipeline.append(rayWorkerThread.remote(metacerberus_parser.top5, key, config['DIR_OUT'],
+                                                       [tsv_filtered, outfile]))
+                # new method
+                outfile = Path(config['DIR_OUT'], STEP[9], key, "HMMER_top_5.tsv")
+                pipeline.append(rayWorkerThread.remote(metacerberus_parser.top5s, key, config['DIR_OUT'],
+                                                       [hmm_tsvs[key], outfile]))
         if func.startswith('parseHmmer'):
-            hmmRollup[key] = value
+            if key not in hmmRollup:
+                hmmRollup[key] = dict()
+            hmmRollup[key].update(value)
             pipeline.append(rayWorkerThread.remote(metacerberus_parser.createCountTables, key, config['DIR_OUT'], [value, config, f"{STEP[9]}/{key}"]))
         if func.startswith('createCountTables'):
-            hmmCounts[key] = value
+            if key not in hmmCounts:
+                hmmCounts[key] = dict()
+            hmmCounts[key].update(value)
 
     # End main pipeline
 
     # Log time of main pipeline
     time_pipeline = str(datetime.timedelta(seconds=time.time()-startTime))
     logTime(config["DIR_OUT"], socket.gethostname(), "Pipeline_time", config["DIR_OUT"], time_pipeline)
 
     # step 10 (Report)
     print("\nSTEP 10: Creating Reports")
 
-    # Copy report files from QC, Parser
-    for key in hmmRollup.keys():
-        os.makedirs(os.path.join(report_path, key), exist_ok=True)
-        shutil.copy( os.path.join(config['DIR_OUT'], config['STEP'][9], key, "HMMER_top_5.tsv"), os.path.join(report_path, key) )
+    ## Copy report files from QC, Parser
+    #for key in hmmRollup.keys():
+    #    Path(report_path, key).mkdir(0o777, True, True)
+    #    src = os.path.join(config['DIR_OUT'], config['STEP'][9], key, "HMMER_top_5.tsv")
+    #    dst = os.path.join(report_path, key)
+    #    shutil.copy(src, dst)
 
     # Write Stats
-    print("Saving Statistics")
+    Path(final_path, "fasta").mkdir(0o777, True, True)
+    print("Creating final reports and statistics")
     protStats = {}
-    for key in hmm_tsv.keys():
-        protStats[key] = metacerberus_prostats.getStats(amino[key], hmm_tsv[key], hmmCounts[key], config, Path(report_path, key, 'annotation_summary.tsv'))
+    for key in hmm_tsvs.keys():
+        # Copy report files from QC, Parser
+        Path(report_path, key).mkdir(0o777, True, True)
+        Path(final_path, key).mkdir(0o777, True, True)
+        src = os.path.join(config['DIR_OUT'], config['STEP'][9], key, "HMMER_top_5.tsv")
+        dst = Path(final_path, key)
+        shutil.copy(src, dst)
+        # Protein statistics & annotation summary
+        summary = Path(final_path, key, 'final_annotation_summary.tsv')
+        protStats[key] = metacerberus_prostats.getStats(amino[key], hmm_tsvs[key], hmmCounts[key], config, dbHMM, summary, Path(final_path, "fasta", f"{key}.faa"))
+        try:
+            src = Path(amino[key]).with_suffix(".ffn")
+            dst = Path(final_path, "fasta", f"{key}.ffn")
+            shutil.copy(src, dst)
+        except: pass
+        try:
+            src = Path(fasta[key])
+            dst = Path(final_path, "fasta", f"{key}.fna")
+            shutil.copy(src, dst)
+        except: pass
+        # Create GFFs #TODO: Incorporate this into getStats (or separate all summary into new module)
+        gff = [x for x in Path(config['DIR_OUT'], STEP[7], key).glob("*.gff")]
+        Path(final_path, "gff").mkdir(511, True, True)
+        if len(gff) == 1:
+            out_gff = Path(final_path, "gff", f"{key}.gff")
+            out_genbank = Path(final_path, f"{key}_template.gbk")
+            metacerberus_report.write_datafiles(gff[0], fasta[key], amino[key], summary, out_gff, out_genbank)
+        else:
+            print("GFF", "NONE")
+            out_gff = Path(final_path, "gff", f"{key}.gff")
+            with out_gff.open('w') as writer:
+                with summary.open() as read_summary:
+                    read_summary.readline()
+                    print("##gff-version  3", file=writer)
+                    for summ in read_summary:
+                        summ = summ.split('\t')
+                        data = [summ[0].split('_')[0], ".", ".", ".", ".", ".", ".", ".", ]
+                        attributes = ';'.join([f"ID={summ[0]}", f"Name={summ[1]}", f"Alias={summ[2]}", f"Dbxref={summ[3]}", f"evalue={summ[4]}", f"product_start={summ[8]}", f"product_end={summ[9]}", f"product_length={summ[10]}"])
+                        print(*data, attributes, sep='\t', file=writer)
+                try:
+                    with open(fasta[key]) as read_fasta:
+                        print("##FASTA", file=writer)
+                        for line in read_fasta:
+                            writer.write(line)
+                except: pass
     metacerberus_report.write_Stats(report_path, readStats, protStats, NStats, config)
     del protStats
 
     # Write Roll-up Tables
     print("Creating Rollup Tables")
     for sample,tables in hmmCounts.items():
         os.makedirs(f"{report_path}/{sample}", exist_ok=True)
         for name,table in tables.items():
             metacerberus_report.writeTables(table, f"{report_path}/{sample}/{name}")
     for sample,tables in hmmRollup.items():
         os.makedirs(f"{report_path}/{sample}", exist_ok=True)
         for name,table in tables.items():
-            shutil.copy(table, Path(report_path, sample, f'{name}_rollup.tsv'))
+            shutil.copy(table, Path(final_path, sample, f'rollup_{name}.tsv'))
 
     # Counts Tables
-    print("Creating Count Tables")
+    print("Mergeing Count Tables")
     dfCounts = dict()
-    for dbName in ['FOAM', 'KEGG', 'COG', 'CAZy', 'PHROG', 'VOG']:
+    for dbname,dbpath in dbHMM.items():
         tsv_list = dict()
         for name in hmm_tsv.keys():
-            table_path = Path(config['DIR_OUT'], STEP[9], name, f'counts_{dbName}.tsv')
+            if dbname.startswith("KOFam"):
+                dbLookup = re.search(r"KOFam_.*_([A-Z]+)", dbname).group(1)
+                dbLookup = dbpath.with_name(f'{dbLookup}.tsv')
+            table_path = Path(config['DIR_OUT'], STEP[9], name, f'counts_{dbname}.tsv')
             if table_path.exists():
                 name = re.sub(rf'^FragGeneScan_|prodigal_|Protein_', '', name)
                 tsv_list[name] = table_path
-        combined_path = Path(config['DIR_OUT'], STEP[10], 'combined', f'counts_{dbName}.tsv')
+        combined_path = Path(config['DIR_OUT'], STEP[10], 'combined', f'counts_{dbname}.tsv')
         metacerberus_parser.merge_tsv(tsv_list, Path(combined_path))
         if combined_path.exists():
-            dfCounts[dbName] = combined_path
+            dfCounts[dbname] = combined_path
         del(combined_path)
 
     # PCA output (HTML)
     pcaFigures = None
     if config['SKIP_PCA']:
         pass
     elif len(hmm_tsv) < 4:
@@ -778,81 +877,89 @@
     else:
         print("PCA Analysis")
         pcaFigures = metacerberus_visual.graphPCA(dfCounts)
         Path(report_path, 'combined').mkdir(parents=True, exist_ok=True)
         metacerberus_report.write_PCA(os.path.join(report_path, "combined"), pcaFigures)
 
     # Run post processing analysis in R
-    if len(hmm_tsv) < 4:
-        print("NOTE: Pathview created only when there are at least four sequence files.\n")
+    if not [True for x in dfCounts if x.startswith("KOFam")]:
+        print("NOTE: Pathview created only when KOFams are used since it uses KOs for its analysis.\n")
+    elif len(hmm_tsv) < 4 or not config['CLASS']:
+        print("NOTE: Pathview created only when there are at least four sequence files, and a class tsv file is specified with --class specifying the class for each input file.\n")
     else:
-        if config['CLASS']:
-            print("\nSTEP 11: Post Analysis with GAGE and Pathview")
-            outpathview = Path(report_path, 'pathview')
-            outpathview.mkdir(exist_ok=True, parents=True)
-            rscript = Path(outpathview, 'run_pathview.sh')
-
-            # Check for internet
-            try:
-                #attempt to connect to Google
-                request.urlopen('http://216.58.195.142', timeout=1)
-                is_internet = True
-            except:
-                is_internet = False
-            
-            with rscript.open('w') as writer:
-                writer.write(f"#!/bin/bash\n\n")
-                for name,countpath in dfCounts.items():
-                    if name not in ['FOAM', 'KEGG']:
-                        continue
-                    shutil.copy(countpath, Path(outpathview, f"{name}_counts.tsv"))
-                    shutil.copy(config['CLASS'], Path(outpathview, f"{name}_class.tsv"))
-                    writer.write(f"mkdir -p {name}\n")
-                    writer.write(f"cd {name}\n")
-                    writer.write(f"pathview-metacerberus.R ../{name}_counts.tsv ../{name}_class.tsv\n")
-                    writer.write(f"cd ..\n")
-                    outcmd = Path(outpathview, name)
-                    outcmd.mkdir(parents=True, exist_ok=True)
-                    if is_internet:
-                        subprocess.run(['pathview-metacerberus.R', countpath, config['CLASS']],
-                                        cwd=outcmd,
-                                        stdout=Path(outcmd, 'stdout.txt').open('w'),
-                                        stderr=Path(outcmd, 'stderr.txt').open('w')
-                                    )
-            if not is_internet:
-                print(f"GAGE and Pathview require internet access to run. Run the script '{rscript}'")
+        print("\nSTEP 11: Post Analysis with GAGE and Pathview")
+        outpathview = Path(report_path, 'pathview')
+        outpathview.mkdir(exist_ok=True, parents=True)
+        rscript = Path(outpathview, 'run_pathview.sh')
+
+        # Check for internet
+        try:
+            #attempt to connect to Google
+            request.urlopen('http://216.58.195.142', timeout=1)
+            is_internet = True
+        except:
+            is_internet = False
+        
+        with rscript.open('w') as writer:
+            writer.write(f"#!/bin/bash\n\n")
+            for name,countpath in dfCounts.items():
+                if not name.startswith("KOFam"):
+                    continue
+                shutil.copy(countpath, Path(outpathview, f"{name}_counts.tsv"))
+                shutil.copy(config['CLASS'], Path(outpathview, f"{name}_class.tsv"))
+                writer.write(f"mkdir -p {name}\n")
+                writer.write(f"cd {name}\n")
+                writer.write(f"pathview-metacerberus.R ../{name}_counts.tsv ../{name}_class.tsv\n")
+                writer.write(f"cd ..\n")
+                outcmd = Path(outpathview, name)
+                outcmd.mkdir(parents=True, exist_ok=True)
+                if is_internet:
+                    subprocess.run(['pathview-metacerberus.R', countpath, config['CLASS']],
+                                    cwd=outcmd,
+                                    stdout=Path(outcmd, 'stdout.txt').open('w'),
+                                    stderr=Path(outcmd, 'stderr.txt').open('w')
+                                )
+        if not is_internet:
+            print(f"GAGE and Pathview require internet access to run. Run the script '{rscript}'")
 
     # Figure outputs (HTML)
     print("Creating combined sunburst and bargraphs")
     figSunburst = {}
     for key,value in hmmCounts.items():
         figSunburst[key] = metacerberus_visual.graphSunburst(value)
-    
-    @ray.remote
-    def graphCharts(key, rollup, counts):
-        return key, metacerberus_visual.graphBarcharts(rollup, counts)
 
+    #@ray.remote
+    #def graphCharts(key, rollup, counts):
+    #    return key, metacerberus_visual.graphBarcharts(rollup, counts)
+    
     jobCharts = []
     for key,value in hmmRollup.items():
-        jobCharts.append( graphCharts.remote(key, value, hmmCounts[key]) )
+        #jobCharts.append( graphCharts.remote(key, value, hmmCounts[key]) )
+        jobCharts.append( rayWorkerThread.remote(metacerberus_visual.graphBarcharts, key, config['DIR_OUT'], [value, hmmCounts[key]]) )
     
     figCharts = {}
     while(jobCharts):
         ready,jobCharts = ray.wait(jobCharts)
         if ready:
-            key,value = ray.get(ready[0])
+            key,value,_ = ray.get(ready[0])
             figCharts[key] = value
 
     metacerberus_report.createReport(figSunburst, figCharts, config, STEP[10])
 
     # Finished!
     print("\nFinished Pipeline")
     end = str(datetime.timedelta(seconds=time.time()-startTime))
     logTime(config["DIR_OUT"], socket.gethostname(), "Total_Time", config["DIR_OUT"], end)
 
+    # Cleaning up
+    temp_dir = Path(ray.nodes()[0]['ObjectStoreSocketName']).parent.parent
+    print("Cleaning up Ray temporary directory", temp_dir)
+    ray.shutdown()
+    shutil.rmtree(temp_dir)
+
     return 0
 
 
 ## Start main method
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `MetaCerberus-1.2.1/bin/pathview-metacerberus.R` & `metacerberus-1.3.0/bin/pathview-metacerberus.R`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/bin/ray-slurm-metacerberus.sh` & `metacerberus-1.3.0/bin/ray-slurm-metacerberus.sh`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/Chunker.py` & `metacerberus-1.3.0/lib/Chunker.py`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/FGS/FragGeneScanRS-Darwin.tar.gz` & `metacerberus-1.3.0/lib/FGS/FragGeneScanRS-Darwin.tar.gz`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/FGS/FragGeneScanRS-Linux.tar.gz` & `metacerberus-1.3.0/lib/FGS/FragGeneScanRS-Linux.tar.gz`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/PHANOTATE/tests/NC_001416.1.fasta` & `metacerberus-1.3.0/lib/dependency_files/lambda-phage.fna`

 * *Files 1% similar despite different names*

```diff
@@ -1,695 +1,608 @@
->NC_001416
-GGGCGGCGACCTCGCGGGTTTTCGCTATTTATGAAAATTTTCCGGTTTAAGGCGTTTCCGTTCTTCTTCG
-TCATAACTTAATGTTTTTATTTAAAATACCCTCTGAAAAGAAAGGAAACGACAGGTGCTGAAAGCGAGGC
-TTTTTGGCCTCTGTCGTTTCCTTTCTCTGTTTTTGTCCGTGGAATGAACAATGGAAGTCAACAAAAAGCA
-GCTGGCTGACATTTTCGGTGCGAGTATCCGTACCATTCAGAACTGGCAGGAACAGGGAATGCCCGTTCTG
-CGAGGCGGTGGCAAGGGTAATGAGGTGCTTTATGACTCTGCCGCCGTCATAAAATGGTATGCCGAAAGGG
-ATGCTGAAATTGAGAACGAAAAGCTGCGCCGGGAGGTTGAAGAACTGCGGCAGGCCAGCGAGGCAGATCT
-CCAGCCAGGAACTATTGAGTACGAACGCCATCGACTTACGCGTGCGCAGGCCGACGCACAGGAACTGAAG
-AATGCCAGAGACTCCGCTGAAGTGGTGGAAACCGCATTCTGTACTTTCGTGCTGTCGCGGATCGCAGGTG
-AAATTGCCAGTATTCTCGACGGGCTCCCCCTGTCGGTGCAGCGGCGTTTTCCGGAACTGGAAAACCGACA
-TGTTGATTTCCTGAAACGGGATATCATCAAAGCCATGAACAAAGCAGCCGCGCTGGATGAACTGATACCG
-GGGTTGCTGAGTGAATATATCGAACAGTCAGGTTAACAGGCTGCGGCATTTTGTCCGCGCCGGGCTTCGC
-TCACTGTTCAGGCCGGAGCCACAGACCGCCGTTGAATGGGCGGATGCTAATTACTATCTCCCGAAAGAAT
-CCGCATACCAGGAAGGGCGCTGGGAAACACTGCCCTTTCAGCGGGCCATCATGAATGCGATGGGCAGCGA
-CTACATCCGTGAGGTGAATGTGGTGAAGTCTGCCCGTGTCGGTTATTCCAAAATGCTGCTGGGTGTTTAT
-GCCTACTTTATAGAGCATAAGCAGCGCAACACCCTTATCTGGTTGCCGACGGATGGTGATGCCGAGAACT
-TTATGAAAACCCACGTTGAGCCGACTATTCGTGATATTCCGTCGCTGCTGGCGCTGGCCCCGTGGTATGG
-CAAAAAGCACCGGGATAACACGCTCACCATGAAGCGTTTCACTAATGGGCGTGGCTTCTGGTGCCTGGGC
-GGTAAAGCGGCAAAAAACTACCGTGAAAAGTCGGTGGATGTGGCGGGTTATGATGAACTTGCTGCTTTTG
-ATGATGATATTGAACAGGAAGGCTCTCCGACGTTCCTGGGTGACAAGCGTATTGAAGGCTCGGTCTGGCC
-AAAGTCCATCCGTGGCTCCACGCCAAAAGTGAGAGGCACCTGTCAGATTGAGCGTGCAGCCAGTGAATCC
-CCGCATTTTATGCGTTTTCATGTTGCCTGCCCGCATTGCGGGGAGGAGCAGTATCTTAAATTTGGCGACA
-AAGAGACGCCGTTTGGCCTCAAATGGACGCCGGATGACCCCTCCAGCGTGTTTTATCTCTGCGAGCATAA
-TGCCTGCGTCATCCGCCAGCAGGAGCTGGACTTTACTGATGCCCGTTATATCTGCGAAAAGACCGGGATC
-TGGACCCGTGATGGCATTCTCTGGTTTTCGTCATCCGGTGAAGAGATTGAGCCACCTGACAGTGTGACCT
-TTCACATCTGGACAGCGTACAGCCCGTTCACCACCTGGGTGCAGATTGTCAAAGACTGGATGAAAACGAA
-AGGGGATACGGGAAAACGTAAAACCTTCGTAAACACCACGCTCGGTGAGACGTGGGAGGCGAAAATTGGC
-GAACGTCCGGATGCTGAAGTGATGGCAGAGCGGAAAGAGCATTATTCAGCGCCCGTTCCTGACCGTGTGG
-CTTACCTGACCGCCGGTATCGACTCCCAGCTGGACCGCTACGAAATGCGCGTATGGGGATGGGGGCCGGG
-TGAGGAAAGCTGGCTGATTGACCGGCAGATTATTATGGGCCGCCACGACGATGAACAGACGCTGCTGCGT
-GTGGATGAGGCCATCAATAAAACCTATACCCGCCGGAATGGTGCAGAAATGTCGATATCCCGTATCTGCT
-GGGATACTGGCGGGATTGACCCGACCATTGTGTATGAACGCTCGAAAAAACATGGGCTGTTCCGGGTGAT
-CCCCATTAAAGGGGCATCCGTCTACGGAAAGCCGGTGGCCAGCATGCCACGTAAGCGAAACAAAAACGGG
-GTTTACCTTACCGAAATCGGTACGGATACCGCGAAAGAGCAGATTTATAACCGCTTCACACTGACGCCGG
-AAGGGGATGAACCGCTTCCCGGTGCCGTTCACTTCCCGAATAACCCGGATATTTTTGATCTGACCGAAGC
-GCAGCAGCTGACTGCTGAAGAGCAGGTCGAAAAATGGGTGGATGGCAGGAAAAAAATACTGTGGGACAGC
-AAAAAGCGACGCAATGAGGCACTCGACTGCTTCGTTTATGCGCTGGCGGCGCTGCGCATCAGTATTTCCC
-GCTGGCAGCTGGATCTCAGTGCGCTGCTGGCGAGCCTGCAGGAAGAGGATGGTGCAGCAACCAACAAGAA
-AACACTGGCAGATTACGCCCGTGCCTTATCCGGAGAGGATGAATGACGCGACAGGAAGAACTTGCCGCTG
-CCCGTGCGGCACTGCATGACCTGATGACAGGTAAACGGGTGGCAACAGTACAGAAAGACGGACGAAGGGT
-GGAGTTTACGGCCACTTCCGTGTCTGACCTGAAAAAATATATTGCAGAGCTGGAAGTGCAGACCGGCATG
-ACACAGCGACGCAGGGGACCTGCAGGATTTTATGTATGAAAACGCCCACCATTCCCACCCTTCTGGGGCC
-GGACGGCATGACATCGCTGCGCGAATATGCCGGTTATCACGGCGGTGGCAGCGGATTTGGAGGGCAGTTG
-CGGTCGTGGAACCCACCGAGTGAAAGTGTGGATGCAGCCCTGTTGCCCAACTTTACCCGTGGCAATGCCC
-GCGCAGACGATCTGGTACGCAATAACGGCTATGCCGCCAACGCCATCCAGCTGCATCAGGATCATATCGT
-CGGGTCTTTTTTCCGGCTCAGTCATCGCCCAAGCTGGCGCTATCTGGGCATCGGGGAGGAAGAAGCCCGT
-GCCTTTTCCCGCGAGGTTGAAGCGGCATGGAAAGAGTTTGCCGAGGATGACTGCTGCTGCATTGACGTTG
-AGCGAAAACGCACGTTTACCATGATGATTCGGGAAGGTGTGGCCATGCACGCCTTTAACGGTGAACTGTT
-CGTTCAGGCCACCTGGGATACCAGTTCGTCGCGGCTTTTCCGGACACAGTTCCGGATGGTCAGCCCGAAG
-CGCATCAGCAACCCGAACAATACCGGCGACAGCCGGAACTGCCGTGCCGGTGTGCAGATTAATGACAGCG
-GTGCGGCGCTGGGATATTACGTCAGCGAGGACGGGTATCCTGGCTGGATGCCGCAGAAATGGACATGGAT
-ACCCCGTGAGTTACCCGGCGGGCGCGCCTCGTTCATTCACGTTTTTGAACCCGTGGAGGACGGGCAGACT
-CGCGGTGCAAATGTGTTTTACAGCGTGATGGAGCAGATGAAGATGCTCGACACGCTGCAGAACACGCAGC
-TGCAGAGCGCCATTGTGAAGGCGATGTATGCCGCCACCATTGAGAGTGAGCTGGATACGCAGTCAGCGAT
-GGATTTTATTCTGGGCGCGAACAGTCAGGAGCAGCGGGAAAGGCTGACCGGCTGGATTGGTGAAATTGCC
-GCGTATTACGCCGCAGCGCCGGTCCGGCTGGGAGGCGCAAAAGTACCGCACCTGATGCCGGGTGACTCAC
-TGAACCTGCAGACGGCTCAGGATACGGATAACGGCTACTCCGTGTTTGAGCAGTCACTGCTGCGGTATAT
-CGCTGCCGGGCTGGGTGTCTCGTATGAGCAGCTTTCCCGGAATTACGCCCAGATGAGCTACTCCACGGCA
-CGGGCCAGTGCGAACGAGTCGTGGGCGTACTTTATGGGGCGGCGAAAATTCGTCGCATCCCGTCAGGCGA
-GCCAGATGTTTCTGTGCTGGCTGGAAGAGGCCATCGTTCGCCGCGTGGTGACGTTACCTTCAAAAGCGCG
-CTTCAGTTTTCAGGAAGCCCGCAGTGCCTGGGGGAACTGCGACTGGATAGGCTCCGGTCGTATGGCCATC
-GATGGTCTGAAAGAAGTTCAGGAAGCGGTGATGCTGATAGAAGCCGGACTGAGTACCTACGAGAAAGAGT
-GCGCAAAACGCGGTGACGACTATCAGGAAATTTTTGCCCAGCAGGTCCGTGAAACGATGGAGCGCCGTGC
-AGCCGGTCTTAAACCGCCCGCCTGGGCGGCTGCAGCATTTGAATCCGGGCTGCGACAATCAACAGAGGAG
-GAGAAGAGTGACAGCAGAGCTGCGTAATCTCCCGCATATTGCCAGCATGGCCTTTAATGAGCCGCTGATG
-CTTGAACCCGCCTATGCGCGGGTTTTCTTTTGTGCGCTTGCAGGCCAGCTTGGGATCAGCAGCCTGACGG
-ATGCGGTGTCCGGCGACAGCCTGACTGCCCAGGAGGCACTCGCGACGCTGGCATTATCCGGTGATGATGA
-CGGACCACGACAGGCCCGCAGTTATCAGGTCATGAACGGCATCGCCGTGCTGCCGGTGTCCGGCACGCTG
-GTCAGCCGGACGCGGGCGCTGCAGCCGTACTCGGGGATGACCGGTTACAACGGCATTATCGCCCGTCTGC
-AACAGGCTGCCAGCGATCCGATGGTGGACGGCATTCTGCTCGATATGGACACGCCCGGCGGGATGGTGGC
-GGGGGCATTTGACTGCGCTGACATCATCGCCCGTGTGCGTGACATAAAACCGGTATGGGCGCTTGCCAAC
-GACATGAACTGCAGTGCAGGTCAGTTGCTTGCCAGTGCCGCCTCCCGGCGTCTGGTCACGCAGACCGCCC
-GGACAGGCTCCATCGGCGTCATGATGGCTCACAGTAATTACGGTGCTGCGCTGGAGAAACAGGGTGTGGA
-AATCACGCTGATTTACAGCGGCAGCCATAAGGTGGATGGCAACCCCTACAGCCATCTTCCGGATGACGTC
-CGGGAGACACTGCAGTCCCGGATGGACGCAACCCGCCAGATGTTTGCGCAGAAGGTGTCGGCATATACCG
-GCCTGTCCGTGCAGGTTGTGCTGGATACCGAGGCTGCAGTGTACAGCGGTCAGGAGGCCATTGATGCCGG
-ACTGGCTGATGAACTTGTTAACAGCACCGATGCGATCACCGTCATGCGTGATGCACTGGATGCACGTAAA
-TCCCGTCTCTCAGGAGGGCGAATGACCAAAGAGACTCAATCAACAACTGTTTCAGCCACTGCTTCGCAGG
-CTGACGTTACTGACGTGGTGCCAGCGACGGAGGGCGAGAACGCCAGCGCGGCGCAGCCGGACGTGAACGC
-GCAGATCACCGCAGCGGTTGCGGCAGAAAACAGCCGCATTATGGGGATCCTCAACTGTGAGGAGGCTCAC
-GGACGCGAAGAACAGGCACGCGTGCTGGCAGAAACCCCCGGTATGACCGTGAAAACGGCCCGCCGCATTC
-TGGCCGCAGCACCACAGAGTGCACAGGCGCGCAGTGACACTGCGCTGGATCGTCTGATGCAGGGGGCACC
-GGCACCGCTGGCTGCAGGTAACCCGGCATCTGATGCCGTTAACGATTTGCTGAACACACCAGTGTAAGGG
-ATGTTTATGACGAGCAAAGAAACCTTTACCCATTACCAGCCGCAGGGCAACAGTGACCCGGCTCATACCG
-CAACCGCGCCCGGCGGATTGAGTGCGAAAGCGCCTGCAATGACCCCGCTGATGCTGGACACCTCCAGCCG
-TAAGCTGGTTGCGTGGGATGGCACCACCGACGGTGCTGCCGTTGGCATTCTTGCGGTTGCTGCTGACCAG
-ACCAGCACCACGCTGACGTTCTACAAGTCCGGCACGTTCCGTTATGAGGATGTGCTCTGGCCGGAGGCTG
-CCAGCGACGAGACGAAAAAACGGACCGCGTTTGCCGGAACGGCAATCAGCATCGTTTAACTTTACCCTTC
-ATCACTAAAGGCCGCCTGTGCGGCTTTTTTTACGGGATTTTTTTATGTCGATGTACACAACCGCCCAACT
-GCTGGCGGCAAATGAGCAGAAATTTAAGTTTGATCCGCTGTTTCTGCGTCTCTTTTTCCGTGAGAGCTAT
-CCCTTCACCACGGAGAAAGTCTATCTCTCACAAATTCCGGGACTGGTAAACATGGCGCTGTACGTTTCGC
-CGATTGTTTCCGGTGAGGTTATCCGTTCCCGTGGCGGCTCCACCTCTGAATTTACGCCGGGATATGTCAA
-GCCGAAGCATGAAGTGAATCCGCAGATGACCCTGCGTCGCCTGCCGGATGAAGATCCGCAGAATCTGGCG
-GACCCGGCTTACCGCCGCCGTCGCATCATCATGCAGAACATGCGTGACGAAGAGCTGGCCATTGCTCAGG
-TCGAAGAGATGCAGGCAGTTTCTGCCGTGCTTAAGGGCAAATACACCATGACCGGTGAAGCCTTCGATCC
-GGTTGAGGTGGATATGGGCCGCAGTGAGGAGAATAACATCACGCAGTCCGGCGGCACGGAGTGGAGCAAG
-CGTGACAAGTCCACGTATGACCCGACCGACGATATCGAAGCCTACGCGCTGAACGCCAGCGGTGTGGTGA
-ATATCATCGTGTTCGATCCGAAAGGCTGGGCGCTGTTCCGTTCCTTCAAAGCCGTCAAGGAGAAGCTGGA
-TACCCGTCGTGGCTCTAATTCCGAGCTGGAGACAGCGGTGAAAGACCTGGGCAAAGCGGTGTCCTATAAG
-GGGATGTATGGCGATGTGGCCATCGTCGTGTATTCCGGACAGTACGTGGAAAACGGCGTCAAAAAGAACT
-TCCTGCCGGACAACACGATGGTGCTGGGGAACACTCAGGCACGCGGTCTGCGCACCTATGGCTGCATTCA
-GGATGCGGACGCACAGCGCGAAGGCATTAACGCCTCTGCCCGTTACCCGAAAAACTGGGTGACCACCGGC
-GATCCGGCGCGTGAGTTCACCATGATTCAGTCAGCACCGCTGATGCTGCTGGCTGACCCTGATGAGTTCG
-TGTCCGTACAACTGGCGTAATCATGGCCCTTCGGGGCCATTGTTTCTCTGTGGAGGAGTCCATGACGAAA
-GATGAACTGATTGCCCGTCTCCGCTCGCTGGGTGAACAACTGAACCGTGATGTCAGCCTGACGGGGACGA
-AAGAAGAACTGGCGCTCCGTGTGGCAGAGCTGAAAGAGGAGCTTGATGACACGGATGAAACTGCCGGTCA
-GGACACCCCTCTCAGCCGGGAAAATGTGCTGACCGGACATGAAAATGAGGTGGGATCAGCGCAGCCGGAT
-ACCGTGATTCTGGATACGTCTGAACTGGTCACGGTCGTGGCACTGGTGAAGCTGCATACTGATGCACTTC
-ACGCCACGCGGGATGAACCTGTGGCATTTGTGCTGCCGGGAACGGCGTTTCGTGTCTCTGCCGGTGTGGC
-AGCCGAAATGACAGAGCGCGGCCTGGCCAGAATGCAATAACGGGAGGCGCTGTGGCTGATTTCGATAACC
-TGTTCGATGCTGCCATTGCCCGCGCCGATGAAACGATACGCGGGTACATGGGAACGTCAGCCACCATTAC
-ATCCGGTGAGCAGTCAGGTGCGGTGATACGTGGTGTTTTTGATGACCCTGAAAATATCAGCTATGCCGGA
-CAGGGCGTGCGCGTTGAAGGCTCCAGCCCGTCCCTGTTTGTCCGGACTGATGAGGTGCGGCAGCTGCGGC
-GTGGAGACACGCTGACCATCGGTGAGGAAAATTTCTGGGTAGATCGGGTTTCGCCGGATGATGGCGGAAG
-TTGTCATCTCTGGCTTGGACGGGGCGTACCGCCTGCCGTTAACCGTCGCCGCTGAAAGGGGGATGTATGG
-CCATAAAAGGTCTTGAGCAGGCCGTTGAAAACCTCAGCCGTATCAGCAAAACGGCGGTGCCTGGTGCCGC
-CGCAATGGCCATTAACCGCGTTGCTTCATCCGCGATATCGCAGTCGGCGTCACAGGTTGCCCGTGAGACA
-AAGGTACGCCGGAAACTGGTAAAGGAAAGGGCCAGGCTGAAAAGGGCCACGGTCAAAAATCCGCAGGCCA
-GAATCAAAGTTAACCGGGGGGATTTGCCCGTAATCAAGCTGGGTAATGCGCGGGTTGTCCTTTCGCGCCG
-CAGGCGTCGTAAAAAGGGGCAGCGTTCATCCCTGAAAGGTGGCGGCAGCGTGCTTGTGGTGGGTAACCGT
-CGTATTCCCGGCGCGTTTATTCAGCAACTGAAAAATGGCCGGTGGCATGTCATGCAGCGTGTGGCTGGGA
-AAAACCGTTACCCCATTGATGTGGTGAAAATCCCGATGGCGGTGCCGCTGACCACGGCGTTTAAACAAAA
-TATTGAGCGGATACGGCGTGAACGTCTTCCGAAAGAGCTGGGCTATGCGCTGCAGCATCAACTGAGGATG
-GTAATAAAGCGATGAAACATACTGAACTCCGTGCAGCCGTACTGGATGCACTGGAGAAGCATGACACCGG
-GGCGACGTTTTTTGATGGTCGCCCCGCTGTTTTTGATGAGGCGGATTTTCCGGCAGTTGCCGTTTATCTC
-ACCGGCGCTGAATACACGGGCGAAGAGCTGGACAGCGATACCTGGCAGGCGGAGCTGCATATCGAAGTTT
-TCCTGCCTGCTCAGGTGCCGGATTCAGAGCTGGATGCGTGGATGGAGTCCCGGATTTATCCGGTGATGAG
-CGATATCCCGGCACTGTCAGATTTGATCACCAGTATGGTGGCCAGCGGCTATGACTACCGGCGCGACGAT
-GATGCGGGCTTGTGGAGTTCAGCCGATCTGACTTATGTCATTACCTATGAAATGTGAGGACGCTATGCCT
-GTACCAAATCCTACAATGCCGGTGAAAGGTGCCGGGACCACCCTGTGGGTTTATAAGGGGAGCGGTGACC
-CTTACGCGAATCCGCTTTCAGACGTTGACTGGTCGCGTCTGGCAAAAGTTAAAGACCTGACGCCCGGCGA
-ACTGACCGCTGAGTCCTATGACGACAGCTATCTCGATGATGAAGATGCAGACTGGACTGCGACCGGGCAG
-GGGCAGAAATCTGCCGGAGATACCAGCTTCACGCTGGCGTGGATGCCCGGAGAGCAGGGGCAGCAGGCGC
-TGCTGGCGTGGTTTAATGAAGGCGATACCCGTGCCTATAAAATCCGCTTCCCGAACGGCACGGTCGATGT
-GTTCCGTGGCTGGGTCAGCAGTATCGGTAAGGCGGTGACGGCGAAGGAAGTGATCACCCGCACGGTGAAA
-GTCACCAATGTGGGACGTCCGTCGATGGCAGAAGATCGCAGCACGGTAACAGCGGCAACCGGCATGACCG
-TGACGCCTGCCAGCACCTCGGTGGTGAAAGGGCAGAGCACCACGCTGACCGTGGCCTTCCAGCCGGAGGG
-CGTAACCGACAAGAGCTTTCGTGCGGTGTCTGCGGATAAAACAAAAGCCACCGTGTCGGTCAGTGGTATG
-ACCATCACCGTGAACGGCGTTGCTGCAGGCAAGGTCAACATTCCGGTTGTATCCGGTAATGGTGAGTTTG
-CTGCGGTTGCAGAAATTACCGTCACCGCCAGTTAATCCGGAGAGTCAGCGATGTTCCTGAAAACCGAATC
-ATTTGAACATAACGGTGTGACCGTCACGCTTTCTGAACTGTCAGCCCTGCAGCGCATTGAGCATCTCGCC
-CTGATGAAACGGCAGGCAGAACAGGCGGAGTCAGACAGCAACCGGAAGTTTACTGTGGAAGACGCCATCA
-GAACCGGCGCGTTTCTGGTGGCGATGTCCCTGTGGCATAACCATCCGCAGAAGACGCAGATGCCGTCCAT
-GAATGAAGCCGTTAAACAGATTGAGCAGGAAGTGCTTACCACCTGGCCCACGGAGGCAATTTCTCATGCT
-GAAAACGTGGTGTACCGGCTGTCTGGTATGTATGAGTTTGTGGTGAATAATGCCCCTGAACAGACAGAGG
-ACGCCGGGCCCGCAGAGCCTGTTTCTGCGGGAAAGTGTTCGACGGTGAGCTGAGTTTTGCCCTGAAACTG
-GCGCGTGAGATGGGGCGACCCGACTGGCGTGCCATGCTTGCCGGGATGTCATCCACGGAGTATGCCGACT
-GGCACCGCTTTTACAGTACCCATTATTTTCATGATGTTCTGCTGGATATGCACTTTTCCGGGCTGACGTA
-CACCGTGCTCAGCCTGTTTTTCAGCGATCCGGATATGCATCCGCTGGATTTCAGTCTGCTGAACCGGCGC
-GAGGCTGACGAAGAGCCTGAAGATGATGTGCTGATGCAGAAAGCGGCAGGGCTTGCCGGAGGTGTCCGCT
-TTGGCCCGGACGGGAATGAAGTTATCCCCGCTTCCCCGGATGTGGCGGACATGACGGAGGATGACGTAAT
-GCTGATGACAGTATCAGAAGGGATCGCAGGAGGAGTCCGGTATGGCTGAACCGGTAGGCGATCTGGTCGT
-TGATTTGAGTCTGGATGCGGCCAGATTTGACGAGCAGATGGCCAGAGTCAGGCGTCATTTTTCTGGTACG
-GAAAGTGATGCGAAAAAAACAGCGGCAGTCGTTGAACAGTCGCTGAGCCGACAGGCGCTGGCTGCACAGA
-AAGCGGGGATTTCCGTCGGGCAGTATAAAGCCGCCATGCGTATGCTGCCTGCACAGTTCACCGACGTGGC
-CACGCAGCTTGCAGGCGGGCAAAGTCCGTGGCTGATCCTGCTGCAACAGGGGGGGCAGGTGAAGGACTCC
-TTCGGCGGGATGATCCCCATGTTCAGGGGGCTTGCCGGTGCGATCACCCTGCCGATGGTGGGGGCCACCT
-CGCTGGCGGTGGCGACCGGTGCGCTGGCGTATGCCTGGTATCAGGGCAACTCAACCCTGTCCGATTTCAA
-CAAAACGCTGGTCCTTTCCGGCAATCAGGCGGGACTGACGGCAGATCGTATGCTGGTCCTGTCCAGAGCC
-GGGCAGGCGGCAGGGCTGACGTTTAACCAGACCAGCGAGTCACTCAGCGCACTGGTTAAGGCGGGGGTAA
-GCGGTGAGGCTCAGATTGCGTCCATCAGCCAGAGTGTGGCGCGTTTCTCCTCTGCATCCGGCGTGGAGGT
-GGACAAGGTCGCTGAAGCCTTCGGGAAGCTGACCACAGACCCGACGTCGGGGCTGACGGCGATGGCTCGC
-CAGTTCCATAACGTGTCGGCGGAGCAGATTGCGTATGTTGCTCAGTTGCAGCGTTCCGGCGATGAAGCCG
-GGGCATTGCAGGCGGCGAACGAGGCCGCAACGAAAGGGTTTGATGACCAGACCCGCCGCCTGAAAGAGAA
-CATGGGCACGCTGGAGACCTGGGCAGACAGGACTGCGCGGGCATTCAAATCCATGTGGGATGCGGTGCTG
-GATATTGGTCGTCCTGATACCGCGCAGGAGATGCTGATTAAGGCAGAGGCTGCGTATAAGAAAGCAGACG
-ACATCTGGAATCTGCGCAAGGATGATTATTTTGTTAACGATGAAGCGCGGGCGCGTTACTGGGATGATCG
-TGAAAAGGCCCGTCTTGCGCTTGAAGCCGCCCGAAAGAAGGCTGAGCAGCAGACTCAACAGGACAAAAAT
-GCGCAGCAGCAGAGCGATACCGAAGCGTCACGGCTGAAATATACCGAAGAGGCGCAGAAGGCTTACGAAC
-GGCTGCAGACGCCGCTGGAGAAATATACCGCCCGTCAGGAAGAACTGAACAAGGCACTGAAAGACGGGAA
-AATCCTGCAGGCGGATTACAACACGCTGATGGCGGCGGCGAAAAAGGATTATGAAGCGACGCTGAAAAAG
-CCGAAACAGTCCAGCGTGAAGGTGTCTGCGGGCGATCGTCAGGAAGACAGTGCTCATGCTGCCCTGCTGA
-CGCTTCAGGCAGAACTCCGGACGCTGGAGAAGCATGCCGGAGCAAATGAGAAAATCAGCCAGCAGCGCCG
-GGATTTGTGGAAGGCGGAGAGTCAGTTCGCGGTACTGGAGGAGGCGGCGCAACGTCGCCAGCTGTCTGCA
-CAGGAGAAATCCCTGCTGGCGCATAAAGATGAGACGCTGGAGTACAAACGCCAGCTGGCTGCACTTGGCG
-ACAAGGTTACGTATCAGGAGCGCCTGAACGCGCTGGCGCAGCAGGCGGATAAATTCGCACAGCAGCAACG
-GGCAAAACGGGCCGCCATTGATGCGAAAAGCCGGGGGCTGACTGACCGGCAGGCAGAACGGGAAGCCACG
-GAACAGCGCCTGAAGGAACAGTATGGCGATAATCCGCTGGCGCTGAATAACGTCATGTCAGAGCAGAAAA
-AGACCTGGGCGGCTGAAGACCAGCTTCGCGGGAACTGGATGGCAGGCCTGAAGTCCGGCTGGAGTGAGTG
-GGAAGAGAGCGCCACGGACAGTATGTCGCAGGTAAAAAGTGCAGCCACGCAGACCTTTGATGGTATTGCA
-CAGAATATGGCGGCGATGCTGACCGGCAGTGAGCAGAACTGGCGCAGCTTCACCCGTTCCGTGCTGTCCA
-TGATGACAGAAATTCTGCTTAAGCAGGCAATGGTGGGGATTGTCGGGAGTATCGGCAGCGCCATTGGCGG
-GGCTGTTGGTGGCGGCGCATCCGCGTCAGGCGGTACAGCCATTCAGGCCGCTGCGGCGAAATTCCATTTT
-GCAACCGGAGGATTTACGGGAACCGGCGGCAAATATGAGCCAGCGGGGATTGTTCACCGTGGTGAGTTTG
-TCTTCACGAAGGAGGCAACCAGCCGGATTGGCGTGGGGAATCTTTACCGGCTGATGCGCGGCTATGCCAC
-CGGCGGTTATGTCGGTACACCGGGCAGCATGGCAGACAGCCGGTCGCAGGCGTCCGGGACGTTTGAGCAG
-AATAACCATGTGGTGATTAACAACGACGGCACGAACGGGCAGATAGGTCCGGCTGCTCTGAAGGCGGTGT
-ATGACATGGCCCGCAAGGGTGCCCGTGATGAAATTCAGACACAGATGCGTGATGGTGGCCTGTTCTCCGG
-AGGTGGACGATGAAGACCTTCCGCTGGAAAGTGAAACCCGGTATGGATGTGGCTTCGGTCCCTTCTGTAA
-GAAAGGTGCGCTTTGGTGATGGCTATTCTCAGCGAGCGCCTGCCGGGCTGAATGCCAACCTGAAAACGTA
-CAGCGTGACGCTTTCTGTCCCCCGTGAGGAGGCCACGGTACTGGAGTCGTTTCTGGAAGAGCACGGGGGC
-TGGAAATCCTTTCTGTGGACGCCGCCTTATGAGTGGCGGCAGATAAAGGTGACCTGCGCAAAATGGTCGT
-CGCGGGTCAGTATGCTGCGTGTTGAGTTCAGCGCAGAGTTTGAACAGGTGGTGAACTGATGCAGGATATC
-CGGCAGGAAACACTGAATGAATGCACCCGTGCGGAGCAGTCGGCCAGCGTGGTGCTCTGGGAAATCGACC
-TGACAGAGGTCGGTGGAGAACGTTATTTTTTCTGTAATGAGCAGAACGAAAAAGGTGAGCCGGTCACCTG
-GCAGGGGCGACAGTATCAGCCGTATCCCATTCAGGGGAGCGGTTTTGAACTGAATGGCAAAGGCACCAGT
-ACGCGCCCCACGCTGACGGTTTCTAACCTGTACGGTATGGTCACCGGGATGGCGGAAGATATGCAGAGTC
-TGGTCGGCGGAACGGTGGTCCGGCGTAAGGTTTACGCCCGTTTTCTGGATGCGGTGAACTTCGTCAACGG
-AAACAGTTACGCCGATCCGGAGCAGGAGGTGATCAGCCGCTGGCGCATTGAGCAGTGCAGCGAACTGAGC
-GCGGTGAGTGCCTCCTTTGTACTGTCCACGCCGACGGAAACGGATGGCGCTGTTTTTCCGGGACGTATCA
-TGCTGGCCAACACCTGCACCTGGACCTATCGCGGTGACGAGTGCGGTTATAGCGGTCCGGCTGTCGCGGA
-TGAATATGACCAGCCAACGTCCGATATCACGAAGGATAAATGCAGCAAATGCCTGAGCGGTTGTAAGTTC
-CGCAATAACGTCGGCAACTTTGGCGGCTTCCTTTCCATTAACAAACTTTCGCAGTAAATCCCATGACACA
-GACAGAATCAGCGATTCTGGCGCACGCCCGGCGATGTGCGCCAGCGGAGTCGTGCGGCTTCGTGGTAAGC
-ACGCCGGAGGGGGAAAGATATTTCCCCTGCGTGAATATCTCCGGTGAGCCGGAGGCTATTTCCGTATGTC
-GCCGGAAGACTGGCTGCAGGCAGAAATGCAGGGTGAGATTGTGGCGCTGGTCCACAGCCACCCCGGTGGT
-CTGCCCTGGCTGAGTGAGGCCGACCGGCGGCTGCAGGTGCAGAGTGATTTGCCGTGGTGGCTGGTCTGCC
-GGGGGACGATTCATAAGTTCCGCTGTGTGCCGCATCTCACCGGGCGGCGCTTTGAGCACGGTGTGACGGA
-CTGTTACACACTGTTCCGGGATGCTTATCATCTGGCGGGGATTGAGATGCCGGACTTTCATCGTGAGGAT
-GACTGGTGGCGTAACGGCCAGAATCTCTATCTGGATAATCTGGAGGCGACGGGGCTGTATCAGGTGCCGT
-TGTCAGCGGCACAGCCGGGCGATGTGCTGCTGTGCTGTTTTGGTTCATCAGTGCCGAATCACGCCGCAAT
-TTACTGCGGCGACGGCGAGCTGCTGCACCATATTCCTGAACAACTGAGCAAACGAGAGAGGTACACCGAC
-AAATGGCAGCGACGCACACACTCCCTCTGGCGTCACCGGGCATGGCGCGCATCTGCCTTTACGGGGATTT
-ACAACGATTTGGTCGCCGCATCGACCTTCGTGTGAAAACGGGGGCTGAAGCCATCCGGGCACTGGCCACA
-CAGCTCCCGGCGTTTCGTCAGAAACTGAGCGACGGCTGGTATCAGGTACGGATTGCCGGGCGGGACGTCA
-GCACGTCCGGGTTAACGGCGCAGTTACATGAGACTCTGCCTGATGGCGCTGTAATTCATATTGTTCCCAG
-AGTCGCCGGGGCCAAGTCAGGTGGCGTATTCCAGATTGTCCTGGGGGCTGCCGCCATTGCCGGATCATTC
-TTTACCGCCGGAGCCACCCTTGCAGCATGGGGGGCAGCCATTGGGGCCGGTGGTATGACCGGCATCCTGT
-TTTCTCTCGGTGCCAGTATGGTGCTCGGTGGTGTGGCGCAGATGCTGGCACCGAAAGCCAGAACTCCCCG
-TATACAGACAACGGATAACGGTAAGCAGAACACCTATTTCTCCTCACTGGATAACATGGTTGCCCAGGGC
-AATGTTCTGCCTGTTCTGTACGGGGAAATGCGCGTGGGGTCACGCGTGGTTTCTCAGGAGATCAGCACGG
-CAGACGAAGGGGACGGTGGTCAGGTTGTGGTGATTGGTCGCTGATGCAAAATGTTTTATGTGAAACCGCC
-TGCGGGCGGTTTTGTCATTTATGGAGCGTGAGGAATGGGTAAAGGAAGCAGTAAGGGGCATACCCCGCGC
-GAAGCGAAGGACAACCTGAAGTCCACGCAGTTGCTGAGTGTGATCGATGCCATCAGCGAAGGGCCGATTG
-AAGGTCCGGTGGATGGCTTAAAAAGCGTGCTGCTGAACAGTACGCCGGTGCTGGACACTGAGGGGAATAC
-CAACATATCCGGTGTCACGGTGGTGTTCCGGGCTGGTGAGCAGGAGCAGACTCCGCCGGAGGGATTTGAA
-TCCTCCGGCTCCGAGACGGTGCTGGGTACGGAAGTGAAATATGACACGCCGATCACCCGCACCATTACGT
-CTGCAAACATCGACCGTCTGCGCTTTACCTTCGGTGTACAGGCACTGGTGGAAACCACCTCAAAGGGTGA
-CAGGAATCCGTCGGAAGTCCGCCTGCTGGTTCAGATACAACGTAACGGTGGCTGGGTGACGGAAAAAGAC
-ATCACCATTAAGGGCAAAACCACCTCGCAGTATCTGGCCTCGGTGGTGATGGGTAACCTGCCGCCGCGCC
-CGTTTAATATCCGGATGCGCAGGATGACGCCGGACAGCACCACAGACCAGCTGCAGAACAAAACGCTCTG
-GTCGTCATACACTGAAATCATCGATGTGAAACAGTGCTACCCGAACACGGCACTGGTCGGCGTGCAGGTG
-GACTCGGAGCAGTTCGGCAGCCAGCAGGTGAGCCGTAATTATCATCTGCGCGGGCGTATTCTGCAGGTGC
-CGTCGAACTATAACCCGCAGACGCGGCAATACAGCGGTATCTGGGACGGAACGTTTAAACCGGCATACAG
-CAACAACATGGCCTGGTGTCTGTGGGATATGCTGACCCATCCGCGCTACGGCATGGGGAAACGTCTTGGT
-GCGGCGGATGTGGATAAATGGGCGCTGTATGTCATCGGCCAGTACTGCGACCAGTCAGTGCCGGACGGCT
-TTGGCGGCACGGAGCCGCGCATCACCTGTAATGCGTACCTGACCACACAGCGTAAGGCGTGGGATGTGCT
-CAGCGATTTCTGCTCGGCGATGCGCTGTATGCCGGTATGGAACGGGCAGACGCTGACGTTCGTGCAGGAC
-CGACCGTCGGATAAGACGTGGACCTATAACCGCAGTAATGTGGTGATGCCGGATGATGGCGCGCCGTTCC
-GCTACAGCTTCAGCGCCCTGAAGGACCGCCATAATGCCGTTGAGGTGAACTGGATTGACCCGAACAACGG
-CTGGGAGACGGCGACAGAGCTTGTTGAAGATACGCAGGCCATTGCCCGTTACGGTCGTAATGTTACGAAG
-ATGGATGCCTTTGGCTGTACCAGCCGGGGGCAGGCACACCGCGCCGGGCTGTGGCTGATTAAAACAGAAC
-TGCTGGAAACGCAGACCGTGGATTTCAGCGTCGGCGCAGAAGGGCTTCGCCATGTACCGGGCGATGTTAT
-TGAAATCTGCGATGATGACTATGCCGGTATCAGCACCGGTGGTCGTGTGCTGGCGGTGAACAGCCAGACC
-CGGACGCTGACGCTCGACCGTGAAATCACGCTGCCATCCTCCGGTACCGCGCTGATAAGCCTGGTTGACG
-GAAGTGGCAATCCGGTCAGCGTGGAGGTTCAGTCCGTCACCGACGGCGTGAAGGTAAAAGTGAGCCGTGT
-TCCTGACGGTGTTGCTGAATACAGCGTATGGGAGCTGAAGCTGCCGACGCTGCGCCAGCGACTGTTCCGC
-TGCGTGAGTATCCGTGAGAACGACGACGGCACGTATGCCATCACCGCCGTGCAGCATGTGCCGGAAAAAG
-AGGCCATCGTGGATAACGGGGCGCACTTTGACGGCGAACAGAGTGGCACGGTGAATGGTGTCACGCCGCC
-AGCGGTGCAGCACCTGACCGCAGAAGTCACTGCAGACAGCGGGGAATATCAGGTGCTGGCGCGATGGGAC
-ACACCGAAGGTGGTGAAGGGCGTGAGTTTCCTGCTCCGTCTGACCGTAACAGCGGACGACGGCAGTGAGC
-GGCTGGTCAGCACGGCCCGGACGACGGAAACCACATACCGCTTCACGCAACTGGCGCTGGGGAACTACAG
-GCTGACAGTCCGGGCGGTAAATGCGTGGGGGCAGCAGGGCGATCCGGCGTCGGTATCGTTCCGGATTGCC
-GCACCGGCAGCACCGTCGAGGATTGAGCTGACGCCGGGCTATTTTCAGATAACCGCCACGCCGCATCTTG
-CCGTTTATGACCCGACGGTACAGTTTGAGTTCTGGTTCTCGGAAAAGCAGATTGCGGATATCAGACAGGT
-TGAAACCAGCACGCGTTATCTTGGTACGGCGCTGTACTGGATAGCCGCCAGTATCAATATCAAACCGGGC
-CATGATTATTACTTTTATATCCGCAGTGTGAACACCGTTGGCAAATCGGCATTCGTGGAGGCCGTCGGTC
-GGGCGAGCGATGATGCGGAAGGTTACCTGGATTTTTTCAAAGGCAAGATAACCGAATCCCATCTCGGCAA
-GGAGCTGCTGGAAAAAGTCGAGCTGACGGAGGATAACGCCAGCAGACTGGAGGAGTTTTCGAAAGAGTGG
-AAGGATGCCAGTGATAAGTGGAATGCCATGTGGGCTGTCAAAATTGAGCAGACCAAAGACGGCAAACATT
-ATGTCGCGGGTATTGGCCTCAGCATGGAGGACACGGAGGAAGGCAAACTGAGCCAGTTTCTGGTTGCCGC
-CAATCGTATCGCATTTATTGACCCGGCAAACGGGAATGAAACGCCGATGTTTGTGGCGCAGGGCAACCAG
-ATATTCATGAACGACGTGTTCCTGAAGCGCCTGACGGCCCCCACCATTACCAGCGGCGGCAATCCTCCGG
-CCTTTTCCCTGACACCGGACGGAAAGCTGACCGCTAAAAATGCGGATATCAGTGGCAGTGTGAATGCGAA
-CTCCGGGACGCTCAGTAATGTGACGATAGCTGAAAACTGTACGATAAACGGTACGCTGAGGGCGGAAAAA
-ATCGTCGGGGACATTGTAAAGGCGGCGAGCGCGGCTTTTCCGCGCCAGCGTGAAAGCAGTGTGGACTGGC
-CGTCAGGTACCCGTACTGTCACCGTGACCGATGACCATCCTTTTGATCGCCAGATAGTGGTGCTTCCGCT
-GACGTTTCGCGGAAGTAAGCGTACTGTCAGCGGCAGGACAACGTATTCGATGTGTTATCTGAAAGTACTG
-ATGAACGGTGCGGTGATTTATGATGGCGCGGCGAACGAGGCGGTACAGGTGTTCTCCCGTATTGTTGACA
-TGCCAGCGGGTCGGGGAAACGTGATCCTGACGTTCACGCTTACGTCCACACGGCATTCGGCAGATATTCC
-GCCGTATACGTTTGCCAGCGATGTGCAGGTTATGGTGATTAAGAAACAGGCGCTGGGCATCAGCGTGGTC
-TGAGTGTGTTACAGAGGTTCGTCCGGGAACGGGCGTTTTATTATAAAACAGTGAGAGGTGAACGATGCGT
-AATGTGTGTATTGCCGTTGCTGTCTTTGCCGCACTTGCGGTGACAGTCACTCCGGCCCGTGCGGAAGGTG
-GACATGGTACGTTTACGGTGGGCTATTTTCAAGTGAAACCGGGTACATTGCCGTCGTTGTCGGGCGGGGA
-TACCGGTGTGAGTCATCTGAAAGGGATTAACGTGAAGTACCGTTATGAGCTGACGGACAGTGTGGGGGTG
-ATGGCTTCCCTGGGGTTCGCCGCGTCGAAAAAGAGCAGCACAGTGATGACCGGGGAGGATACGTTTCACT
-ATGAGAGCCTGCGTGGACGTTATGTGAGCGTGATGGCCGGACCGGTTTTACAAATCAGTAAGCAGGTCAG
-TGCGTACGCCATGGCCGGAGTGGCTCACAGTCGGTGGTCCGGCAGTACAATGGATTACCGTAAGACGGAA
-ATCACTCCCGGGTATATGAAAGAGACGACCACTGCCAGGGACGAAAGTGCAATGCGGCATACCTCAGTGG
-CGTGGAGTGCAGGTATACAGATTAATCCGGCAGCGTCCGTCGTTGTTGATATTGCTTATGAAGGCTCCGG
-CAGTGGCGACTGGCGTACTGACGGATTCATCGTTGGGGTCGGTTATAAATTCTGATTAGCCAGGTAACAC
-AGTGTTATGACAGCCCGCCGGAACCGGTGGGCTTTTTTGTGGGGTGAATATGGCAGTAAAGATTTCAGGA
-GTCCTGAAAGACGGCACAGGAAAACCGGTACAGAACTGCACCATTCAGCTGAAAGCCAGACGTAACAGCA
-CCACGGTGGTGGTGAACACGGTGGGCTCAGAGAATCCGGATGAAGCCGGGCGTTACAGCATGGATGTGGA
-GTACGGTCAGTACAGTGTCATCCTGCAGGTTGACGGTTTTCCACCATCGCACGCCGGGACCATCACCGTG
-TATGAAGATTCACAACCGGGGACGCTGAATGATTTTCTCTGTGCCATGACGGAGGATGATGCCCGGCCGG
-AGGTGCTGCGTCGTCTTGAACTGATGGTGGAAGAGGTGGCGCGTAACGCGTCCGTGGTGGCACAGAGTAC
-GGCAGACGCGAAGAAATCAGCCGGCGATGCCAGTGCATCAGCTGCTCAGGTCGCGGCCCTTGTGACTGAT
-GCAACTGACTCAGCACGCGCCGCCAGCACGTCCGCCGGACAGGCTGCATCGTCAGCTCAGGAAGCGTCCT
-CCGGCGCAGAAGCGGCATCAGCAAAGGCCACTGAAGCGGAAAAAAGTGCCGCAGCCGCAGAGTCCTCAAA
-AAACGCGGCGGCCACCAGTGCCGGTGCGGCGAAAACGTCAGAAACGAATGCTGCAGCGTCACAACAATCA
-GCCGCCACGTCTGCCTCCACCGCGGCCACGAAAGCGTCAGAGGCCGCCACTTCAGCACGAGATGCGGTGG
-CCTCAAAAGAGGCAGCAAAATCATCAGAAACGAACGCATCATCAAGTGCCGGTCGTGCAGCTTCCTCGGC
-AACGGCGGCAGAAAATTCTGCCAGGGCGGCAAAAACGTCCGAGACGAATGCCAGGTCATCTGAAACAGCA
-GCGGAACGGAGCGCCTCTGCCGCGGCAGACGCAAAAACAGCGGCGGCGGGGAGTGCGTCAACGGCATCCA
-CGAAGGCGACAGAGGCTGCGGGAAGTGCGGTATCAGCATCGCAGAGCAAAAGTGCGGCAGAAGCGGCGGC
-AATACGTGCAAAAAATTCGGCAAAACGTGCAGAAGATATAGCTTCAGCTGTCGCGCTTGAGGATGCGGAC
-ACAACGAGAAAGGGGATAGTGCAGCTCAGCAGTGCAACCAACAGCACGTCTGAAACGCTTGCTGCAACGC
-CAAAGGCGGTTAAGGTGGTAATGGATGAAACGAACAGAAAAGCCCACTGGACAGTCCGGCACTGACCGGA
-ACGCCAACAGCACCAACCGCGCTCAGGGGAACAAACAATACCCAGATTGCGAACACCGCTTTTGTACTGG
-CCGCGATTGCAGATGTTATCGACGCGTCACCTGACGCACTGAATACGCTGAATGAACTGGCCGCAGCGCT
-CGGGAATGATCCAGATTTTGCTACCACCATGACTAACGCGCTTGCGGGTAAACAACCGAAGAATGCGACA
-CTGACGGCGCTGGCAGGGCTTTCCACGGCGAAAAATAAATTACCGTATTTTGCGGAAAATGATGCCGCCA
-GCCTGACTGAACTGACTCAGGTTGGCAGGGATATTCTGGCAAAAAATTCCGTTGCAGATGTTCTTGAATA
-CCTTGGGGCCGGTGAGAATTCGGCCTTTCCGGCAGGTGCGCCGATCCCGTGGCCATCAGATATCGTTCCG
-TCTGGCTACGTCCTGATGCAGGGGCAGGCGTTTGACAAATCAGCCTACCCAAAACTTGCTGTCGCGTATC
-CATCGGGTGTGCTTCCTGATATGCGAGGCTGGACAATCAAGGGGAAACCCGCCAGCGGTCGTGCTGTATT
-GTCTCAGGAACAGGATGGAATTAAGTCGCACACCCACAGTGCCAGTGCATCCGGTACGGATTTGGGGACG
-AAAACCACATCGTCGTTTGATTACGGGACGAAAACAACAGGCAGTTTCGATTACGGCACCAAATCGACGA
-ATAACACGGGGGCTCATGCTCACAGTCTGAGCGGTTCAACAGGGGCCGCGGGTGCTCATGCCCACACAAG
-TGGTTTAAGGATGAACAGTTCTGGCTGGAGTCAGTATGGAACAGCAACCATTACAGGAAGTTTATCCACA
-GTTAAAGGAACCAGCACACAGGGTATTGCTTATTTATCGAAAACGGACAGTCAGGGCAGCCACAGTCACT
-CATTGTCCGGTACAGCCGTGAGTGCCGGTGCACATGCGCATACAGTTGGTATTGGTGCGCACCAGCATCC
-GGTTGTTATCGGTGCTCATGCCCATTCTTTCAGTATTGGTTCACACGGACACACCATCACCGTTAACGCT
-GCGGGTAACGCGGAAAACACCGTCAAAAACATTGCATTTAACTATATTGTGAGGCTTGCATAATGGCATT
-CAGAATGAGTGAACAACCACGGACCATAAAAATTTATAATCTGCTGGCCGGAACTAATGAATTTATTGGT
-GAAGGTGACGCATATATTCCGCCTCATACCGGTCTGCCTGCAAACAGTACCGATATTGCACCGCCAGATA
-TTCCGGCTGGCTTTGTGGCTGTTTTCAACAGTGATGAGGCATCGTGGCATCTCGTTGAAGACCATCGGGG
-TAAAACCGTCTATGACGTGGCTTCCGGCGACGCGTTATTTATTTCTGAACTCGGTCCGTTACCGGAAAAT
-TTTACCTGGTTATCGCCGGGAGGGGAATATCAGAAGTGGAACGGCACAGCCTGGGTGAAGGATACGGAAG
-CAGAAAAACTGTTCCGGATCCGGGAGGCGGAAGAAACAAAAAAAAGCCTGATGCAGGTAGCCAGTGAGCA
-TATTGCGCCGCTTCAGGATGCTGCAGATCTGGAAATTGCAACGAAGGAAGAAACCTCGTTGCTGGAAGCC
-TGGAAGAAGTATCGGGTGTTGCTGAACCGTGTTGATACATCAACTGCACCTGATATTGAGTGGCCTGCTG
-TCCCTGTTATGGAGTAATCGTTTTGTGATATGCCGCAGAAACGTTGTATGAAATAACGTTCTGCGGTTAG
-TTAGTATATTGTAAAGCTGAGTATTGGTTTATTTGGCGATTATTATCTTCAGGAGAATAATGGAAGTTCT
-ATGACTCAATTGTTCATAGTGTTTACATCACCGCCAATTGCTTTTAAGACTGAACGCATGAAATATGGTT
-TTTCGTCATGTTTTGAGTCTGCTGTTGATATTTCTAAAGTCGGTTTTTTTTCTTCGTTTTCTCTAACTAT
-TTTCCATGAAATACATTTTTGATTATTATTTGAATCAATTCCAATTACCTGAAGTCTTTCATCTATAATT
-GGCATTGTATGTATTGGTTTATTGGAGTAGATGCTTGCTTTTCTGAGCCATAGCTCTGATATCCAAATGA
-AGCCATAGGCATTTGTTATTTTGGCTCTGTCAGCTGCATAACGCCAAAAAATATATTTATCTGCTTGATC
-TTCAAATGTTGTATTGATTAAATCAATTGGATGGAATTGTTTATCATAAAAAATTAATGTTTGAATGTGA
-TAACCGTCCTTTAAAAAAGTCGTTTCTGCAAGCTTGGCTGTATAGTCAACTAACTCTTCTGTCGAAGTGA
-TATTTTTAGGCTTATCTACCAGTTTTAGACGCTCTTTAATATCTTCAGGAATTATTTTATTGTCATATTG
-TATCATGCTAAATGACAATTTGCTTATGGAGTAATCTTTTAATTTTAAATAAGTTATTCTCCTGGCTTCA
-TCAAATAAAGAGTCGAATGATGTTGGCGAAATCACATCGTCACCCATTGGATTGTTTATTTGTATGCCAA
-GAGAGTTACAGCAGTTATACATTCTGCCATAGATTATAGCTAAGGCATGTAATAATTCGTAATCTTTTAG
-CGTATTAGCGACCCATCGTCTTTCTGATTTAATAATAGATGATTCAGTTAAATATGAAGGTAATTTCTTT
-TGTGCAAGTCTGACTAACTTTTTTATACCAATGTTTAACATACTTTCATTTGTAATAAACTCAATGTCAT
-TTTCTTCAATGTAAGATGAAATAAGAGTAGCCTTTGCCTCGCTATACATTTCTAAATCGCCTTGTTTTTC
-TATCGTATTGCGAGAATTTTTAGCCCAAGCCATTAATGGATCATTTTTCCATTTTTCAATAACATTATTG
-TTATACCAAATGTCATATCCTATAATCTGGTTTTTGTTTTTTTGAATAATAAATGTTACTGTTCTTGCGG
-TTTGGAGGAATTGATTCAAATTCAAGCGAAATAATTCAGGGTCAAAATATGTATCAATGCAGCATTTGAG
-CAAGTGCGATAAATCTTTAAGTCTTCTTTCCCATGGTTTTTTAGTCATAAAACTCTCCATTTTGATAGGT
-TGCATGCTAGATGCTGATATATTTTAGAGGTGATAAAATTAACTGCTTAACTGTCAATGTAATACAAGTT
-GTTTGATCTTTGCAATGATTCTTATCAGAAACCATATAGTAAATTAGTTACACAGGAAATTTTTAATATT
-ATTATTATCATTCATTATGTATTAAAATTAGAGTTGTGGCTTGGCTCTGCTAACACGTTGCTCATAGGAG
-ATATGGTAGAGCCGCAGACACGTCGTATGCAGGAACGTGCTGCGGCTGGCTGGTGAACTTCCGATAGTGC
-GGGTGTTGAATGATTTCCAGTTGCTACCGATTTTACATATTTTTTGCATGAGAGAATTTGTACCACCTCC
-CACCGACCATCTATGACTGTACGCCACTGTCCCTAGGACTGCTATGTGCCGGAGCGGACATTACAAACGT
-CCTTCTCGGTGCATGCCACTGTTGCCAATGACCTGCCTAGGAATTGGTTAGCAAGTTACTACCGGATTTT
-GTAAAAACAGCCCTCCTCATATAAAAAGTATTCGTTCACTTCCGATAAGCGTCGTAATTTTCTATCTTTC
-ATCATATTCTAGATCCCTCTGAAAAAATCTTCCGAGTTTGCTAGGCACTGATACATAACTCTTTTCCAAT
-AATTGGGGAAGTCATTCAAATCTATAATAGGTTTCAGATTTGCTTCAATAAATTCTGACTGTAGCTGCTG
-AAACGTTGCGGTTGAACTATATTTCCTTATAACTTTTACGAAAGAGTTTCTTTGAGTAATCACTTCACTC
-AAGTGCTTCCCTGCCTCCAAACGATACCTGTTAGCAATATTTAATAGCTTGAAATGATGAAGAGCTCTGT
-GTTTGTCTTCCTGCCTCCAGTTCGCCGGGCATTCAACATAAAAACTGATAGCACCCGGAGTTCCGGAAAC
-GAAATTTGCATATACCCATTGCTCACGAAAAAAAATGTCCTTGTCGATATAGGGATGAATCGCTTGGTGT
-ACCTCATCTACTGCGAAAACTTGACCTTTCTCTCCCATATTGCAGTCGCGGCACGATGGAACTAAATTAA
-TAGGCATCACCGAAAATTCAGGATAATGTGCAATAGGAAGAAAATGATCTATATTTTTTGTCTGTCCTAT
-ATCACCACAAAATGGACATTTTTCACCTGATGAAACAAGCATGTCATCGTAATATGTTCTAGCGGGTTTG
-TTTTTATCTCGGAGATTATTTTCATAAAGCTTTTCTAATTTAACCTTTGTCAGGTTACCAACTACTAAGG
-TTGTAGGCTCAAGAGGGTGTGTCCTGTCGTAGGTAAATAACTGACCTGTCGAGCTTAATATTCTATATTG
-TTGTTCTTTCTGCAAAAAAGTGGGGAAGTGAGTAATGAAATTATTTCTAACATTTATCTGCATCATACCT
-TCCGAGCATTTATTAAGCATTTCGCTATAAGTTCTCGCTGGAAGAGGTAGTTTTTTCATTGTACTTTACC
-TTCATCTCTGTTCATTATCATCGCTTTTAAAACGGTTCGACCTTCTAATCCTATCTGACCATTATAATTT
-TTTAGAATGGTTTCATAAGAAAGCTCTGAATCAACGGACTGCGATAATAAGTGGTGGTATCCAGAATTTG
-TCACTTCAAGTAAAAACACCTCACGAGTTAAAACACCTAAGTTCTCACCGAATGTCTCAATATCCGGACG
-GATAATATTTATTGCTTCTCTTGACCGTAGGACTTTCCACATGCAGGATTTTGGAACCTCTTGCAGTACT
-ACTGGGGAATGAGTTGCAATTATTGCTACACCATTGCGTGCATCGAGTAAGTCGCTTAATGTTCGTAAAA
-AAGCAGAGAGCAAAGGTGGATGCAGATGAACCTCTGGTTCATCGAATAAAACTAATGACTTTTCGCCAAC
-GACATCTACTAATCTTGTGATAGTAAATAAAACAATTGCATGTCCAGAGCTCATTCGAAGCAGATATTTC
-TGGATATTGTCATAAAACAATTTAGTGAATTTATCATCGTCCACTTGAATCTGTGGTTCATTACGTCTTA
-ACTCTTCATATTTAGAAATGAGGCTGATGAGTTCCATATTTGAAAAGTTTTCATCACTACTTAGTTTTTT
-GATAGCTTCAAGCCAGAGTTGTCTTTTTCTATCTACTCTCATACAACCAATAAATGCTGAAATGAATTCT
-AAGCGGAGATCGCCTAGTGATTTTAAACTATTGCTGGCAGCATTCTTGAGTCCAATATAAAAGTATTGTG
-TACCTTTTGCTGGGTCAGGTTGTTCTTTAGGAGGAGTAAAAGGATCAAATGCACTAAACGAAACTGAAAC
-AAGCGATCGAAAATATCCCTTTGGGATTCTTGACTCGATAAGTCTATTATTTTCAGAGAAAAAATATTCA
-TTGTTTTCTGGGTTGGTGATTGCACCAATCATTCCATTCAAAATTGTTGTTTTACCACACCCATTCCGCC
-CGATAAAAGCATGAATGTTCGTGCTGGGCATAGAATTAACCGTCACCTCAAAAGGTATAGTTAAATCACT
-GAATCCGGGAGCACTTTTTCTATTAAATGAAAAGTGGAAATCTGACAATTCTGGCAAACCATTTAACACA
-CGTGCGAACTGTCCATGAATTTCTGAAAGAGTTACCCCTCTAAGTAATGAGGTGTTAAGGACGCTTTCAT
-TTTCAATGTCGGCTAATCGATTTGGCCATACTACTAAATCCTGAATAGCTTTAAGAAGGTTATGTTTAAA
-ACCATCGCTTAATTTGCTGAGATTAACATAGTAGTCAATGCTTTCACCTAAGGAAAAAAACATTTCAGGG
-AGTTGACTGAATTTTTTATCTATTAATGAATAAGTGCTTACTTCTTCTTTTTGACCTACAAAACCAATTT
-TAACATTTCCGATATCGCATTTTTCACCATGCTCATCAAAGACAGTAAGATAAAACATTGTAACAAAGGA
-ATAGTCATTCCAACCATCTGCTCGTAGGAATGCCTTATTTTTTTCTACTGCAGGAATATACCCGCCTCTT
-TCAATAACACTAAACTCCAACATATAGTAACCCTTAATTTTATTAAAATAACCGCAATTTATTTGGCGGC
-AACACAGGATCTCTCTTTTAAGTTACTCTCTATTACATACGTTTTCCATCTAAAAATTAGTAGTATTGAA
-CTTAACGGGGCATCGTATTGTAGTTTTCCATATTTAGCTTTCTGCTTCCTTTTGGATAACCCACTGTTAT
-TCATGTTGCATGGTGCACTGTTTATACCAACGATATAGTCTATTAATGCATATATAGTATCGCCGAACGA
-TTAGCTCTTCAGGCTTCTGAAGAAGCGTTTCAAGTACTAATAAGCCGATAGATAGCCACGGACTTCGTAG
-CCATTTTTCATAAGTGTTAACTTCCGCTCCTCGCTCATAACAGACATTCACTACAGTTATGGCGGAAAGG
-TATGCATGCTGGGTGTGGGGAAGTCGTGAAAGAAAAGAAGTCAGCTGCGTCGTTTGACATCACTGCTATC
-TTCTTACTGGTTATGCAGGTCGTAGTGGGTGGCACACAAAGCTTTGCACTGGATTGCGAGGCTTTGTGCT
-TCTCTGGAGTGCGACAGGTTTGATGACAAAAAATTAGCGCAAGAAGACAAAAATCACCTTGCGCTAATGC
-TCTGTTACAGGTCACTAATACCATCTAAGTAGTTGATTCATAGTGACTGCATATGTTGTGTTTTACAGTA
-TTATGTAGTCTGTTTTTTATGCAAAATCTAATTTAATATATTGATATTTATATCATTTTACGTTTCTCGT
-TCAGCTTTTTTATACTAAGTTGGCATTATAAAAAAGCATTGCTTATCAATTTGTTGCAACGAACAGGTCA
-CTATCAGTCAAAATAAAATCATTATTTGATTTCAATTTTGTCCCACTCCCTGCCTCTGTCATCACGATAC
-TGTGATGCCATGGTGTCCGACTTATGCCCGAGAAGATGTTGAGCAAACTTATCGCTTATCTGCTTCTCAT
-AGAGTCTTGCAGACAAACTGCGCAACTCGTGAAAGGTAGGCGGATCCCCTTCGAAGGAAAGACCTGATGC
-TTTTCGTGCGCGCATAAAATACCTTGATACTGTGCCGGATGAAAGCGGTTCGCGACGAGTAGATGCAATT
-ATGGTTTCTCCGCCAAGAATCTCTTTGCATTTATCAAGTGTTTCCTTCATTGATATTCCGAGAGCATCAA
-TATGCAATGCTGTTGGGATGGCAATTTTTACGCCTGTTTTGCTTTGCTCGACATAAAGATATCCATCTAC
-GATATCAGACCACTTCATTTCGCATAAATCACCAACTCGTTGCCCGGTAACAACAGCCAGTTCCATTGCA
-AGTCTGAGCCAACATGGTGATGATTCTGCTGCTTGATAAATTTTCAGGTATTCGTCAGCCGTAAGTCTTG
-ATCTCCTTACCTCTGATTTTGCTGCGCGAGTGGCAGCGACATGGTTTGTTGTTATATGGCCTTCAGCTAT
-TGCCTCTCGGAATGCATCGCTCAGTGTTGATCTGATTAACTTGGCTGACGCCGCCTTGCCCTCGTCTATG
-TATCCATTGAGCATTGCCGCAATTTCTTTTGTGGTGATGTCTTCAAGTGGAGCATCAGGCAGACCCCTCC
-TTATTGCTTTAATTTTGCTCATGTAATTTATGAGTGTCTTCTGCTTGATTCCTCTGCTGGCCAGGATTTT
-TTCGTAGCGATCAAGCCATGAATGTAACGTAACGGAATTATCACTGTTGATTCTCGCTGTCAGAGGCTTG
-TGTTTGTGTCCTGAAAATAACTCAATGTTGGCCTGTATAGCTTCAGTGATTGCGATTCGCCTGTCTCTGC
-CTAATCCAAACTCTTTACCCGTCCTTGGGTCCCTGTAGCAGTAATATCCATTGTTTCTTATATAAAGGTT
-AGGGGGTAAATCCCGGCGCTCATGACTTCGCCTTCTTCCCATTTCTGATCCTCTTCAAAAGGCCACCTGT
-TACTGGTCGATTTAAGTCAACCTTTACCGCTGATTCGTGGAACAGATACTCTCTTCCATCCTTAACCGGA
-GGTGGGAATATCCTGCATTCCCGAACCCATCGACGAACTGTTTCAAGGCTTCTTGGACGTCGCTGGCGTG
-CGTTCCACTCCTGAAGTGTCAAGTACATCGCAAAGTCTCCGCAATTACACGCAAGAAAAAACCGCCATCA
-GGCGGCTTGGTGTTCTTTCAGTTCTTCAATTCGAATATTGGTTACGTCTGCATGTGCTATCTGCGCCCAT
-ATCATCCAGTGGTCGTAGCAGTCGTTGATGTTCTCCGCTTCGATAACTCTGTTGAATGGCTCTCCATTCC
-ATTCTCCTGTGACTCGGAAGTGCATTTATCATCTCCATAAAACAAAACCCGCCGTAGCGAGTTCAGATAA
-AATAAATCCCCGCGAGTGCGAGGATTGTTATGTAATATTGGGTTTAATCATCTATATGTTTTGTACAGAG
-AGGGCAAGTATCGTTTCCACCGTACTCGTGATAATAATTTTGCACGGTATCAGTCATTTCTCGCACATTG
-CAGAATGGGGATTTGTCTTCATTAGACTTATAAACCTTCATGGAATATTTGTATGCCGACTCTATATCTA
-TACCTTCATCTACATAAACACCTTCGTGATGTCTGCATGGAGACAAGACACCGGATCTGCACAACATTGA
-TAACGCCCAATCTTTTTGCTCAGACTCTAACTCATTGATACTCATTTATAAACTCCTTGCAATGTATGTC
-GTTTCAGCTAAACGGTATCAGCAATGTTTATGTAAAGAAACAGTAAGATAATACTCAACCCGATGTTTGA
-GTACGGTCATCATCTGACACTACAGACTCTGGCATCGCTGTGAAGACGACGCGAAATTCAGCATTTTCAC
-AAGCGTTATCTTTTACAAAACCGATCTCACTCTCCTTTGATGCGAATGCCAGCGTCAGACATCATATGCA
-GATACTCACCTGCATCCTGAACCCATTGACCTCCAACCCCGTAATAGCGATGCGTAATGATGTCGATAGT
-TACTAACGGGTCTTGTTCGATTAACTGCCGCAGAAACTCTTCCAGGTCACCAGTGCAGTGCTTGATAACA
-GGAGTCTTCCCAGGATGGCGAACAACAAGAAACTGGTTTCCGTCTTCACGGACTTCGTTGCTTTCCAGTT
-TAGCAATACGCTTACTCCCATCCGAGATAACACCTTCGTAATACTCACGCTGCTCGTTGAGTTTTGATTT
-TGCTGTTTCAAGCTCAACACGCAGTTTCCCTACTGTTAGCGCAATATCCTCGTTCTCCTGGTCGCGGCGT
-TTGATGTATTGCTGGTTTCTTTCCCGTTCATCCAGCAGTTCCAGCACAATCGATGGTGTTACCAATTCAT
-GGAAAAGGTCTGCGTCAAATCCCCAGTCGTCATGCATTGCCTGCTCTGCCGCTTCACGCAGTGCCTGAGA
-GTTAATTTCGCTCACTTCGAACCTCTCTGTTTACTGATAAGTTCCAGATCCTCCTGGCAACTTGCACAAG
-TCCGACAACCCTGAACGACCAGGCGTCTTCGTTCATCTATCGGATCGCCACACTCACAACAATGAGTGGC
-AGATATAGCCTGGTGGTTCAGGCGGCGCATTTTTATTGCTGTGTTGCGCTGTAATTCTTCTATTTCTGAT
-GCTGAATCAATGATGTCTGCCATCTTTCATTAATCCCTGAACTGTTGGTTAATACGCTTGAGGGTGAATG
-CGAATAATAAAAAAGGAGCCTGTAGCTCCCTGATGATTTTGCTTTTCATGTTCATCGTTCCTTAAAGACG
-CCGTTTAACATGCCGATTGCCAGGCTTAAATGAGTCGGTGTGAATCCCATCAGCGTTACCGTTTCGCGGT
-GCTTCTTCAGTACGCTACGGCAAATGTCATCGACGTTTTTATCCGGAAACTGCTGTCTGGCTTTTTTTGA
-TTTCAGAATTAGCCTGACGGGCAATGCTGCGAAGGGCGTTTTCCTGCTGAGGTGTCATTGAACAAGTCCC
-ATGTCGGCAAGCATAAGCACACAGAATATGAAGCCCGCTGCCAGAAAAATGCATTCCGTGGTTGTCATAC
-CTGGTTTCTCTCATCTGCTTCTGCTTTCGCCACCATCATTTCCAGCTTTTGTGAAAGGGATGCGGCTAAC
-GTATGAAATTCTTCGTCTGTTTCTACTGGTATTGGCACAAACCTGATTCCAATTTGAGCAAGGCTATGTG
-CCATCTCGATACTCGTTCTTAACTCAACAGAAGATGCTTTGTGCATACAGCCCCTCGTTTATTATTTATC
-TCCTCAGCCAGCCGCTGTGCTTTCAGTGGATTTCGGATAACAGAAAGGCCGGGAAATACCCAGCCTCGCT
-TTGTAACGGAGTAGACGAAAGTGATTGCGCCTACCCGGATATTATCGTGAGGATGCGTCATCGCCATTGC
-TCCCCAAATACAAAACCAATTTCAGCCAGTGCCTCGTCCATTTTTTCGATGAACTCCGGCACGATCTCGT
-CAAAACTCGCCATGTACTTTTCATCCCGCTCAATCACGACATAATGCAGGCCTTCACGCTTCATACGCGG
-GTCATAGTTGGCAAAGTACCAGGCATTTTTTCGCGTCACCCACATGCTGTACTGCACCTGGGCCATGTAA
-GCTGACTTTATGGCCTCGAAACCACCGAGCCGGAACTTCATGAAATCCCGGGAGGTAAACGGGCATTTCA
-GTTCAAGGCCGTTGCCGTCACTGCATAAACCATCGGGAGAGCAGGCGGTACGCATACTTTCGTCGCGATA
-GATGATCGGGGATTCAGTAACATTCACGCCGGAAGTGAATTCAAACAGGGTTCTGGCGTCGTTCTCGTAC
-TGTTTTCCCCAGGCCAGTGCTTTAGCGTTAACTTCCGGAGCCACACCGGTGCAAACCTCAGCAAGCAGGG
-TGTGGAAGTAGGACATTTTCATGTCAGGCCACTTCTTTCCGGAGCGGGGTTTTGCTATCACGTTGTGAAC
-TTCTGAAGCGGTGATGACGCCGAGCCGTAATTTGTGCCACGCATCATCCCCCTGTTCGACAGCTCTCACA
-TCGATCCCGGTACGCTGCAGGATAATGTCCGGTGTCATGCTGCCACCTTCTGCTCTGCGGCTTTCTGTTT
-CAGGAATCCAAGAGCTTTTACTGCTTCGGCCTGTGTCAGTTCTGACGATGCACGAATGTCGCGGCGAAAT
-ATCTGGGAACAGAGCGGCAATAAGTCGTCATCCCATGTTTTATCCAGGGCGATCAGCAGAGTGTTAATCT
-CCTGCATGGTTTCATCGTTAACCGGAGTGATGTCGCGTTCCGGCTGACGTTCTGCAGTGTATGCAGTATT
-TTCGACAATGCGCTCGGCTTCATCCTTGTCATAGATACCAGCAAATCCGAAGGCCAGACGGGCACACTGA
-ATCATGGCTTTATGACGTAACATCCGTTTGGGATGCGACTGCCACGGCCCCGTGATTTCTCTGCCTTCGC
-GAGTTTTGAATGGTTCGCGGCGGCATTCATCCATCCATTCGGTAACGCAGATCGGATGATTACGGTCCTT
-GCGGTAAATCCGGCATGTACAGGATTCATTGTCCTGCTCAAAGTCCATGCCATCAAACTGCTGGTTTTCA
-TTGATGATGCGGGACCAGCCATCAACGCCCACCACCGGAACGATGCCATTCTGCTTATCAGGAAAGGCGT
-AAATTTCTTTCGTCCACGGATTAAGGCCGTACTGGTTGGCAACGATCAGTAATGCGATGAACTGCGCATC
-GCTGGCATCACCTTTAAATGCCGTCTGGCGAAGAGTGGTGATCAGTTCCTGTGGGTCGACAGAATCCATG
-CCGACACGTTCAGCCAGCTTCCCAGCCAGCGTTGCGAGTGCAGTACTCATTCGTTTTATACCTCTGAATC
-AATATCAACCTGGTGGTGAGCAATGGTTTCAACCATGTACCGGATGTGTTCTGCCATGCGCTCCTGAAAC
-TCAACATCGTCATCAAACGCACGGGTAATGGATTTTTTGCTGGCCCCGTGGCGTTGCAAATGATCGATGC
-ATAGCGATTCAAACAGGTGCTGGGGCAGGCCTTTTTCCATGTCGTCTGCCAGTTCTGCCTCTTTCTCTTC
-ACGGGCGAGCTGCTGGTAGTGACGCGCCCAGCTCTGAGCCTCAAGACGATCCTGAATGTAATAAGCGTTC
-ATGGCTGAACTCCTGAAATAGCTGTGAAAATATCGCCCGCGAAATGCCGGGCTGATTAGGAAAACAGGAA
-AGGGGGTTAGTGAATGCTTTTGCTTGATCTCAGTTTCAGTATTAATATCCATTTTTTATAAGCGTCGACG
-GCTTCACGAAACATCTTTTCATCGCCAATAAAAGTGGCGATAGTGAATTTAGTCTGGATAGCCATAAGTG
-TTTGATCCATTCTTTGGGACTCCTGGCTGATTAAGTATGTCGATAAGGCGTTTCCATCCGTCACGTAATT
-TACGGGTGATTCGTTCAAGTAAAGATTCGGAAGGGCAGCCAGCAACAGGCCACCCTGCAATGGCATATTG
-CATGGTGTGCTCCTTATTTATACATAACGAAAAACGCCTCGAGTGAAGCGTTATTGGTATGCGGTAAAAC
-CGCACTCAGGCGGCCTTGATAGTCATATCATCTGAATCAAATATTCCTGATGTATCGATATCGGTAATTC
-TTATTCCTTCGCTACCATCCATTGGAGGCCATCCTTCCTGACCATTTCCATCATTCCAGTCGAACTCACA
-CACAACACCATATGCATTTAAGTCGCTTGAAATTGCTATAAGCAGAGCATGTTGCGCCAGCATGATTAAT
-ACAGCATTTAATACAGAGCCGTGTTTATTGAGTCGGTATTCAGAGTCTGACCAGAAATTATTAATCTGGT
-GAAGTTTTTCCTCTGTCATTACGTCATGGTCGATTTCAATTTCTATTGATGCTTTCCAGTCGTAATCAAT
-GATGTATTTTTTGATGTTTGACATCTGTTCATATCCTCACAGATAAAAAATCGCCCTCACACTGGAGGGC
-AAAGAAGATTTCCAATAATCAGAACAAGTCGGCTCCTGTTTAGTTACGAGCGACATTGCTCCGTGTATTC
-ACTCGTTGGAATGAATACACAGTGCAGTGTTTATTCTGTTATTTATGCCAAAAATAAAGGCCACTATCAG
-GCAGCTTTGTTGTTCTGTTTACCAAGTTCTCTGGCAATCATTGCCGTCGTTCGTATTGCCCATTTATCGA
-CATATTTCCCATCTTCCATTACAGGAAACATTTCTTCAGGCTTAACCATGCATTCCGATTGCAGCTTGCA
-TCCATTGCATCGCTTGAATTGTCCACACCATTGATTTTTATCAATAGTCGTAGTCATACGGATAGTCCTG
-GTATTGTTCCATCACATCCTGAGGATGCTCTTCGAACTCTTCAAATTCTTCTTCCATATATCACCTTAAA
-TAGTGGATTGCGGTAGTAAAGATTGTGCCTGTCTTTTAACCACATCAGGCTCGGTGGTTCTCGTGTACCC
-CTACAGCGAGAAATCGGATAAACTATTACAACCCCTACAGTTTGATGAGTATAGAAATGGATCCACTCGT
-TATTCTCGGACGAGTGTTCAGTAATGAACCTCTGGAGAGAACCATGTATATGATCGTTATCTGGGTTGGA
-CTTCTGCTTTTAAGCCCAGATAACTGGCCTGAATATGTTAATGAGAGAATCGGTATTCCTCATGTGTGGC
-ATGTTTTCGTCTTTGCTCTTGCATTTTCGCTAGCAATTAATGTGCATCGATTATCAGCTATTGCCAGCGC
-CAGATATAAGCGATTTAAGCTAAGAAAACGCATTAAGATGCAAAACGATAAAGTGCGATCAGTAATTCAA
-AACCTTACAGAAGAGCAATCTATGGTTTTGTGCGCAGCCCTTAATGAAGGCAGGAAGTATGTGGTTACAT
-CAAAACAATTCCCATACATTAGTGAGTTGATTGAGCTTGGTGTGTTGAACAAAACTTTTTCCCGATGGAA
-TGGAAAGCATATATTATTCCCTATTGAGGATATTTACTGGACTGAATTAGTTGCCAGCTATGATCCATAT
-AATATTGAGATAAAGCCAAGGCCAATATCTAAGTAACTAGATAAGAGGAATCGATTTTCCCTTAATTTTC
-TGGCGTCCACTGCATGTTATGCCGCGTTCGCCAGGCTTGCTGTACCATGTGCGCTGATTCTTGCGCTCAA
-TACGTTGCAGGTTGCTTTCAATCTGTTTGTGGTATTCAGCCAGCACTGTAAGGTCTATCGGATTTAGTGC
-GCTTTCTACTCGTGATTTCGGTTTGCGATTCAGCGAGAGAATAGGGCGGTTAACTGGTTTTGCGCTTACC
-CCAACCAACAGGGGATTTGCTGCTTTCCATTGAGCCTGTTTCTCTGCGCGACGTTCGCGGCGGCGTGTTT
-GTGCATCCATCTGGATTCTCCTGTCAGTTAGCTTTGGTGGTGTGTGGCAGTTGTAGTCCTGAACGAAAAC
-CCCCCGCGATTGGCACATTGGCAGCTAATCCGGAATCGCACTTACGGCCAATGCTTCGTTTCGTATCACA
-CACCCCAAAGCCTTCTGCTTTGAATGCTGCCCTTCTTCAGGGCTTAATTTTTAAGAGCGTCACCTTCATG
-GTGGTCAGTGCGTCCTGCTGATGTGCTCAGTATCACCGCCAGTGGTATTTATGTCAACACCGCCAGAGAT
-AATTTATCACCGCAGATGGTTATCTGTATGTTTTTTATATGAATTTATTTTTTGCAGGGGGGCATTGTTT
-GGTAGGTGAGAGATCTGAATTGCTATGTTTAGTGAGTTGTATCTATTTATTTTTCAATAAATACAATTGG
-TTATGTGTTTTGGGGGCGATCGTGAGGCAAAGAAAACCCGGCGCTGAGGCCGGGTTATTCTTGTTCTCTG
-GTCAAATTATATAGTTGGAAAACAAGGATGCATATATGAATGAACGATGCAGAGGCAATGCCGATGGCGA
-TAGTGGGTATCATGTAGCCGCTTATGCTGGAAAGAAGCAATAACCCGCAGAAAAACAAAGCTCCAAGCTC
-AACAAAACTAAGGGCATAGACAATAACTACCGATGTCATATACCCATACTCTCTAATCTTGGCCAGTCGG
-CGCGTTCTGCTTCCGATTAGAAACGTCAAGGCAGCAATCAGGATTGCAATCATGGTTCCTGCATATGATG
-ACAATGTCGCCCCAAGACCATCTCTATGAGCTGAAAAAGAAACACCAGGAATGTAGTGGCGGAAAAGGAG
-ATAGCAAATGCTTACGATAACGTAAGGAATTATTACTATGTAAACACCAGGCATGATTCTGTTCCGCATA
-ATTACTCCTGATAATTAATCCTTAACTTTGCCCACCTGCCTTTTAAAACATTCCAGTATATCACTTTTCA
-TTCTTGCGTAGCAATATGCCATCTCTTCAGCTATCTCAGCATTGGTGACCTTGTTCAGAGGCGCTGAGAG
-ATGGCCTTTTTCTGATAGATAATGTTCTGTTAAAATATCTCCGGCCTCATCTTTTGCCCGCAGGCTAATG
-TCTGAAAATTGAGGTGACGGGTTAAAAATAATATCCTTGGCAACCTTTTTTATATCCCTTTTAAATTTTG
-GCTTAATGACTATATCCAATGAGTCAAAAAGCTCCCCTTCAATATCTGTTGCCCCTAAGACCTTTAATAT
-ATCGCCAAATACAGGTAGCTTGGCTTCTACCTTCACCGTTGTTCGGCCGATGAAATGCATATGCATAACA
-TCGTCTTTGGTGGTTCCCCTCATCAGTGGCTCTATCTGAACGCGCTCTCCACTGCTTAATGACATTCCTT
-TCCCGATTAAAAAATCTGTCAGATCGGATGTGGTCGGCCCGAAAACAGTTCTGGCAAAACCAATGGTGTC
-GCCTTCAACAAACAAAAAAGATGGGAATCCCAATGATTCGTCATCTGCGAGGCTGTTCTTAATATCTTCA
-ACTGAAGCTTTAGAGCGATTTATCTTCTGAACCAGACTCTTGTCATTTGTTTTGGTAAAGAGAAAAGTTT
-TTCCATCGATTTTATGAATATACAAATAATTGGAGCCAACCTGCAGGTGATGATTATCAGCCAGCAGAGA
-ATTAAGGAAAACAGACAGGTTTATTGAGCGCTTATCTTTCCCTTTATTTTTGCTGCGGTAAGTCGCATAA
-AAACCATTCTTCATAATTCAATCCATTTACTATGTTATGTTCTGAGGGGAGTGAAAATTCCCCTAATTCG
-ATGAAGATTCTTGCTCAATTGTTATCAGCTATGCGCCGACCAGAACACCTTGCCGATCAGCCAAACGTCT
-CTTCAGGCCACTGACTAGCGATAACTTTCCCCACAACGGAACAACTCTCATTGCATGGGATCATTGGGTA
-CTGTGGGTTTAGTGGTTGTAAAAACACCTGACCGCTATCCCTGATCAGTTTCTTGAAGGTAAACTCATCA
-CCCCCAAGTCTGGCTATGCAGAAATCACCTGGCTCAACAGCCTGCTCAGGGTCAACGAGAATTAACATTC
-CGTCAGGAAAGCTTGGCTTGGAGCCTGTTGGTGCGGTCATGGAATTACCTTCAACCTCAAGCCAGAATGC
-AGAATCACTGGCTTTTTTGGTTGTGCTTACCCATCTCTCCGCATCACCTTTGGTAAAGGTTCTAAGCTCA
-GGTGAGAACATCCCTGCCTGAACATGAGAAAAAACAGGGTACTCATACTCACTTCTAAGTGACGGCTGCA
-TACTAACCGCTTCATACATCTCGTAGATTTCTCTGGCGATTGAAGGGCTAAATTCTTCAACGCTAACTTT
-GAGAATTTTTGCAAGCAATGCGGCGTTATAAGCATTTAATGCATTGATGCCATTAAATAAAGCACCAACG
-CCTGACTGCCCCATCCCCATCTTGTCTGCGACAGATTCCTGGGATAAGCCAAGTTCATTTTTCTTTTTTT
-CATAAATTGCTTTAAGGCGACGTGCGTCCTCAAGCTGCTCTTGTGTTAATGGTTTCTTTTTTGTGCTCAT
-ACGTTAAATCTATCACCGCAAGGGATAAATATCTAACACCGTGCGTGTTGACTATTTTACCTCTGGCGGT
-GATAATGGTTGCATGTACTAAGGAGGTTGTATGGAACAACGCATAACCCTGAAAGATTATGCAATGCGCT
-TTGGGCAAACCAAGACAGCTAAAGATCTCGGCGTATATCAAAGCGCGATCAACAAGGCCATTCATGCAGG
-CCGAAAGATTTTTTTAACTATAAACGCTGATGGAAGCGTTTATGCGGAAGAGGTAAAGCCCTTCCCGAGT
-AACAAAAAAACAACAGCATAAATAACCCCGCTCTTACACATTCCAGCCCTGAAAAAGGGCATCAAATTAA
-ACCACACCTATGGTGTATGCATTTATTTGCATACATTCAATCAATTGTTATCTAAGGAAATACTTACATA
-TGGTTCGTGCAAACAAACGCAACGAGGCTCTACGAATCGAGAGTGCGTTGCTTAACAAAATCGCAATGCT
-TGGAACTGAGAAGACAGCGGAAGCTGTGGGCGTTGATAAGTCGCAGATCAGCAGGTGGAAGAGGGACTGG
-ATTCCAAAGTTCTCAATGCTGCTTGCTGTTCTTGAATGGGGGGTCGTTGACGACGACATGGCTCGATTGG
-CGCGACAAGTTGCTGCGATTCTCACCAATAAAAAACGCCCGGCGGCAACCGAGCGTTCTGAACAAATCCA
-GATGGAGTTCTGAGGTCATTACTGGATCTATCAACAGGAGTCATTATGACAAATACAGCAAAAATACTCA
-ACTTCGGCAGAGGTAACTTTGCCGGACAGGAGCGTAATGTGGCAGATCTCGATGATGGTTACGCCAGACT
-ATCAAATATGCTGCTTGAGGCTTATTCGGGCGCAGATCTGACCAAGCGACAGTTTAAAGTGCTGCTTGCC
-ATTCTGCGTAAAACCTATGGGTGGAATAAACCAATGGACAGAATCACCGATTCTCAACTTAGCGAGATTA
-CAAAGTTACCTGTCAAACGGTGCAATGAAGCCAAGTTAGAACTCGTCAGAATGAATATTATCAAGCAGCA
-AGGCGGCATGTTTGGACCAAATAAAAACATCTCAGAATGGTGCATCCCTCAAAACGAGGGAAAATCCCCT
-AAAACGAGGGATAAAACATCCCTCAAATTGGGGGATTGCTATCCCTCAAAACAGGGGGACACAAAAGACA
-CTATTACAAAAGAAAAAAGAAAAGATTATTCGTCAGAGAATTCTGGCGAATCCTCTGACCAGCCAGAAAA
-CGACCTTTCTGTGGTGAAACCGGATGCTGCAATTCAGAGCGGCAGCAAGTGGGGGACAGCAGAAGACCTG
-ACCGCCGCAGAGTGGATGTTTGACATGGTGAAGACTATCGCACCATCAGCCAGAAAACCGAATTTTGCTG
-GGTGGGCTAACGATATCCGCCTGATGCGTGAACGTGACGGACGTAACCACCGCGACATGTGTGTGCTGTT
-CCGCTGGGCATGCCAGGACAACTTCTGGTCCGGTAACGTGCTGAGCCCGGCCAAACTCCGCGATAAGTGG
-ACCCAACTCGAAATCAACCGTAACAAGCAACAGGCAGGCGTGACAGCCAGCAAACCAAAACTCGACCTGA
-CAAACACAGACTGGATTTACGGGGTGGATCTATGAAAAACATCGCCGCACAGATGGTTAACTTTGACCGT
-GAGCAGATGCGTCGGATCGCCAACAACATGCCGGAACAGTACGACGAAAAGCCGCAGGTACAGCAGGTAG
-CGCAGATCATCAACGGTGTGTTCAGCCAGTTACTGGCAACTTTCCCGGCGAGCCTGGCTAACCGTGACCA
-GAACGAAGTGAACGAAATCCGTCGCCAGTGGGTTCTGGCTTTTCGGGAAAACGGGATCACCACGATGGAA
-CAGGTTAACGCAGGAATGCGCGTAGCCCGTCGGCAGAATCGACCATTTCTGCCATCACCCGGGCAGTTTG
-TTGCATGGTGCCGGGAAGAAGCATCCGTTACCGCCGGACTGCCAAACGTCAGCGAGCTGGTTGATATGGT
-TTACGAGTATTGCCGGAAGCGAGGCCTGTATCCGGATGCGGAGTCTTATCCGTGGAAATCAAACGCGCAC
-TACTGGCTGGTTACCAACCTGTATCAGAACATGCGGGCCAATGCGCTTACTGATGCGGAATTACGCCGTA
-AGGCCGCAGATGAGCTTGTCCATATGACTGCGAGAATTAACCGTGGTGAGGCGATCCCTGAACCAGTAAA
-ACAACTTCCTGTCATGGGCGGTAGACCTCTAAATCGTGCACAGGCTCTGGCGAAGATCGCAGAAATCAAA
-GCTAAGTTCGGACTGAAAGGAGCAAGTGTATGACGGGCAAAGAGGCAATTATTCATTACCTGGGGACGCA
-TAATAGCTTCTGTGCGCCGGACGTTGCCGCGCTAACAGGCGCAACAGTAACCAGCATAAATCAGGCCGCG
-GCTAAAATGGCACGGGCAGGTCTTCTGGTTATCGAAGGTAAGGTCTGGCGAACGGTGTATTACCGGTTTG
-CTACCAGGGAAGAACGGGAAGGAAAGATGAGCACGAACCTGGTTTTTAAGGAGTGTCGCCAGAGTGCCGC
-GATGAAACGGGTATTGGCGGTATATGGAGTTAAAAGATGACCATCTACATTACTGAGCTAATAACAGGCC
-TGCTGGTAATCGCAGGCCTTTTTATTTGGGGGAGAGGGAAGTCATGAAAAAACTAACCTTTGAAATTCGA
-TCTCCAGCACATCAGCAAAACGCTATTCACGCAGTACAGCAAATCCTTCCAGACCCAACCAAACCAATCG
-TAGTAACCATTCAGGAACGCAACCGCAGCTTAGACCAAAACAGGAAGCTATGGGCCTGCTTAGGTGACGT
-CTCTCGTCAGGTTGAATGGCATGGTCGCTGGCTGGATGCAGAAAGCTGGAAGTGTGTGTTTACCGCAGCA
-TTAAAGCAGCAGGATGTTGTTCCTAACCTTGCCGGGAATGGCTTTGTGGTAATAGGCCAGTCAACCAGCA
-GGATGCGTGTAGGCGAATTTGCGGAGCTATTAGAGCTTATACAGGCATTCGGTACAGAGCGTGGCGTTAA
-GTGGTCAGACGAAGCGAGACTGGCTCTGGAGTGGAAAGCGAGATGGGGAGACAGGGCTGCATGATAAATG
-TCGTTAGTTTCTCCGGTGGCAGGACGTCAGCATATTTGCTCTGGCTAATGGAGCAAAAGCGACGGGCAGG
-TAAAGACGTGCATTACGTTTTCATGGATACAGGTTGTGAACATCCAATGACATATCGGTTTGTCAGGGAA
-GTTGTGAAGTTCTGGGATATACCGCTCACCGTATTGCAGGTTGATATCAACCCGGAGCTTGGACAGCCAA
-ATGGTTATACGGTATGGGAACCAAAGGATATTCAGACGCGAATGCCTGTTCTGAAGCCATTTATCGATAT
-GGTAAAGAAATATGGCACTCCATACGTCGGCGGCGCGTTCTGCACTGACAGATTAAAACTCGTTCCCTTC
-ACCAAATACTGTGATGACCATTTCGGGCGAGGGAATTACACCACGTGGATTGGCATCAGAGCTGATGAAC
-CGAAGCGGCTAAAGCCAAAGCCTGGAATCAGATATCTTGCTGAACTGTCAGACTTTGAGAAGGAAGATAT
-CCTCGCATGGTGGAAGCAACAACCATTCGATTTGCAAATACCGGAACATCTCGGTAACTGCATATTCTGC
-ATTAAAAAATCAACGCAAAAAATCGGACTTGCCTGCAAAGATGAGGAGGGATTGCAGCGTGTTTTTAATG
-AGGTCATCACGGGATCCCATGTGCGTGACGGACATCGGGAAACGCCAAAGGAGATTATGTACCGAGGAAG
-AATGTCGCTGGACGGTATCGCGAAAATGTATTCAGAAAATGATTATCAAGCCCTGTATCAGGACATGGTA
-CGAGCTAAAAGATTCGATACCGGCTCTTGTTCTGAGTCATGCGAAATATTTGGAGGGCAGCTTGATTTCG
-ACTTCGGGAGGGAAGCTGCATGATGCGATGTTATCGGTGCGGTGAATGCAAAGAAGATAACCGCTTCCGA
-CCAAATCAACCTTACTGGAATCGATGGTGTCTCCGGTGTGAAAGAACACCAACAGGGGTGTTACCACTAC
-CGCAGGAAAAGGAGGACGTGTGGCGAGACAGCGACGAAGTATCACCGACATAATCTGCGAAAACTGCAAA
-TACCTTCCAACGAAACGCACCAGAAATAAACCCAAGCCAATCCCAAAAGAATCTGACGTAAAAACCTTCA
-ACTACACGGCTCACCTGTGGGATATCCGGTGGCTAAGACGTCGTGCGAGGAAAACAAGGTGATTGACCAA
-AATCGAAGTTACGAACAAGAAAGCGTCGAGCGAGCTTTAACGTGCGCTAACTGCGGTCAGAAGCTGCATG
-TGCTGGAAGTTCACGTGTGTGAGCACTGCTGCGCAGAACTGATGAGCGATCCGAATAGCTCGATGCACGA
-GGAAGAAGATGATGGCTAAACCAGCGCGAAGACGATGTAAAAACGATGAATGCCGGGAATGGTTTCACCC
-TGCATTCGCTAATCAGTGGTGGTGCTCTCCAGAGTGTGGAACCAAGATAGCACTCGAACGACGAAGTAAA
-GAACGCGAAAAAGCGGAAAAAGCAGCAGAGAAGAAACGACGACGAGAGGAGCAGAAACAGAAAGATAAAC
-TTAAGATTCGAAAACTCGCCTTAAAGCCCCGCAGTTACTGGATTAAACAAGCCCAACAAGCCGTAAACGC
-CTTCATCAGAGAAAGAGACCGCGACTTACCATGTATCTCGTGCGGAACGCTCACGTCTGCTCAGTGGGAT
-GCCGGACATTACCGGACAACTGCTGCGGCACCTCAACTCCGATTTAATGAACGCAATATTCACAAGCAAT
-GCGTGGTGTGCAACCAGCACAAAAGCGGAAATCTCGTTCCGTATCGCGTCGAACTGATTAGCCGCATCGG
-GCAGGAAGCAGTAGACGAAATCGAATCAAACCATAACCGCCATCGCTGGACTATCGAAGAGTGCAAGGCG
-ATCAAGGCAGAGTACCAACAGAAACTCAAAGACCTGCGAAATAGCAGAAGTGAGGCCGCATGACGTTCTC
-AGTAAAAACCATTCCAGACATGCTCGTTGAAGCATACGGAAATCAGACAGAAGTAGCACGCAGACTGAAA
-TGTAGTCGCGGTACGGTCAGAAAATACGTTGATGATAAAGACGGGAAAATGCACGCCATCGTCAACGACG
-TTCTCATGGTTCATCGCGGATGGAGTGAAAGAGATGCGCTATTACGAAAAAATTGATGGCAGCAAATACC
-GAAATATTTGGGTAGTTGGCGATCTGCACGGATGCTACACGAACCTGATGAACAAACTGGATACGATTGG
-ATTCGACAACAAAAAAGACCTGCTTATCTCGGTGGGCGATTTGGTTGATCGTGGTGCAGAGAACGTTGAA
-TGCCTGGAATTAATCACATTCCCCTGGTTCAGAGCTGTACGTGGAAACCATGAGCAAATGATGATTGATG
-GCTTATCAGAGCGTGGAAACGTTAATCACTGGCTGCTTAATGGCGGTGGCTGGTTCTTTAATCTCGATTA
-CGACAAAGAAATTCTGGCTAAAGCTCTTGCCCATAAAGCAGATGAACTTCCGTTAATCATCGAACTGGTG
-AGCAAAGATAAAAAATATGTTATCTGCCACGCCGATTATCCCTTTGACGAATACGAGTTTGGAAAGCCAG
-TTGATCATCAGCAGGTAATCTGGAACCGCGAACGAATCAGCAACTCACAAAACGGGATCGTGAAAGAAAT
-CAAAGGCGCGGACACGTTCATCTTTGGTCATACGCCAGCAGTGAAACCACTCAAGTTTGCCAACCAAATG
-TATATCGATACCGGCGCAGTGTTCTGCGGAAACCTAACATTGATTCAGGTACAGGGAGAAGGCGCATGAG
-ACTCGAAAGCGTAGCTAAATTTCATTCGCCAAAAAGCCCGATGATGAGCGACTCACCACGGGCCACGGCT
-TCTGACTCTCTTTCCGGTACTGATGTGATGGCTGCTATGGGGATGGCGCAATCACAAGCCGGATTCGGTA
-TGGCTGCATTCTGCGGTAAGCACGAACTCAGCCAGAACGACAAACAAAAGGCTATCAACTATCTGATGCA
-ATTTGCACACAAGGTATCGGGGAAATACCGTGGTGTGGCAAAGCTTGAAGGAAATACTAAGGCAAAGGTA
-CTGCAAGTGCTCGCAACATTCGCTTATGCGGATTATTGCCGTAGTGCCGCGACGCCGGGGGCAAGATGCA
-GAGATTGCCATGGTACAGGCCGTGCGGTTGATATTGCCAAAACAGAGCTGTGGGGGAGAGTTGTCGAGAA
-AGAGTGCGGAAGATGCAAAGGCGTCGGCTATTCAAGGATGCCAGCAAGCGCAGCATATCGCGCTGTGACG
-ATGCTAATCCCAAACCTTACCCAACCCACCTGGTCACGCACTGTTAAGCCGCTGTATGACGCTCTGGTGG
-TGCAATGCCACAAAGAAGAGTCAATCGCAGACAACATTTTGAATGCGGTCACACGTTAGCAGCATGATTG
-CCACGGATGGCAACATATTAACGGCATGATATTGACTTATTGAATAAAATTGGGTAAATTTGACTCAACG
-ATGGGTTAATTCGCTCGTTGTGGTAGTGAGATGAAAAGAGGCGGCGCTTACTACCGATTCCGCCTAGTTG
-GTCACTTCGACGTATCGTCTGGAACTCCAACCATCGCAGGCAGAGAGGTCTGCAAAATGCAATCCCGAAA
-CAGTTCGCAGGTAATAGTTAGAGCCTGCATAACGGTTTCGGGATTTTTTATATCTGCACAACAGGTAAGA
-GCATTGAGTCGATAATCGTGAAGAGTCGGCGAGCCTGGTTAGCCAGTGCTCTTTCCGTTGTGCTGAATTA
-AGCGAATACCGGAAGCAGAACCGGATCACCAAATGCGTACAGGCGTCATCGCCGCCCAGCAACAGCACAA
-CCCAAACTGAGCCGTAGCCACTGTCTGTCCTGAATTCATTAGTAATAGTTACGCTGCGGCCTTTTACACA
-TGACCTTCGTGAAAGCGGGTGGCAGGAGGTCGCGCTAACAACCTCCTGCCGTTTTGCCCGTGCATATCGG
-TCACGAACAAATCTGATTACTAAACACAGTAGCCTGGATTTGTTCTATCAGTAATCGACCTTATTCCTAA
-TTAAATAGAGCAAATCCCCTTATTGGGGGTAAGACATGAAGATGCCAGAAAAACATGACCTGTTGGCCGC
-CATTCTCGCGGCAAAGGAACAAGGCATCGGGGCAATCCTTGCGTTTGCAATGGCGTACCTTCGCGGCAGA
-TATAATGGCGGTGCGTTTACAAAAACAGTAATCGACGCAACGATGTGCGCCATTATCGCCTGGTTCATTC
-GTGACCTTCTCGACTTCGCCGGACTAAGTAGCAATCTCGCTTATATAACGAGCGTGTTTATCGGCTACAT
-CGGTACTGACTCGATTGGTTCGCTTATCAAACGCTTCGCTGCTAAAAAAGCCGGAGTAGAAGATGGTAGA
-AATCAATAATCAACGTAAGGCGTTCCTCGATATGCTGGCGTGGTCGGAGGGAACTGATAACGGACGTCAG
-AAAACCAGAAATCATGGTTATGACGTCATTGTAGGCGGAGAGCTATTTACTGATTACTCCGATCACCCTC
-GCAAACTTGTCACGCTAAACCCAAAACTCAAATCAACAGGCGCCGGACGCTACCAGCTTCTTTCCCGTTG
-GTGGGATGCCTACCGCAAGCAGCTTGGCCTGAAAGACTTCTCTCCGAAAAGTCAGGACGCTGTGGCATTG
-CAGCAGATTAAGGAGCGTGGCGCTTTACCTATGATTGATCGTGGTGATATCCGTCAGGCAATCGACCGTT
-GCAGCAATATCTGGGCTTCACTGCCGGGCGCTGGTTATGGTCAGTTCGAGCATAAGGCTGACAGCCTGAT
-TGCAAAATTCAAAGAAGCGGGCGGAACGGTCAGAGAGATTGATGTATGAGCAGAGTCACCGCGATTATCT
-CCGCTCTGGTTATCTGCATCATCGTCTGCCTGTCATGGGCTGTTAATCATTACCGTGATAACGCCATTAC
-CTACAAAGCCCAGCGCGACAAAAATGCCAGAGAACTGAAGCTGGCGAACGCGGCAATTACTGACATGCAG
-ATGCGTCAGCGTGATGTTGCTGCGCTCGATGCAAAATACACGAAGGAGTTAGCTGATGCTAAAGCTGAAA
-ATGATGCTCTGCGTGATGATGTTGCCGCTGGTCGTCGTCGGTTGCACATCAAAGCAGTCTGTCAGTCAGT
-GCGTGAAGCCACCACCGCCTCCGGCGTGGATAATGCAGCCTCCCCCCGACTGGCAGACACCGCTGAACGG
-GATTATTTCACCCTCAGAGAGAGGCTGATCACTATGCAAAAACAACTGGAAGGAACCCAGAAGTATATTA
-ATGAGCAGTGCAGATAGAGTTGCCCATATCGATGGGCAACTCATGCAATTATTGTGAGCAATACACACGC
-GCTTCCAGCGGAGTATAAATGCCTAAAGTAATAAAACCGAGCAATCCATTTACGAATGTTTGCTGGGTTT
-CTGTTTTAACAACATTTTCTGCGCCGCCACAAATTTTGGCTGCATCGACAGTTTTCTTCTGCCCAATTCC
-AGAAACGAAGAAATGATGGGTGATGGTTTCCTTTGGTGCTACTGCTGCCGGTTTGTTTTGAACAGTAAAC
-GTCTGTTGAGCACATCCTGTAATAAGCAGGGCCAGCGCAGTAGCGAGTAGCATTTTTTTCATGGTGTTAT
-TCCCGATGCTTTTTGAAGTTCGCAGAATCGTATGTGTAGAAAATTAAACAAACCCTAAACAATGAGTTGA
-AATTTCATATTGTTAATATTTATTAATGTATGTCAGGTGCGATGAATCGTCATTGTATTCCCGGATTAAC
-TATGTCCACAGCCCTGACGGGGAACTTCTCTGCGGGAGTGTCCGGGAATAATTAAAACGATGCACACAGG
-GTTTAGCGCGTACACGTATTGCATTATGCCAACGCCCCGGTGCTGACACGGAAGAAACCGGACGTTATGA
-TTTAGCGTGGAAAGATTTGTGTAGTGTTCTGAATGCTCTCAGTAAATAGTAATGAATTATCAAAGGTATA
-GTAATATCTTTTATGTTCATGGATATTTGTAACCCATCGGAAAACTCCTGCTTTAGCAAGATTTTCCCTG
-TATTGCTGAAATGTGATTTCTCTTGATTTCAACCTATCATAGGACGTTTCTATAAGATGCGTGTTTCTTG
-AGAATTTAACATTTACAACCTTTTTAAGTCCTTTTATTAACACGGTGTTATCGTTTTCTAACACGATGTG
-AATATTATCTGTGGCTAGATAGTAAATATAATGTGAGACGTTGTGACGTTTTAGTTCAGAATAAAACAAT
-TCACAGTCTAAATCTTTTCGCACTTGATCGAATATTTCTTTAAAAATGGCAACCTGAGCCATTGGTAAAA
-CCTTCCATGTGATACGAGGGCGCGTAGTTTGCATTATCGTTTTTATCGTTTCAATCTGGTCTGACCTCCT
-TGTGTTTTGTTGATGATTTATGTCAAATATTAGGAATGTTTTCACTTAATAGTATTGGTTGCGTAACAAA
-GTGCGGTCCTGCTGGCATTCTGGAGGGAAATACAACCGACAGATGTATGTAAGGCCAACGTGCTCAAATC
-TTCATACAGAAAGATTTGAAGTAATATTTTAACCGCTAGATGAAGAGCAAGCGCATGGAGCGACAAAATG
-AATAAAGAACAATCTGCTGATGATCCCTCCGTGGATCTGATTCGTGTAAAAAATATGCTTAATAGCACCA
-TTTCTATGAGTTACCCTGATGTTGTAATTGCATGTATAGAACATAAGGTGTCTCTGGAAGCATTCAGAGC
-AATTGAGGCAGCGTTGGTGAAGCACGATAATAATATGAAGGATTATTCCCTGGTGGTTGACTGATCACCA
-TAACTGCTAATCATTCAAACTATTTAGTCTGTGACAGAGCCAACACGCAGTCTGTCACTGTCAGGAAAGT
-GGTAAAACTGCAACTCAATTACTGCAATGCCCTCGTAATTAAGTGAATTTACAATATCGTCCTGTTCGGA
-GGGAAGAACGCGGGATGTTCATTCTTCATCACTTTTAATTGATGTATATGCTCTCTTTTCTGACGTTAGT
-CTCCGACGGCAGGCTTCAATGACCCAGGCTGAGAAATTCCCGGACCCTTTTTGCTCAAGAGCGATGTTAA
-TTTGTTCAATCATTTGGTTAGGAAAGCGGATGTTGCGGGTTGTTGTTCTGCGGGTTCTGTTCTTCGTTGA
-CATGAGGTTGCCCCGTATTCAGTGTCGCTGATTTGTATTGTCTGAAGTTGTTTTTACGTTAAGTTGATGC
-AGATCAATTAATACGATACCTGCGTCATAATTGATTATTTGACGTGGTTTGATGGCCTCCACGCACGTTG
-TGATATGTAGATGATAATCATTATCACTTTACGGGTCCTTTCCGGTGATCCGACAGGTTACG
-
+>NC_001416.1 Enterobacteria phage lambda, complete genome
+GGGCGGCGACCTCGCGGGTTTTCGCTATTTATGAAAATTTTCCGGTTTAAGGCGTTTCCGTTCTTCTTCGTCATAACTTA
+ATGTTTTTATTTAAAATACCCTCTGAAAAGAAAGGAAACGACAGGTGCTGAAAGCGAGGCTTTTTGGCCTCTGTCGTTTC
+CTTTCTCTGTTTTTGTCCGTGGAATGAACAATGGAAGTCAACAAAAAGCAGCTGGCTGACATTTTCGGTGCGAGTATCCG
+TACCATTCAGAACTGGCAGGAACAGGGAATGCCCGTTCTGCGAGGCGGTGGCAAGGGTAATGAGGTGCTTTATGACTCTG
+CCGCCGTCATAAAATGGTATGCCGAAAGGGATGCTGAAATTGAGAACGAAAAGCTGCGCCGGGAGGTTGAAGAACTGCGG
+CAGGCCAGCGAGGCAGATCTCCAGCCAGGAACTATTGAGTACGAACGCCATCGACTTACGCGTGCGCAGGCCGACGCACA
+GGAACTGAAGAATGCCAGAGACTCCGCTGAAGTGGTGGAAACCGCATTCTGTACTTTCGTGCTGTCGCGGATCGCAGGTG
+AAATTGCCAGTATTCTCGACGGGCTCCCCCTGTCGGTGCAGCGGCGTTTTCCGGAACTGGAAAACCGACATGTTGATTTC
+CTGAAACGGGATATCATCAAAGCCATGAACAAAGCAGCCGCGCTGGATGAACTGATACCGGGGTTGCTGAGTGAATATAT
+CGAACAGTCAGGTTAACAGGCTGCGGCATTTTGTCCGCGCCGGGCTTCGCTCACTGTTCAGGCCGGAGCCACAGACCGCC
+GTTGAATGGGCGGATGCTAATTACTATCTCCCGAAAGAATCCGCATACCAGGAAGGGCGCTGGGAAACACTGCCCTTTCA
+GCGGGCCATCATGAATGCGATGGGCAGCGACTACATCCGTGAGGTGAATGTGGTGAAGTCTGCCCGTGTCGGTTATTCCA
+AAATGCTGCTGGGTGTTTATGCCTACTTTATAGAGCATAAGCAGCGCAACACCCTTATCTGGTTGCCGACGGATGGTGAT
+GCCGAGAACTTTATGAAAACCCACGTTGAGCCGACTATTCGTGATATTCCGTCGCTGCTGGCGCTGGCCCCGTGGTATGG
+CAAAAAGCACCGGGATAACACGCTCACCATGAAGCGTTTCACTAATGGGCGTGGCTTCTGGTGCCTGGGCGGTAAAGCGG
+CAAAAAACTACCGTGAAAAGTCGGTGGATGTGGCGGGTTATGATGAACTTGCTGCTTTTGATGATGATATTGAACAGGAA
+GGCTCTCCGACGTTCCTGGGTGACAAGCGTATTGAAGGCTCGGTCTGGCCAAAGTCCATCCGTGGCTCCACGCCAAAAGT
+GAGAGGCACCTGTCAGATTGAGCGTGCAGCCAGTGAATCCCCGCATTTTATGCGTTTTCATGTTGCCTGCCCGCATTGCG
+GGGAGGAGCAGTATCTTAAATTTGGCGACAAAGAGACGCCGTTTGGCCTCAAATGGACGCCGGATGACCCCTCCAGCGTG
+TTTTATCTCTGCGAGCATAATGCCTGCGTCATCCGCCAGCAGGAGCTGGACTTTACTGATGCCCGTTATATCTGCGAAAA
+GACCGGGATCTGGACCCGTGATGGCATTCTCTGGTTTTCGTCATCCGGTGAAGAGATTGAGCCACCTGACAGTGTGACCT
+TTCACATCTGGACAGCGTACAGCCCGTTCACCACCTGGGTGCAGATTGTCAAAGACTGGATGAAAACGAAAGGGGATACG
+GGAAAACGTAAAACCTTCGTAAACACCACGCTCGGTGAGACGTGGGAGGCGAAAATTGGCGAACGTCCGGATGCTGAAGT
+GATGGCAGAGCGGAAAGAGCATTATTCAGCGCCCGTTCCTGACCGTGTGGCTTACCTGACCGCCGGTATCGACTCCCAGC
+TGGACCGCTACGAAATGCGCGTATGGGGATGGGGGCCGGGTGAGGAAAGCTGGCTGATTGACCGGCAGATTATTATGGGC
+CGCCACGACGATGAACAGACGCTGCTGCGTGTGGATGAGGCCATCAATAAAACCTATACCCGCCGGAATGGTGCAGAAAT
+GTCGATATCCCGTATCTGCTGGGATACTGGCGGGATTGACCCGACCATTGTGTATGAACGCTCGAAAAAACATGGGCTGT
+TCCGGGTGATCCCCATTAAAGGGGCATCCGTCTACGGAAAGCCGGTGGCCAGCATGCCACGTAAGCGAAACAAAAACGGG
+GTTTACCTTACCGAAATCGGTACGGATACCGCGAAAGAGCAGATTTATAACCGCTTCACACTGACGCCGGAAGGGGATGA
+ACCGCTTCCCGGTGCCGTTCACTTCCCGAATAACCCGGATATTTTTGATCTGACCGAAGCGCAGCAGCTGACTGCTGAAG
+AGCAGGTCGAAAAATGGGTGGATGGCAGGAAAAAAATACTGTGGGACAGCAAAAAGCGACGCAATGAGGCACTCGACTGC
+TTCGTTTATGCGCTGGCGGCGCTGCGCATCAGTATTTCCCGCTGGCAGCTGGATCTCAGTGCGCTGCTGGCGAGCCTGCA
+GGAAGAGGATGGTGCAGCAACCAACAAGAAAACACTGGCAGATTACGCCCGTGCCTTATCCGGAGAGGATGAATGACGCG
+ACAGGAAGAACTTGCCGCTGCCCGTGCGGCACTGCATGACCTGATGACAGGTAAACGGGTGGCAACAGTACAGAAAGACG
+GACGAAGGGTGGAGTTTACGGCCACTTCCGTGTCTGACCTGAAAAAATATATTGCAGAGCTGGAAGTGCAGACCGGCATG
+ACACAGCGACGCAGGGGACCTGCAGGATTTTATGTATGAAAACGCCCACCATTCCCACCCTTCTGGGGCCGGACGGCATG
+ACATCGCTGCGCGAATATGCCGGTTATCACGGCGGTGGCAGCGGATTTGGAGGGCAGTTGCGGTCGTGGAACCCACCGAG
+TGAAAGTGTGGATGCAGCCCTGTTGCCCAACTTTACCCGTGGCAATGCCCGCGCAGACGATCTGGTACGCAATAACGGCT
+ATGCCGCCAACGCCATCCAGCTGCATCAGGATCATATCGTCGGGTCTTTTTTCCGGCTCAGTCATCGCCCAAGCTGGCGC
+TATCTGGGCATCGGGGAGGAAGAAGCCCGTGCCTTTTCCCGCGAGGTTGAAGCGGCATGGAAAGAGTTTGCCGAGGATGA
+CTGCTGCTGCATTGACGTTGAGCGAAAACGCACGTTTACCATGATGATTCGGGAAGGTGTGGCCATGCACGCCTTTAACG
+GTGAACTGTTCGTTCAGGCCACCTGGGATACCAGTTCGTCGCGGCTTTTCCGGACACAGTTCCGGATGGTCAGCCCGAAG
+CGCATCAGCAACCCGAACAATACCGGCGACAGCCGGAACTGCCGTGCCGGTGTGCAGATTAATGACAGCGGTGCGGCGCT
+GGGATATTACGTCAGCGAGGACGGGTATCCTGGCTGGATGCCGCAGAAATGGACATGGATACCCCGTGAGTTACCCGGCG
+GGCGCGCCTCGTTCATTCACGTTTTTGAACCCGTGGAGGACGGGCAGACTCGCGGTGCAAATGTGTTTTACAGCGTGATG
+GAGCAGATGAAGATGCTCGACACGCTGCAGAACACGCAGCTGCAGAGCGCCATTGTGAAGGCGATGTATGCCGCCACCAT
+TGAGAGTGAGCTGGATACGCAGTCAGCGATGGATTTTATTCTGGGCGCGAACAGTCAGGAGCAGCGGGAAAGGCTGACCG
+GCTGGATTGGTGAAATTGCCGCGTATTACGCCGCAGCGCCGGTCCGGCTGGGAGGCGCAAAAGTACCGCACCTGATGCCG
+GGTGACTCACTGAACCTGCAGACGGCTCAGGATACGGATAACGGCTACTCCGTGTTTGAGCAGTCACTGCTGCGGTATAT
+CGCTGCCGGGCTGGGTGTCTCGTATGAGCAGCTTTCCCGGAATTACGCCCAGATGAGCTACTCCACGGCACGGGCCAGTG
+CGAACGAGTCGTGGGCGTACTTTATGGGGCGGCGAAAATTCGTCGCATCCCGTCAGGCGAGCCAGATGTTTCTGTGCTGG
+CTGGAAGAGGCCATCGTTCGCCGCGTGGTGACGTTACCTTCAAAAGCGCGCTTCAGTTTTCAGGAAGCCCGCAGTGCCTG
+GGGGAACTGCGACTGGATAGGCTCCGGTCGTATGGCCATCGATGGTCTGAAAGAAGTTCAGGAAGCGGTGATGCTGATAG
+AAGCCGGACTGAGTACCTACGAGAAAGAGTGCGCAAAACGCGGTGACGACTATCAGGAAATTTTTGCCCAGCAGGTCCGT
+GAAACGATGGAGCGCCGTGCAGCCGGTCTTAAACCGCCCGCCTGGGCGGCTGCAGCATTTGAATCCGGGCTGCGACAATC
+AACAGAGGAGGAGAAGAGTGACAGCAGAGCTGCGTAATCTCCCGCATATTGCCAGCATGGCCTTTAATGAGCCGCTGATG
+CTTGAACCCGCCTATGCGCGGGTTTTCTTTTGTGCGCTTGCAGGCCAGCTTGGGATCAGCAGCCTGACGGATGCGGTGTC
+CGGCGACAGCCTGACTGCCCAGGAGGCACTCGCGACGCTGGCATTATCCGGTGATGATGACGGACCACGACAGGCCCGCA
+GTTATCAGGTCATGAACGGCATCGCCGTGCTGCCGGTGTCCGGCACGCTGGTCAGCCGGACGCGGGCGCTGCAGCCGTAC
+TCGGGGATGACCGGTTACAACGGCATTATCGCCCGTCTGCAACAGGCTGCCAGCGATCCGATGGTGGACGGCATTCTGCT
+CGATATGGACACGCCCGGCGGGATGGTGGCGGGGGCATTTGACTGCGCTGACATCATCGCCCGTGTGCGTGACATAAAAC
+CGGTATGGGCGCTTGCCAACGACATGAACTGCAGTGCAGGTCAGTTGCTTGCCAGTGCCGCCTCCCGGCGTCTGGTCACG
+CAGACCGCCCGGACAGGCTCCATCGGCGTCATGATGGCTCACAGTAATTACGGTGCTGCGCTGGAGAAACAGGGTGTGGA
+AATCACGCTGATTTACAGCGGCAGCCATAAGGTGGATGGCAACCCCTACAGCCATCTTCCGGATGACGTCCGGGAGACAC
+TGCAGTCCCGGATGGACGCAACCCGCCAGATGTTTGCGCAGAAGGTGTCGGCATATACCGGCCTGTCCGTGCAGGTTGTG
+CTGGATACCGAGGCTGCAGTGTACAGCGGTCAGGAGGCCATTGATGCCGGACTGGCTGATGAACTTGTTAACAGCACCGA
+TGCGATCACCGTCATGCGTGATGCACTGGATGCACGTAAATCCCGTCTCTCAGGAGGGCGAATGACCAAAGAGACTCAAT
+CAACAACTGTTTCAGCCACTGCTTCGCAGGCTGACGTTACTGACGTGGTGCCAGCGACGGAGGGCGAGAACGCCAGCGCG
+GCGCAGCCGGACGTGAACGCGCAGATCACCGCAGCGGTTGCGGCAGAAAACAGCCGCATTATGGGGATCCTCAACTGTGA
+GGAGGCTCACGGACGCGAAGAACAGGCACGCGTGCTGGCAGAAACCCCCGGTATGACCGTGAAAACGGCCCGCCGCATTC
+TGGCCGCAGCACCACAGAGTGCACAGGCGCGCAGTGACACTGCGCTGGATCGTCTGATGCAGGGGGCACCGGCACCGCTG
+GCTGCAGGTAACCCGGCATCTGATGCCGTTAACGATTTGCTGAACACACCAGTGTAAGGGATGTTTATGACGAGCAAAGA
+AACCTTTACCCATTACCAGCCGCAGGGCAACAGTGACCCGGCTCATACCGCAACCGCGCCCGGCGGATTGAGTGCGAAAG
+CGCCTGCAATGACCCCGCTGATGCTGGACACCTCCAGCCGTAAGCTGGTTGCGTGGGATGGCACCACCGACGGTGCTGCC
+GTTGGCATTCTTGCGGTTGCTGCTGACCAGACCAGCACCACGCTGACGTTCTACAAGTCCGGCACGTTCCGTTATGAGGA
+TGTGCTCTGGCCGGAGGCTGCCAGCGACGAGACGAAAAAACGGACCGCGTTTGCCGGAACGGCAATCAGCATCGTTTAAC
+TTTACCCTTCATCACTAAAGGCCGCCTGTGCGGCTTTTTTTACGGGATTTTTTTATGTCGATGTACACAACCGCCCAACT
+GCTGGCGGCAAATGAGCAGAAATTTAAGTTTGATCCGCTGTTTCTGCGTCTCTTTTTCCGTGAGAGCTATCCCTTCACCA
+CGGAGAAAGTCTATCTCTCACAAATTCCGGGACTGGTAAACATGGCGCTGTACGTTTCGCCGATTGTTTCCGGTGAGGTT
+ATCCGTTCCCGTGGCGGCTCCACCTCTGAATTTACGCCGGGATATGTCAAGCCGAAGCATGAAGTGAATCCGCAGATGAC
+CCTGCGTCGCCTGCCGGATGAAGATCCGCAGAATCTGGCGGACCCGGCTTACCGCCGCCGTCGCATCATCATGCAGAACA
+TGCGTGACGAAGAGCTGGCCATTGCTCAGGTCGAAGAGATGCAGGCAGTTTCTGCCGTGCTTAAGGGCAAATACACCATG
+ACCGGTGAAGCCTTCGATCCGGTTGAGGTGGATATGGGCCGCAGTGAGGAGAATAACATCACGCAGTCCGGCGGCACGGA
+GTGGAGCAAGCGTGACAAGTCCACGTATGACCCGACCGACGATATCGAAGCCTACGCGCTGAACGCCAGCGGTGTGGTGA
+ATATCATCGTGTTCGATCCGAAAGGCTGGGCGCTGTTCCGTTCCTTCAAAGCCGTCAAGGAGAAGCTGGATACCCGTCGT
+GGCTCTAATTCCGAGCTGGAGACAGCGGTGAAAGACCTGGGCAAAGCGGTGTCCTATAAGGGGATGTATGGCGATGTGGC
+CATCGTCGTGTATTCCGGACAGTACGTGGAAAACGGCGTCAAAAAGAACTTCCTGCCGGACAACACGATGGTGCTGGGGA
+ACACTCAGGCACGCGGTCTGCGCACCTATGGCTGCATTCAGGATGCGGACGCACAGCGCGAAGGCATTAACGCCTCTGCC
+CGTTACCCGAAAAACTGGGTGACCACCGGCGATCCGGCGCGTGAGTTCACCATGATTCAGTCAGCACCGCTGATGCTGCT
+GGCTGACCCTGATGAGTTCGTGTCCGTACAACTGGCGTAATCATGGCCCTTCGGGGCCATTGTTTCTCTGTGGAGGAGTC
+CATGACGAAAGATGAACTGATTGCCCGTCTCCGCTCGCTGGGTGAACAACTGAACCGTGATGTCAGCCTGACGGGGACGA
+AAGAAGAACTGGCGCTCCGTGTGGCAGAGCTGAAAGAGGAGCTTGATGACACGGATGAAACTGCCGGTCAGGACACCCCT
+CTCAGCCGGGAAAATGTGCTGACCGGACATGAAAATGAGGTGGGATCAGCGCAGCCGGATACCGTGATTCTGGATACGTC
+TGAACTGGTCACGGTCGTGGCACTGGTGAAGCTGCATACTGATGCACTTCACGCCACGCGGGATGAACCTGTGGCATTTG
+TGCTGCCGGGAACGGCGTTTCGTGTCTCTGCCGGTGTGGCAGCCGAAATGACAGAGCGCGGCCTGGCCAGAATGCAATAA
+CGGGAGGCGCTGTGGCTGATTTCGATAACCTGTTCGATGCTGCCATTGCCCGCGCCGATGAAACGATACGCGGGTACATG
+GGAACGTCAGCCACCATTACATCCGGTGAGCAGTCAGGTGCGGTGATACGTGGTGTTTTTGATGACCCTGAAAATATCAG
+CTATGCCGGACAGGGCGTGCGCGTTGAAGGCTCCAGCCCGTCCCTGTTTGTCCGGACTGATGAGGTGCGGCAGCTGCGGC
+GTGGAGACACGCTGACCATCGGTGAGGAAAATTTCTGGGTAGATCGGGTTTCGCCGGATGATGGCGGAAGTTGTCATCTC
+TGGCTTGGACGGGGCGTACCGCCTGCCGTTAACCGTCGCCGCTGAAAGGGGGATGTATGGCCATAAAAGGTCTTGAGCAG
+GCCGTTGAAAACCTCAGCCGTATCAGCAAAACGGCGGTGCCTGGTGCCGCCGCAATGGCCATTAACCGCGTTGCTTCATC
+CGCGATATCGCAGTCGGCGTCACAGGTTGCCCGTGAGACAAAGGTACGCCGGAAACTGGTAAAGGAAAGGGCCAGGCTGA
+AAAGGGCCACGGTCAAAAATCCGCAGGCCAGAATCAAAGTTAACCGGGGGGATTTGCCCGTAATCAAGCTGGGTAATGCG
+CGGGTTGTCCTTTCGCGCCGCAGGCGTCGTAAAAAGGGGCAGCGTTCATCCCTGAAAGGTGGCGGCAGCGTGCTTGTGGT
+GGGTAACCGTCGTATTCCCGGCGCGTTTATTCAGCAACTGAAAAATGGCCGGTGGCATGTCATGCAGCGTGTGGCTGGGA
+AAAACCGTTACCCCATTGATGTGGTGAAAATCCCGATGGCGGTGCCGCTGACCACGGCGTTTAAACAAAATATTGAGCGG
+ATACGGCGTGAACGTCTTCCGAAAGAGCTGGGCTATGCGCTGCAGCATCAACTGAGGATGGTAATAAAGCGATGAAACAT
+ACTGAACTCCGTGCAGCCGTACTGGATGCACTGGAGAAGCATGACACCGGGGCGACGTTTTTTGATGGTCGCCCCGCTGT
+TTTTGATGAGGCGGATTTTCCGGCAGTTGCCGTTTATCTCACCGGCGCTGAATACACGGGCGAAGAGCTGGACAGCGATA
+CCTGGCAGGCGGAGCTGCATATCGAAGTTTTCCTGCCTGCTCAGGTGCCGGATTCAGAGCTGGATGCGTGGATGGAGTCC
+CGGATTTATCCGGTGATGAGCGATATCCCGGCACTGTCAGATTTGATCACCAGTATGGTGGCCAGCGGCTATGACTACCG
+GCGCGACGATGATGCGGGCTTGTGGAGTTCAGCCGATCTGACTTATGTCATTACCTATGAAATGTGAGGACGCTATGCCT
+GTACCAAATCCTACAATGCCGGTGAAAGGTGCCGGGACCACCCTGTGGGTTTATAAGGGGAGCGGTGACCCTTACGCGAA
+TCCGCTTTCAGACGTTGACTGGTCGCGTCTGGCAAAAGTTAAAGACCTGACGCCCGGCGAACTGACCGCTGAGTCCTATG
+ACGACAGCTATCTCGATGATGAAGATGCAGACTGGACTGCGACCGGGCAGGGGCAGAAATCTGCCGGAGATACCAGCTTC
+ACGCTGGCGTGGATGCCCGGAGAGCAGGGGCAGCAGGCGCTGCTGGCGTGGTTTAATGAAGGCGATACCCGTGCCTATAA
+AATCCGCTTCCCGAACGGCACGGTCGATGTGTTCCGTGGCTGGGTCAGCAGTATCGGTAAGGCGGTGACGGCGAAGGAAG
+TGATCACCCGCACGGTGAAAGTCACCAATGTGGGACGTCCGTCGATGGCAGAAGATCGCAGCACGGTAACAGCGGCAACC
+GGCATGACCGTGACGCCTGCCAGCACCTCGGTGGTGAAAGGGCAGAGCACCACGCTGACCGTGGCCTTCCAGCCGGAGGG
+CGTAACCGACAAGAGCTTTCGTGCGGTGTCTGCGGATAAAACAAAAGCCACCGTGTCGGTCAGTGGTATGACCATCACCG
+TGAACGGCGTTGCTGCAGGCAAGGTCAACATTCCGGTTGTATCCGGTAATGGTGAGTTTGCTGCGGTTGCAGAAATTACC
+GTCACCGCCAGTTAATCCGGAGAGTCAGCGATGTTCCTGAAAACCGAATCATTTGAACATAACGGTGTGACCGTCACGCT
+TTCTGAACTGTCAGCCCTGCAGCGCATTGAGCATCTCGCCCTGATGAAACGGCAGGCAGAACAGGCGGAGTCAGACAGCA
+ACCGGAAGTTTACTGTGGAAGACGCCATCAGAACCGGCGCGTTTCTGGTGGCGATGTCCCTGTGGCATAACCATCCGCAG
+AAGACGCAGATGCCGTCCATGAATGAAGCCGTTAAACAGATTGAGCAGGAAGTGCTTACCACCTGGCCCACGGAGGCAAT
+TTCTCATGCTGAAAACGTGGTGTACCGGCTGTCTGGTATGTATGAGTTTGTGGTGAATAATGCCCCTGAACAGACAGAGG
+ACGCCGGGCCCGCAGAGCCTGTTTCTGCGGGAAAGTGTTCGACGGTGAGCTGAGTTTTGCCCTGAAACTGGCGCGTGAGA
+TGGGGCGACCCGACTGGCGTGCCATGCTTGCCGGGATGTCATCCACGGAGTATGCCGACTGGCACCGCTTTTACAGTACC
+CATTATTTTCATGATGTTCTGCTGGATATGCACTTTTCCGGGCTGACGTACACCGTGCTCAGCCTGTTTTTCAGCGATCC
+GGATATGCATCCGCTGGATTTCAGTCTGCTGAACCGGCGCGAGGCTGACGAAGAGCCTGAAGATGATGTGCTGATGCAGA
+AAGCGGCAGGGCTTGCCGGAGGTGTCCGCTTTGGCCCGGACGGGAATGAAGTTATCCCCGCTTCCCCGGATGTGGCGGAC
+ATGACGGAGGATGACGTAATGCTGATGACAGTATCAGAAGGGATCGCAGGAGGAGTCCGGTATGGCTGAACCGGTAGGCG
+ATCTGGTCGTTGATTTGAGTCTGGATGCGGCCAGATTTGACGAGCAGATGGCCAGAGTCAGGCGTCATTTTTCTGGTACG
+GAAAGTGATGCGAAAAAAACAGCGGCAGTCGTTGAACAGTCGCTGAGCCGACAGGCGCTGGCTGCACAGAAAGCGGGGAT
+TTCCGTCGGGCAGTATAAAGCCGCCATGCGTATGCTGCCTGCACAGTTCACCGACGTGGCCACGCAGCTTGCAGGCGGGC
+AAAGTCCGTGGCTGATCCTGCTGCAACAGGGGGGGCAGGTGAAGGACTCCTTCGGCGGGATGATCCCCATGTTCAGGGGG
+CTTGCCGGTGCGATCACCCTGCCGATGGTGGGGGCCACCTCGCTGGCGGTGGCGACCGGTGCGCTGGCGTATGCCTGGTA
+TCAGGGCAACTCAACCCTGTCCGATTTCAACAAAACGCTGGTCCTTTCCGGCAATCAGGCGGGACTGACGGCAGATCGTA
+TGCTGGTCCTGTCCAGAGCCGGGCAGGCGGCAGGGCTGACGTTTAACCAGACCAGCGAGTCACTCAGCGCACTGGTTAAG
+GCGGGGGTAAGCGGTGAGGCTCAGATTGCGTCCATCAGCCAGAGTGTGGCGCGTTTCTCCTCTGCATCCGGCGTGGAGGT
+GGACAAGGTCGCTGAAGCCTTCGGGAAGCTGACCACAGACCCGACGTCGGGGCTGACGGCGATGGCTCGCCAGTTCCATA
+ACGTGTCGGCGGAGCAGATTGCGTATGTTGCTCAGTTGCAGCGTTCCGGCGATGAAGCCGGGGCATTGCAGGCGGCGAAC
+GAGGCCGCAACGAAAGGGTTTGATGACCAGACCCGCCGCCTGAAAGAGAACATGGGCACGCTGGAGACCTGGGCAGACAG
+GACTGCGCGGGCATTCAAATCCATGTGGGATGCGGTGCTGGATATTGGTCGTCCTGATACCGCGCAGGAGATGCTGATTA
+AGGCAGAGGCTGCGTATAAGAAAGCAGACGACATCTGGAATCTGCGCAAGGATGATTATTTTGTTAACGATGAAGCGCGG
+GCGCGTTACTGGGATGATCGTGAAAAGGCCCGTCTTGCGCTTGAAGCCGCCCGAAAGAAGGCTGAGCAGCAGACTCAACA
+GGACAAAAATGCGCAGCAGCAGAGCGATACCGAAGCGTCACGGCTGAAATATACCGAAGAGGCGCAGAAGGCTTACGAAC
+GGCTGCAGACGCCGCTGGAGAAATATACCGCCCGTCAGGAAGAACTGAACAAGGCACTGAAAGACGGGAAAATCCTGCAG
+GCGGATTACAACACGCTGATGGCGGCGGCGAAAAAGGATTATGAAGCGACGCTGAAAAAGCCGAAACAGTCCAGCGTGAA
+GGTGTCTGCGGGCGATCGTCAGGAAGACAGTGCTCATGCTGCCCTGCTGACGCTTCAGGCAGAACTCCGGACGCTGGAGA
+AGCATGCCGGAGCAAATGAGAAAATCAGCCAGCAGCGCCGGGATTTGTGGAAGGCGGAGAGTCAGTTCGCGGTACTGGAG
+GAGGCGGCGCAACGTCGCCAGCTGTCTGCACAGGAGAAATCCCTGCTGGCGCATAAAGATGAGACGCTGGAGTACAAACG
+CCAGCTGGCTGCACTTGGCGACAAGGTTACGTATCAGGAGCGCCTGAACGCGCTGGCGCAGCAGGCGGATAAATTCGCAC
+AGCAGCAACGGGCAAAACGGGCCGCCATTGATGCGAAAAGCCGGGGGCTGACTGACCGGCAGGCAGAACGGGAAGCCACG
+GAACAGCGCCTGAAGGAACAGTATGGCGATAATCCGCTGGCGCTGAATAACGTCATGTCAGAGCAGAAAAAGACCTGGGC
+GGCTGAAGACCAGCTTCGCGGGAACTGGATGGCAGGCCTGAAGTCCGGCTGGAGTGAGTGGGAAGAGAGCGCCACGGACA
+GTATGTCGCAGGTAAAAAGTGCAGCCACGCAGACCTTTGATGGTATTGCACAGAATATGGCGGCGATGCTGACCGGCAGT
+GAGCAGAACTGGCGCAGCTTCACCCGTTCCGTGCTGTCCATGATGACAGAAATTCTGCTTAAGCAGGCAATGGTGGGGAT
+TGTCGGGAGTATCGGCAGCGCCATTGGCGGGGCTGTTGGTGGCGGCGCATCCGCGTCAGGCGGTACAGCCATTCAGGCCG
+CTGCGGCGAAATTCCATTTTGCAACCGGAGGATTTACGGGAACCGGCGGCAAATATGAGCCAGCGGGGATTGTTCACCGT
+GGTGAGTTTGTCTTCACGAAGGAGGCAACCAGCCGGATTGGCGTGGGGAATCTTTACCGGCTGATGCGCGGCTATGCCAC
+CGGCGGTTATGTCGGTACACCGGGCAGCATGGCAGACAGCCGGTCGCAGGCGTCCGGGACGTTTGAGCAGAATAACCATG
+TGGTGATTAACAACGACGGCACGAACGGGCAGATAGGTCCGGCTGCTCTGAAGGCGGTGTATGACATGGCCCGCAAGGGT
+GCCCGTGATGAAATTCAGACACAGATGCGTGATGGTGGCCTGTTCTCCGGAGGTGGACGATGAAGACCTTCCGCTGGAAA
+GTGAAACCCGGTATGGATGTGGCTTCGGTCCCTTCTGTAAGAAAGGTGCGCTTTGGTGATGGCTATTCTCAGCGAGCGCC
+TGCCGGGCTGAATGCCAACCTGAAAACGTACAGCGTGACGCTTTCTGTCCCCCGTGAGGAGGCCACGGTACTGGAGTCGT
+TTCTGGAAGAGCACGGGGGCTGGAAATCCTTTCTGTGGACGCCGCCTTATGAGTGGCGGCAGATAAAGGTGACCTGCGCA
+AAATGGTCGTCGCGGGTCAGTATGCTGCGTGTTGAGTTCAGCGCAGAGTTTGAACAGGTGGTGAACTGATGCAGGATATC
+CGGCAGGAAACACTGAATGAATGCACCCGTGCGGAGCAGTCGGCCAGCGTGGTGCTCTGGGAAATCGACCTGACAGAGGT
+CGGTGGAGAACGTTATTTTTTCTGTAATGAGCAGAACGAAAAAGGTGAGCCGGTCACCTGGCAGGGGCGACAGTATCAGC
+CGTATCCCATTCAGGGGAGCGGTTTTGAACTGAATGGCAAAGGCACCAGTACGCGCCCCACGCTGACGGTTTCTAACCTG
+TACGGTATGGTCACCGGGATGGCGGAAGATATGCAGAGTCTGGTCGGCGGAACGGTGGTCCGGCGTAAGGTTTACGCCCG
+TTTTCTGGATGCGGTGAACTTCGTCAACGGAAACAGTTACGCCGATCCGGAGCAGGAGGTGATCAGCCGCTGGCGCATTG
+AGCAGTGCAGCGAACTGAGCGCGGTGAGTGCCTCCTTTGTACTGTCCACGCCGACGGAAACGGATGGCGCTGTTTTTCCG
+GGACGTATCATGCTGGCCAACACCTGCACCTGGACCTATCGCGGTGACGAGTGCGGTTATAGCGGTCCGGCTGTCGCGGA
+TGAATATGACCAGCCAACGTCCGATATCACGAAGGATAAATGCAGCAAATGCCTGAGCGGTTGTAAGTTCCGCAATAACG
+TCGGCAACTTTGGCGGCTTCCTTTCCATTAACAAACTTTCGCAGTAAATCCCATGACACAGACAGAATCAGCGATTCTGG
+CGCACGCCCGGCGATGTGCGCCAGCGGAGTCGTGCGGCTTCGTGGTAAGCACGCCGGAGGGGGAAAGATATTTCCCCTGC
+GTGAATATCTCCGGTGAGCCGGAGGCTATTTCCGTATGTCGCCGGAAGACTGGCTGCAGGCAGAAATGCAGGGTGAGATT
+GTGGCGCTGGTCCACAGCCACCCCGGTGGTCTGCCCTGGCTGAGTGAGGCCGACCGGCGGCTGCAGGTGCAGAGTGATTT
+GCCGTGGTGGCTGGTCTGCCGGGGGACGATTCATAAGTTCCGCTGTGTGCCGCATCTCACCGGGCGGCGCTTTGAGCACG
+GTGTGACGGACTGTTACACACTGTTCCGGGATGCTTATCATCTGGCGGGGATTGAGATGCCGGACTTTCATCGTGAGGAT
+GACTGGTGGCGTAACGGCCAGAATCTCTATCTGGATAATCTGGAGGCGACGGGGCTGTATCAGGTGCCGTTGTCAGCGGC
+ACAGCCGGGCGATGTGCTGCTGTGCTGTTTTGGTTCATCAGTGCCGAATCACGCCGCAATTTACTGCGGCGACGGCGAGC
+TGCTGCACCATATTCCTGAACAACTGAGCAAACGAGAGAGGTACACCGACAAATGGCAGCGACGCACACACTCCCTCTGG
+CGTCACCGGGCATGGCGCGCATCTGCCTTTACGGGGATTTACAACGATTTGGTCGCCGCATCGACCTTCGTGTGAAAACG
+GGGGCTGAAGCCATCCGGGCACTGGCCACACAGCTCCCGGCGTTTCGTCAGAAACTGAGCGACGGCTGGTATCAGGTACG
+GATTGCCGGGCGGGACGTCAGCACGTCCGGGTTAACGGCGCAGTTACATGAGACTCTGCCTGATGGCGCTGTAATTCATA
+TTGTTCCCAGAGTCGCCGGGGCCAAGTCAGGTGGCGTATTCCAGATTGTCCTGGGGGCTGCCGCCATTGCCGGATCATTC
+TTTACCGCCGGAGCCACCCTTGCAGCATGGGGGGCAGCCATTGGGGCCGGTGGTATGACCGGCATCCTGTTTTCTCTCGG
+TGCCAGTATGGTGCTCGGTGGTGTGGCGCAGATGCTGGCACCGAAAGCCAGAACTCCCCGTATACAGACAACGGATAACG
+GTAAGCAGAACACCTATTTCTCCTCACTGGATAACATGGTTGCCCAGGGCAATGTTCTGCCTGTTCTGTACGGGGAAATG
+CGCGTGGGGTCACGCGTGGTTTCTCAGGAGATCAGCACGGCAGACGAAGGGGACGGTGGTCAGGTTGTGGTGATTGGTCG
+CTGATGCAAAATGTTTTATGTGAAACCGCCTGCGGGCGGTTTTGTCATTTATGGAGCGTGAGGAATGGGTAAAGGAAGCA
+GTAAGGGGCATACCCCGCGCGAAGCGAAGGACAACCTGAAGTCCACGCAGTTGCTGAGTGTGATCGATGCCATCAGCGAA
+GGGCCGATTGAAGGTCCGGTGGATGGCTTAAAAAGCGTGCTGCTGAACAGTACGCCGGTGCTGGACACTGAGGGGAATAC
+CAACATATCCGGTGTCACGGTGGTGTTCCGGGCTGGTGAGCAGGAGCAGACTCCGCCGGAGGGATTTGAATCCTCCGGCT
+CCGAGACGGTGCTGGGTACGGAAGTGAAATATGACACGCCGATCACCCGCACCATTACGTCTGCAAACATCGACCGTCTG
+CGCTTTACCTTCGGTGTACAGGCACTGGTGGAAACCACCTCAAAGGGTGACAGGAATCCGTCGGAAGTCCGCCTGCTGGT
+TCAGATACAACGTAACGGTGGCTGGGTGACGGAAAAAGACATCACCATTAAGGGCAAAACCACCTCGCAGTATCTGGCCT
+CGGTGGTGATGGGTAACCTGCCGCCGCGCCCGTTTAATATCCGGATGCGCAGGATGACGCCGGACAGCACCACAGACCAG
+CTGCAGAACAAAACGCTCTGGTCGTCATACACTGAAATCATCGATGTGAAACAGTGCTACCCGAACACGGCACTGGTCGG
+CGTGCAGGTGGACTCGGAGCAGTTCGGCAGCCAGCAGGTGAGCCGTAATTATCATCTGCGCGGGCGTATTCTGCAGGTGC
+CGTCGAACTATAACCCGCAGACGCGGCAATACAGCGGTATCTGGGACGGAACGTTTAAACCGGCATACAGCAACAACATG
+GCCTGGTGTCTGTGGGATATGCTGACCCATCCGCGCTACGGCATGGGGAAACGTCTTGGTGCGGCGGATGTGGATAAATG
+GGCGCTGTATGTCATCGGCCAGTACTGCGACCAGTCAGTGCCGGACGGCTTTGGCGGCACGGAGCCGCGCATCACCTGTA
+ATGCGTACCTGACCACACAGCGTAAGGCGTGGGATGTGCTCAGCGATTTCTGCTCGGCGATGCGCTGTATGCCGGTATGG
+AACGGGCAGACGCTGACGTTCGTGCAGGACCGACCGTCGGATAAGACGTGGACCTATAACCGCAGTAATGTGGTGATGCC
+GGATGATGGCGCGCCGTTCCGCTACAGCTTCAGCGCCCTGAAGGACCGCCATAATGCCGTTGAGGTGAACTGGATTGACC
+CGAACAACGGCTGGGAGACGGCGACAGAGCTTGTTGAAGATACGCAGGCCATTGCCCGTTACGGTCGTAATGTTACGAAG
+ATGGATGCCTTTGGCTGTACCAGCCGGGGGCAGGCACACCGCGCCGGGCTGTGGCTGATTAAAACAGAACTGCTGGAAAC
+GCAGACCGTGGATTTCAGCGTCGGCGCAGAAGGGCTTCGCCATGTACCGGGCGATGTTATTGAAATCTGCGATGATGACT
+ATGCCGGTATCAGCACCGGTGGTCGTGTGCTGGCGGTGAACAGCCAGACCCGGACGCTGACGCTCGACCGTGAAATCACG
+CTGCCATCCTCCGGTACCGCGCTGATAAGCCTGGTTGACGGAAGTGGCAATCCGGTCAGCGTGGAGGTTCAGTCCGTCAC
+CGACGGCGTGAAGGTAAAAGTGAGCCGTGTTCCTGACGGTGTTGCTGAATACAGCGTATGGGAGCTGAAGCTGCCGACGC
+TGCGCCAGCGACTGTTCCGCTGCGTGAGTATCCGTGAGAACGACGACGGCACGTATGCCATCACCGCCGTGCAGCATGTG
+CCGGAAAAAGAGGCCATCGTGGATAACGGGGCGCACTTTGACGGCGAACAGAGTGGCACGGTGAATGGTGTCACGCCGCC
+AGCGGTGCAGCACCTGACCGCAGAAGTCACTGCAGACAGCGGGGAATATCAGGTGCTGGCGCGATGGGACACACCGAAGG
+TGGTGAAGGGCGTGAGTTTCCTGCTCCGTCTGACCGTAACAGCGGACGACGGCAGTGAGCGGCTGGTCAGCACGGCCCGG
+ACGACGGAAACCACATACCGCTTCACGCAACTGGCGCTGGGGAACTACAGGCTGACAGTCCGGGCGGTAAATGCGTGGGG
+GCAGCAGGGCGATCCGGCGTCGGTATCGTTCCGGATTGCCGCACCGGCAGCACCGTCGAGGATTGAGCTGACGCCGGGCT
+ATTTTCAGATAACCGCCACGCCGCATCTTGCCGTTTATGACCCGACGGTACAGTTTGAGTTCTGGTTCTCGGAAAAGCAG
+ATTGCGGATATCAGACAGGTTGAAACCAGCACGCGTTATCTTGGTACGGCGCTGTACTGGATAGCCGCCAGTATCAATAT
+CAAACCGGGCCATGATTATTACTTTTATATCCGCAGTGTGAACACCGTTGGCAAATCGGCATTCGTGGAGGCCGTCGGTC
+GGGCGAGCGATGATGCGGAAGGTTACCTGGATTTTTTCAAAGGCAAGATAACCGAATCCCATCTCGGCAAGGAGCTGCTG
+GAAAAAGTCGAGCTGACGGAGGATAACGCCAGCAGACTGGAGGAGTTTTCGAAAGAGTGGAAGGATGCCAGTGATAAGTG
+GAATGCCATGTGGGCTGTCAAAATTGAGCAGACCAAAGACGGCAAACATTATGTCGCGGGTATTGGCCTCAGCATGGAGG
+ACACGGAGGAAGGCAAACTGAGCCAGTTTCTGGTTGCCGCCAATCGTATCGCATTTATTGACCCGGCAAACGGGAATGAA
+ACGCCGATGTTTGTGGCGCAGGGCAACCAGATATTCATGAACGACGTGTTCCTGAAGCGCCTGACGGCCCCCACCATTAC
+CAGCGGCGGCAATCCTCCGGCCTTTTCCCTGACACCGGACGGAAAGCTGACCGCTAAAAATGCGGATATCAGTGGCAGTG
+TGAATGCGAACTCCGGGACGCTCAGTAATGTGACGATAGCTGAAAACTGTACGATAAACGGTACGCTGAGGGCGGAAAAA
+ATCGTCGGGGACATTGTAAAGGCGGCGAGCGCGGCTTTTCCGCGCCAGCGTGAAAGCAGTGTGGACTGGCCGTCAGGTAC
+CCGTACTGTCACCGTGACCGATGACCATCCTTTTGATCGCCAGATAGTGGTGCTTCCGCTGACGTTTCGCGGAAGTAAGC
+GTACTGTCAGCGGCAGGACAACGTATTCGATGTGTTATCTGAAAGTACTGATGAACGGTGCGGTGATTTATGATGGCGCG
+GCGAACGAGGCGGTACAGGTGTTCTCCCGTATTGTTGACATGCCAGCGGGTCGGGGAAACGTGATCCTGACGTTCACGCT
+TACGTCCACACGGCATTCGGCAGATATTCCGCCGTATACGTTTGCCAGCGATGTGCAGGTTATGGTGATTAAGAAACAGG
+CGCTGGGCATCAGCGTGGTCTGAGTGTGTTACAGAGGTTCGTCCGGGAACGGGCGTTTTATTATAAAACAGTGAGAGGTG
+AACGATGCGTAATGTGTGTATTGCCGTTGCTGTCTTTGCCGCACTTGCGGTGACAGTCACTCCGGCCCGTGCGGAAGGTG
+GACATGGTACGTTTACGGTGGGCTATTTTCAAGTGAAACCGGGTACATTGCCGTCGTTGTCGGGCGGGGATACCGGTGTG
+AGTCATCTGAAAGGGATTAACGTGAAGTACCGTTATGAGCTGACGGACAGTGTGGGGGTGATGGCTTCCCTGGGGTTCGC
+CGCGTCGAAAAAGAGCAGCACAGTGATGACCGGGGAGGATACGTTTCACTATGAGAGCCTGCGTGGACGTTATGTGAGCG
+TGATGGCCGGACCGGTTTTACAAATCAGTAAGCAGGTCAGTGCGTACGCCATGGCCGGAGTGGCTCACAGTCGGTGGTCC
+GGCAGTACAATGGATTACCGTAAGACGGAAATCACTCCCGGGTATATGAAAGAGACGACCACTGCCAGGGACGAAAGTGC
+AATGCGGCATACCTCAGTGGCGTGGAGTGCAGGTATACAGATTAATCCGGCAGCGTCCGTCGTTGTTGATATTGCTTATG
+AAGGCTCCGGCAGTGGCGACTGGCGTACTGACGGATTCATCGTTGGGGTCGGTTATAAATTCTGATTAGCCAGGTAACAC
+AGTGTTATGACAGCCCGCCGGAACCGGTGGGCTTTTTTGTGGGGTGAATATGGCAGTAAAGATTTCAGGAGTCCTGAAAG
+ACGGCACAGGAAAACCGGTACAGAACTGCACCATTCAGCTGAAAGCCAGACGTAACAGCACCACGGTGGTGGTGAACACG
+GTGGGCTCAGAGAATCCGGATGAAGCCGGGCGTTACAGCATGGATGTGGAGTACGGTCAGTACAGTGTCATCCTGCAGGT
+TGACGGTTTTCCACCATCGCACGCCGGGACCATCACCGTGTATGAAGATTCACAACCGGGGACGCTGAATGATTTTCTCT
+GTGCCATGACGGAGGATGATGCCCGGCCGGAGGTGCTGCGTCGTCTTGAACTGATGGTGGAAGAGGTGGCGCGTAACGCG
+TCCGTGGTGGCACAGAGTACGGCAGACGCGAAGAAATCAGCCGGCGATGCCAGTGCATCAGCTGCTCAGGTCGCGGCCCT
+TGTGACTGATGCAACTGACTCAGCACGCGCCGCCAGCACGTCCGCCGGACAGGCTGCATCGTCAGCTCAGGAAGCGTCCT
+CCGGCGCAGAAGCGGCATCAGCAAAGGCCACTGAAGCGGAAAAAAGTGCCGCAGCCGCAGAGTCCTCAAAAAACGCGGCG
+GCCACCAGTGCCGGTGCGGCGAAAACGTCAGAAACGAATGCTGCAGCGTCACAACAATCAGCCGCCACGTCTGCCTCCAC
+CGCGGCCACGAAAGCGTCAGAGGCCGCCACTTCAGCACGAGATGCGGTGGCCTCAAAAGAGGCAGCAAAATCATCAGAAA
+CGAACGCATCATCAAGTGCCGGTCGTGCAGCTTCCTCGGCAACGGCGGCAGAAAATTCTGCCAGGGCGGCAAAAACGTCC
+GAGACGAATGCCAGGTCATCTGAAACAGCAGCGGAACGGAGCGCCTCTGCCGCGGCAGACGCAAAAACAGCGGCGGCGGG
+GAGTGCGTCAACGGCATCCACGAAGGCGACAGAGGCTGCGGGAAGTGCGGTATCAGCATCGCAGAGCAAAAGTGCGGCAG
+AAGCGGCGGCAATACGTGCAAAAAATTCGGCAAAACGTGCAGAAGATATAGCTTCAGCTGTCGCGCTTGAGGATGCGGAC
+ACAACGAGAAAGGGGATAGTGCAGCTCAGCAGTGCAACCAACAGCACGTCTGAAACGCTTGCTGCAACGCCAAAGGCGGT
+TAAGGTGGTAATGGATGAAACGAACAGAAAAGCCCACTGGACAGTCCGGCACTGACCGGAACGCCAACAGCACCAACCGC
+GCTCAGGGGAACAAACAATACCCAGATTGCGAACACCGCTTTTGTACTGGCCGCGATTGCAGATGTTATCGACGCGTCAC
+CTGACGCACTGAATACGCTGAATGAACTGGCCGCAGCGCTCGGGAATGATCCAGATTTTGCTACCACCATGACTAACGCG
+CTTGCGGGTAAACAACCGAAGAATGCGACACTGACGGCGCTGGCAGGGCTTTCCACGGCGAAAAATAAATTACCGTATTT
+TGCGGAAAATGATGCCGCCAGCCTGACTGAACTGACTCAGGTTGGCAGGGATATTCTGGCAAAAAATTCCGTTGCAGATG
+TTCTTGAATACCTTGGGGCCGGTGAGAATTCGGCCTTTCCGGCAGGTGCGCCGATCCCGTGGCCATCAGATATCGTTCCG
+TCTGGCTACGTCCTGATGCAGGGGCAGGCGTTTGACAAATCAGCCTACCCAAAACTTGCTGTCGCGTATCCATCGGGTGT
+GCTTCCTGATATGCGAGGCTGGACAATCAAGGGGAAACCCGCCAGCGGTCGTGCTGTATTGTCTCAGGAACAGGATGGAA
+TTAAGTCGCACACCCACAGTGCCAGTGCATCCGGTACGGATTTGGGGACGAAAACCACATCGTCGTTTGATTACGGGACG
+AAAACAACAGGCAGTTTCGATTACGGCACCAAATCGACGAATAACACGGGGGCTCATGCTCACAGTCTGAGCGGTTCAAC
+AGGGGCCGCGGGTGCTCATGCCCACACAAGTGGTTTAAGGATGAACAGTTCTGGCTGGAGTCAGTATGGAACAGCAACCA
+TTACAGGAAGTTTATCCACAGTTAAAGGAACCAGCACACAGGGTATTGCTTATTTATCGAAAACGGACAGTCAGGGCAGC
+CACAGTCACTCATTGTCCGGTACAGCCGTGAGTGCCGGTGCACATGCGCATACAGTTGGTATTGGTGCGCACCAGCATCC
+GGTTGTTATCGGTGCTCATGCCCATTCTTTCAGTATTGGTTCACACGGACACACCATCACCGTTAACGCTGCGGGTAACG
+CGGAAAACACCGTCAAAAACATTGCATTTAACTATATTGTGAGGCTTGCATAATGGCATTCAGAATGAGTGAACAACCAC
+GGACCATAAAAATTTATAATCTGCTGGCCGGAACTAATGAATTTATTGGTGAAGGTGACGCATATATTCCGCCTCATACC
+GGTCTGCCTGCAAACAGTACCGATATTGCACCGCCAGATATTCCGGCTGGCTTTGTGGCTGTTTTCAACAGTGATGAGGC
+ATCGTGGCATCTCGTTGAAGACCATCGGGGTAAAACCGTCTATGACGTGGCTTCCGGCGACGCGTTATTTATTTCTGAAC
+TCGGTCCGTTACCGGAAAATTTTACCTGGTTATCGCCGGGAGGGGAATATCAGAAGTGGAACGGCACAGCCTGGGTGAAG
+GATACGGAAGCAGAAAAACTGTTCCGGATCCGGGAGGCGGAAGAAACAAAAAAAAGCCTGATGCAGGTAGCCAGTGAGCA
+TATTGCGCCGCTTCAGGATGCTGCAGATCTGGAAATTGCAACGAAGGAAGAAACCTCGTTGCTGGAAGCCTGGAAGAAGT
+ATCGGGTGTTGCTGAACCGTGTTGATACATCAACTGCACCTGATATTGAGTGGCCTGCTGTCCCTGTTATGGAGTAATCG
+TTTTGTGATATGCCGCAGAAACGTTGTATGAAATAACGTTCTGCGGTTAGTTAGTATATTGTAAAGCTGAGTATTGGTTT
+ATTTGGCGATTATTATCTTCAGGAGAATAATGGAAGTTCTATGACTCAATTGTTCATAGTGTTTACATCACCGCCAATTG
+CTTTTAAGACTGAACGCATGAAATATGGTTTTTCGTCATGTTTTGAGTCTGCTGTTGATATTTCTAAAGTCGGTTTTTTT
+TCTTCGTTTTCTCTAACTATTTTCCATGAAATACATTTTTGATTATTATTTGAATCAATTCCAATTACCTGAAGTCTTTC
+ATCTATAATTGGCATTGTATGTATTGGTTTATTGGAGTAGATGCTTGCTTTTCTGAGCCATAGCTCTGATATCCAAATGA
+AGCCATAGGCATTTGTTATTTTGGCTCTGTCAGCTGCATAACGCCAAAAAATATATTTATCTGCTTGATCTTCAAATGTT
+GTATTGATTAAATCAATTGGATGGAATTGTTTATCATAAAAAATTAATGTTTGAATGTGATAACCGTCCTTTAAAAAAGT
+CGTTTCTGCAAGCTTGGCTGTATAGTCAACTAACTCTTCTGTCGAAGTGATATTTTTAGGCTTATCTACCAGTTTTAGAC
+GCTCTTTAATATCTTCAGGAATTATTTTATTGTCATATTGTATCATGCTAAATGACAATTTGCTTATGGAGTAATCTTTT
+AATTTTAAATAAGTTATTCTCCTGGCTTCATCAAATAAAGAGTCGAATGATGTTGGCGAAATCACATCGTCACCCATTGG
+ATTGTTTATTTGTATGCCAAGAGAGTTACAGCAGTTATACATTCTGCCATAGATTATAGCTAAGGCATGTAATAATTCGT
+AATCTTTTAGCGTATTAGCGACCCATCGTCTTTCTGATTTAATAATAGATGATTCAGTTAAATATGAAGGTAATTTCTTT
+TGTGCAAGTCTGACTAACTTTTTTATACCAATGTTTAACATACTTTCATTTGTAATAAACTCAATGTCATTTTCTTCAAT
+GTAAGATGAAATAAGAGTAGCCTTTGCCTCGCTATACATTTCTAAATCGCCTTGTTTTTCTATCGTATTGCGAGAATTTT
+TAGCCCAAGCCATTAATGGATCATTTTTCCATTTTTCAATAACATTATTGTTATACCAAATGTCATATCCTATAATCTGG
+TTTTTGTTTTTTTGAATAATAAATGTTACTGTTCTTGCGGTTTGGAGGAATTGATTCAAATTCAAGCGAAATAATTCAGG
+GTCAAAATATGTATCAATGCAGCATTTGAGCAAGTGCGATAAATCTTTAAGTCTTCTTTCCCATGGTTTTTTAGTCATAA
+AACTCTCCATTTTGATAGGTTGCATGCTAGATGCTGATATATTTTAGAGGTGATAAAATTAACTGCTTAACTGTCAATGT
+AATACAAGTTGTTTGATCTTTGCAATGATTCTTATCAGAAACCATATAGTAAATTAGTTACACAGGAAATTTTTAATATT
+ATTATTATCATTCATTATGTATTAAAATTAGAGTTGTGGCTTGGCTCTGCTAACACGTTGCTCATAGGAGATATGGTAGA
+GCCGCAGACACGTCGTATGCAGGAACGTGCTGCGGCTGGCTGGTGAACTTCCGATAGTGCGGGTGTTGAATGATTTCCAG
+TTGCTACCGATTTTACATATTTTTTGCATGAGAGAATTTGTACCACCTCCCACCGACCATCTATGACTGTACGCCACTGT
+CCCTAGGACTGCTATGTGCCGGAGCGGACATTACAAACGTCCTTCTCGGTGCATGCCACTGTTGCCAATGACCTGCCTAG
+GAATTGGTTAGCAAGTTACTACCGGATTTTGTAAAAACAGCCCTCCTCATATAAAAAGTATTCGTTCACTTCCGATAAGC
+GTCGTAATTTTCTATCTTTCATCATATTCTAGATCCCTCTGAAAAAATCTTCCGAGTTTGCTAGGCACTGATACATAACT
+CTTTTCCAATAATTGGGGAAGTCATTCAAATCTATAATAGGTTTCAGATTTGCTTCAATAAATTCTGACTGTAGCTGCTG
+AAACGTTGCGGTTGAACTATATTTCCTTATAACTTTTACGAAAGAGTTTCTTTGAGTAATCACTTCACTCAAGTGCTTCC
+CTGCCTCCAAACGATACCTGTTAGCAATATTTAATAGCTTGAAATGATGAAGAGCTCTGTGTTTGTCTTCCTGCCTCCAG
+TTCGCCGGGCATTCAACATAAAAACTGATAGCACCCGGAGTTCCGGAAACGAAATTTGCATATACCCATTGCTCACGAAA
+AAAAATGTCCTTGTCGATATAGGGATGAATCGCTTGGTGTACCTCATCTACTGCGAAAACTTGACCTTTCTCTCCCATAT
+TGCAGTCGCGGCACGATGGAACTAAATTAATAGGCATCACCGAAAATTCAGGATAATGTGCAATAGGAAGAAAATGATCT
+ATATTTTTTGTCTGTCCTATATCACCACAAAATGGACATTTTTCACCTGATGAAACAAGCATGTCATCGTAATATGTTCT
+AGCGGGTTTGTTTTTATCTCGGAGATTATTTTCATAAAGCTTTTCTAATTTAACCTTTGTCAGGTTACCAACTACTAAGG
+TTGTAGGCTCAAGAGGGTGTGTCCTGTCGTAGGTAAATAACTGACCTGTCGAGCTTAATATTCTATATTGTTGTTCTTTC
+TGCAAAAAAGTGGGGAAGTGAGTAATGAAATTATTTCTAACATTTATCTGCATCATACCTTCCGAGCATTTATTAAGCAT
+TTCGCTATAAGTTCTCGCTGGAAGAGGTAGTTTTTTCATTGTACTTTACCTTCATCTCTGTTCATTATCATCGCTTTTAA
+AACGGTTCGACCTTCTAATCCTATCTGACCATTATAATTTTTTAGAATGGTTTCATAAGAAAGCTCTGAATCAACGGACT
+GCGATAATAAGTGGTGGTATCCAGAATTTGTCACTTCAAGTAAAAACACCTCACGAGTTAAAACACCTAAGTTCTCACCG
+AATGTCTCAATATCCGGACGGATAATATTTATTGCTTCTCTTGACCGTAGGACTTTCCACATGCAGGATTTTGGAACCTC
+TTGCAGTACTACTGGGGAATGAGTTGCAATTATTGCTACACCATTGCGTGCATCGAGTAAGTCGCTTAATGTTCGTAAAA
+AAGCAGAGAGCAAAGGTGGATGCAGATGAACCTCTGGTTCATCGAATAAAACTAATGACTTTTCGCCAACGACATCTACT
+AATCTTGTGATAGTAAATAAAACAATTGCATGTCCAGAGCTCATTCGAAGCAGATATTTCTGGATATTGTCATAAAACAA
+TTTAGTGAATTTATCATCGTCCACTTGAATCTGTGGTTCATTACGTCTTAACTCTTCATATTTAGAAATGAGGCTGATGA
+GTTCCATATTTGAAAAGTTTTCATCACTACTTAGTTTTTTGATAGCTTCAAGCCAGAGTTGTCTTTTTCTATCTACTCTC
+ATACAACCAATAAATGCTGAAATGAATTCTAAGCGGAGATCGCCTAGTGATTTTAAACTATTGCTGGCAGCATTCTTGAG
+TCCAATATAAAAGTATTGTGTACCTTTTGCTGGGTCAGGTTGTTCTTTAGGAGGAGTAAAAGGATCAAATGCACTAAACG
+AAACTGAAACAAGCGATCGAAAATATCCCTTTGGGATTCTTGACTCGATAAGTCTATTATTTTCAGAGAAAAAATATTCA
+TTGTTTTCTGGGTTGGTGATTGCACCAATCATTCCATTCAAAATTGTTGTTTTACCACACCCATTCCGCCCGATAAAAGC
+ATGAATGTTCGTGCTGGGCATAGAATTAACCGTCACCTCAAAAGGTATAGTTAAATCACTGAATCCGGGAGCACTTTTTC
+TATTAAATGAAAAGTGGAAATCTGACAATTCTGGCAAACCATTTAACACACGTGCGAACTGTCCATGAATTTCTGAAAGA
+GTTACCCCTCTAAGTAATGAGGTGTTAAGGACGCTTTCATTTTCAATGTCGGCTAATCGATTTGGCCATACTACTAAATC
+CTGAATAGCTTTAAGAAGGTTATGTTTAAAACCATCGCTTAATTTGCTGAGATTAACATAGTAGTCAATGCTTTCACCTA
+AGGAAAAAAACATTTCAGGGAGTTGACTGAATTTTTTATCTATTAATGAATAAGTGCTTACTTCTTCTTTTTGACCTACA
+AAACCAATTTTAACATTTCCGATATCGCATTTTTCACCATGCTCATCAAAGACAGTAAGATAAAACATTGTAACAAAGGA
+ATAGTCATTCCAACCATCTGCTCGTAGGAATGCCTTATTTTTTTCTACTGCAGGAATATACCCGCCTCTTTCAATAACAC
+TAAACTCCAACATATAGTAACCCTTAATTTTATTAAAATAACCGCAATTTATTTGGCGGCAACACAGGATCTCTCTTTTA
+AGTTACTCTCTATTACATACGTTTTCCATCTAAAAATTAGTAGTATTGAACTTAACGGGGCATCGTATTGTAGTTTTCCA
+TATTTAGCTTTCTGCTTCCTTTTGGATAACCCACTGTTATTCATGTTGCATGGTGCACTGTTTATACCAACGATATAGTC
+TATTAATGCATATATAGTATCGCCGAACGATTAGCTCTTCAGGCTTCTGAAGAAGCGTTTCAAGTACTAATAAGCCGATA
+GATAGCCACGGACTTCGTAGCCATTTTTCATAAGTGTTAACTTCCGCTCCTCGCTCATAACAGACATTCACTACAGTTAT
+GGCGGAAAGGTATGCATGCTGGGTGTGGGGAAGTCGTGAAAGAAAAGAAGTCAGCTGCGTCGTTTGACATCACTGCTATC
+TTCTTACTGGTTATGCAGGTCGTAGTGGGTGGCACACAAAGCTTTGCACTGGATTGCGAGGCTTTGTGCTTCTCTGGAGT
+GCGACAGGTTTGATGACAAAAAATTAGCGCAAGAAGACAAAAATCACCTTGCGCTAATGCTCTGTTACAGGTCACTAATA
+CCATCTAAGTAGTTGATTCATAGTGACTGCATATGTTGTGTTTTACAGTATTATGTAGTCTGTTTTTTATGCAAAATCTA
+ATTTAATATATTGATATTTATATCATTTTACGTTTCTCGTTCAGCTTTTTTATACTAAGTTGGCATTATAAAAAAGCATT
+GCTTATCAATTTGTTGCAACGAACAGGTCACTATCAGTCAAAATAAAATCATTATTTGATTTCAATTTTGTCCCACTCCC
+TGCCTCTGTCATCACGATACTGTGATGCCATGGTGTCCGACTTATGCCCGAGAAGATGTTGAGCAAACTTATCGCTTATC
+TGCTTCTCATAGAGTCTTGCAGACAAACTGCGCAACTCGTGAAAGGTAGGCGGATCCCCTTCGAAGGAAAGACCTGATGC
+TTTTCGTGCGCGCATAAAATACCTTGATACTGTGCCGGATGAAAGCGGTTCGCGACGAGTAGATGCAATTATGGTTTCTC
+CGCCAAGAATCTCTTTGCATTTATCAAGTGTTTCCTTCATTGATATTCCGAGAGCATCAATATGCAATGCTGTTGGGATG
+GCAATTTTTACGCCTGTTTTGCTTTGCTCGACATAAAGATATCCATCTACGATATCAGACCACTTCATTTCGCATAAATC
+ACCAACTCGTTGCCCGGTAACAACAGCCAGTTCCATTGCAAGTCTGAGCCAACATGGTGATGATTCTGCTGCTTGATAAA
+TTTTCAGGTATTCGTCAGCCGTAAGTCTTGATCTCCTTACCTCTGATTTTGCTGCGCGAGTGGCAGCGACATGGTTTGTT
+GTTATATGGCCTTCAGCTATTGCCTCTCGGAATGCATCGCTCAGTGTTGATCTGATTAACTTGGCTGACGCCGCCTTGCC
+CTCGTCTATGTATCCATTGAGCATTGCCGCAATTTCTTTTGTGGTGATGTCTTCAAGTGGAGCATCAGGCAGACCCCTCC
+TTATTGCTTTAATTTTGCTCATGTAATTTATGAGTGTCTTCTGCTTGATTCCTCTGCTGGCCAGGATTTTTTCGTAGCGA
+TCAAGCCATGAATGTAACGTAACGGAATTATCACTGTTGATTCTCGCTGTCAGAGGCTTGTGTTTGTGTCCTGAAAATAA
+CTCAATGTTGGCCTGTATAGCTTCAGTGATTGCGATTCGCCTGTCTCTGCCTAATCCAAACTCTTTACCCGTCCTTGGGT
+CCCTGTAGCAGTAATATCCATTGTTTCTTATATAAAGGTTAGGGGGTAAATCCCGGCGCTCATGACTTCGCCTTCTTCCC
+ATTTCTGATCCTCTTCAAAAGGCCACCTGTTACTGGTCGATTTAAGTCAACCTTTACCGCTGATTCGTGGAACAGATACT
+CTCTTCCATCCTTAACCGGAGGTGGGAATATCCTGCATTCCCGAACCCATCGACGAACTGTTTCAAGGCTTCTTGGACGT
+CGCTGGCGTGCGTTCCACTCCTGAAGTGTCAAGTACATCGCAAAGTCTCCGCAATTACACGCAAGAAAAAACCGCCATCA
+GGCGGCTTGGTGTTCTTTCAGTTCTTCAATTCGAATATTGGTTACGTCTGCATGTGCTATCTGCGCCCATATCATCCAGT
+GGTCGTAGCAGTCGTTGATGTTCTCCGCTTCGATAACTCTGTTGAATGGCTCTCCATTCCATTCTCCTGTGACTCGGAAG
+TGCATTTATCATCTCCATAAAACAAAACCCGCCGTAGCGAGTTCAGATAAAATAAATCCCCGCGAGTGCGAGGATTGTTA
+TGTAATATTGGGTTTAATCATCTATATGTTTTGTACAGAGAGGGCAAGTATCGTTTCCACCGTACTCGTGATAATAATTT
+TGCACGGTATCAGTCATTTCTCGCACATTGCAGAATGGGGATTTGTCTTCATTAGACTTATAAACCTTCATGGAATATTT
+GTATGCCGACTCTATATCTATACCTTCATCTACATAAACACCTTCGTGATGTCTGCATGGAGACAAGACACCGGATCTGC
+ACAACATTGATAACGCCCAATCTTTTTGCTCAGACTCTAACTCATTGATACTCATTTATAAACTCCTTGCAATGTATGTC
+GTTTCAGCTAAACGGTATCAGCAATGTTTATGTAAAGAAACAGTAAGATAATACTCAACCCGATGTTTGAGTACGGTCAT
+CATCTGACACTACAGACTCTGGCATCGCTGTGAAGACGACGCGAAATTCAGCATTTTCACAAGCGTTATCTTTTACAAAA
+CCGATCTCACTCTCCTTTGATGCGAATGCCAGCGTCAGACATCATATGCAGATACTCACCTGCATCCTGAACCCATTGAC
+CTCCAACCCCGTAATAGCGATGCGTAATGATGTCGATAGTTACTAACGGGTCTTGTTCGATTAACTGCCGCAGAAACTCT
+TCCAGGTCACCAGTGCAGTGCTTGATAACAGGAGTCTTCCCAGGATGGCGAACAACAAGAAACTGGTTTCCGTCTTCACG
+GACTTCGTTGCTTTCCAGTTTAGCAATACGCTTACTCCCATCCGAGATAACACCTTCGTAATACTCACGCTGCTCGTTGA
+GTTTTGATTTTGCTGTTTCAAGCTCAACACGCAGTTTCCCTACTGTTAGCGCAATATCCTCGTTCTCCTGGTCGCGGCGT
+TTGATGTATTGCTGGTTTCTTTCCCGTTCATCCAGCAGTTCCAGCACAATCGATGGTGTTACCAATTCATGGAAAAGGTC
+TGCGTCAAATCCCCAGTCGTCATGCATTGCCTGCTCTGCCGCTTCACGCAGTGCCTGAGAGTTAATTTCGCTCACTTCGA
+ACCTCTCTGTTTACTGATAAGTTCCAGATCCTCCTGGCAACTTGCACAAGTCCGACAACCCTGAACGACCAGGCGTCTTC
+GTTCATCTATCGGATCGCCACACTCACAACAATGAGTGGCAGATATAGCCTGGTGGTTCAGGCGGCGCATTTTTATTGCT
+GTGTTGCGCTGTAATTCTTCTATTTCTGATGCTGAATCAATGATGTCTGCCATCTTTCATTAATCCCTGAACTGTTGGTT
+AATACGCTTGAGGGTGAATGCGAATAATAAAAAAGGAGCCTGTAGCTCCCTGATGATTTTGCTTTTCATGTTCATCGTTC
+CTTAAAGACGCCGTTTAACATGCCGATTGCCAGGCTTAAATGAGTCGGTGTGAATCCCATCAGCGTTACCGTTTCGCGGT
+GCTTCTTCAGTACGCTACGGCAAATGTCATCGACGTTTTTATCCGGAAACTGCTGTCTGGCTTTTTTTGATTTCAGAATT
+AGCCTGACGGGCAATGCTGCGAAGGGCGTTTTCCTGCTGAGGTGTCATTGAACAAGTCCCATGTCGGCAAGCATAAGCAC
+ACAGAATATGAAGCCCGCTGCCAGAAAAATGCATTCCGTGGTTGTCATACCTGGTTTCTCTCATCTGCTTCTGCTTTCGC
+CACCATCATTTCCAGCTTTTGTGAAAGGGATGCGGCTAACGTATGAAATTCTTCGTCTGTTTCTACTGGTATTGGCACAA
+ACCTGATTCCAATTTGAGCAAGGCTATGTGCCATCTCGATACTCGTTCTTAACTCAACAGAAGATGCTTTGTGCATACAG
+CCCCTCGTTTATTATTTATCTCCTCAGCCAGCCGCTGTGCTTTCAGTGGATTTCGGATAACAGAAAGGCCGGGAAATACC
+CAGCCTCGCTTTGTAACGGAGTAGACGAAAGTGATTGCGCCTACCCGGATATTATCGTGAGGATGCGTCATCGCCATTGC
+TCCCCAAATACAAAACCAATTTCAGCCAGTGCCTCGTCCATTTTTTCGATGAACTCCGGCACGATCTCGTCAAAACTCGC
+CATGTACTTTTCATCCCGCTCAATCACGACATAATGCAGGCCTTCACGCTTCATACGCGGGTCATAGTTGGCAAAGTACC
+AGGCATTTTTTCGCGTCACCCACATGCTGTACTGCACCTGGGCCATGTAAGCTGACTTTATGGCCTCGAAACCACCGAGC
+CGGAACTTCATGAAATCCCGGGAGGTAAACGGGCATTTCAGTTCAAGGCCGTTGCCGTCACTGCATAAACCATCGGGAGA
+GCAGGCGGTACGCATACTTTCGTCGCGATAGATGATCGGGGATTCAGTAACATTCACGCCGGAAGTGAATTCAAACAGGG
+TTCTGGCGTCGTTCTCGTACTGTTTTCCCCAGGCCAGTGCTTTAGCGTTAACTTCCGGAGCCACACCGGTGCAAACCTCA
+GCAAGCAGGGTGTGGAAGTAGGACATTTTCATGTCAGGCCACTTCTTTCCGGAGCGGGGTTTTGCTATCACGTTGTGAAC
+TTCTGAAGCGGTGATGACGCCGAGCCGTAATTTGTGCCACGCATCATCCCCCTGTTCGACAGCTCTCACATCGATCCCGG
+TACGCTGCAGGATAATGTCCGGTGTCATGCTGCCACCTTCTGCTCTGCGGCTTTCTGTTTCAGGAATCCAAGAGCTTTTA
+CTGCTTCGGCCTGTGTCAGTTCTGACGATGCACGAATGTCGCGGCGAAATATCTGGGAACAGAGCGGCAATAAGTCGTCA
+TCCCATGTTTTATCCAGGGCGATCAGCAGAGTGTTAATCTCCTGCATGGTTTCATCGTTAACCGGAGTGATGTCGCGTTC
+CGGCTGACGTTCTGCAGTGTATGCAGTATTTTCGACAATGCGCTCGGCTTCATCCTTGTCATAGATACCAGCAAATCCGA
+AGGCCAGACGGGCACACTGAATCATGGCTTTATGACGTAACATCCGTTTGGGATGCGACTGCCACGGCCCCGTGATTTCT
+CTGCCTTCGCGAGTTTTGAATGGTTCGCGGCGGCATTCATCCATCCATTCGGTAACGCAGATCGGATGATTACGGTCCTT
+GCGGTAAATCCGGCATGTACAGGATTCATTGTCCTGCTCAAAGTCCATGCCATCAAACTGCTGGTTTTCATTGATGATGC
+GGGACCAGCCATCAACGCCCACCACCGGAACGATGCCATTCTGCTTATCAGGAAAGGCGTAAATTTCTTTCGTCCACGGA
+TTAAGGCCGTACTGGTTGGCAACGATCAGTAATGCGATGAACTGCGCATCGCTGGCATCACCTTTAAATGCCGTCTGGCG
+AAGAGTGGTGATCAGTTCCTGTGGGTCGACAGAATCCATGCCGACACGTTCAGCCAGCTTCCCAGCCAGCGTTGCGAGTG
+CAGTACTCATTCGTTTTATACCTCTGAATCAATATCAACCTGGTGGTGAGCAATGGTTTCAACCATGTACCGGATGTGTT
+CTGCCATGCGCTCCTGAAACTCAACATCGTCATCAAACGCACGGGTAATGGATTTTTTGCTGGCCCCGTGGCGTTGCAAA
+TGATCGATGCATAGCGATTCAAACAGGTGCTGGGGCAGGCCTTTTTCCATGTCGTCTGCCAGTTCTGCCTCTTTCTCTTC
+ACGGGCGAGCTGCTGGTAGTGACGCGCCCAGCTCTGAGCCTCAAGACGATCCTGAATGTAATAAGCGTTCATGGCTGAAC
+TCCTGAAATAGCTGTGAAAATATCGCCCGCGAAATGCCGGGCTGATTAGGAAAACAGGAAAGGGGGTTAGTGAATGCTTT
+TGCTTGATCTCAGTTTCAGTATTAATATCCATTTTTTATAAGCGTCGACGGCTTCACGAAACATCTTTTCATCGCCAATA
+AAAGTGGCGATAGTGAATTTAGTCTGGATAGCCATAAGTGTTTGATCCATTCTTTGGGACTCCTGGCTGATTAAGTATGT
+CGATAAGGCGTTTCCATCCGTCACGTAATTTACGGGTGATTCGTTCAAGTAAAGATTCGGAAGGGCAGCCAGCAACAGGC
+CACCCTGCAATGGCATATTGCATGGTGTGCTCCTTATTTATACATAACGAAAAACGCCTCGAGTGAAGCGTTATTGGTAT
+GCGGTAAAACCGCACTCAGGCGGCCTTGATAGTCATATCATCTGAATCAAATATTCCTGATGTATCGATATCGGTAATTC
+TTATTCCTTCGCTACCATCCATTGGAGGCCATCCTTCCTGACCATTTCCATCATTCCAGTCGAACTCACACACAACACCA
+TATGCATTTAAGTCGCTTGAAATTGCTATAAGCAGAGCATGTTGCGCCAGCATGATTAATACAGCATTTAATACAGAGCC
+GTGTTTATTGAGTCGGTATTCAGAGTCTGACCAGAAATTATTAATCTGGTGAAGTTTTTCCTCTGTCATTACGTCATGGT
+CGATTTCAATTTCTATTGATGCTTTCCAGTCGTAATCAATGATGTATTTTTTGATGTTTGACATCTGTTCATATCCTCAC
+AGATAAAAAATCGCCCTCACACTGGAGGGCAAAGAAGATTTCCAATAATCAGAACAAGTCGGCTCCTGTTTAGTTACGAG
+CGACATTGCTCCGTGTATTCACTCGTTGGAATGAATACACAGTGCAGTGTTTATTCTGTTATTTATGCCAAAAATAAAGG
+CCACTATCAGGCAGCTTTGTTGTTCTGTTTACCAAGTTCTCTGGCAATCATTGCCGTCGTTCGTATTGCCCATTTATCGA
+CATATTTCCCATCTTCCATTACAGGAAACATTTCTTCAGGCTTAACCATGCATTCCGATTGCAGCTTGCATCCATTGCAT
+CGCTTGAATTGTCCACACCATTGATTTTTATCAATAGTCGTAGTCATACGGATAGTCCTGGTATTGTTCCATCACATCCT
+GAGGATGCTCTTCGAACTCTTCAAATTCTTCTTCCATATATCACCTTAAATAGTGGATTGCGGTAGTAAAGATTGTGCCT
+GTCTTTTAACCACATCAGGCTCGGTGGTTCTCGTGTACCCCTACAGCGAGAAATCGGATAAACTATTACAACCCCTACAG
+TTTGATGAGTATAGAAATGGATCCACTCGTTATTCTCGGACGAGTGTTCAGTAATGAACCTCTGGAGAGAACCATGTATA
+TGATCGTTATCTGGGTTGGACTTCTGCTTTTAAGCCCAGATAACTGGCCTGAATATGTTAATGAGAGAATCGGTATTCCT
+CATGTGTGGCATGTTTTCGTCTTTGCTCTTGCATTTTCGCTAGCAATTAATGTGCATCGATTATCAGCTATTGCCAGCGC
+CAGATATAAGCGATTTAAGCTAAGAAAACGCATTAAGATGCAAAACGATAAAGTGCGATCAGTAATTCAAAACCTTACAG
+AAGAGCAATCTATGGTTTTGTGCGCAGCCCTTAATGAAGGCAGGAAGTATGTGGTTACATCAAAACAATTCCCATACATT
+AGTGAGTTGATTGAGCTTGGTGTGTTGAACAAAACTTTTTCCCGATGGAATGGAAAGCATATATTATTCCCTATTGAGGA
+TATTTACTGGACTGAATTAGTTGCCAGCTATGATCCATATAATATTGAGATAAAGCCAAGGCCAATATCTAAGTAACTAG
+ATAAGAGGAATCGATTTTCCCTTAATTTTCTGGCGTCCACTGCATGTTATGCCGCGTTCGCCAGGCTTGCTGTACCATGT
+GCGCTGATTCTTGCGCTCAATACGTTGCAGGTTGCTTTCAATCTGTTTGTGGTATTCAGCCAGCACTGTAAGGTCTATCG
+GATTTAGTGCGCTTTCTACTCGTGATTTCGGTTTGCGATTCAGCGAGAGAATAGGGCGGTTAACTGGTTTTGCGCTTACC
+CCAACCAACAGGGGATTTGCTGCTTTCCATTGAGCCTGTTTCTCTGCGCGACGTTCGCGGCGGCGTGTTTGTGCATCCAT
+CTGGATTCTCCTGTCAGTTAGCTTTGGTGGTGTGTGGCAGTTGTAGTCCTGAACGAAAACCCCCCGCGATTGGCACATTG
+GCAGCTAATCCGGAATCGCACTTACGGCCAATGCTTCGTTTCGTATCACACACCCCAAAGCCTTCTGCTTTGAATGCTGC
+CCTTCTTCAGGGCTTAATTTTTAAGAGCGTCACCTTCATGGTGGTCAGTGCGTCCTGCTGATGTGCTCAGTATCACCGCC
+AGTGGTATTTATGTCAACACCGCCAGAGATAATTTATCACCGCAGATGGTTATCTGTATGTTTTTTATATGAATTTATTT
+TTTGCAGGGGGGCATTGTTTGGTAGGTGAGAGATCTGAATTGCTATGTTTAGTGAGTTGTATCTATTTATTTTTCAATAA
+ATACAATTGGTTATGTGTTTTGGGGGCGATCGTGAGGCAAAGAAAACCCGGCGCTGAGGCCGGGTTATTCTTGTTCTCTG
+GTCAAATTATATAGTTGGAAAACAAGGATGCATATATGAATGAACGATGCAGAGGCAATGCCGATGGCGATAGTGGGTAT
+CATGTAGCCGCTTATGCTGGAAAGAAGCAATAACCCGCAGAAAAACAAAGCTCCAAGCTCAACAAAACTAAGGGCATAGA
+CAATAACTACCGATGTCATATACCCATACTCTCTAATCTTGGCCAGTCGGCGCGTTCTGCTTCCGATTAGAAACGTCAAG
+GCAGCAATCAGGATTGCAATCATGGTTCCTGCATATGATGACAATGTCGCCCCAAGACCATCTCTATGAGCTGAAAAAGA
+AACACCAGGAATGTAGTGGCGGAAAAGGAGATAGCAAATGCTTACGATAACGTAAGGAATTATTACTATGTAAACACCAG
+GCATGATTCTGTTCCGCATAATTACTCCTGATAATTAATCCTTAACTTTGCCCACCTGCCTTTTAAAACATTCCAGTATA
+TCACTTTTCATTCTTGCGTAGCAATATGCCATCTCTTCAGCTATCTCAGCATTGGTGACCTTGTTCAGAGGCGCTGAGAG
+ATGGCCTTTTTCTGATAGATAATGTTCTGTTAAAATATCTCCGGCCTCATCTTTTGCCCGCAGGCTAATGTCTGAAAATT
+GAGGTGACGGGTTAAAAATAATATCCTTGGCAACCTTTTTTATATCCCTTTTAAATTTTGGCTTAATGACTATATCCAAT
+GAGTCAAAAAGCTCCCCTTCAATATCTGTTGCCCCTAAGACCTTTAATATATCGCCAAATACAGGTAGCTTGGCTTCTAC
+CTTCACCGTTGTTCGGCCGATGAAATGCATATGCATAACATCGTCTTTGGTGGTTCCCCTCATCAGTGGCTCTATCTGAA
+CGCGCTCTCCACTGCTTAATGACATTCCTTTCCCGATTAAAAAATCTGTCAGATCGGATGTGGTCGGCCCGAAAACAGTT
+CTGGCAAAACCAATGGTGTCGCCTTCAACAAACAAAAAAGATGGGAATCCCAATGATTCGTCATCTGCGAGGCTGTTCTT
+AATATCTTCAACTGAAGCTTTAGAGCGATTTATCTTCTGAACCAGACTCTTGTCATTTGTTTTGGTAAAGAGAAAAGTTT
+TTCCATCGATTTTATGAATATACAAATAATTGGAGCCAACCTGCAGGTGATGATTATCAGCCAGCAGAGAATTAAGGAAA
+ACAGACAGGTTTATTGAGCGCTTATCTTTCCCTTTATTTTTGCTGCGGTAAGTCGCATAAAAACCATTCTTCATAATTCA
+ATCCATTTACTATGTTATGTTCTGAGGGGAGTGAAAATTCCCCTAATTCGATGAAGATTCTTGCTCAATTGTTATCAGCT
+ATGCGCCGACCAGAACACCTTGCCGATCAGCCAAACGTCTCTTCAGGCCACTGACTAGCGATAACTTTCCCCACAACGGA
+ACAACTCTCATTGCATGGGATCATTGGGTACTGTGGGTTTAGTGGTTGTAAAAACACCTGACCGCTATCCCTGATCAGTT
+TCTTGAAGGTAAACTCATCACCCCCAAGTCTGGCTATGCAGAAATCACCTGGCTCAACAGCCTGCTCAGGGTCAACGAGA
+ATTAACATTCCGTCAGGAAAGCTTGGCTTGGAGCCTGTTGGTGCGGTCATGGAATTACCTTCAACCTCAAGCCAGAATGC
+AGAATCACTGGCTTTTTTGGTTGTGCTTACCCATCTCTCCGCATCACCTTTGGTAAAGGTTCTAAGCTCAGGTGAGAACA
+TCCCTGCCTGAACATGAGAAAAAACAGGGTACTCATACTCACTTCTAAGTGACGGCTGCATACTAACCGCTTCATACATC
+TCGTAGATTTCTCTGGCGATTGAAGGGCTAAATTCTTCAACGCTAACTTTGAGAATTTTTGCAAGCAATGCGGCGTTATA
+AGCATTTAATGCATTGATGCCATTAAATAAAGCACCAACGCCTGACTGCCCCATCCCCATCTTGTCTGCGACAGATTCCT
+GGGATAAGCCAAGTTCATTTTTCTTTTTTTCATAAATTGCTTTAAGGCGACGTGCGTCCTCAAGCTGCTCTTGTGTTAAT
+GGTTTCTTTTTTGTGCTCATACGTTAAATCTATCACCGCAAGGGATAAATATCTAACACCGTGCGTGTTGACTATTTTAC
+CTCTGGCGGTGATAATGGTTGCATGTACTAAGGAGGTTGTATGGAACAACGCATAACCCTGAAAGATTATGCAATGCGCT
+TTGGGCAAACCAAGACAGCTAAAGATCTCGGCGTATATCAAAGCGCGATCAACAAGGCCATTCATGCAGGCCGAAAGATT
+TTTTTAACTATAAACGCTGATGGAAGCGTTTATGCGGAAGAGGTAAAGCCCTTCCCGAGTAACAAAAAAACAACAGCATA
+AATAACCCCGCTCTTACACATTCCAGCCCTGAAAAAGGGCATCAAATTAAACCACACCTATGGTGTATGCATTTATTTGC
+ATACATTCAATCAATTGTTATCTAAGGAAATACTTACATATGGTTCGTGCAAACAAACGCAACGAGGCTCTACGAATCGA
+GAGTGCGTTGCTTAACAAAATCGCAATGCTTGGAACTGAGAAGACAGCGGAAGCTGTGGGCGTTGATAAGTCGCAGATCA
+GCAGGTGGAAGAGGGACTGGATTCCAAAGTTCTCAATGCTGCTTGCTGTTCTTGAATGGGGGGTCGTTGACGACGACATG
+GCTCGATTGGCGCGACAAGTTGCTGCGATTCTCACCAATAAAAAACGCCCGGCGGCAACCGAGCGTTCTGAACAAATCCA
+GATGGAGTTCTGAGGTCATTACTGGATCTATCAACAGGAGTCATTATGACAAATACAGCAAAAATACTCAACTTCGGCAG
+AGGTAACTTTGCCGGACAGGAGCGTAATGTGGCAGATCTCGATGATGGTTACGCCAGACTATCAAATATGCTGCTTGAGG
+CTTATTCGGGCGCAGATCTGACCAAGCGACAGTTTAAAGTGCTGCTTGCCATTCTGCGTAAAACCTATGGGTGGAATAAA
+CCAATGGACAGAATCACCGATTCTCAACTTAGCGAGATTACAAAGTTACCTGTCAAACGGTGCAATGAAGCCAAGTTAGA
+ACTCGTCAGAATGAATATTATCAAGCAGCAAGGCGGCATGTTTGGACCAAATAAAAACATCTCAGAATGGTGCATCCCTC
+AAAACGAGGGAAAATCCCCTAAAACGAGGGATAAAACATCCCTCAAATTGGGGGATTGCTATCCCTCAAAACAGGGGGAC
+ACAAAAGACACTATTACAAAAGAAAAAAGAAAAGATTATTCGTCAGAGAATTCTGGCGAATCCTCTGACCAGCCAGAAAA
+CGACCTTTCTGTGGTGAAACCGGATGCTGCAATTCAGAGCGGCAGCAAGTGGGGGACAGCAGAAGACCTGACCGCCGCAG
+AGTGGATGTTTGACATGGTGAAGACTATCGCACCATCAGCCAGAAAACCGAATTTTGCTGGGTGGGCTAACGATATCCGC
+CTGATGCGTGAACGTGACGGACGTAACCACCGCGACATGTGTGTGCTGTTCCGCTGGGCATGCCAGGACAACTTCTGGTC
+CGGTAACGTGCTGAGCCCGGCCAAACTCCGCGATAAGTGGACCCAACTCGAAATCAACCGTAACAAGCAACAGGCAGGCG
+TGACAGCCAGCAAACCAAAACTCGACCTGACAAACACAGACTGGATTTACGGGGTGGATCTATGAAAAACATCGCCGCAC
+AGATGGTTAACTTTGACCGTGAGCAGATGCGTCGGATCGCCAACAACATGCCGGAACAGTACGACGAAAAGCCGCAGGTA
+CAGCAGGTAGCGCAGATCATCAACGGTGTGTTCAGCCAGTTACTGGCAACTTTCCCGGCGAGCCTGGCTAACCGTGACCA
+GAACGAAGTGAACGAAATCCGTCGCCAGTGGGTTCTGGCTTTTCGGGAAAACGGGATCACCACGATGGAACAGGTTAACG
+CAGGAATGCGCGTAGCCCGTCGGCAGAATCGACCATTTCTGCCATCACCCGGGCAGTTTGTTGCATGGTGCCGGGAAGAA
+GCATCCGTTACCGCCGGACTGCCAAACGTCAGCGAGCTGGTTGATATGGTTTACGAGTATTGCCGGAAGCGAGGCCTGTA
+TCCGGATGCGGAGTCTTATCCGTGGAAATCAAACGCGCACTACTGGCTGGTTACCAACCTGTATCAGAACATGCGGGCCA
+ATGCGCTTACTGATGCGGAATTACGCCGTAAGGCCGCAGATGAGCTTGTCCATATGACTGCGAGAATTAACCGTGGTGAG
+GCGATCCCTGAACCAGTAAAACAACTTCCTGTCATGGGCGGTAGACCTCTAAATCGTGCACAGGCTCTGGCGAAGATCGC
+AGAAATCAAAGCTAAGTTCGGACTGAAAGGAGCAAGTGTATGACGGGCAAAGAGGCAATTATTCATTACCTGGGGACGCA
+TAATAGCTTCTGTGCGCCGGACGTTGCCGCGCTAACAGGCGCAACAGTAACCAGCATAAATCAGGCCGCGGCTAAAATGG
+CACGGGCAGGTCTTCTGGTTATCGAAGGTAAGGTCTGGCGAACGGTGTATTACCGGTTTGCTACCAGGGAAGAACGGGAA
+GGAAAGATGAGCACGAACCTGGTTTTTAAGGAGTGTCGCCAGAGTGCCGCGATGAAACGGGTATTGGCGGTATATGGAGT
+TAAAAGATGACCATCTACATTACTGAGCTAATAACAGGCCTGCTGGTAATCGCAGGCCTTTTTATTTGGGGGAGAGGGAA
+GTCATGAAAAAACTAACCTTTGAAATTCGATCTCCAGCACATCAGCAAAACGCTATTCACGCAGTACAGCAAATCCTTCC
+AGACCCAACCAAACCAATCGTAGTAACCATTCAGGAACGCAACCGCAGCTTAGACCAAAACAGGAAGCTATGGGCCTGCT
+TAGGTGACGTCTCTCGTCAGGTTGAATGGCATGGTCGCTGGCTGGATGCAGAAAGCTGGAAGTGTGTGTTTACCGCAGCA
+TTAAAGCAGCAGGATGTTGTTCCTAACCTTGCCGGGAATGGCTTTGTGGTAATAGGCCAGTCAACCAGCAGGATGCGTGT
+AGGCGAATTTGCGGAGCTATTAGAGCTTATACAGGCATTCGGTACAGAGCGTGGCGTTAAGTGGTCAGACGAAGCGAGAC
+TGGCTCTGGAGTGGAAAGCGAGATGGGGAGACAGGGCTGCATGATAAATGTCGTTAGTTTCTCCGGTGGCAGGACGTCAG
+CATATTTGCTCTGGCTAATGGAGCAAAAGCGACGGGCAGGTAAAGACGTGCATTACGTTTTCATGGATACAGGTTGTGAA
+CATCCAATGACATATCGGTTTGTCAGGGAAGTTGTGAAGTTCTGGGATATACCGCTCACCGTATTGCAGGTTGATATCAA
+CCCGGAGCTTGGACAGCCAAATGGTTATACGGTATGGGAACCAAAGGATATTCAGACGCGAATGCCTGTTCTGAAGCCAT
+TTATCGATATGGTAAAGAAATATGGCACTCCATACGTCGGCGGCGCGTTCTGCACTGACAGATTAAAACTCGTTCCCTTC
+ACCAAATACTGTGATGACCATTTCGGGCGAGGGAATTACACCACGTGGATTGGCATCAGAGCTGATGAACCGAAGCGGCT
+AAAGCCAAAGCCTGGAATCAGATATCTTGCTGAACTGTCAGACTTTGAGAAGGAAGATATCCTCGCATGGTGGAAGCAAC
+AACCATTCGATTTGCAAATACCGGAACATCTCGGTAACTGCATATTCTGCATTAAAAAATCAACGCAAAAAATCGGACTT
+GCCTGCAAAGATGAGGAGGGATTGCAGCGTGTTTTTAATGAGGTCATCACGGGATCCCATGTGCGTGACGGACATCGGGA
+AACGCCAAAGGAGATTATGTACCGAGGAAGAATGTCGCTGGACGGTATCGCGAAAATGTATTCAGAAAATGATTATCAAG
+CCCTGTATCAGGACATGGTACGAGCTAAAAGATTCGATACCGGCTCTTGTTCTGAGTCATGCGAAATATTTGGAGGGCAG
+CTTGATTTCGACTTCGGGAGGGAAGCTGCATGATGCGATGTTATCGGTGCGGTGAATGCAAAGAAGATAACCGCTTCCGA
+CCAAATCAACCTTACTGGAATCGATGGTGTCTCCGGTGTGAAAGAACACCAACAGGGGTGTTACCACTACCGCAGGAAAA
+GGAGGACGTGTGGCGAGACAGCGACGAAGTATCACCGACATAATCTGCGAAAACTGCAAATACCTTCCAACGAAACGCAC
+CAGAAATAAACCCAAGCCAATCCCAAAAGAATCTGACGTAAAAACCTTCAACTACACGGCTCACCTGTGGGATATCCGGT
+GGCTAAGACGTCGTGCGAGGAAAACAAGGTGATTGACCAAAATCGAAGTTACGAACAAGAAAGCGTCGAGCGAGCTTTAA
+CGTGCGCTAACTGCGGTCAGAAGCTGCATGTGCTGGAAGTTCACGTGTGTGAGCACTGCTGCGCAGAACTGATGAGCGAT
+CCGAATAGCTCGATGCACGAGGAAGAAGATGATGGCTAAACCAGCGCGAAGACGATGTAAAAACGATGAATGCCGGGAAT
+GGTTTCACCCTGCATTCGCTAATCAGTGGTGGTGCTCTCCAGAGTGTGGAACCAAGATAGCACTCGAACGACGAAGTAAA
+GAACGCGAAAAAGCGGAAAAAGCAGCAGAGAAGAAACGACGACGAGAGGAGCAGAAACAGAAAGATAAACTTAAGATTCG
+AAAACTCGCCTTAAAGCCCCGCAGTTACTGGATTAAACAAGCCCAACAAGCCGTAAACGCCTTCATCAGAGAAAGAGACC
+GCGACTTACCATGTATCTCGTGCGGAACGCTCACGTCTGCTCAGTGGGATGCCGGACATTACCGGACAACTGCTGCGGCA
+CCTCAACTCCGATTTAATGAACGCAATATTCACAAGCAATGCGTGGTGTGCAACCAGCACAAAAGCGGAAATCTCGTTCC
+GTATCGCGTCGAACTGATTAGCCGCATCGGGCAGGAAGCAGTAGACGAAATCGAATCAAACCATAACCGCCATCGCTGGA
+CTATCGAAGAGTGCAAGGCGATCAAGGCAGAGTACCAACAGAAACTCAAAGACCTGCGAAATAGCAGAAGTGAGGCCGCA
+TGACGTTCTCAGTAAAAACCATTCCAGACATGCTCGTTGAAGCATACGGAAATCAGACAGAAGTAGCACGCAGACTGAAA
+TGTAGTCGCGGTACGGTCAGAAAATACGTTGATGATAAAGACGGGAAAATGCACGCCATCGTCAACGACGTTCTCATGGT
+TCATCGCGGATGGAGTGAAAGAGATGCGCTATTACGAAAAAATTGATGGCAGCAAATACCGAAATATTTGGGTAGTTGGC
+GATCTGCACGGATGCTACACGAACCTGATGAACAAACTGGATACGATTGGATTCGACAACAAAAAAGACCTGCTTATCTC
+GGTGGGCGATTTGGTTGATCGTGGTGCAGAGAACGTTGAATGCCTGGAATTAATCACATTCCCCTGGTTCAGAGCTGTAC
+GTGGAAACCATGAGCAAATGATGATTGATGGCTTATCAGAGCGTGGAAACGTTAATCACTGGCTGCTTAATGGCGGTGGC
+TGGTTCTTTAATCTCGATTACGACAAAGAAATTCTGGCTAAAGCTCTTGCCCATAAAGCAGATGAACTTCCGTTAATCAT
+CGAACTGGTGAGCAAAGATAAAAAATATGTTATCTGCCACGCCGATTATCCCTTTGACGAATACGAGTTTGGAAAGCCAG
+TTGATCATCAGCAGGTAATCTGGAACCGCGAACGAATCAGCAACTCACAAAACGGGATCGTGAAAGAAATCAAAGGCGCG
+GACACGTTCATCTTTGGTCATACGCCAGCAGTGAAACCACTCAAGTTTGCCAACCAAATGTATATCGATACCGGCGCAGT
+GTTCTGCGGAAACCTAACATTGATTCAGGTACAGGGAGAAGGCGCATGAGACTCGAAAGCGTAGCTAAATTTCATTCGCC
+AAAAAGCCCGATGATGAGCGACTCACCACGGGCCACGGCTTCTGACTCTCTTTCCGGTACTGATGTGATGGCTGCTATGG
+GGATGGCGCAATCACAAGCCGGATTCGGTATGGCTGCATTCTGCGGTAAGCACGAACTCAGCCAGAACGACAAACAAAAG
+GCTATCAACTATCTGATGCAATTTGCACACAAGGTATCGGGGAAATACCGTGGTGTGGCAAAGCTTGAAGGAAATACTAA
+GGCAAAGGTACTGCAAGTGCTCGCAACATTCGCTTATGCGGATTATTGCCGTAGTGCCGCGACGCCGGGGGCAAGATGCA
+GAGATTGCCATGGTACAGGCCGTGCGGTTGATATTGCCAAAACAGAGCTGTGGGGGAGAGTTGTCGAGAAAGAGTGCGGA
+AGATGCAAAGGCGTCGGCTATTCAAGGATGCCAGCAAGCGCAGCATATCGCGCTGTGACGATGCTAATCCCAAACCTTAC
+CCAACCCACCTGGTCACGCACTGTTAAGCCGCTGTATGACGCTCTGGTGGTGCAATGCCACAAAGAAGAGTCAATCGCAG
+ACAACATTTTGAATGCGGTCACACGTTAGCAGCATGATTGCCACGGATGGCAACATATTAACGGCATGATATTGACTTAT
+TGAATAAAATTGGGTAAATTTGACTCAACGATGGGTTAATTCGCTCGTTGTGGTAGTGAGATGAAAAGAGGCGGCGCTTA
+CTACCGATTCCGCCTAGTTGGTCACTTCGACGTATCGTCTGGAACTCCAACCATCGCAGGCAGAGAGGTCTGCAAAATGC
+AATCCCGAAACAGTTCGCAGGTAATAGTTAGAGCCTGCATAACGGTTTCGGGATTTTTTATATCTGCACAACAGGTAAGA
+GCATTGAGTCGATAATCGTGAAGAGTCGGCGAGCCTGGTTAGCCAGTGCTCTTTCCGTTGTGCTGAATTAAGCGAATACC
+GGAAGCAGAACCGGATCACCAAATGCGTACAGGCGTCATCGCCGCCCAGCAACAGCACAACCCAAACTGAGCCGTAGCCA
+CTGTCTGTCCTGAATTCATTAGTAATAGTTACGCTGCGGCCTTTTACACATGACCTTCGTGAAAGCGGGTGGCAGGAGGT
+CGCGCTAACAACCTCCTGCCGTTTTGCCCGTGCATATCGGTCACGAACAAATCTGATTACTAAACACAGTAGCCTGGATT
+TGTTCTATCAGTAATCGACCTTATTCCTAATTAAATAGAGCAAATCCCCTTATTGGGGGTAAGACATGAAGATGCCAGAA
+AAACATGACCTGTTGGCCGCCATTCTCGCGGCAAAGGAACAAGGCATCGGGGCAATCCTTGCGTTTGCAATGGCGTACCT
+TCGCGGCAGATATAATGGCGGTGCGTTTACAAAAACAGTAATCGACGCAACGATGTGCGCCATTATCGCCTGGTTCATTC
+GTGACCTTCTCGACTTCGCCGGACTAAGTAGCAATCTCGCTTATATAACGAGCGTGTTTATCGGCTACATCGGTACTGAC
+TCGATTGGTTCGCTTATCAAACGCTTCGCTGCTAAAAAAGCCGGAGTAGAAGATGGTAGAAATCAATAATCAACGTAAGG
+CGTTCCTCGATATGCTGGCGTGGTCGGAGGGAACTGATAACGGACGTCAGAAAACCAGAAATCATGGTTATGACGTCATT
+GTAGGCGGAGAGCTATTTACTGATTACTCCGATCACCCTCGCAAACTTGTCACGCTAAACCCAAAACTCAAATCAACAGG
+CGCCGGACGCTACCAGCTTCTTTCCCGTTGGTGGGATGCCTACCGCAAGCAGCTTGGCCTGAAAGACTTCTCTCCGAAAA
+GTCAGGACGCTGTGGCATTGCAGCAGATTAAGGAGCGTGGCGCTTTACCTATGATTGATCGTGGTGATATCCGTCAGGCA
+ATCGACCGTTGCAGCAATATCTGGGCTTCACTGCCGGGCGCTGGTTATGGTCAGTTCGAGCATAAGGCTGACAGCCTGAT
+TGCAAAATTCAAAGAAGCGGGCGGAACGGTCAGAGAGATTGATGTATGAGCAGAGTCACCGCGATTATCTCCGCTCTGGT
+TATCTGCATCATCGTCTGCCTGTCATGGGCTGTTAATCATTACCGTGATAACGCCATTACCTACAAAGCCCAGCGCGACA
+AAAATGCCAGAGAACTGAAGCTGGCGAACGCGGCAATTACTGACATGCAGATGCGTCAGCGTGATGTTGCTGCGCTCGAT
+GCAAAATACACGAAGGAGTTAGCTGATGCTAAAGCTGAAAATGATGCTCTGCGTGATGATGTTGCCGCTGGTCGTCGTCG
+GTTGCACATCAAAGCAGTCTGTCAGTCAGTGCGTGAAGCCACCACCGCCTCCGGCGTGGATAATGCAGCCTCCCCCCGAC
+TGGCAGACACCGCTGAACGGGATTATTTCACCCTCAGAGAGAGGCTGATCACTATGCAAAAACAACTGGAAGGAACCCAG
+AAGTATATTAATGAGCAGTGCAGATAGAGTTGCCCATATCGATGGGCAACTCATGCAATTATTGTGAGCAATACACACGC
+GCTTCCAGCGGAGTATAAATGCCTAAAGTAATAAAACCGAGCAATCCATTTACGAATGTTTGCTGGGTTTCTGTTTTAAC
+AACATTTTCTGCGCCGCCACAAATTTTGGCTGCATCGACAGTTTTCTTCTGCCCAATTCCAGAAACGAAGAAATGATGGG
+TGATGGTTTCCTTTGGTGCTACTGCTGCCGGTTTGTTTTGAACAGTAAACGTCTGTTGAGCACATCCTGTAATAAGCAGG
+GCCAGCGCAGTAGCGAGTAGCATTTTTTTCATGGTGTTATTCCCGATGCTTTTTGAAGTTCGCAGAATCGTATGTGTAGA
+AAATTAAACAAACCCTAAACAATGAGTTGAAATTTCATATTGTTAATATTTATTAATGTATGTCAGGTGCGATGAATCGT
+CATTGTATTCCCGGATTAACTATGTCCACAGCCCTGACGGGGAACTTCTCTGCGGGAGTGTCCGGGAATAATTAAAACGA
+TGCACACAGGGTTTAGCGCGTACACGTATTGCATTATGCCAACGCCCCGGTGCTGACACGGAAGAAACCGGACGTTATGA
+TTTAGCGTGGAAAGATTTGTGTAGTGTTCTGAATGCTCTCAGTAAATAGTAATGAATTATCAAAGGTATAGTAATATCTT
+TTATGTTCATGGATATTTGTAACCCATCGGAAAACTCCTGCTTTAGCAAGATTTTCCCTGTATTGCTGAAATGTGATTTC
+TCTTGATTTCAACCTATCATAGGACGTTTCTATAAGATGCGTGTTTCTTGAGAATTTAACATTTACAACCTTTTTAAGTC
+CTTTTATTAACACGGTGTTATCGTTTTCTAACACGATGTGAATATTATCTGTGGCTAGATAGTAAATATAATGTGAGACG
+TTGTGACGTTTTAGTTCAGAATAAAACAATTCACAGTCTAAATCTTTTCGCACTTGATCGAATATTTCTTTAAAAATGGC
+AACCTGAGCCATTGGTAAAACCTTCCATGTGATACGAGGGCGCGTAGTTTGCATTATCGTTTTTATCGTTTCAATCTGGT
+CTGACCTCCTTGTGTTTTGTTGATGATTTATGTCAAATATTAGGAATGTTTTCACTTAATAGTATTGGTTGCGTAACAAA
+GTGCGGTCCTGCTGGCATTCTGGAGGGAAATACAACCGACAGATGTATGTAAGGCCAACGTGCTCAAATCTTCATACAGA
+AAGATTTGAAGTAATATTTTAACCGCTAGATGAAGAGCAAGCGCATGGAGCGACAAAATGAATAAAGAACAATCTGCTGA
+TGATCCCTCCGTGGATCTGATTCGTGTAAAAAATATGCTTAATAGCACCATTTCTATGAGTTACCCTGATGTTGTAATTG
+CATGTATAGAACATAAGGTGTCTCTGGAAGCATTCAGAGCAATTGAGGCAGCGTTGGTGAAGCACGATAATAATATGAAG
+GATTATTCCCTGGTGGTTGACTGATCACCATAACTGCTAATCATTCAAACTATTTAGTCTGTGACAGAGCCAACACGCAG
+TCTGTCACTGTCAGGAAAGTGGTAAAACTGCAACTCAATTACTGCAATGCCCTCGTAATTAAGTGAATTTACAATATCGT
+CCTGTTCGGAGGGAAGAACGCGGGATGTTCATTCTTCATCACTTTTAATTGATGTATATGCTCTCTTTTCTGACGTTAGT
+CTCCGACGGCAGGCTTCAATGACCCAGGCTGAGAAATTCCCGGACCCTTTTTGCTCAAGAGCGATGTTAATTTGTTCAAT
+CATTTGGTTAGGAAAGCGGATGTTGCGGGTTGTTGTTCTGCGGGTTCTGTTCTTCGTTGACATGAGGTTGCCCCGTATTC
+AGTGTCGCTGATTTGTATTGTCTGAAGTTGTTTTTACGTTAAGTTGATGCAGATCAATTAATACGATACCTGCGTCATAA
+TTGATTATTTGACGTGGTTTGATGGCCTCCACGCACGTTGTGATATGTAGATGATAATCATTATCACTTTACGGGTCCTT
+TCCGGTGATCCGACAGGTTACG
```

### Comparing `MetaCerberus-1.2.1/lib/PHANOTATE/tests/phiX174.fasta` & `metacerberus-1.3.0/lib/dependency_files/phix174_ill.ref.fna`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,78 @@
->phiX174 complete genome
-GTGTGAGGTTATAACGCCGAAGCGGTAAAAATTTTAATTTTTGCCGCTGAGGGGTTGACC
-AAGCGAAGCGCGGTAGGTTTTCTGCTTAGGAGTTTAATCATGTTTCAGACTTTTATTTCT
-CGCCATAATTCAAACTTTTTTTCTGATAAGCTGGTTCTCACTTCTGTTACTCCAGCTTCT
-TCGGCACCTGTTTTACAGACACCTAAAGCTACATCGTCAACGTTATATTTTGATAGTTTG
-ACGGTTAATGCTGGTAATGGTGGTTTTCTTCATTGCATTCAGATGGATACATCTGTCAAC
-GCCGCTAATCAGGTTGTTTCTGTTGGTGCTGATATTGCTTTTGATGCCGACCCTAAATTT
-TTTGCCTGTTTGGTTCGCTTTGAGTCTTCTTCGGTTCCGACTACCCTCCCGACTGCCTAT
-GATGTTTATCCTTTGAATGGTCGCCATGATGGTGGTTATTATACCGTCAAGGACTGTGTG
-ACTATTGACGTCCTTCCCCGTACGCCGGGCAATAACGTTTATGTTGGTTTCATGGTTTGG
-TCTAACTTTACCGCTACTAAATGCCGCGGATTGGTTTCGCTGAATCAGGTTATTAAAGAG
-ATTATTTGTCTCCAGCCACTTAAGTGAGGTGATTTATGTTTGGTGCTATTGCTGGCGGTA
-TTGCTTCTGCTCTTGCTGGTGGCGCCATGTCTAAATTGTTTGGAGGCGGTCAAAAAGCCG
-CCTCCGGTGGCATTCAAGGTGATGTGCTTGCTACCGATAACAATACTGTAGGCATGGGTG
-ATGCTGGTATTAAATCTGCCATTCAAGGCTCTAATGTTCCTAACCCTGATGAGGCCGCCC
-CTAGTTTTGTTTCTGGTGCTATGGCTAAAGCTGGTAAAGGACTTCTTGAAGGTACGTTGC
-AGGCTGGCACTTCTGCCGTTTCTGATAAGTTGCTTGATTTGGTTGGACTTGGTGGCAAGT
-CTGCCGCTGATAAAGGAAAGGATACTCGTGATTATCTTGCTGCTGCATTTCCTGAGCTTA
-ATGCTTGGGAGCGTGCTGGTGCTGATGCTTCCTCTGCTGGTATGGTTGACGCCGGATTTG
-AGAATCAAAAAGAGCTTACTAAAATGCAACTGGACAATCAGAAAGAGATTGCCGAGATGC
-AAAATGAGACTCAAAAAGAGATTGCTGGCATTCAGTCGGCGACTTCACGCCAGAATACGA
-AAGACCAGGTATATGCACAAAATGAGATGCTTGCTTATCAACAGAAGGAGTCTACTGCTC
-GCGTTGCGTCTATTATGGAAAACACCAATCTTTCCAAGCAACAGCAGGTTTCCGAGATTA
-TGCGCCAAATGCTTACTCAAGCTCAAACGGCTGGTCAGTATTTTACCAATGACCAAATCA
-AAGAAATGACTCGCAAGGTTAGTGCTGAGGTTGACTTAGTTCATCAGCAAACGCAGAATC
-AGCGGTATGGCTCTTCTCATATTGGCGCTACTGCAAAGGATATTTCTAATGTCGTCACTG
-ATGCTGCTTCTGGTGTGGTTGATATTTTTCATGGTATTGATAAAGCTGTTGCCGATACTT
-GGAACAATTTCTGGAAAGACGGTAAAGCTGATGGTATTGGCTCTAATTTGTCTAGGAAAT
-AACCGTCAGGATTGACACCCTCCCAATTGTATGTTTTCATGCCTCCAAATCTTGGAGGCT
-TTTTTATGGTTCGTTCTTATTACCCTTCTGAATGTCACGCTGATTATTTTGACTTTGAGC
-GTATCGAGGCTCTTAAACCTGCTATTGAGGCTTGTGGCATTTCTACTCTTTCTCAATCCC
-CAATGCTTGGCTTCCATAAGCAGATGGATAACCGCATCAAGCTCTTGGAAGAGATTCTGT
-CTTTTCGTATGCAGGGCGTTGAGTTCGATAATGGTGATATGTATGTTGACGGCCATAAGG
-CTGCTTCTGACGTTCGTGATGAGTTTGTATCTGTTACTGAGAAGTTAATGGATGAATTGG
-CACAATGCTACAATGTGCTCCCCCAACTTGATATTAATAACACTATAGACCACCGCCCCG
-AAGGGGACGAAAAATGGTTTTTAGAGAACGAGAAGACGGTTACGCAGTTTTGCCGCAAGC
-TGGCTGCTGAACGCCCTCTTAAGGATATTCGCGATGAGTATAATTACCCCAAAAAGAAAG
-GTATTAAGGATGAGTGTTCAAGATTGCTGGAGGCCTCCACTATGAAATCGCGTAGAGGCT
-TTGCTATTCAGCGTTTGATGAATGCAATGCGACAGGCTCATGCTGATGGTTGGTTTATCG
-TTTTTGACACTCTCACGTTGGCTGACGACCGATTAGAGGCGTTTTATGATAATCCCAATG
-CTTTGCGTGACTATTTTCGTGATATTGGTCGTATGGTTCTTGCTGCCGAGGGTCGCAAGG
-CTAATGATTCACACGCCGACTGCTATCAGTATTTTTGTGTGCCTGAGTATGGTACAGCTA
-ATGGCCGTCTTCATTTCCATGCGGTGCACTTTATGCGGACACTTCCTACAGGTAGCGTTG
-ACCCTAATTTTGGTCGTCGGGTACGCAATCGCCGCCAGTTAAATAGCTTGCAAAATACGT
-GGCCTTATGGTTACAGTATGCCCATCGCAGTTCGCTACACGCAGGACGCTTTTTCACGTT
-CTGGTTGGTTGTGGCCTGTTGATGCTAAAGGTGAGCCGCTTAAAGCTACCAGTTATATGG
-CTGTTGGTTTCTATGTGGCTAAATACGTTAACAAAAAGTCAGATATGGACCTTGCTGCTA
-AAGGTCTAGGAGCTAAAGAATGGAACAACTCACTAAAAACCAAGCTGTCGCTACTTCCCA
-AGAAGCTGTTCAGAATCAGAATGAGCCGCAACTTCGGGATGAAAATGCTCACAATGACAA
-ATCTGTCCACGGAGTGCTTAATCCAACTTACCAAGCTGGGTTACGACGCGACGCCGTTCA
-ACCAGATATTGAAGCAGAACGCAAAAAGAGAGATGAGATTGAGGCTGGGAAAAGTTACTG
-TAGCCGACGTTTTGGCGGCGCAACCTGTGACGACAAATCTGCTCAAATTTATGCGCGCTT
-CGATAAAAATGATTGGCGTATCCAACCTGCAGAGTTTTATCGCTTCCATGACGCAGAAGT
-TAACACTTTCGGATATTTCTGATGAGTCGAAAAATTATCTTGATAAAGCAGGAATTACTA
-CTGCTTGTTTACGAATTAAATCGAAGTGGACTGCTGGCGGAAAATGAGAAAATTCGACCT
-ATCCTTGCGCAGCTCGAGAAGCTCTTACTTTGCGACCTTTCGCCATCAACTAACGATTCT
-GTCAAAAACTGACGCGTTGGATGAGGAGAAGTGGCTTAATATGCTTGGCACGTTCGTCAA
-GGACTGGTTTAGATATGAGTCACATTTTGTTCATGGTAGAGATTCTCTTGTTGACATTTT
-AAAAGAGCGTGGATTACTATCTGAGTCCGATGCTGTTCAACCACTAATAGGTAAGAAATC
-ATGAGTCAAGTTACTGAACAATCCGTACGTTTCCAGACCGCTTTGGCCTCTATTAAGCTC
-ATTCAGGCTTCTGCCGTTTTGGATTTAACCGAAGATGATTTCGATTTTCTGACGAGTAAC
-AAAGTTTGGATTGCTACTGACCGCTCTCGTGCTCGTCGCTGCGTTGAGGCTTGCGTTTAT
-GGTACGCTGGACTTTGTGGGATACCCTCGCTTTCCTGCTCCTGTTGAGTTTATTGCTGCC
-GTCATTGCTTATTATGTTCATCCCGTCAACATTCAAACGGCCTGTCTCATCATGGAAGGC
-GCTGAATTTACGGAAAACATTATTAATGGCGTCGAGCGTCCGGTTAAAGCCGCTGAATTG
-TTCGCGTTTACCTTGCGTGTACGCGCAGGAAACACTGACGTTCTTACTGACGCAGAAGAA
-AACGTGCGTCAAAAATTACGTGCGGAAGGAGTGATGTAATGTCTAAAGGTAAAAAACGTT
-CTGGCGCTCGCCCTGGTCGTCCGCAGCCGTTGCGAGGTACTAAAGGCAAGCGTAAAGGCG
-CTCGTCTTTGGTATGTAGGTGGTCAACAATTTTAATTGCAGGGGCTTCGGCCCCTTACTT
-GAGGATAAATTATGTCTAATATTCAAACTGGCGCCGAGCGTATGCCGCATGACCTTTCCC
-ATCTTGGCTTCCTTGCTGGTCAGATTGGTCGTCTTATTACCATTTCAACTACTCCGGTTA
-TCGCTGGCGACTCCTTCGAGATGGACGCCGTTGGCGCTCTCCGTCTTTCTCCATTGCGTC
-GTGGCCTTGCTATTGACTCTACTGTAGACATTTTTACTTTTTATGTCCCTCATCGTCACG
-TTTATGGTGAACAGTGGATTAAGTTCATGAAGGATGGTGTTAATGCCACTCCTCTCCCGA
-CTGTTAACACTACTGGTTATATTGACCATGCCGCTTTTCTTGGCACGATTAACCCTGATA
-CCAATAAAATCCCTAAGCATTTGTTTCAGGGTTATTTGAATATCTATAACAACTATTTTA
-AAGCGCCGTGGATGCCTGACCGTACCGAGGCTAACCCTAATGAGCTTAATCAAGATGATG
-CTCGTTATGGTTTCCGTTGCTGCCATCTCAAAAACATTTGGACTGCTCCGCTTCCTCCTG
-AGACTGAGCTTTCTCGCCAAATGACGACTTCTACCACATCTATTGACATTATGGGTCTGC
-AAGCTGCTTATGCTAATTTGCATACTGACCAAGAACGTGATTACTTCATGCAGCGTTACC
-ATGATGTTATTTCTTCATTTGGAGGTAAAACCTCTTATGACGCTGACAACCGTCCTTTAC
-TTGTCATGCGCTCTAATCTCTGGGCATCTGGCTATGATGTTGATGGAACTGACCAAACGT
-CGTTAGGCCAGTTTTCTGGTCGTGTTCAACAGACCTATAAACATTCTGTGCCGCGTTTCT
-TTGTTCCTGAGCATGGCACTATGTTTACTCTTGCGCTTGTTCGTTTTCCGCCTACTGCGA
-CTAAAGAGATTCAGTACCTTAACGCTAAAGGTGCTTTGACTTATACCGATATTGCTGGCG
-ACCCTGTTTTGTATGGCAACTTGCCGCCGCGTGAAATTTCTATGAAGGATGTTTTCCGTT
-CTGGTGATTCGTCTAAGAAGTTTAAGATTGCTGAGGGTCAGTGGTATCGTTATGCGCCTT
-CGTATGTTTCTCCTGCTTATCACCTTCTTGAAGGCTTCCCATTCATTCAGGAACCGCCTT
-CTGGTGATTTGCAAGAACGCGTACTTATTCGCCACCATGATTATGACCAGTGTTTCCAGT
-CCGTTCAGTTGTTGCAGTGGAATAGTCAGGTTAAATTTAATGTGACCGTTTATCGCAATC
-TGCCGACCACTCGCGATTCAATCATGACTTCGTGATAAAAGATTGA
+>gi|9626372|ref|NC_001422.1| Coliphage phiX174, complete genome
+GAGTTTTATCGCTTCCATGACGCAGAAGTTAACACTTTCGGATATTTCTGATGAGTCGAAAAATTATCTT
+GATAAAGCAGGAATTACTACTGCTTGTTTACGAATTAAATCGAAGTGGACTGCTGGCGGAAAATGAGAAA
+ATTCGACCTATCCTTGCGCAGCTCGAGAAGCTCTTACTTTGCGACCTTTCGCCATCAACTAACGATTCTG
+TCAAAAACTGACGCGTTGGATGAGGAGAAGTGGCTTAATATGCTTGGCACGTTCGTCAAGGACTGGTTTA
+GATATGAGTCACATTTTGTTCATGGTAGAGATTCTCTTGTTGACATTTTAAAAGAGCGTGGATTACTATC
+TGAGTCCGATGCTGTTCAACCACTAATAGGTAAGAAATCATGAGTCAAGTTACTGAACAATCCGTACGTT
+TCCAGACCGCTTTGGCCTCTATTAAGCTCATTCAGGCTTCTGCCGTTTTGGATTTAACCGAAGATGATTT
+CGATTTTCTGACGAGTAACAAAGTTTGGATTGCTACTGACCGCTCTCGTGCTCGTCGCTGCGTTGAGGCT
+TGCGTTTATGGTACGCTGGACTTTGTAGGATACCCTCGCTTTCCTGCTCCTGTTGAGTTTATTGCTGCCG
+TCATTGCTTATTATGTTCATCCCGTCAACATTCAAACGGCCTGTCTCATCATGGAAGGCGCTGAATTTAC
+GGAAAACATTATTAATGGCGTCGAGCGTCCGGTTAAAGCCGCTGAATTGTTCGCGTTTACCTTGCGTGTA
+CGCGCAGGAAACACTGACGTTCTTACTGACGCAGAAGAAAACGTGCGTCAAAAATTACGTGCAGAAGGAG
+TGATGTAATGTCTAAAGGTAAAAAACGTTCTGGCGCTCGCCCTGGTCGTCCGCAGCCGTTGCGAGGTACT
+AAAGGCAAGCGTAAAGGCGCTCGTCTTTGGTATGTAGGTGGTCAACAATTTTAATTGCAGGGGCTTCGGC
+CCCTTACTTGAGGATAAATTATGTCTAATATTCAAACTGGCGCCGAGCGTATGCCGCATGACCTTTCCCA
+TCTTGGCTTCCTTGCTGGTCAGATTGGTCGTCTTATTACCATTTCAACTACTCCGGTTATCGCTGGCGAC
+TCCTTCGAGATGGACGCCGTTGGCGCTCTCCGTCTTTCTCCATTGCGTCGTGGCCTTGCTATTGACTCTA
+CTGTAGACATTTTTACTTTTTATGTCCCTCATCGTCACGTTTATGGTGAACAGTGGATTAAGTTCATGAA
+GGATGGTGTTAATGCCACTCCTCTCCCGACTGTTAACACTACTGGTTATATTGACCATGCCGCTTTTCTT
+GGCACGATTAACCCTGATACCAATAAAATCCCTAAGCATTTGTTTCAGGGTTATTTGAATATCTATAACA
+ACTATTTTAAAGCGCCGTGGATGCCTGACCGTACCGAGGCTAACCCTAATGAGCTTAATCAAGATGATGC
+TCGTTATGGTTTCCGTTGCTGCCATCTCAAAAACATTTGGACTGCTCCGCTTCCTCCTGAGACTGAGCTT
+TCTCGCCAAATGACGACTTCTACCACATCTATTGACATTATGGGTCTGCAAGCTGCTTATGCTAATTTGC
+ATACTGACCAAGAACGTGATTACTTCATGCAGCGTTACCATGATGTTATTTCTTCATTTGGAGGTAAAAC
+CTCTTATGACGCTGACAACCGTCCTTTACTTGTCATGCGCTCTAATCTCTGGGCATCTGGCTATGATGTT
+GATGGAACTGACCAAACGTCGTTAGGCCAGTTTTCTGGTCGTGTTCAACAGACCTATAAACATTCTGTGC
+CGCGTTTCTTTGTTCCTGAGCATGGCACTATGTTTACTCTTGCGCTTGTTCGTTTTCCGCCTACTGCGAC
+TAAAGAGATTCAGTACCTTAACGCTAAAGGTGCTTTGACTTATACCGATATTGCTGGCGACCCTGTTTTG
+TATGGCAACTTGCCGCCGCGTGAAATTTCTATGAAGGATGTTTTCCGTTCTGGTGATTCGTCTAAGAAGT
+TTAAGATTGCTGAGGGTCAGTGGTATCGTTATGCGCCTTCGTATGTTTCTCCTGCTTATCACCTTCTTGA
+AGGCTTCCCATTCATTCAGGAACCGCCTTCTGGTGATTTGCAAGAACGCGTACTTATTCGCCACCATGAT
+TATGACCAGTGTTTCCAGTCCGTTCAGTTGTTGCAGTGGAATAGTCAGGTTAAATTTAATGTGACCGTTT
+ATCGCAATCTGCCGACCACTCGCGATTCAATCATGACTTCGTGATAAAAGATTGAGTGTGAGGTTATAAC
+GCCGAAGCGGTAAAAATTTTAATTTTTGCCGCTGAGGGGTTGACCAAGCGAAGCGCGGTAGGTTTTCTGC
+TTAGGAGTTTAATCATGTTTCAGACTTTTATTTCTCGCCATAATTCAAACTTTTTTTCTGATAAGCTGGT
+TCTCACTTCTGTTACTCCAGCTTCTTCGGCACCTGTTTTACAGACACCTAAAGCTACATCGTCAACGTTA
+TATTTTGATAGTTTGACGGTTAATGCTGGTAATGGTGGTTTTCTTCATTGCATTCAGATGGATACATCTG
+TCAACGCCGCTAATCAGGTTGTTTCTGTTGGTGCTGATATTGCTTTTGATGCCGACCCTAAATTTTTTGC
+CTGTTTGGTTCGCTTTGAGTCTTCTTCGGTTCCGACTACCCTCCCGACTGCCTATGATGTTTATCCTTTG
+GATGGTCGCCATGATGGTGGTTATTATACCGTCAAGGACTGTGTGACTATTGACGTCCTTCCTCGTACGC
+CGGGCAATAATGTTTATGTTGGTTTCATGGTTTGGTCTAACTTTACCGCTACTAAATGCCGCGGATTGGT
+TTCGCTGAATCAGGTTATTAAAGAGATTATTTGTCTCCAGCCACTTAAGTGAGGTGATTTATGTTTGGTG
+CTATTGCTGGCGGTATTGCTTCTGCTCTTGCTGGTGGCGCCATGTCTAAATTGTTTGGAGGCGGTCAAAA
+AGCCGCCTCCGGTGGCATTCAAGGTGATGTGCTTGCTACCGATAACAATACTGTAGGCATGGGTGATGCT
+GGTATTAAATCTGCCATTCAAGGCTCTAATGTTCCTAACCCTGATGAGGCCGCCCCTAGTTTTGTTTCTG
+GTGCTATGGCTAAAGCTGGTAAAGGACTTCTTGAAGGTACGTTGCAGGCTGGCACTTCTGCCGTTTCTGA
+TAAGTTGCTTGATTTGGTTGGACTTGGTGGCAAGTCTGCCGCTGATAAAGGAAAGGATACTCGTGATTAT
+CTTGCTGCTGCATTTCCTGAGCTTAATGCTTGGGAGCGTGCTGGTGCTGATGCTTCCTCTGCTGGTATGG
+TTGACGCCGGATTTGAGAATCAAAAAGAGCTTACTAAAATGCAACTGGACAATCAGAAAGAGATTGCCGA
+GATGCAAAATGAGACTCAAAAAGAGATTGCTGGCATTCAGTCGGCGACTTCACGCCAGAATACGAAAGAC
+CAGGTATATGCACAAAATGAGATGCTTGCTTATCAACAGAAGGAGTCTACTGCTCGCGTTGCGTCTATTA
+TGGAAAACACCAATCTTTCCAAGCAACAGCAGGTTTCCGAGATTATGCGCCAAATGCTTACTCAAGCTCA
+AACGGCTGGTCAGTATTTTACCAATGACCAAATCAAAGAAATGACTCGCAAGGTTAGTGCTGAGGTTGAC
+TTAGTTCATCAGCAAACGCAGAATCAGCGGTATGGCTCTTCTCATATTGGCGCTACTGCAAAGGATATTT
+CTAATGTCGTCACTGATGCTGCTTCTGGTGTGGTTGATATTTTTCATGGTATTGATAAAGCTGTTGCCGA
+TACTTGGAACAATTTCTGGAAAGACGGTAAAGCTGATGGTATTGGCTCTAATTTGTCTAGGAAATAACCG
+TCAGGATTGACACCCTCCCAATTGTATGTTTTCATGCCTCCAAATCTTGGAGGCTTTTTTATGGTTCGTT
+CTTATTACCCTTCTGAATGTCACGCTGATTATTTTGACTTTGAGCGTATCGAGGCTCTTAAACCTGCTAT
+TGAGGCTTGTGGCATTTCTACTCTTTCTCAATCCCCAATGCTTGGCTTCCATAAGCAGATGGATAACCGC
+ATCAAGCTCTTGGAAGAGATTCTGTCTTTTCGTATGCAGGGCGTTGAGTTCGATAATGGTGATATGTATG
+TTGACGGCCATAAGGCTGCTTCTGACGTTCGTGATGAGTTTGTATCTGTTACTGAGAAGTTAATGGATGA
+ATTGGCACAATGCTACAATGTGCTCCCCCAACTTGATATTAATAACACTATAGACCACCGCCCCGAAGGG
+GACGAAAAATGGTTTTTAGAGAACGAGAAGACGGTTACGCAGTTTTGCCGCAAGCTGGCTGCTGAACGCC
+CTCTTAAGGATATTCGCGATGAGTATAATTACCCCAAAAAGAAAGGTATTAAGGATGAGTGTTCAAGATT
+GCTGGAGGCCTCCACTATGAAATCGCGTAGAGGCTTTGCTATTCAGCGTTTGATGAATGCAATGCGACAG
+GCTCATGCTGATGGTTGGTTTATCGTTTTTGACACTCTCACGTTGGCTGACGACCGATTAGAGGCGTTTT
+ATGATAATCCCAATGCTTTGCGTGACTATTTTCGTGATATTGGTCGTATGGTTCTTGCTGCCGAGGGTCG
+CAAGGCTAATGATTCACACGCCGACTGCTATCAGTATTTTTGTGTGCCTGAGTATGGTACAGCTAATGGC
+CGTCTTCATTTCCATGCGGTGCACTTTATGCGGACACTTCCTACAGGTAGCGTTGACCCTAATTTTGGTC
+GTCGGGTACGCAATCGCCGCCAGTTAAATAGCTTGCAAAATACGTGGCCTTATGGTTACAGTATGCCCAT
+CGCAGTTCGCTACACGCAGGACGCTTTTTCACGTTCTGGTTGGTTGTGGCCTGTTGATGCTAAAGGTGAG
+CCGCTTAAAGCTACCAGTTATATGGCTGTTGGTTTCTATGTGGCTAAATACGTTAACAAAAAGTCAGATA
+TGGACCTTGCTGCTAAAGGTCTAGGAGCTAAAGAATGGAACAACTCACTAAAAACCAAGCTGTCGCTACT
+TCCCAAGAAGCTGTTCAGAATCAGAATGAGCCGCAACTTCGGGATGAAAATGCTCACAATGACAAATCTG
+TCCACGGAGTGCTTAATCCAACTTACCAAGCTGGGTTACGACGCGACGCCGTTCAACCAGATATTGAAGC
+AGAACGCAAAAAGAGAGATGAGATTGAGGCTGGGAAAAGTTACTGTAGCCGACGTTTTGGCGGCGCAACC
+TGTGACGACAAATCTGCTCAAATTTATGCGCGCTTCGATAAAAATGATTGGCGTATCCAACCTGCA
```

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_decon.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_decon.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_formatFasta.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_formatFasta.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_genecall.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_genecall.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_hmm.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_hmm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_merge.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_merge.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_metastats.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_metastats.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_parser.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_prostats.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_prostats.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_qc.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_qc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_report.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_report.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_setup.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_setup.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_trim.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_trim.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/__pycache__/metacerberus_visual.cpython-39.pyc` & `metacerberus-1.3.0/lib/__pycache__/metacerberus_visual.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/dependency_files/PacBio_quality-control.fna` & `metacerberus-1.3.0/lib/dependency_files/PacBio_quality-control.fna`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/dependency_files/adapters.fna` & `metacerberus-1.3.0/lib/dependency_files/adapters.fna`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/454_10` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/454_10`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/454_30` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/454_30`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/454_5` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/454_5`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/complete` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/complete`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/gene` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/gene`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/illumina_1` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/illumina_1`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/illumina_10` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/illumina_10`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/illumina_5` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/illumina_5`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/noncoding` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/noncoding`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/pwm` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/pwm`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/rgene` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/rgene`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/sanger_10` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/sanger_10`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/sanger_5` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/sanger_5`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/start` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/start`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/start1` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/start1`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/stop` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/stop`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/fraggenescanplus_dependences/stop1` & `metacerberus-1.3.0/lib/fraggenescanplus_dependences/stop1`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/metacerberus.config` & `metacerberus-1.3.0/lib/metacerberus.config`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_decon.py` & `metacerberus-1.3.0/lib/metacerberus_decon.py`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_formatFasta.py` & `metacerberus-1.3.0/lib/metacerberus_formatFasta.py`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_genecall.py` & `metacerberus-1.3.0/lib/metacerberus_genecall.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 """metacerberus_genecall.py: Module for finding Open Reading Frames (ORF) in FASTA nucleotide files
 Uses prodigal
 Uses FGS+
 """
 
 from pathlib import Path
-import re
 import subprocess
-import pkg_resources as pkg
 
 
 # Eukaryotic option
 def findORF_fgs(contig, config, subdir):
     path = Path(config['DIR_OUT'], subdir)
     done = path / "complete"
 
@@ -19,15 +17,21 @@
     faaOut  = path / "proteins.faa"
 
     if not config['REPLACE'] and done.exists() and faaOut.exists():
             return faaOut
     done.unlink(missing_ok=True)
     path.mkdir(exist_ok=True, parents=True)
 
-    command = f"{config['EXE_FGS']} -p {config['CPUS']} -s {contig} -o {baseOut} -w 1 -t complete"
+    train = "complete"
+    if config['ILLUMINA']:
+         train = "illumina_10"
+    elif config['NANOPORE'] or config['PACBIO']:
+         train = "454_30"
+
+    command = f"{config['EXE_FGS']} -p {config['CPUS']} -s {contig} -o {baseOut} -w 1 -t {train}"
     try:
         with Path(path,"stdout.txt").open('w') as fout, Path(path,"stderr.txt").open('w') as ferr:
             subprocess.run(command, shell=True, check=True, stdout=fout, stderr=ferr)
     except Exception as e:
         print(e)
         return None
 
@@ -37,21 +41,22 @@
 
 # Microbial option
 def findORF_prod(contig, config, subdir):
     path = Path(config['DIR_OUT'], subdir)
     done = path / "complete"
 
     faaOut = path / "proteins.faa"
+    fnaOut = faaOut.with_suffix(".ffn")
 
     if not config['REPLACE'] and done.exists() and faaOut.exists():
         return faaOut
     done.unlink(missing_ok=True)
     path.mkdir(exist_ok=True, parents=True)
 
-    command = f"{config['EXE_PRODIGAL']} -i {contig} -o {path}/genes.gff -a {faaOut} -f gff"
+    command = f"{config['EXE_PRODIGAL']} -i {contig} -o {path}/genes.gff -a {faaOut} -d {fnaOut} -f gff"
     try:
         with Path(path, 'stdout.txt').open('w') as fout, Path(path, 'stderr.txt').open('w') as ferr:
             subprocess.run(command, shell=True, check=True, stdout=fout, stderr=ferr)
     except Exception as e:
         print(e)
 
     done.touch()    
@@ -60,21 +65,22 @@
 
 # Metagenome option
 def findORF_meta(contig, config, subdir):
     path = Path(config['DIR_OUT'], subdir)
     done = path / "complete"
 
     faaOut = path / "proteins.faa"
+    fnaOut = faaOut.with_suffix(".ffn")
 
     if not config['REPLACE'] and done.exists() and faaOut.exists():
         return faaOut
     done.unlink(missing_ok=True)
     path.mkdir(exist_ok=True, parents=True)
 
-    command = f"{config['EXE_PRODIGAL']} -i {contig} -o {path}/genes.gff -a {faaOut} -f gff -p meta"
+    command = f"{config['EXE_PRODIGAL']} -i {contig} -o {path}/genes.gff -a {faaOut} -d {fnaOut} -f gff -p meta"
     try:
         with Path(path, "stdout.txt").open('w') as fout, Path(path, "stderr.txt").open('w') as ferr:
             subprocess.run(command, shell=True, check=True, stdout=fout, stderr=ferr)
     except Exception as e:
         print(e)
 
     done.touch()
@@ -82,21 +88,22 @@
 
 # Giant Virus
 def findORF_prodgv(contig, config, subdir, meta=False):
     path = Path(config['DIR_OUT'], subdir)
     done = path / "complete"
 
     faaOut  = path / "proteins.faa"
+    fnaOut = faaOut.with_suffix(".ffn")
 
     if not config['REPLACE'] and done.exists() and faaOut.exists():
             return faaOut
     done.unlink(missing_ok=True)
     path.mkdir(exist_ok=True, parents=True)
 
-    command = f"{config['EXE_PRODIGAL-GV']} -i {contig} -a {faaOut} -o {path / 'proteins.gbk'} {'-p meta' if meta else ''}"
+    command = f"{config['EXE_PRODIGAL-GV']} -i {contig} -a {faaOut} -d {fnaOut} -o {path / 'proteins.gbk'} {'-p meta' if meta else ''}"
     print(command)
     try:
         with Path(path,"stdout.txt").open('w') as fout, Path(path,"stderr.txt").open('w') as ferr:
             subprocess.run(command, shell=True, check=True, stdout=fout, stderr=ferr)
     except Exception as e:
         print(e)
         return None
```

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_hmm.py` & `metacerberus-1.3.0/lib/metacerberus_hmm.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,71 +60,74 @@
     return outlist
 
 
 # Filter HMM results
 def filterHMM(hmm_tsv:Path, outfile:Path, dbpath:Path):
     outfile.parent.mkdir(parents=True, exist_ok=True)
 
-    hmm,key = hmm_tsv.stem.split(sep='-', maxsplit=1)
-    if hmm in ['COG', 'CAZy', 'PHROG', 'VOG']:
-        lookup_list = [hmm]
-    else:
-        lookup_list = ['KEGG']
-
-    with outfile.open('w') as writer, outfile.with_suffix('.log').open('w') as logger:
-        for name in lookup_list:
-            dbLookup = Path(dbpath, f"{name}-onto_rel1.tsv").read_text()
-            BH_target = dict()
-            with open(hmm_tsv, "r") as reader:
-                for i,line in enumerate(reader, 1):
-                    line = line.split('\t')
-                    try:
-                        target = line[0]
-                        query = line[1]
-                        e_value = float(line[2])
-                        score = float(line[3])
-                        length = int(line[4])
-                        start = int(line[5])
-                        end = int(line[6])
-                    except:
-                        print("Failed to read line:", i, hmm_tsv, file=logger)
-                        continue
-                    # Check if Query is in the Database
-                    if not re.search(query, dbLookup, re.MULTILINE):
-                        continue
-
-                    # Count Proper Hits
-                    # 1) Overlapping: Count best score
-                    # 2) Unique: Count both
-                    if target not in BH_target:
-                        BH_target[target] = [(query, e_value, score, length, start, end)]
-                    else: # More than one match/target
-                        #keys = list(BH_target[target].keys())
-                        item = (query, e_value, score, length, start, end)
-                        add = False
-                        overlap = False
-                        for c,match in enumerate(BH_target[target]):
-                            # Check for overlap
-                            if start <= match[5] and end >= match[4]:
-                                overlap_len = min(end, match[5]) - max(start, match[4])
-                                if overlap_len > 10:
-                                    # Winner takes all
-                                    overlap = True
-                                    if score == match[2]:
-                                        add = True
-                                    elif score > match[2]:
-                                        BH_target[target][c] = item
-                                else:
-                                    #print("NO OVERLAP:", overlap_len, file=logger)
-                                    pass
-                        if add or not overlap:
-                            # Equal score OR Dual domain
-                            BH_target[target] += [item]
-                    # next line
-                    continue
-            # Write filtered overlaps to file
-            for target in sorted(BH_target):
-                for match in set(BH_target[target]):
-                    query, e_value, score, length, start, end = match
-                    print(target, query, e_value, score, length, start, end, sep='\t', file=writer)
+    for i in range(1, len(dbpath.suffixes)):
+        dbpath = Path(dbpath.with_suffix(''))
+    dbLookup = dbpath.with_suffix('.tsv')
+    match = re.search(r"^KOFam_[a-z]+_([A-Z]+)", hmm_tsv.name)
+    if match:
+        dbLookup = dbpath.with_name(f'{match.group(1)}.tsv')
+    dbLookup = dbLookup.read_text()
+
+    BH_target = dict()
+    logfile = outfile.with_suffix('.log')
+    with hmm_tsv.open() as reader, logfile.open('w') as logger:
+        for i,line in enumerate(reader, 1):
+            line = line.split('\t')
+            try:
+                target = line[0]
+                query = line[1]
+                e_value = float(line[2])
+                score = float(line[3])
+                length = int(line[4])
+                start = int(line[5])
+                end = int(line[6])
+            except:
+                print("Failed to read line:", i, hmm_tsv, file=logger)
+                continue
+            # Check if Query is in the Database
+            if not re.search(query, dbLookup, re.MULTILINE):
+                continue
+            
+            # Count Proper Hits
+            # 1) Overlapping: Count best score
+            # 2) Unique: Count both
+            if target not in BH_target:
+                BH_target[target] = [(query, e_value, score, length, start, end)]
+            else: # More than one match/target
+                #keys = list(BH_target[target].keys())
+                item = (query, e_value, score, length, start, end)
+                add = False
+                overlap = False
+                for c,match in enumerate(BH_target[target]):
+                    # Check for overlap
+                    if start <= match[5] and end >= match[4]:
+                        overlap_len = min(end, match[5]) - max(start, match[4])
+                        if overlap_len > 10:
+                            overlap = True
+                            # Equal Score
+                            if e_value == match[1] and score == match[2]:
+                                add = True
+                            # Winner takes all
+                            elif e_value < match[1]:
+                                BH_target[target][c] = item
+                            elif e_value == match[1]:
+                                if score > match[2]:
+                                    BH_target[target][c] = item
+                if add or not overlap:
+                    # Equal score OR Dual domain
+                    BH_target[target] += [item]
+            # next line
+            continue
+    # Write filtered overlaps to file
+    with outfile.open('w') as writer:
+        print("target", "query", "e-value", "score", "length", "start", "end", sep='\t', file=writer)
+        for target in sorted(BH_target):
+            for match in set(BH_target[target]):
+                query, e_value, score, length, start, end = match
+                print(target, query, e_value, score, length, start, end, sep='\t', file=writer)
 
     return outfile
```

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_logo.jpg` & `metacerberus-1.3.0/lib/metacerberus_logo.jpg`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_metastats.py` & `metacerberus-1.3.0/lib/metacerberus_metastats.py`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_parser.py` & `metacerberus-1.3.0/lib/metacerberus_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,37 +6,110 @@
 """
 
 def warn(*args, **kwargs):
     pass
 import warnings
 warnings.warn = warn
 
-import os
+import re
 from pathlib import Path
 import pandas as pd
 
 
-def parseHmmer(hmm_tsv, config, subdir):
+def top5s(hmm_tsv:dict, outfile:Path):
+    outfile.parent.mkdir(0o777, True, True)
+
+    # Calculate Best Hit
+    BH_top5 = {}
+    for hmm,filename in hmm_tsv.items():
+        with open(filename, "r") as reader:
+            reader.readline()
+            for line in reader:
+                line = line.split('\t')
+                target = line[0]
+                query = line[1]
+                e_value = line[2]
+                score = float(line[3])
+                ec = '' #TODO: Match query to EC
+
+                # store top 5 per query
+                match = [target, query, ec, e_value, score, hmm]
+                if target not in BH_top5:
+                    BH_top5[target] = [match]
+                elif len(BH_top5[target]) < 5:
+                    BH_top5[target].append(match)
+                else:
+                    BH_top5[target].sort(key = lambda x: x[3], reverse=False)
+                    if score > float(BH_top5[target][0][3]):
+                        BH_top5[target][0] = match
+
+    # Save Top 5 hits tsv rollup
+    with outfile.open('w') as writer:
+        print("Target Name", "ID", "EC value", "E-Value (sequence)", "Score (domain)", "hmmDB", sep='\t', file=writer)
+        for target in sorted(BH_top5.keys()):
+            BH_top5[target].sort(key = lambda x: x[3], reverse=True)
+            for line in BH_top5[target]:
+                print(*line, sep='\t', file=writer)
+    return outfile
+
+
+def top5(hmm_tsv:Path, outfile:Path):
+    outfile.parent.mkdir(0o777, True, True)
+
+    # Calculate Best Hit
+    BH_top5 = {}
+    with open(hmm_tsv, "r") as reader:
+        reader.readline()
+        for line in reader:
+            line = line.split('\t')
+            target = line[0]
+            query = line[1]
+            e_value = line[2]
+            score = float(line[3])
+            ec = '' #TODO: Match query to EC
+
+            # store top 5 per query
+            match = [target, query, ec, e_value, score]
+            if target not in BH_top5:
+                BH_top5[target] = [match]
+            elif len(BH_top5[target]) < 5:
+                BH_top5[target].append(match)
+            else:
+                BH_top5[target].sort(key = lambda x: x[3], reverse=False)
+                if score > float(BH_top5[target][0][3]):
+                    BH_top5[target][0] = match
+
+    # Save Top 5 hits tsv rollup
+    with outfile.open('w') as writer:
+        print("Target Name", "ID", "EC value", "E-Value (sequence)", "Score (domain)", sep='\t', file=writer)
+        for target in sorted(BH_top5.keys()):
+            BH_top5[target].sort(key = lambda x: x[3], reverse=True)
+            for line in BH_top5[target]:
+                print(*line, sep='\t', file=writer)
+    return outfile
+
+
+def parseHmmer(hmm_tsv, config, subdir, dbname, dbpath):
     path = Path(config['DIR_OUT'], subdir)
     path.mkdir(exist_ok=True, parents=True)
 
-    done = path / "complete"
-    if not config['REPLACE'] and done.exists():
-        rollup_files = dict()
-        for name in ['FOAM', 'KEGG', 'COG', 'CAZy', 'PHROG', 'VOG']:
-            outfile = Path(path, f"HMMER_BH_{name}_rollup.tsv")
-            if outfile.exists():
-                rollup_files[name] = outfile
-        return rollup_files
-    done.unlink(missing_ok=True)
+    #done = path / "complete"
+    #if not config['REPLACE'] and done.exists():
+    #    print("AH CRAP!!!")
+    #    rollup_files = dict()
+    #    outfile = Path(path, f"HMMER_BH_{dbname}_rollup.tsv")
+    #    if outfile.exists():
+    #        rollup_files[name] = outfile
+    #        return rollup_files
+    #done.unlink(missing_ok=True)
 
 
     minscore = config["MINSCORE"]
 
-    top5File = Path(path, "HMMER_top_5.tsv")
+    top5File = Path(path, f"HMMER-{dbname}_top_5.tsv")
 
 
     # Calculate Best Hit
     BH_query = {}
     BH_top5 = {}
     #"target", "query", "e-value", "score", "length", "start", "end"
     with open(hmm_tsv, "r") as reader:
@@ -89,59 +162,61 @@
         IDs = [ID for ID in line[1].split(",")]
         for ID in IDs:
             if ID not in ID_counts:
                 ID_counts[ID] = 0
             ID_counts[ID] += 1
 
     # Write rollup files to disk
-
-    dbPath = Path(config['PATHDB'])
-    dfRollups = rollupAll(ID_counts, dbPath, path)
+    dbRollup = rollup(ID_counts, dbname, dbpath, path)
     rollup_files = dict()
-    for name,df in dfRollups.items():
-        if len(df.index) > 1:
-            outfile = Path(path, f"HMMER_BH_{name}_rollup.tsv")
-            df.to_csv(outfile, index=False, header=True, sep='\t')
-            rollup_files[name] = outfile
+    if len(dbRollup) > 1:
+        outfile = Path(path, f"HMMER_BH_{dbname}_rollup2.tsv")
+        with open(outfile, 'w') as writer:
+            for line in dbRollup:
+                print(*line, sep='\t', file=writer)
+        rollup_files[dbname] = outfile
 
-    done.touch()
+    #done.touch()
     return rollup_files
 
-######### Roll-Up All #########
-def rollupAll(COUNTS: dict, lookupPath: str, outpath: str):
-    dfLookup = dict()
-    dfRollup = dict()
-    count_file = dict()
-    for name in ['FOAM', 'KEGG', 'COG', 'CAZy', 'PHROG', 'VOG']:
-        count_file[name] = Path(outpath, f'counts_{name}.tsv').open('w')
-        print('ID', 'count', sep='\t', file=count_file[name])
-        dbPath = Path(lookupPath, f"{name}-onto_rel1.tsv")
-        dfLookup[name] = pd.read_csv(dbPath, sep='\t').fillna('')
-        dfRollup[name] = pd.DataFrame()
-
-    errfile = os.path.join(outpath, 'lookup.err')
-    with open(errfile, 'w') as errlog:
+######### Roll-Up #########
+def rollup(COUNTS:dict, dbname:str, dbpath:Path, outpath:str):
+    while(dbpath.suffixes):
+        dbpath = Path(dbpath.with_suffix(''))
+    dbpath = dbpath.with_suffix('.tsv')
+    if dbname.startswith("KOFam"):
+        match = re.search(r"KOFam_.*_([A-Z]+)", dbname).group(1)
+        dbpath = dbpath.with_name(f'{match}.tsv')
+
+    dbLookup = dict()
+    with open(dbpath) as reader:
+        cols = reader.readline().rstrip('\n').split('\t')
+        for line in reader:
+            line = line.rstrip('\n').split('\t')
+            ID = line[cols.index('ID')]    
+            if line[cols.index('Function')]:
+                if ID not in dbLookup:
+                    dbLookup[ID] = list()
+                dbLookup[ID] += [line]
+
+    dbRollup = [cols+['Count']]
+    count_file = Path(outpath, f'counts_{dbname}.tsv')
+    with count_file.open('w') as count_writer, Path(outpath, 'lookup.err').open('w') as errlog:
+        print('ID', 'count', sep='\t', file=count_writer)
         for ID,count in sorted(COUNTS.items()):
-            found = False
-            for name in ['FOAM', 'KEGG', 'COG', 'CAZy', 'PHROG', 'VOG']:
-                rows = pd.DataFrame(dfLookup[name][dfLookup[name].ID==ID])
-                if not rows.empty:
-                    found = True
-                    rows.drop(rows[rows['Function']==''].index, inplace=True)
-                    if rows.empty:
-                        print("WARNING:'", ID, "'Does not have a 'Function' in the Lookup File:", name, file=errlog)
-                        continue
-                    print(ID, count, sep='\t', file=count_file[name])
-                    rows['Count'] = count
-                    dfRollup[name] = pd.concat([dfRollup[name],rows])
-            if not found:
-                print("WARNING:'", ID, "'not found in any Lookup File", file=errlog)
+            if ID in dbLookup:
+                rows:list = dbLookup[ID]
+                print(ID, count, sep='\t', file=count_writer)
+                for row in rows:
+                    dbRollup += [row+[count]]
+            else:
+                print("WARNING:'", ID, "'not found in any Lookup File, or does not have a 'Function'", file=errlog)
                 continue
     
-    return dfRollup
+    return dbRollup
 
 
 ########## Counts Table #########
 def createCountTables(rollup_files:dict, config:dict, subdir: str):
     done = Path(config['DIR_OUT']) / subdir / "complete"
     dfCounts = dict()
```

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_qc.py` & `metacerberus-1.3.0/lib/metacerberus_qc.py`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_report.py` & `metacerberus-1.3.0/lib/metacerberus_report.py`

 * *Files 20% similar despite different names*

```diff
@@ -358,7 +358,113 @@
                     var event = document.createEvent("HTMLEvents");
                     event.initEvent("resize", true, false);
                     document.dispatchEvent(event);
                 }});""")
     with open(outfile, 'w') as writer:
         writer.write(doc.render())
     return
+
+
+# Save Annotated GFF and GenBank files
+#TODO: Add embl
+def write_datafiles(gff:Path, fasta:Path, amino:Path, summary:Path, out_gff:Path, out_genbank:Path):
+    gff_data = dict()
+    with out_gff.open('w') as writer_gff, out_gff.with_suffix(".gtf").open('w') as writer_gtf:
+        print("##gff-version 2", file=writer_gtf)
+        with open(gff) as read_gff, summary.open() as read_summary:
+            read_summary.readline()
+            for line in read_gff:
+                if line.startswith('#'):
+                    writer_gff.write(line)
+                else:
+                    data = line.split('\t')[0:8]
+                    summ = read_summary.readline().split('\t')
+                    attributes = [f"ID={summ[0]}", f"Name={summ[1]}",
+                                        f"Alias={summ[2]}", f"Dbxref={summ[3]}", f"evalue={summ[4]}",
+                                        f"product_start={summ[8]}", f"product_end={summ[9]}", f"product_length={summ[10]}"]
+                    print(*data, ';'.join(attributes), sep='\t', file=writer_gff)
+                    print(*data, ';'.join(attributes), sep='\t', file=writer_gtf)
+                    if data[0] not in gff_data:
+                        gff_data[data[0]] = list()
+                    att = dict()
+                    for a in attributes:
+                        a = a.split('=')
+                        att[a[0]] = a[1]
+                    gff_data[data[0]] += [data + [att]]
+        # Write contigs to end of GFF (ROARY compatible)
+        # Create GENBANK template
+        print("##FASTA", file=writer_gff)
+        with open(fasta) as read_fasta, out_genbank.open('w') as writer_gbk:
+            locus = False
+            line = read_fasta.readline()
+            while line:
+                if line.startswith(">"):
+                    writer_gff.write(line)
+                    locus = line.strip()[1:]
+                    print(f"{'LOCUS':<12}{locus}", file=writer_gbk)
+                    print(f"{'DEFINITION':<12}", file=writer_gbk)
+                    print(f"{'ACCESSION':<12}", file=writer_gbk)
+                    print(f"{'VERSION':<12}", file=writer_gbk)
+                    print(f"{'KEYWORDS':<12}", file=writer_gbk)
+                    print(f"{'SOURCE':<12}", file=writer_gbk)
+                    print(f"{'  ORGANISM':<12}", file=writer_gbk)
+                    print(f"{'REFERENCE':<12}1", file=writer_gbk)
+                    print(f"{'  AUTHORS':<12}", file=writer_gbk)
+                    print(f"{'  TITLE':<12}", file=writer_gbk)
+                    print(f"{'  JOURNAL':<12}", file=writer_gbk)
+                    print(f"{'  PUBMED':<12}", file=writer_gbk)
+                    print(f"{'COMMENT':<12}", file=writer_gbk)
+                    print(f"{'FEATURES':<21}Location/Qualifiers", file=writer_gbk)
+                    seq = list()
+                    line = read_fasta.readline()
+                    while line:
+                        if line.startswith(">"):
+                            break
+                        writer_gff.write(line)
+                        seq += [line.strip()]
+                        line = read_fasta.readline()
+                    seq = "".join(seq)
+                    locus = locus.split()[0]
+                    print(f'{"     source":<21}{f"1..{len(seq)}"}', file=writer_gbk)
+                    print(f'{"":<21}/organism=""', file=writer_gbk)
+                    if locus in gff_data:
+                        for data in gff_data[locus]:
+                            attributes = data[-1]
+                            start = data[3]
+                            end = data[4]
+                            print(f'{"     CDS":<21}{f"{start}..{end}"}', file=writer_gbk)
+                            print(f'{"":<21}/product="{attributes["Name"]}"', file=writer_gbk)
+                            print(f'{"":<21}/db_xref="{attributes["Dbxref"]}"', file=writer_gbk)
+                            translation = f'/translation="'
+                            seq_faa = []
+                            with open(amino) as read_faa:
+                                line_faa = read_faa.readline()
+                                while line_faa:
+                                    if line_faa.startswith(">"):
+                                        if attributes["ID"]  == line_faa.strip().split()[0][1:]:
+                                            line_faa = read_faa.readline()
+                                            while line_faa:
+                                                if line_faa.startswith(">"):
+                                                    break
+                                                seq_faa += [line_faa.strip()]
+                                                line_faa = read_faa.readline()
+                                    if len(seq_faa) > 0:
+                                        break
+                                    line_faa = read_faa.readline()
+                            translation += ''.join(seq_faa + ['"'])
+                            for i in range(0, len(translation), 48):
+                                print(f'{"":<21}{translation[i:i+48]}', file=writer_gbk)
+                    print(f'{"ORIGIN":<12}', file=writer_gbk)
+                    row = list()
+                    start = 1
+                    for s in range(0, len(seq), 10):
+                        row += [seq[s:s+10]]
+                        if len(row) == 6:
+                            print(f'{start:>9} {" ".join(row)}', file=writer_gbk)
+                            row = list()
+                            start += 60
+                    print(f'{start:>9} {" ".join(row)}', file=writer_gbk)
+                    print("//", file=writer_gbk)
+                    continue
+                line = read_fasta.readline()
+
+    return
```

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_trim.py` & `metacerberus-1.3.0/lib/metacerberus_trim.py`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/metacerberus_visual.py` & `metacerberus-1.3.0/lib/metacerberus_visual.py`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/plotly-2.0.0.min.js` & `metacerberus-1.3.0/lib/plotly-2.0.0.min.js`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/lib/style.css` & `metacerberus-1.3.0/lib/style.css`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.2.1/setup.py` & `metacerberus-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 
 # read long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MetaCerberus",
-    version="1.2.1",
+    version="1.3.0",
     author="Jose L. Figueroa III, Richard A. White III",
     author_email="jlfiguer@uncc.edu",
     description="Versatile Functional Ontology Assignments for Metagenomes via Hidden Markov Model (HMM) searching with environmental focus of shotgun meta'omics data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raw-lab/metacerberus",
     scripts=['bin/metacerberus.py',                                     # scripts to copy to 'bin' path
              'bin/ray-slurm-metacerberus.sh',
              'bin/pathview-metacerberus.R'],
     packages=['meta_cerberus'],                                         # list of packages, installed to site-packages folder
     package_dir=dict(meta_cerberus='lib'),                              # dict with 'package'='relative dir'
     package_data=dict(meta_cerberus=package_files('lib/')),             # add non-python data to package, relative paths
     license="BSD License",  # metadata
     platforms=['Unix'],     # metadata
-    classifiers=[           # This is the new updated way for metadata, but old way seems to still be used in some of the output
-        "Development Status :: 4 - Beta",
+    classifiers=[           # This is the new updated way for metadata (PyPi??), but old way seems to still be used in some of the output
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Operating System :: Unix",
@@ -46,13 +46,12 @@
     install_requires=[
             'setuptools',
             'ray',
             'metaomestats',
             'configargparse',
             'kaleido',
             'scikit-learn',
-            'pandas',
             'plotly',
             'psutil',
             'dominate',
             ],
 )
```

