# Comparing `tmp/sastadev-0.2.0.tar.gz` & `tmp/sastadev-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sastadev-0.2.0.tar", last modified: Fri Apr 26 09:02:22 2024, max compression
+gzip compressed data, was "sastadev-0.2.1.tar", last modified: Wed May 15 15:33:47 2024, max compression
```

## Comparing `sastadev-0.2.0.tar` & `sastadev-0.2.1.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.631200 sastadev-0.2.0/
--rw-r--r--   0 a3248526   (502) staff       (20)     1533 2023-05-09 07:39:30.000000 sastadev-0.2.0/LICENSE
--rw-r--r--   0 a3248526   (502) staff       (20)     3440 2024-04-26 09:02:22.630978 sastadev-0.2.0/PKG-INFO
--rw-r--r--   0 a3248526   (502) staff       (20)     3048 2023-12-06 08:36:28.000000 sastadev-0.2.0/README.md
--rw-r--r--   0 a3248526   (502) staff       (20)      375 2024-04-26 09:00:24.000000 sastadev-0.2.0/pyproject.toml
--rw-r--r--   0 a3248526   (502) staff       (20)       38 2024-04-26 09:02:22.631264 sastadev-0.2.0/setup.cfg
--rw-r--r--   0 a3248526   (502) staff       (20)      976 2024-04-26 09:00:36.000000 sastadev-0.2.0/setup.py
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.579544 sastadev-0.2.0/src/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.594257 sastadev-0.2.0/src/sastadev/
--rw-r--r--   0 a3248526   (502) staff       (20)    11603 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/ASTApostfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)    43549 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/CHAT_Annotation.py
--rw-r--r--   0 a3248526   (502) staff       (20)    22704 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/SAFreader.py
--rw-r--r--   0 a3248526   (502) staff       (20)     2303 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/SRFreader.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1163 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/STAPpostfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7260 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/Sziplus.py
--rw-r--r--   0 a3248526   (502) staff       (20)    10335 2023-11-09 09:41:57.000000 sastadev-0.2.0/src/sastadev/TARSPpostfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5863 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/TARSPscreening.py
--rw-r--r--   0 a3248526   (502) staff       (20)       64 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/__init__.py
--rw-r--r--   0 a3248526   (502) staff       (20)    62496 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/__main__.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3381 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/allresults.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3108 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/alpino.py
--rw-r--r--   0 a3248526   (502) staff       (20)     4850 2023-11-09 09:41:57.000000 sastadev-0.2.0/src/sastadev/alpinoparsing.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1480 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/anonymization.py
--rw-r--r--   0 a3248526   (502) staff       (20)    13788 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/asta_neo.py
--rw-r--r--   0 a3248526   (502) staff       (20)    14736 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/asta_queries.py
--rw-r--r--   0 a3248526   (502) staff       (20)    15340 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/astaforms.py
--rw-r--r--   0 a3248526   (502) staff       (20)      415 2024-03-27 15:52:57.000000 sastadev-0.2.0/src/sastadev/auchannsettings.py
--rw-r--r--   0 a3248526   (502) staff       (20)    25155 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/basicreplacements.py
--rw-r--r--   0 a3248526   (502) staff       (20)    11294 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/celexlexicon.py
--rw-r--r--   0 a3248526   (502) staff       (20)     8474 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/chatundo.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3667 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/checkcorrection.py
--rw-r--r--   0 a3248526   (502) staff       (20)     9671 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/cleanCHILDEStokens.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3613 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/compounds.py
--rw-r--r--   0 a3248526   (502) staff       (20)      783 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/conf.py
--rw-r--r--   0 a3248526   (502) staff       (20)      494 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/constants.py
--rw-r--r--   0 a3248526   (502) staff       (20)    60201 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/corrector.py
--rw-r--r--   0 a3248526   (502) staff       (20)    44303 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/correcttreebank.py
--rw-r--r--   0 a3248526   (502) staff       (20)      770 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/counterfunctions.py
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.596117 sastadev-0.2.0/src/sastadev/data/
--rw-r--r--   0 a3248526   (502) staff       (20)     5819 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/DutchIrregularVerbs.tsv
--rw-r--r--   0 a3248526   (502) staff       (20)     1562 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/anonymization.json
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.579852 sastadev-0.2.0/src/sastadev/data/celexlexicon/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.610416 sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/
--rw-r--r--   0 a3248526   (502) staff       (20) 10433870 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DMLCD.txt
--rw-r--r--   0 a3248526   (502) staff       (20) 11540324 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt
--rw-r--r--   0 a3248526   (502) staff       (20)  4092534 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DSLCD.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.617302 sastadev-0.2.0/src/sastadev/data/compoundfiles/
--rw-r--r--   0 a3248526   (502) staff       (20)  4216927 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt
--rw-r--r--   0 a3248526   (502) staff       (20)  1403658 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt
--rw-r--r--   0 a3248526   (502) staff       (20)   332732 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip
--rw-r--r--   0 a3248526   (502) staff       (20)      390 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/expandedqueries.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.620892 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/
--rw-r--r--   0 a3248526   (502) staff       (20)      145 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/filledpauseslexicon.txt
--rw-r--r--   0 a3248526   (502) staff       (20)      495 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/notanalyzewords.txt
--rw-r--r--   0 a3248526   (502) staff       (20)      113 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/oldfilledpauseslexicon.txt
--rw-r--r--   0 a3248526   (502) staff       (20)       60 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/vuwordslexicon.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.621409 sastadev-0.2.0/src/sastadev/data/form_templates/
--rw-r--r--   0 a3248526   (502) staff       (20)    48437 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    13350 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/form_templates/TARSP Form Current.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)   159165 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/inflectioncorrection.tsv.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.622289 sastadev-0.2.0/src/sastadev/data/macros/
--rw-r--r--   0 a3248526   (502) staff       (20)    12994 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/macros/newimperatives.txt
--rw-r--r--   0 a3248526   (502) staff       (20)      388 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/macros/newrobusthwwi.txt
--rw-r--r--   0 a3248526   (502) staff       (20)    23141 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/macros/sastamacros1.txt
--rw-r--r--   0 a3248526   (502) staff       (20)    10375 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/macros/sastamacros2.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.623706 sastadev-0.2.0/src/sastadev/data/methods/
--rw-r--r--   0 a3248526   (502) staff       (20)    12471 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/methods/ASTA_07062021.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    12824 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/methods/ASTA_Index_Current.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    12808 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/methods/ASTA_Index_Current_old.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    17518 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/methods/STAP_07062021.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    17537 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/methods/STAP_Index_Current.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    25892 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    26318 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/methods/TARSP_07062021.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    25871 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/methods/TARSP_Index_Current.xlsx
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.624636 sastadev-0.2.0/src/sastadev/data/names/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.626880 sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/
--rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv
--rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv
--rw-r--r--   0 a3248526   (502) staff       (20)    66586 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.627905 sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/
--rw-r--r--   0 a3248526   (502) staff       (20)  1088716 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml
--rw-r--r--   0 a3248526   (502) staff       (20)     1442 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl
--rw-r--r--   0 a3248526   (502) staff       (20)   134136 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1.zip
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.628229 sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/
--rw-r--r--   0 a3248526   (502) staff       (20)     8762 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv
--rw-r--r--   0 a3248526   (502) staff       (20)     7950 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.628387 sastadev-0.2.0/src/sastadev/data/names/nameparts/
--rw-r--r--   0 a3248526   (502) staff       (20)   104652 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/nameparts/namepartlexicon.csv
--rw-r--r--   0 a3248526   (502) staff       (20)  2160410 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/voornamentop10000.xml
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.628611 sastadev-0.2.0/src/sastadev/data/nochildwords/
--rw-r--r--   0 a3248526   (502) staff       (20)        5 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/nochildwords/nochildwords.txt
--rw-r--r--   0 a3248526   (502) staff       (20)   108483 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/old_inflectioncorrection.tsv.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.628755 sastadev-0.2.0/src/sastadev/data/top3000/
--rw-r--r--   0 a3248526   (502) staff       (20)   187619 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/top3000/Woordenlijsten Current.xlsx
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.629015 sastadev-0.2.0/src/sastadev/data/wordsunknowntoalpino/
--rw-r--r--   0 a3248526   (502) staff       (20)      140 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/wordsunknowntoalpino/wordsunknowntoalpino.txt
--rw-r--r--   0 a3248526   (502) staff       (20)    35888 2023-11-09 09:41:57.000000 sastadev-0.2.0/src/sastadev/dedup.py
--rw-r--r--   0 a3248526   (502) staff       (20)    24636 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/deregularise.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7380 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/exampletrees.py
--rw-r--r--   0 a3248526   (502) staff       (20)      993 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/expandquery.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3793 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/external_functions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1630 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/filefunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     9032 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/find_ngram.py
--rw-r--r--   0 a3248526   (502) staff       (20)      473 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/forms.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6814 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/generatemacros.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5251 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/goldcountreader.py
--rw-r--r--   0 a3248526   (502) staff       (20)    17456 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/iedims.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5607 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/imperatives.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1366 2024-04-16 10:12:10.000000 sastadev-0.2.0/src/sastadev/imply.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6653 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/lexicon.py
--rw-r--r--   0 a3248526   (502) staff       (20)    18574 2024-03-27 15:55:43.000000 sastadev-0.2.0/src/sastadev/longqueries.py
--rw-r--r--   0 a3248526   (502) staff       (20)      959 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/macrolength.py
--rw-r--r--   0 a3248526   (502) staff       (20)     2831 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/macros.py
--rw-r--r--   0 a3248526   (502) staff       (20)      321 2024-04-16 09:53:39.000000 sastadev-0.2.0/src/sastadev/memoize.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6478 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/metadata.py
--rw-r--r--   0 a3248526   (502) staff       (20)      583 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/methodinfo.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7016 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/methods.py
--rw-r--r--   0 a3248526   (502) staff       (20)    14928 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/mismatches.py
--rw-r--r--   0 a3248526   (502) staff       (20)     9027 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/mksilver.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1542 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/mwe2pep.py
--rw-r--r--   0 a3248526   (502) staff       (20)    60916 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/mysastadev.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1462 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/namepartlexicon.py
--rw-r--r--   0 a3248526   (502) staff       (20)    17785 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/normalise_lemma.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1028 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/phonetics.py
--rw-r--r--   0 a3248526   (502) staff       (20)        0 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/py.typed
--rw-r--r--   0 a3248526   (502) staff       (20)     2276 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/query.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6157 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/queryfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3281 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/rawalpinoparsing.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1718 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/readcsv.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7826 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/readmethod.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7720 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/reduceresults.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1954 2024-03-27 15:58:14.000000 sastadev-0.2.0/src/sastadev/resultsbyutterance.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1599 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/rpf1.py
--rw-r--r--   0 a3248526   (502) staff       (20)    14312 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/sasta_explanation.py
--rw-r--r--   0 a3248526   (502) staff       (20)    13568 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/sastacore.py
--rw-r--r--   0 a3248526   (502) staff       (20)     2988 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/sastatok.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1975 2024-04-16 08:16:53.000000 sastadev-0.2.0/src/sastadev/sastatoken.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3243 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/sastatypes.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1329 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/sentence_parser.py
--rw-r--r--   0 a3248526   (502) staff       (20)    13555 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/smallclauses.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3869 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/smartcompoundcomparison.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3540 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/stapforms.py
--rw-r--r--   0 a3248526   (502) staff       (20)    16421 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/stringfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)    31189 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/sva.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6564 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/syllablecount.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1614 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/targets.py
--rw-r--r--   0 a3248526   (502) staff       (20)     4846 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/tarspform.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6435 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/tblex.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1475 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/tokeniseCHILDES.py
--rw-r--r--   0 a3248526   (502) staff       (20)      880 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/tokenmd.py
--rw-r--r--   0 a3248526   (502) staff       (20)     4341 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/top3000.py
--rw-r--r--   0 a3248526   (502) staff       (20)    81828 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/treebankfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)      299 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/tryderegularize.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1108 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/tryexcelfilter.py
--rw-r--r--   0 a3248526   (502) staff       (20)      561 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/trygaatie.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1076 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/update_inflectioncorrection.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1994 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/vuandnonwords.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1523 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/vunonwordlexicons.py
--rw-r--r--   0 a3248526   (502) staff       (20)     2117 2024-04-24 10:52:29.000000 sastadev-0.2.0/src/sastadev/xenx.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5144 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/xlsx.py
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.594992 sastadev-0.2.0/src/sastadev.egg-info/
--rw-r--r--   0 a3248526   (502) staff       (20)     3440 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/PKG-INFO
--rw-r--r--   0 a3248526   (502) staff       (20)     5234 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/SOURCES.txt
--rw-r--r--   0 a3248526   (502) staff       (20)        1 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/dependency_links.txt
--rw-r--r--   0 a3248526   (502) staff       (20)       52 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/entry_points.txt
--rw-r--r--   0 a3248526   (502) staff       (20)       51 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/requires.txt
--rw-r--r--   0 a3248526   (502) staff       (20)        9 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/top_level.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:23.202918 sastadev-0.2.0/tests/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:25.294840 sastadev-0.2.0/tests/__pycache__/
--rw-r--r--   0 a3248526   (502) staff       (20)    15132 2024-04-26 09:02:23.206920 sastadev-0.2.0/tests/__pycache__/test_adjacency.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     1316 2024-04-26 09:02:23.235139 sastadev-0.2.0/tests/__pycache__/test_explanation.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     2655 2024-04-26 09:02:24.739838 sastadev-0.2.0/tests/__pycache__/test_hyphens.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     7255 2024-04-26 09:02:24.740787 sastadev-0.2.0/tests/__pycache__/test_indexexpansion.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     6907 2024-04-26 09:02:24.742413 sastadev-0.2.0/tests/__pycache__/test_lxml.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     2145 2024-04-26 09:02:24.744441 sastadev-0.2.0/tests/__pycache__/test_smallclauses.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)    15020 2024-04-26 09:02:25.294693 sastadev-0.2.0/tests/__pycache__/test_vobij.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)    13386 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_adjacency.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1438 2024-04-26 09:00:24.000000 sastadev-0.2.0/tests/test_explanation.py
--rw-r--r--   0 a3248526   (502) staff       (20)      634 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_hyphens.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6946 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_indexexpansion.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7187 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_lxml.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1971 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_smallclauses.py
--rw-r--r--   0 a3248526   (502) staff       (20)    14153 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_vobij.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.831775 sastadev-0.2.1/
+-rw-r--r--   0 a3248526   (502) staff       (20)     1533 2023-05-09 07:39:30.000000 sastadev-0.2.1/LICENSE
+-rw-r--r--   0 a3248526   (502) staff       (20)     3440 2024-05-15 15:33:47.831604 sastadev-0.2.1/PKG-INFO
+-rw-r--r--   0 a3248526   (502) staff       (20)     3048 2023-12-06 08:36:28.000000 sastadev-0.2.1/README.md
+-rw-r--r--   0 a3248526   (502) staff       (20)      375 2024-04-26 09:00:24.000000 sastadev-0.2.1/pyproject.toml
+-rw-r--r--   0 a3248526   (502) staff       (20)       38 2024-05-15 15:33:47.831830 sastadev-0.2.1/setup.cfg
+-rw-r--r--   0 a3248526   (502) staff       (20)      976 2024-05-15 15:33:25.000000 sastadev-0.2.1/setup.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.752740 sastadev-0.2.1/src/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.778994 sastadev-0.2.1/src/sastadev/
+-rw-r--r--   0 a3248526   (502) staff       (20)    11603 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/ASTApostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    43549 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/CHAT_Annotation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    19031 2024-05-15 15:33:25.000000 sastadev-0.2.1/src/sastadev/SAFreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2303 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/SRFreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1163 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/STAPpostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7260 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/Sziplus.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    10335 2023-11-09 09:41:57.000000 sastadev-0.2.1/src/sastadev/TARSPpostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5863 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/TARSPscreening.py
+-rw-r--r--   0 a3248526   (502) staff       (20)       64 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/__init__.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    62496 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/__main__.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3381 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/allresults.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3108 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/alpino.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4850 2023-11-09 09:41:57.000000 sastadev-0.2.1/src/sastadev/alpinoparsing.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1480 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/anonymization.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13788 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/asta_neo.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14736 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/asta_queries.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    15340 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/astaforms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      415 2024-03-27 15:52:57.000000 sastadev-0.2.1/src/sastadev/auchannsettings.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    25155 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/basicreplacements.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    11294 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/celexlexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     8474 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/chatundo.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3667 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/checkcorrection.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9671 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/cleanCHILDEStokens.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3613 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/compounds.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      783 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/conf.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      494 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/constants.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    60201 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/corrector.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    44303 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/correcttreebank.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      770 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/counterfunctions.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.781121 sastadev-0.2.1/src/sastadev/data/
+-rw-r--r--   0 a3248526   (502) staff       (20)     5819 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/DutchIrregularVerbs.tsv
+-rw-r--r--   0 a3248526   (502) staff       (20)     1562 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/anonymization.json
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.752958 sastadev-0.2.1/src/sastadev/data/celexlexicon/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.799470 sastadev-0.2.1/src/sastadev/data/celexlexicon/dutch/
+-rw-r--r--   0 a3248526   (502) staff       (20) 10433870 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/celexlexicon/dutch/DMLCD.txt
+-rw-r--r--   0 a3248526   (502) staff       (20) 11540324 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)  4092534 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/celexlexicon/dutch/DSLCD.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.811381 sastadev-0.2.1/src/sastadev/data/compoundfiles/
+-rw-r--r--   0 a3248526   (502) staff       (20)  4216927 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)  1403658 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)   332732 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip
+-rw-r--r--   0 a3248526   (502) staff       (20)      390 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/expandedqueries.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.815187 sastadev-0.2.1/src/sastadev/data/filledpauseslexicon/
+-rw-r--r--   0 a3248526   (502) staff       (20)      145 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/filledpauseslexicon/filledpauseslexicon.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)      495 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/filledpauseslexicon/notanalyzewords.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)      113 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/filledpauseslexicon/oldfilledpauseslexicon.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)       60 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/filledpauseslexicon/vuwordslexicon.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.815693 sastadev-0.2.1/src/sastadev/data/form_templates/
+-rw-r--r--   0 a3248526   (502) staff       (20)    48437 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    13350 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/form_templates/TARSP Form Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)   159165 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/inflectioncorrection.tsv.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.816377 sastadev-0.2.1/src/sastadev/data/macros/
+-rw-r--r--   0 a3248526   (502) staff       (20)    12994 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/macros/newimperatives.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)      388 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/macros/newrobusthwwi.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)    23141 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/macros/sastamacros1.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)    10375 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/macros/sastamacros2.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.818509 sastadev-0.2.1/src/sastadev/data/methods/
+-rw-r--r--   0 a3248526   (502) staff       (20)    12471 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/methods/ASTA_07062021.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    12824 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/methods/ASTA_Index_Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    12808 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/methods/ASTA_Index_Current_old.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    17518 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/methods/STAP_07062021.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    17537 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/methods/STAP_Index_Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    25892 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    26318 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/methods/TARSP_07062021.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    25871 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/methods/TARSP_Index_Current.xlsx
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.819500 sastadev-0.2.1/src/sastadev/data/names/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.825711 sastadev-0.2.1/src/sastadev/data/names/Woonplaatsen/
+-rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)    66586 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.827908 sastadev-0.2.1/src/sastadev/data/names/fn10k_versie1/
+-rw-r--r--   0 a3248526   (502) staff       (20)  1088716 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml
+-rw-r--r--   0 a3248526   (502) staff       (20)     1442 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl
+-rw-r--r--   0 a3248526   (502) staff       (20)   134136 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/fn10k_versie1.zip
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.828360 sastadev-0.2.1/src/sastadev/data/names/hoofdsteden/
+-rw-r--r--   0 a3248526   (502) staff       (20)     8762 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)     7950 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.828549 sastadev-0.2.1/src/sastadev/data/names/nameparts/
+-rw-r--r--   0 a3248526   (502) staff       (20)   104652 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/nameparts/namepartlexicon.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)  2160410 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/data/names/voornamentop10000.xml
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.828811 sastadev-0.2.1/src/sastadev/data/nochildwords/
+-rw-r--r--   0 a3248526   (502) staff       (20)        5 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/nochildwords/nochildwords.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)   108483 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/old_inflectioncorrection.tsv.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.828969 sastadev-0.2.1/src/sastadev/data/top3000/
+-rw-r--r--   0 a3248526   (502) staff       (20)   187619 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/top3000/Woordenlijsten Current.xlsx
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.829221 sastadev-0.2.1/src/sastadev/data/wordsunknowntoalpino/
+-rw-r--r--   0 a3248526   (502) staff       (20)      140 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/data/wordsunknowntoalpino/wordsunknowntoalpino.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)    35888 2023-11-09 09:41:57.000000 sastadev-0.2.1/src/sastadev/dedup.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    24636 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/deregularise.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7380 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/exampletrees.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      993 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/expandquery.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3793 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/external_functions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1630 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/filefunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9032 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/find_ngram.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      473 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/forms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6814 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/generatemacros.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5251 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/goldcountreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    17456 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/iedims.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5607 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/imperatives.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1366 2024-04-16 10:12:10.000000 sastadev-0.2.1/src/sastadev/imply.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6653 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/lexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    18574 2024-03-27 15:55:43.000000 sastadev-0.2.1/src/sastadev/longqueries.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      959 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/macrolength.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2831 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/macros.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      321 2024-04-16 09:53:39.000000 sastadev-0.2.1/src/sastadev/memoize.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6478 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/metadata.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      583 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/methodinfo.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7016 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/methods.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14928 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/mismatches.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9027 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/mksilver.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1542 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/mwe2pep.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    60916 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/mysastadev.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1462 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/namepartlexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    17785 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/normalise_lemma.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1028 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/phonetics.py
+-rw-r--r--   0 a3248526   (502) staff       (20)        0 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/py.typed
+-rw-r--r--   0 a3248526   (502) staff       (20)     2276 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/query.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6157 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/queryfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3281 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/rawalpinoparsing.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1718 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/readcsv.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7826 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/readmethod.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7720 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/reduceresults.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1954 2024-03-27 15:58:14.000000 sastadev-0.2.1/src/sastadev/resultsbyutterance.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1599 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/rpf1.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14312 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/sasta_explanation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13568 2024-05-15 13:22:51.000000 sastadev-0.2.1/src/sastadev/sastacore.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2988 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/sastatok.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1975 2024-04-16 08:16:53.000000 sastadev-0.2.1/src/sastadev/sastatoken.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3243 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/sastatypes.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1329 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/sentence_parser.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13555 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/smallclauses.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3869 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/smartcompoundcomparison.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3540 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/stapforms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    16421 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/stringfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    31189 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/sva.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6564 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/syllablecount.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1614 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/targets.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4846 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/tarspform.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6435 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/tblex.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1475 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/tokeniseCHILDES.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      880 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/tokenmd.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4341 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/top3000.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    81828 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/treebankfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      299 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/tryderegularize.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1108 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/tryexcelfilter.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      561 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/trygaatie.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1076 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/update_inflectioncorrection.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1994 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/vuandnonwords.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1523 2024-04-26 09:00:24.000000 sastadev-0.2.1/src/sastadev/vunonwordlexicons.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2117 2024-04-24 10:52:29.000000 sastadev-0.2.1/src/sastadev/xenx.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5144 2023-08-29 13:46:10.000000 sastadev-0.2.1/src/sastadev/xlsx.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:47.779815 sastadev-0.2.1/src/sastadev.egg-info/
+-rw-r--r--   0 a3248526   (502) staff       (20)     3440 2024-05-15 15:33:47.000000 sastadev-0.2.1/src/sastadev.egg-info/PKG-INFO
+-rw-r--r--   0 a3248526   (502) staff       (20)     5234 2024-05-15 15:33:47.000000 sastadev-0.2.1/src/sastadev.egg-info/SOURCES.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)        1 2024-05-15 15:33:47.000000 sastadev-0.2.1/src/sastadev.egg-info/dependency_links.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)       52 2024-05-15 15:33:47.000000 sastadev-0.2.1/src/sastadev.egg-info/entry_points.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)       51 2024-05-15 15:33:47.000000 sastadev-0.2.1/src/sastadev.egg-info/requires.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)        9 2024-05-15 15:33:47.000000 sastadev-0.2.1/src/sastadev.egg-info/top_level.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:48.473412 sastadev-0.2.1/tests/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-05-15 15:33:50.722478 sastadev-0.2.1/tests/__pycache__/
+-rw-r--r--   0 a3248526   (502) staff       (20)    15132 2024-05-15 15:33:48.479396 sastadev-0.2.1/tests/__pycache__/test_adjacency.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     1316 2024-05-15 15:33:48.520056 sastadev-0.2.1/tests/__pycache__/test_explanation.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     2655 2024-05-15 15:33:50.132898 sastadev-0.2.1/tests/__pycache__/test_hyphens.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     7255 2024-05-15 15:33:50.134261 sastadev-0.2.1/tests/__pycache__/test_indexexpansion.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     6907 2024-05-15 15:33:50.136545 sastadev-0.2.1/tests/__pycache__/test_lxml.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     2145 2024-05-15 15:33:50.140087 sastadev-0.2.1/tests/__pycache__/test_smallclauses.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)    15020 2024-05-15 15:33:50.722224 sastadev-0.2.1/tests/__pycache__/test_vobij.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)    13386 2023-08-29 13:46:10.000000 sastadev-0.2.1/tests/test_adjacency.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1438 2024-04-26 09:00:24.000000 sastadev-0.2.1/tests/test_explanation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      634 2023-08-29 13:46:10.000000 sastadev-0.2.1/tests/test_hyphens.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6946 2023-08-29 13:46:10.000000 sastadev-0.2.1/tests/test_indexexpansion.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7187 2023-08-29 13:46:10.000000 sastadev-0.2.1/tests/test_lxml.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1971 2023-08-29 13:46:10.000000 sastadev-0.2.1/tests/test_smallclauses.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14153 2023-08-29 13:46:10.000000 sastadev-0.2.1/tests/test_vobij.py
```

### Comparing `sastadev-0.2.0/LICENSE` & `sastadev-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/PKG-INFO` & `sastadev-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sastadev
-Version: 0.2.0
+Version: 0.2.1
 Summary: Linguistic functions for SASTA tool
 Home-page: https://github.com/UUDigitalHumanitieslab/sastadev
 Author: Research Software Lab - Centre for Digital Humanities - Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: BSD-3-Clause
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `sastadev-0.2.0/README.md` & `sastadev-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/setup.py` & `sastadev-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name='sastadev',
-    version='0.2.0',
+    version='0.2.1',
     description='Linguistic functions for SASTA tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/UUDigitalHumanitieslab/sastadev',
     author='Research Software Lab - Centre for Digital Humanities - Utrecht University',
     author_email='digitalhumanities@uu.nl',
     package_dir={'': 'src'},
```

### Comparing `sastadev-0.2.0/src/sastadev/ASTApostfunctions.py` & `sastadev-0.2.1/src/sastadev/ASTApostfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/CHAT_Annotation.py` & `sastadev-0.2.1/src/sastadev/CHAT_Annotation.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/SAFreader.py` & `sastadev-0.2.1/src/sastadev/SAFreader.py`

 * *Files 11% similar despite different names*

```diff
@@ -158,112 +158,14 @@
             cleanlevel = clean(thelevel)
             result = (cleanlevel, cleanlabel)
             results.append(result)
 
     return results
 
 
-def oldget_annotations(infilename: FileName, patterns: Tuple[Pattern, Pattern]) \
-        -> Tuple[UttWordDict, Dict[Tuple[Level, Item], List[Tuple[UttId, Position]]]]:
-    '''
-    Reads the file with name filename in SASTA Annotation Format
-    :param infilename:
-    :param patterns
-    :return: a dictionary  with as  key a tuple (level, item) and as value a list of (uttid, tokenposition) pairs
-    '''
-
-    thedata = defaultdict(list)
-
-    allutts = {}
-
-    # To open Workbook
-    header, data = xlsx.getxlsxdata(infilename)
-
-    levelcol = 1
-    uttidcol = 0
-    stagescol = -1
-    commentscol = -1
-    unalignedcol = -1
-
-    # uttlevel = 'utt'
-
-    uttcount = 0
-
-    for col, val in enumerate(header):
-        if iswordcolumn(val):
-            lastwordcol = col
-            if isfirstwordcolumn(val):
-                firstwordcol = col
-        elif clean(val) in speakerheaders:
-            spkcol = col
-        elif clean(val) in uttidheaders:
-            uttidcol = col
-        elif clean(val) in levelheaders:
-            levelcol = col
-        elif clean(val) in stagesheaders:
-            stagescol = col
-        elif clean(val) in commentsheaders:
-            commentscol = col
-        elif clean(val) in unalignedheaders:
-            unalignedcol = col
-        else:
-            pass  # maybe warn here that an unknow column header has been encountered?
-
-    for row in data:
-        if row[uttidcol] != "":
-            # this might go wrong if there is no integer there @@make it robust
-            uttid = str(int(row[uttidcol]))
-        thelevel = row[levelcol]
-        thelevel = clean(thelevel)
-        all_levels.add(thelevel)
-        # if thelevel == uttlevel:
-        #    uttcount += 1
-        curuttwlist = []
-        for colctr in range(firstwordcol, len(row)):
-            if thelevel.lower() in uttidheaders:
-                rawcurcellval = str(row[colctr])
-                curcellval = getname(rawcurcellval)
-                if curcellval != '':
-                    curuttwlist.append(curcellval)
-            elif thelevel in literallevels and colctr != stagescol and colctr != commentscol:
-                rawthelabel = str(row[colctr])
-                thelabel = getname(rawthelabel)
-                if colctr > lastwordcol:
-                    tokenposition = 0
-                else:
-                    tokenposition = colctr - firstwordcol + 1
-                cleanlevel = thelevel
-                cleanlabel = thelabel
-                if cleanlabel != '':
-                    thedata[(cleanlevel, cleanlabel)].append(
-                        (uttid, tokenposition))
-            elif not isuttlevel(thelevel) and colctr != stagescol and colctr != commentscol:
-                thelabelstr = row[colctr]
-                thelevel = row[levelcol]
-                if colctr == unalignedcol:
-                    prefix = ''
-                if lastwordcol + 1 <= colctr < len(row):
-                    # prefix = headers[colctr] aangepast om het simpeler te houden
-                    prefix = ""
-                else:
-                    prefix = ""
-                cleanlevelsandlabels = getcleanlevelsandlabels(
-                    thelabelstr, thelevel, prefix, patterns)
-                if colctr > lastwordcol or colctr == unalignedcol:
-                    tokenposition = 0
-                else:
-                    tokenposition = colctr - firstwordcol + 1
-                for (cleanlevel, cleanlabel) in cleanlevelsandlabels:
-                    thedata[(cleanlevel, cleanlabel)].append(
-                        (uttid, tokenposition))
-        if curuttwlist != []:
-            allutts[uttid] = curuttwlist
-    return allutts, thedata
-
-
 def get_annotations(infilename: FileName, allitems: List[str], themethod: Method) \
         -> Tuple[UttWordDict, Dict[Tuple[Level, Item], List[Tuple[UttId, Position]]]]:
     '''
     Reads the file with name filename in SASTA Annotation Format
     :param infilename:
     :param allitems: list of all valid items
     :param themethod: the method
@@ -303,25 +205,27 @@
         elif clean(val) in commentsheaders:
             commentscol = col
         elif clean(val) in unalignedheaders:
             unalignedcol = col
         else:
             pass  # maybe warn here that an unknow column header has been encountered?
 
+    startcol = min(
+        [col for col in [firstwordcol, unalignedcol, commentscol, stagescol]])
     for row in data:
         if row[uttidcol] != "":
             # this might go wrong if there is no integer there @@make it robust
             uttid = str(int(row[uttidcol]))
         thelevel = row[levelcol]
         thelevel = clean(thelevel)
         all_levels.add(thelevel)
         # if thelevel == uttlevel:
         #    uttcount += 1
         curuttwlist = []
-        for colctr in range(firstwordcol, len(row)):
+        for colctr in range(startcol, len(row)):
             if thelevel.lower() in uttidheaders:
                 rawcurcellval = str(row[colctr])
                 curcellval = getname(rawcurcellval)
                 if curcellval != '':
                     curuttwlist.append(curcellval)
             elif thelevel in literallevels and colctr != stagescol and colctr != commentscol:
                 rawthelabel = str(row[colctr])
```

### Comparing `sastadev-0.2.0/src/sastadev/SRFreader.py` & `sastadev-0.2.1/src/sastadev/SRFreader.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/STAPpostfunctions.py` & `sastadev-0.2.1/src/sastadev/STAPpostfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/Sziplus.py` & `sastadev-0.2.1/src/sastadev/Sziplus.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/TARSPpostfunctions.py` & `sastadev-0.2.1/src/sastadev/TARSPpostfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/TARSPscreening.py` & `sastadev-0.2.1/src/sastadev/TARSPscreening.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/__main__.py` & `sastadev-0.2.1/src/sastadev/__main__.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/allresults.py` & `sastadev-0.2.1/src/sastadev/allresults.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/alpino.py` & `sastadev-0.2.1/src/sastadev/alpino.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/alpinoparsing.py` & `sastadev-0.2.1/src/sastadev/alpinoparsing.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/anonymization.py` & `sastadev-0.2.1/src/sastadev/anonymization.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/asta_neo.py` & `sastadev-0.2.1/src/sastadev/asta_neo.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/asta_queries.py` & `sastadev-0.2.1/src/sastadev/asta_queries.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/astaforms.py` & `sastadev-0.2.1/src/sastadev/astaforms.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/basicreplacements.py` & `sastadev-0.2.1/src/sastadev/basicreplacements.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/celexlexicon.py` & `sastadev-0.2.1/src/sastadev/celexlexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/chatundo.py` & `sastadev-0.2.1/src/sastadev/chatundo.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/checkcorrection.py` & `sastadev-0.2.1/src/sastadev/checkcorrection.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/cleanCHILDEStokens.py` & `sastadev-0.2.1/src/sastadev/cleanCHILDEStokens.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/compounds.py` & `sastadev-0.2.1/src/sastadev/compounds.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/conf.py` & `sastadev-0.2.1/src/sastadev/conf.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/corrector.py` & `sastadev-0.2.1/src/sastadev/corrector.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/correcttreebank.py` & `sastadev-0.2.1/src/sastadev/correcttreebank.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/counterfunctions.py` & `sastadev-0.2.1/src/sastadev/counterfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/DutchIrregularVerbs.tsv` & `sastadev-0.2.1/src/sastadev/data/DutchIrregularVerbs.tsv`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/anonymization.json` & `sastadev-0.2.1/src/sastadev/data/anonymization.json`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DMLCD.txt` & `sastadev-0.2.1/src/sastadev/data/celexlexicon/dutch/DMLCD.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt` & `sastadev-0.2.1/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DSLCD.txt` & `sastadev-0.2.1/src/sastadev/data/celexlexicon/dutch/DSLCD.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt` & `sastadev-0.2.1/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt` & `sastadev-0.2.1/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip` & `sastadev-0.2.1/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx` & `sastadev-0.2.1/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/form_templates/TARSP Form Current.xlsx` & `sastadev-0.2.1/src/sastadev/data/form_templates/TARSP Form Current.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/inflectioncorrection.tsv.txt` & `sastadev-0.2.1/src/sastadev/data/inflectioncorrection.tsv.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/macros/newimperatives.txt` & `sastadev-0.2.1/src/sastadev/data/macros/newimperatives.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/macros/sastamacros1.txt` & `sastadev-0.2.1/src/sastadev/data/macros/sastamacros1.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/macros/sastamacros2.txt` & `sastadev-0.2.1/src/sastadev/data/macros/sastamacros2.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/methods/ASTA_07062021.xlsx` & `sastadev-0.2.1/src/sastadev/data/methods/ASTA_07062021.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/methods/ASTA_Index_Current.xlsx` & `sastadev-0.2.1/src/sastadev/data/methods/ASTA_Index_Current.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/methods/ASTA_Index_Current_old.xlsx` & `sastadev-0.2.1/src/sastadev/data/methods/ASTA_Index_Current_old.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/methods/STAP_07062021.xlsx` & `sastadev-0.2.1/src/sastadev/data/methods/STAP_07062021.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/methods/STAP_Index_Current.xlsx` & `sastadev-0.2.1/src/sastadev/data/methods/STAP_Index_Current.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx` & `sastadev-0.2.1/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/methods/TARSP_07062021.xlsx` & `sastadev-0.2.1/src/sastadev/data/methods/TARSP_07062021.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/methods/TARSP_Index_Current.xlsx` & `sastadev-0.2.1/src/sastadev/data/methods/TARSP_Index_Current.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv` & `sastadev-0.2.1/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv` & `sastadev-0.2.1/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv` & `sastadev-0.2.1/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml` & `sastadev-0.2.1/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl` & `sastadev-0.2.1/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1.zip` & `sastadev-0.2.1/src/sastadev/data/names/fn10k_versie1.zip`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv` & `sastadev-0.2.1/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt` & `sastadev-0.2.1/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/nameparts/namepartlexicon.csv` & `sastadev-0.2.1/src/sastadev/data/names/nameparts/namepartlexicon.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/names/voornamentop10000.xml` & `sastadev-0.2.1/src/sastadev/data/names/voornamentop10000.xml`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/old_inflectioncorrection.tsv.txt` & `sastadev-0.2.1/src/sastadev/data/old_inflectioncorrection.tsv.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/data/top3000/Woordenlijsten Current.xlsx` & `sastadev-0.2.1/src/sastadev/data/top3000/Woordenlijsten Current.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/dedup.py` & `sastadev-0.2.1/src/sastadev/dedup.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/deregularise.py` & `sastadev-0.2.1/src/sastadev/deregularise.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/exampletrees.py` & `sastadev-0.2.1/src/sastadev/exampletrees.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/expandquery.py` & `sastadev-0.2.1/src/sastadev/expandquery.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/external_functions.py` & `sastadev-0.2.1/src/sastadev/external_functions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/filefunctions.py` & `sastadev-0.2.1/src/sastadev/filefunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/find_ngram.py` & `sastadev-0.2.1/src/sastadev/find_ngram.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/generatemacros.py` & `sastadev-0.2.1/src/sastadev/generatemacros.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/goldcountreader.py` & `sastadev-0.2.1/src/sastadev/goldcountreader.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/iedims.py` & `sastadev-0.2.1/src/sastadev/iedims.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/imperatives.py` & `sastadev-0.2.1/src/sastadev/imperatives.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/imply.py` & `sastadev-0.2.1/src/sastadev/imply.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/lexicon.py` & `sastadev-0.2.1/src/sastadev/lexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/longqueries.py` & `sastadev-0.2.1/src/sastadev/longqueries.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/macrolength.py` & `sastadev-0.2.1/src/sastadev/macrolength.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/macros.py` & `sastadev-0.2.1/src/sastadev/macros.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/metadata.py` & `sastadev-0.2.1/src/sastadev/metadata.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/methodinfo.py` & `sastadev-0.2.1/src/sastadev/methodinfo.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/methods.py` & `sastadev-0.2.1/src/sastadev/methods.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/mismatches.py` & `sastadev-0.2.1/src/sastadev/mismatches.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/mksilver.py` & `sastadev-0.2.1/src/sastadev/mksilver.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/mwe2pep.py` & `sastadev-0.2.1/src/sastadev/mwe2pep.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/mysastadev.py` & `sastadev-0.2.1/src/sastadev/mysastadev.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/namepartlexicon.py` & `sastadev-0.2.1/src/sastadev/namepartlexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/normalise_lemma.py` & `sastadev-0.2.1/src/sastadev/normalise_lemma.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/phonetics.py` & `sastadev-0.2.1/src/sastadev/phonetics.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/query.py` & `sastadev-0.2.1/src/sastadev/query.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/queryfunctions.py` & `sastadev-0.2.1/src/sastadev/queryfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/rawalpinoparsing.py` & `sastadev-0.2.1/src/sastadev/rawalpinoparsing.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/readcsv.py` & `sastadev-0.2.1/src/sastadev/readcsv.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/readmethod.py` & `sastadev-0.2.1/src/sastadev/readmethod.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/reduceresults.py` & `sastadev-0.2.1/src/sastadev/reduceresults.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/resultsbyutterance.py` & `sastadev-0.2.1/src/sastadev/resultsbyutterance.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/rpf1.py` & `sastadev-0.2.1/src/sastadev/rpf1.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/sasta_explanation.py` & `sastadev-0.2.1/src/sastadev/sasta_explanation.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/sastacore.py` & `sastadev-0.2.1/src/sastadev/sastacore.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/sastatok.py` & `sastadev-0.2.1/src/sastadev/sastatok.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/sastatoken.py` & `sastadev-0.2.1/src/sastadev/sastatoken.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/sastatypes.py` & `sastadev-0.2.1/src/sastadev/sastatypes.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/sentence_parser.py` & `sastadev-0.2.1/src/sastadev/sentence_parser.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/smallclauses.py` & `sastadev-0.2.1/src/sastadev/smallclauses.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/smartcompoundcomparison.py` & `sastadev-0.2.1/src/sastadev/smartcompoundcomparison.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/stapforms.py` & `sastadev-0.2.1/src/sastadev/stapforms.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/stringfunctions.py` & `sastadev-0.2.1/src/sastadev/stringfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/sva.py` & `sastadev-0.2.1/src/sastadev/sva.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/syllablecount.py` & `sastadev-0.2.1/src/sastadev/syllablecount.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/targets.py` & `sastadev-0.2.1/src/sastadev/targets.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/tarspform.py` & `sastadev-0.2.1/src/sastadev/tarspform.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/tblex.py` & `sastadev-0.2.1/src/sastadev/tblex.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/tokeniseCHILDES.py` & `sastadev-0.2.1/src/sastadev/tokeniseCHILDES.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/tokenmd.py` & `sastadev-0.2.1/src/sastadev/tokenmd.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/top3000.py` & `sastadev-0.2.1/src/sastadev/top3000.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/treebankfunctions.py` & `sastadev-0.2.1/src/sastadev/treebankfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/tryexcelfilter.py` & `sastadev-0.2.1/src/sastadev/tryexcelfilter.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/trygaatie.py` & `sastadev-0.2.1/src/sastadev/trygaatie.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/update_inflectioncorrection.py` & `sastadev-0.2.1/src/sastadev/update_inflectioncorrection.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/vuandnonwords.py` & `sastadev-0.2.1/src/sastadev/vuandnonwords.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/vunonwordlexicons.py` & `sastadev-0.2.1/src/sastadev/vunonwordlexicons.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/xenx.py` & `sastadev-0.2.1/src/sastadev/xenx.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev/xlsx.py` & `sastadev-0.2.1/src/sastadev/xlsx.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/src/sastadev.egg-info/PKG-INFO` & `sastadev-0.2.1/src/sastadev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sastadev
-Version: 0.2.0
+Version: 0.2.1
 Summary: Linguistic functions for SASTA tool
 Home-page: https://github.com/UUDigitalHumanitieslab/sastadev
 Author: Research Software Lab - Centre for Digital Humanities - Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: BSD-3-Clause
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `sastadev-0.2.0/src/sastadev.egg-info/SOURCES.txt` & `sastadev-0.2.1/src/sastadev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/tests/__pycache__/test_adjacency.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.1/tests/__pycache__/test_adjacency.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 13386 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -875,15 +875,15 @@
 000036a0: 019b 0064 029d 0383 027d 027c 0253 0029  ...d.....}.|.S.)
 000036b0: 034e 7a0e 2f2f 6e6f 6465 5b40 776f 7264  .Nz.//node[@word
 000036c0: 3d22 7a02 225d 2901 7204 0000 0029 035a  ="z."]).r....).Z
 000036d0: 0573 7472 6565 da04 776f 7264 da06 7265  .stree..word..re
 000036e0: 7375 6c74 a900 720c 0000 00fa 4b2f 5573  sult..r.....K/Us
 000036f0: 6572 732f 6133 3234 3835 3236 2f67 6974  ers/a3248526/git
 00003700: 2f73 6173 7461 6465 765f 7061 636b 6167  /sastadev_packag
-00003710: 652f 7361 7374 6164 6576 2d30 2e32 2e30  e/sastadev-0.2.0
+00003710: 652f 7361 7374 6164 6576 2d30 2e32 2e31  e/sastadev-0.2.1
 00003720: 2f74 6573 7473 2f74 6573 745f 6164 6a61  /tests/test_adja
 00003730: 6365 6e63 792e 7079 da07 6765 746e 6f64  cency.py..getnod
 00003740: 6583 0000 0073 0400 0000 0001 1201 720e  e....s........r.
 00003750: 0000 00da 0269 735a 056e 6f67 616c 5429  .....isZ.nogalT)
 00003760: 0172 0f00 0000 2901 7a12 2528 7079 3029  .r....).z.%(py0)
 00003770: 7320 6973 2025 2870 7933 2973 720b 0000  s is %(py3)sr...
 00003780: 0029 02da 0370 7930 da03 7079 337a 0e61  .)...py0..py3z.a
```

### Comparing `sastadev-0.2.0/tests/__pycache__/test_explanation.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.1/tests/__pycache__/test_explanation.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 26 09:00:24 2024 UTC, .py size: 1438 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 00000340: 6e6c 6973 745a 1370 6f73 7465 7870 6c61  nlistZ.postexpla
 00000350: 6e61 7469 6f6e 6c69 7374 5a0e 6578 706c  nationlistZ.expl
 00000360: 616e 6174 696f 6e73 7472 5a09 616c 6967  anationstrZ.alig
 00000370: 6e6d 656e 74a9 0072 1100 0000 fa4d 2f55  nment..r.....M/U
 00000380: 7365 7273 2f61 3332 3438 3532 362f 6769  sers/a3248526/gi
 00000390: 742f 7361 7374 6164 6576 5f70 6163 6b61  t/sastadev_packa
 000003a0: 6765 2f73 6173 7461 6465 762d 302e 322e  ge/sastadev-0.2.
-000003b0: 302f 7465 7374 732f 7465 7374 5f65 7870  0/tests/test_exp
+000003b0: 312f 7465 7374 732f 7465 7374 5f65 7870  1/tests/test_exp
 000003c0: 6c61 6e61 7469 6f6e 2e70 79da 0474 6573  lanation.py..tes
 000003d0: 7410 0000 0073 2400 0000 0003 0401 0a01  t....s$.........
 000003e0: 0801 0401 0801 0803 0c02 0c01 0601 0e01  ................
 000003f0: 1a02 0801 0c02 0401 0801 0201 1cff 7213  ..............r.
 00000400: 0000 00da 085f 5f6d 6169 6e5f 5f29 13da  .....__main__)..
 00000410: 0862 7569 6c74 696e 73da 0c40 7079 5f62  .builtins..@py_b
 00000420: 7569 6c74 696e 73da 195f 7079 7465 7374  uiltins.._pytest
```

### Comparing `sastadev-0.2.0/tests/__pycache__/test_hyphens.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.1/tests/__pycache__/test_hyphens.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 634 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 00000870: 795f 666f 726d 6174 3130 5a0b 4070 795f  y_format10Z.@py_
 00000880: 6173 7365 7274 345a 0b40 7079 5f61 7373  assert4Z.@py_ass
 00000890: 6572 7437 5a0b 4070 795f 666f 726d 6174  ert7Z.@py_format
 000008a0: 395a 0c40 7079 5f66 6f72 6d61 7431 31a9  9Z.@py_format11.
 000008b0: 0072 1500 0000 fa49 2f55 7365 7273 2f61  .r.....I/Users/a
 000008c0: 3332 3438 3532 362f 6769 742f 7361 7374  3248526/git/sast
 000008d0: 6164 6576 5f70 6163 6b61 6765 2f73 6173  adev_package/sas
-000008e0: 7461 6465 762d 302e 322e 302f 7465 7374  tadev-0.2.0/test
+000008e0: 7461 6465 762d 302e 322e 312f 7465 7374  tadev-0.2.1/test
 000008f0: 732f 7465 7374 5f68 7970 6865 6e73 2e70  s/test_hyphens.p
 00000900: 79da 0474 6573 7405 0000 0073 7e00 0000  y..test....s~...
 00000910: 0002 0400 0800 0c00 0800 0400 5600 0c00  ............V...
 00000920: 0e00 1001 0400 0a00 0400 0800 0600 7c00  ..............|.
 00000930: 0c00 0e00 1001 0400 0a00 0400 0800 0600  ................
 00000940: 8000 0c00 0e00 1001 0400 0a00 0400 0800  ................
 00000950: 0600 8000 0c00 0e00 1001 0400 0a00 0600  ................
```

### Comparing `sastadev-0.2.0/tests/__pycache__/test_indexexpansion.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.1/tests/__pycache__/test_indexexpansion.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 6946 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 000016f0: 0119 00a1 0193 0271 0453 00a9 0029 0372  .......q.S...).r
 00001700: 0200 0000 da0a 6672 6f6d 7374 7269 6e67  ......fromstring
 00001710: da0c 7374 7265 6573 7472 696e 6773 2902  ..streestrings).
 00001720: da02 2e30 da01 6972 0600 0000 7206 0000  ...0..ir....r...
 00001730: 00fa 502f 5573 6572 732f 6133 3234 3835  ..P/Users/a32485
 00001740: 3236 2f67 6974 2f73 6173 7461 6465 765f  26/git/sastadev_
 00001750: 7061 636b 6167 652f 7361 7374 6164 6576  package/sastadev
-00001760: 2d30 2e32 2e30 2f74 6573 7473 2f74 6573  -0.2.0/tests/tes
+00001760: 2d30 2e32 2e31 2f74 6573 7473 2f74 6573  -0.2.1/tests/tes
 00001770: 745f 696e 6465 7865 7870 616e 7369 6f6e  t_indexexpansion
 00001780: 2e70 79da 0a3c 6469 6374 636f 6d70 3e42  .py..<dictcomp>B
 00001790: 0000 0073 0600 0000 0600 0200 0200 720c  ...s..........r.
 000017a0: 0000 007a 1774 6573 7420 636f 6465 2064  ...z.test code d
 000017b0: 6f65 7320 6e6f 7420 776f 726b 2901 da06  oes not work)...
 000017c0: 7265 6173 6f6e 6300 0000 0000 0000 0000  reasonc.........
 000017d0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
```

### Comparing `sastadev-0.2.0/tests/__pycache__/test_lxml.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.1/tests/__pycache__/test_lxml.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 7187 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 00000250: 7265 7375 6c74 735a 0a6e 6f64 6572 6573  resultsZ.noderes
 00000260: 756c 7472 0f00 0000 da03 706f 735a 0670  ultr......posZ.p
 00000270: 6f73 6361 7472 1100 0000 7212 0000 00da  oscatr....r.....
 00000280: 0672 6573 756c 74a9 0072 1b00 0000 fa46  .result..r.....F
 00000290: 2f55 7365 7273 2f61 3332 3438 3532 362f  /Users/a3248526/
 000002a0: 6769 742f 7361 7374 6164 6576 5f70 6163  git/sastadev_pac
 000002b0: 6b61 6765 2f73 6173 7461 6465 762d 302e  kage/sastadev-0.
-000002c0: 322e 302f 7465 7374 732f 7465 7374 5f6c  2.0/tests/test_l
+000002c0: 322e 312f 7465 7374 732f 7465 7374 5f6c  2.1/tests/test_l
 000002d0: 786d 6c2e 7079 da0a 6765 7472 6573 756c  xml.py..getresul
 000002e0: 7473 2000 0000 7316 0000 0000 010a 0104  ts ...s.........
 000002f0: 0108 010a 010a 0110 010a 010a 010a 010c  ................
 00000300: 0172 1d00 0000 6300 0000 0000 0000 0000  .r....c.........
 00000310: 0000 000f 0000 0009 0000 0043 0000 0073  ...........C...s
 00000320: d801 0000 6700 7d00 7c00 a000 6401 a101  ....g.}.|...d...
 00000330: 0100 7c00 a000 6402 a101 0100 7c00 a000  ..|...d.....|...
```

### Comparing `sastadev-0.2.0/tests/__pycache__/test_smallclauses.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.1/tests/__pycache__/test_smallclauses.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 1971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 00000200: 06da 026f 73da 0470 6174 68da 046a 6f69  ...os..path..joi
 00000210: 6e72 0c00 0000 da08 4441 5441 524f 4f54  nr......DATAROOT
 00000220: 7202 0000 0029 035a 0764 6174 6173 6574  r....).Z.dataset
 00000230: da08 6669 6c65 6e61 6d65 da06 7265 7375  ..filename..resu
 00000240: 6c74 a900 7213 0000 00fa 4e2f 5573 6572  lt..r.....N/User
 00000250: 732f 6133 3234 3835 3236 2f67 6974 2f73  s/a3248526/git/s
 00000260: 6173 7461 6465 765f 7061 636b 6167 652f  astadev_package/
-00000270: 7361 7374 6164 6576 2d30 2e32 2e30 2f74  sastadev-0.2.0/t
+00000270: 7361 7374 6164 6576 2d30 2e32 2e31 2f74  sastadev-0.2.1/t
 00000280: 6573 7473 2f74 6573 745f 736d 616c 6c63  ests/test_smallc
 00000290: 6c61 7573 6573 2e70 79da 0567 6574 666e  lauses.py..getfn
 000002a0: 0b00 0000 7304 0000 0000 0114 0172 1500  ....s........r..
 000002b0: 0000 5a06 7363 7465 7374 7a13 736d 616c  ..Z.sctestz.smal
 000002c0: 6c63 6c61 7573 6574 6573 742e 786d 6c5a  lclausetest.xmlZ
 000002d0: 0b73 6368 6c69 6368 7469 6e67 7a0e 5441  .schlichtingz.TA
 000002e0: 5256 4232 5f49 4432 2e78 6d6c 5a09 6d69  RVB2_ID2.xmlZ.mi
```

### Comparing `sastadev-0.2.0/tests/__pycache__/test_vobij.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.1/tests/__pycache__/test_vobij.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 14153 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -830,15 +830,15 @@
 000033d0: 0000 6900 7c00 5d14 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
 000033e0: 7400 a001 7c02 a101 9302 7104 5300 a900  t...|.....q.S...
 000033f0: 2902 7202 0000 00da 0a66 726f 6d73 7472  ).r......fromstr
 00003400: 696e 6729 03da 022e 30da 0169 da02 7473  ing)....0..i..ts
 00003410: 7208 0000 0072 0800 0000 fa47 2f55 7365  r....r.....G/Use
 00003420: 7273 2f61 3332 3438 3532 362f 6769 742f  rs/a3248526/git/
 00003430: 7361 7374 6164 6576 5f70 6163 6b61 6765  sastadev_package
-00003440: 2f73 6173 7461 6465 762d 302e 322e 302f  /sastadev-0.2.0/
+00003440: 2f73 6173 7461 6465 762d 302e 322e 312f  /sastadev-0.2.1/
 00003450: 7465 7374 732f 7465 7374 5f76 6f62 696a  tests/test_vobij
 00003460: 2e70 79da 0a3c 6469 6374 636f 6d70 3e8e  .py..<dictcomp>.
 00003470: 0000 0073 0600 0000 0600 0600 0200 720e  ...s..........r.
 00003480: 0000 005a 0234 305a 0233 3063 0000 0000  ...Z.40Z.30c....
 00003490: 0000 0000 0000 0000 0800 0000 0b00 0000  ................
 000034a0: 4300 0000 73e0 0100 0074 00a0 01a1 0044  C...s....t.....D
 000034b0: 0090 015d d05c 027d 007d 0164 0164 0284  ...].\.}.}.d.d..
```

### Comparing `sastadev-0.2.0/tests/test_adjacency.py` & `sastadev-0.2.1/tests/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/tests/test_explanation.py` & `sastadev-0.2.1/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/tests/test_hyphens.py` & `sastadev-0.2.1/tests/test_hyphens.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/tests/test_indexexpansion.py` & `sastadev-0.2.1/tests/test_indexexpansion.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/tests/test_lxml.py` & `sastadev-0.2.1/tests/test_lxml.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/tests/test_smallclauses.py` & `sastadev-0.2.1/tests/test_smallclauses.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.2.0/tests/test_vobij.py` & `sastadev-0.2.1/tests/test_vobij.py`

 * *Files identical despite different names*

