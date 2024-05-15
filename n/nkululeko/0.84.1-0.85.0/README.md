# Comparing `tmp/nkululeko-0.84.1.tar.gz` & `tmp/nkululeko-0.85.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.84.1.tar", last modified: Mon May 13 11:54:13 2024, max compression
+gzip compressed data, was "nkululeko-0.85.0.tar", last modified: Wed May 15 15:35:32 2024, max compression
```

## Comparing `nkululeko-0.84.1.tar` & `nkululeko-0.85.0.tar`

### file list

```diff
@@ -1,226 +1,227 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.058281 nkululeko-0.84.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17692 2024-05-13 11:53:35.000000 nkululeko-0.84.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.84.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36420 2024-05-13 11:54:13.058281 nkululeko-0.84.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.84.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.038281 nkululeko-0.84.1/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.84.1/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.84.1/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.84.1/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.84.1/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.84.1/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.84.1/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.84.1/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.84.1/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.84.1/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.84.1/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.84.1/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.84.1/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.84.1/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.84.1/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.84.1/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.84.1/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.84.1/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.84.1/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.84.1/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.84.1/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.84.1/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.84.1/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.84.1/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.84.1/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.038281 nkululeko-0.84.1/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.84.1/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.038281 nkululeko-0.84.1/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.84.1/meta/demos/demo_best_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.84.1/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.84.1/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.84.1/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.050281 nkululeko-0.84.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.84.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.84.1/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.84.1/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.050281 nkululeko-0.84.1/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.84.1/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.84.1/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.84.1/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.84.1/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.84.1/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.050281 nkululeko-0.84.1/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.84.1/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.84.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-13 11:53:50.000000 nkululeko-0.84.1/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.050281 nkululeko-0.84.1/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.84.1/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.84.1/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.84.1/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.84.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.84.1/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.84.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30225 2024-05-03 12:01:47.000000 nkululeko-0.84.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.84.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.84.1/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.84.1/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4576 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_whisper.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.84.1/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.84.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.84.1/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.84.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.84.1/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.84.1/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.84.1/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.84.1/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9288 2024-04-25 13:02:38.000000 nkululeko-0.84.1/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.84.1/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4910 2024-05-13 09:34:11.000000 nkululeko-0.84.1/nkululeko/models/finetune_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11601 2024-05-03 14:31:11.000000 nkululeko-0.84.1/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.84.1/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.84.1/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.84.1/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.84.1/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.84.1/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.84.1/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9854 2024-05-03 14:29:13.000000 nkululeko-0.84.1/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.84.1/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.84.1/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.84.1/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.84.1/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.84.1/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.84.1/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.84.1/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.84.1/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.84.1/nkululeko/nkuluflag.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.84.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/predict.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.84.1/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.84.1/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.84.1/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.84.1/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.84.1/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.84.1/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.84.1/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3354 2024-05-13 11:40:51.000000 nkululeko-0.84.1/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.84.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.84.1/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.84.1/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.84.1/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.84.1/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.84.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.84.1/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8131 2024-05-13 09:34:11.000000 nkululeko-0.84.1/nkululeko/test_pretrain.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.84.1/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.84.1/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13816 2024-05-13 11:40:51.000000 nkululeko-0.84.1/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36420 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5135 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.84.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-13 11:54:13.058281 nkululeko-0.84.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.84.1/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.038281 nkululeko-0.84.1/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.84.1/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17771 2024-05-15 15:10:15.000000 nkululeko-0.85.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.85.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36499 2024-05-15 15:35:31.997574 nkululeko-0.85.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.85.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.985575 nkululeko-0.85.0/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.85.0/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.85.0/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.85.0/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.85.0/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.85.0/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.85.0/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.85.0/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.85.0/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.85.0/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.85.0/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.85.0/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.85.0/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.85.0/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.85.0/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.85.0/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.85.0/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.85.0/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.85.0/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.85.0/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.85.0/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.85.0/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.85.0/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.85.0/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.85.0/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.85.0/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.85.0/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.85.0/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.85.0/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.85.0/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.85.0/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.985575 nkululeko-0.85.0/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.85.0/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.985575 nkululeko-0.85.0/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.989575 nkululeko-0.85.0/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.85.0/meta/demos/demo_best_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.85.0/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.85.0/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.85.0/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.993575 nkululeko-0.85.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.85.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.85.0/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.85.0/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.993575 nkululeko-0.85.0/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.85.0/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.85.0/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.85.0/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.85.0/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.85.0/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.993575 nkululeko-0.85.0/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.85.0/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.85.0/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.85.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-15 15:10:33.000000 nkululeko-0.85.0/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.993575 nkululeko-0.85.0/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.85.0/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.85.0/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.85.0/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.85.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.85.0/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.85.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30465 2024-05-15 15:09:05.000000 nkululeko-0.85.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.85.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.85.0/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.85.0/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-05-15 15:09:05.000000 nkululeko-0.85.0/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.85.0/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.85.0/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.85.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.85.0/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.85.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.85.0/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.85.0/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.85.0/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.85.0/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10464 2024-05-15 15:09:05.000000 nkululeko-0.85.0/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.85.0/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5091 2024-05-15 15:09:05.000000 nkululeko-0.85.0/nkululeko/models/finetune_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11639 2024-05-15 15:09:05.000000 nkululeko-0.85.0/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.85.0/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.85.0/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.85.0/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.85.0/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.85.0/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.85.0/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9854 2024-05-03 14:29:13.000000 nkululeko-0.85.0/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.85.0/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.85.0/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.85.0/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.85.0/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.85.0/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    15650 2024-05-15 15:09:05.000000 nkululeko-0.85.0/nkululeko/models/model_tuned.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.85.0/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.85.0/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.85.0/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.85.0/nkululeko/nkuluflag.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.85.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.85.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.85.0/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.85.0/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.85.0/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.85.0/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.85.0/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.85.0/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.85.0/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.85.0/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3354 2024-05-13 11:40:51.000000 nkululeko-0.85.0/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.85.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.85.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.85.0/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.85.0/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.85.0/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.85.0/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.85.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.85.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.85.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8465 2024-05-15 15:09:05.000000 nkululeko-0.85.0/nkululeko/test_pretrain.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.85.0/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.85.0/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.85.0/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13816 2024-05-13 11:40:51.000000 nkululeko-0.85.0/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36499 2024-05-15 15:35:31.000000 nkululeko-0.85.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5167 2024-05-15 15:35:31.000000 nkululeko-0.85.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-15 15:35:31.000000 nkululeko-0.85.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-15 15:35:31.000000 nkululeko-0.85.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-15 15:35:31.000000 nkululeko-0.85.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.85.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-15 15:35:31.997574 nkululeko-0.85.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.85.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.985575 nkululeko-0.85.0/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-15 15:35:31.997574 nkululeko-0.85.0/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.85.0/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.84.1/CHANGELOG.md` & `nkululeko-0.85.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.85.0
+--------------
+* first version with finetuning wav2vec2 layers
+
 Version 0.84.1
 --------------
 * made resample independent of config file
 
 Version 0.84.0
 --------------
 * added SHAP analysis
```

### Comparing `nkululeko-0.84.1/LICENSE` & `nkululeko-0.85.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/PKG-INFO` & `nkululeko-0.85.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.84.1
+Version: 0.85.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.85.0
+--------------
+* first version with finetuning wav2vec2 layers
+
 Version 0.84.1
 --------------
 * made resample independent of config file
 
 Version 0.84.0
 --------------
 * added SHAP analysis
```

### Comparing `nkululeko-0.84.1/README.md` & `nkululeko-0.85.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/aesdd/process_database.py` & `nkululeko-0.85.0/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/androids/process_database.py` & `nkululeko-0.85.0/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/androids_orig/process_database.py` & `nkululeko-0.85.0/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/androids_test/process_database.py` & `nkululeko-0.85.0/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/ased/process_database.py` & `nkululeko-0.85.0/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/asvp-esd/process_database.py` & `nkululeko-0.85.0/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/baved/process_database.py` & `nkululeko-0.85.0/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/cafe/process_database.py` & `nkululeko-0.85.0/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/clac/process_database.py` & `nkululeko-0.85.0/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/cmu-mosei/process_database.py` & `nkululeko-0.85.0/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/demos/process_database.py` & `nkululeko-0.85.0/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/ekorpus/process_database.py` & `nkululeko-0.85.0/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/emns/process_database.py` & `nkululeko-0.85.0/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/emofilm/convert_to_16k.py` & `nkululeko-0.85.0/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/emofilm/process_database.py` & `nkululeko-0.85.0/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/emorynlp/process_database.py` & `nkululeko-0.85.0/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/emov-db/process_database.py` & `nkululeko-0.85.0/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/emovo/process_database.py` & `nkululeko-0.85.0/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/emozionalmente/create.py` & `nkululeko-0.85.0/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/enterface/process_database.py` & `nkululeko-0.85.0/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/esd/process_database.py` & `nkululeko-0.85.0/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/gerparas/process_database.py` & `nkululeko-0.85.0/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/iemocap/process_database.py` & `nkululeko-0.85.0/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/jl/process_database.py` & `nkululeko-0.85.0/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/jtes/process_database.py` & `nkululeko-0.85.0/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/meld/process_database.py` & `nkululeko-0.85.0/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/mesd/process_database.py` & `nkululeko-0.85.0/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/mess/process_database.py` & `nkululeko-0.85.0/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/mlendsnd/process_database.py` & `nkululeko-0.85.0/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/msp-improv/process_database2.py` & `nkululeko-0.85.0/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/msp-podcast/process_database.py` & `nkululeko-0.85.0/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/oreau2/process_database.py` & `nkululeko-0.85.0/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/portuguese/process_database.py` & `nkululeko-0.85.0/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/ravdess/process_database.py` & `nkululeko-0.85.0/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/ravdess/process_database_speaker.py` & `nkululeko-0.85.0/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/savee/process_database.py` & `nkululeko-0.85.0/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/shemo/process_database.py` & `nkululeko-0.85.0/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/subesco/process_database.py` & `nkululeko-0.85.0/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/tess/process_database.py` & `nkululeko-0.85.0/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/thorsten-emotional/process_database.py` & `nkululeko-0.85.0/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/urdu/process_database.py` & `nkululeko-0.85.0/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/data/vivae/process_database.py` & `nkululeko-0.85.0/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/docs/source/conf.py` & `nkululeko-0.85.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/meta/demos/demo_best_model.py` & `nkululeko-0.85.0/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/meta/demos/my_experiment.py` & `nkululeko-0.85.0/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/meta/demos/my_experiment_local.py` & `nkululeko-0.85.0/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/meta/demos/plot_faster_anim.py` & `nkululeko-0.85.0/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/aug_train.py` & `nkululeko-0.85.0/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/augment.py` & `nkululeko-0.85.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/augmenting/augmenter.py` & `nkululeko-0.85.0/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.85.0/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.85.0/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/augmenting/resampler.py` & `nkululeko-0.85.0/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_age.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.85.0/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.85.0/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/cacheddataset.py` & `nkululeko-0.85.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/data/dataset.py` & `nkululeko-0.85.0/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/data/dataset_csv.py` & `nkululeko-0.85.0/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/demo.py` & `nkululeko-0.85.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/demo_feats.py` & `nkululeko-0.85.0/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/demo_predictor.py` & `nkululeko-0.85.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/experiment.py` & `nkululeko-0.85.0/nkululeko/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,20 @@
 
         The string FEATS.feats_type is read from the config, defaults to os.
 
         """
         df_train, df_test = self.df_train, self.df_test
         feats_name = "_".join(ast.literal_eval(glob_conf.config["DATA"]["databases"]))
         self.feats_test, self.feats_train = pd.DataFrame(), pd.DataFrame()
-        feats_types = self.util.config_val_list("FEATS", "type", ["os"])
+        feats_types = self.util.config_val_list("FEATS", "type", [])
+        # for some models no features are needed
+        if len(feats_types) == 0:
+            self.util.debug("no feature extractor specified.")
+            self.feats_train, self.feats_test = pd.DataFrame(), pd.DataFrame()
+            return
         self.feature_extractor = FeatureExtractor(
             df_train, feats_types, feats_name, "train"
         )
         self.feats_train = self.feature_extractor.extract()
         self.feature_extractor = FeatureExtractor(
             df_test, feats_types, feats_name, "test"
         )
```

### Comparing `nkululeko-0.84.1/nkululeko/explore.py` & `nkululeko-0.85.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/export.py` & `nkululeko-0.85.0/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_auddim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feats_whisper.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feats_whisper.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,30 +28,27 @@
 
     def init_model(self):
         # load model
         self.util.debug("loading whisper model...")
         model_name = f"openai/{self.feat_type}"
         self.model = WhisperModel.from_pretrained(model_name).to(self.device)
         print(f"intialized Whisper model on {self.device}")
-        self.feature_extractor = AutoFeatureExtractor.from_pretrained(
-            model_name)
+        self.feature_extractor = AutoFeatureExtractor.from_pretrained(model_name)
         self.model_initialized = True
 
     def extract(self):
         """Extract the features or load them from disk if present."""
         store = self.util.get_path("store")
         storage = f"{store}{self.name}.pkl"
-        extract = self.util.config_val(
-            "FEATS", "needs_feature_extraction", False)
+        extract = self.util.config_val("FEATS", "needs_feature_extraction", False)
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or no_reuse or not os.path.isfile(storage):
             if not self.model_initialized:
                 self.init_model()
-            self.util.debug(
-                "extracting whisper embeddings, this might take a while...")
+            self.util.debug("extracting whisper embeddings, this might take a while...")
             emb_series = []
             for (file, start, end), _ in audeer.progress_bar(
                 self.data_df.iterrows(),
                 total=len(self.data_df),
                 desc=f"Running whisper on {len(self.data_df)} audiofiles",
             ):
                 if end == pd.NaT:
```

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/featureset.py` & `nkululeko-0.85.0/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.85.0/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/feature_extractor.py` & `nkululeko-0.85.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/file_checker.py` & `nkululeko-0.85.0/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/filter_data.py` & `nkululeko-0.85.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/glob_conf.py` & `nkululeko-0.85.0/nkululeko/glob_conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/losses/loss_ccc.py` & `nkululeko-0.85.0/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.85.0/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/modelrunner.py` & `nkululeko-0.85.0/nkululeko/modelrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,60 +43,77 @@
             glob_conf.config["EXP"]["epochs"] = "1"
         patience = self.util.config_val("MODEL", "patience", False)
         patience_counter = -1
         if self.util.high_is_good():
             highest = 0
         else:
             highest = 100000
-        # for all epochs
-        for epoch in range(epoch_num):
-            if only_test:
-                self.model.load(self.run, epoch)
-                self.util.debug(f"reusing model: {self.model.store_path}")
-                self.model.reset_test(self.df_test, self.feats_test)
-            else:
-                self.model.set_id(self.run, epoch)
-                self.model.train()
+        if self.model.model_type == "finetuned":
+            # epochs are handled by Huggingface API
+            self.model.train()
             report = self.model.predict()
+            # todo: findout the best epoch
+            epoch = epoch_num
             report.set_id(self.run, epoch)
             plot_name = self.util.get_plot_name() + f"_{self.run}_{epoch:03d}_cnf"
             reports.append(report)
             self.util.debug(
                 f"run: {self.run} epoch: {epoch}: result: "
                 f"{reports[-1].get_result().get_test_result()}"
             )
             if plot_epochs:
                 self.util.debug(f"plotting conf matrix to {plot_name}")
                 report.plot_confmatrix(plot_name, epoch)
-            store_models = self.util.config_val("EXP", "save", False)
-            plot_best_model = self.util.config_val("PLOT", "best_model", False)
-            if (store_models or plot_best_model) and (
-                not only_test
-            ):  # in any case the model needs to be stored to disk.
-                self.model.store()
-            if patience:
-                patience = int(patience)
-                result = report.result.get_result()
-                if self.util.high_is_good():
-                    if result > highest:
-                        highest = result
-                        patience_counter = 0
-                    else:
-                        patience_counter += 1
+        else:
+            # for all epochs
+            for epoch in range(epoch_num):
+                if only_test:
+                    self.model.load(self.run, epoch)
+                    self.util.debug(f"reusing model: {self.model.store_path}")
+                    self.model.reset_test(self.df_test, self.feats_test)
                 else:
-                    if result < highest:
-                        highest = result
-                        patience_counter = 0
+                    self.model.set_id(self.run, epoch)
+                    self.model.train()
+                report = self.model.predict()
+                report.set_id(self.run, epoch)
+                plot_name = self.util.get_plot_name() + f"_{self.run}_{epoch:03d}_cnf"
+                reports.append(report)
+                self.util.debug(
+                    f"run: {self.run} epoch: {epoch}: result: "
+                    f"{reports[-1].get_result().get_test_result()}"
+                )
+                if plot_epochs:
+                    self.util.debug(f"plotting conf matrix to {plot_name}")
+                    report.plot_confmatrix(plot_name, epoch)
+                store_models = self.util.config_val("EXP", "save", False)
+                plot_best_model = self.util.config_val("PLOT", "best_model", False)
+                if (store_models or plot_best_model) and (
+                    not only_test
+                ):  # in any case the model needs to be stored to disk.
+                    self.model.store()
+                if patience:
+                    patience = int(patience)
+                    result = report.result.get_result()
+                    if self.util.high_is_good():
+                        if result > highest:
+                            highest = result
+                            patience_counter = 0
+                        else:
+                            patience_counter += 1
                     else:
-                        patience_counter += 1
-                if patience_counter >= patience:
-                    self.util.debug(
-                        f"reached patience ({str(patience)}): early stopping"
-                    )
-                    break
+                        if result < highest:
+                            highest = result
+                            patience_counter = 0
+                        else:
+                            patience_counter += 1
+                    if patience_counter >= patience:
+                        self.util.debug(
+                            f"reached patience ({str(patience)}): early stopping"
+                        )
+                        break
 
         if not plot_epochs:
             # Do at least one confusion matrix plot
             self.util.debug(f"plotting confusion matrix to {plot_name}")
             reports[-1].plot_confmatrix(plot_name, epoch)
         return reports, epoch
 
@@ -129,14 +146,20 @@
             )
         elif model_type == "bayes":
             from nkululeko.models.model_bayes import Bayes_model
 
             self.model = Bayes_model(
                 self.df_train, self.df_test, self.feats_train, self.feats_test
             )
+        elif model_type == "finetune":
+            from nkululeko.models.model_tuned import Pretrained_model
+
+            self.model = Pretrained_model(
+                self.df_train, self.df_test, self.feats_train, self.feats_test
+            )
         elif model_type == "gmm":
             from nkululeko.models.model_gmm import GMM_model
 
             self.model = GMM_model(
                 self.df_train, self.df_test, self.feats_train, self.feats_test
             )
         elif model_type == "knn":
```

### Comparing `nkululeko-0.84.1/nkululeko/models/finetune_model.py` & `nkululeko-0.85.0/nkululeko/models/finetune_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Code based on @jwagner
+"""
+
 import dataclasses
 import typing
 
 import torch
 import transformers
 from transformers.models.wav2vec2.modeling_wav2vec2 import (
     Wav2Vec2PreTrainedModel,
@@ -144,14 +148,19 @@
 
         else:
 
             return ModelOutput(
                 logits_cat=logits_cat,
             )
 
+    def predict(self, signal):
+        result = self(torch.from_numpy(signal))
+        result = result[0].detach().numpy()[0]
+        return result
+
 
 class ModelWithPreProcessing(Model):
 
     def __init__(self, config):
         super().__init__(config)
 
     def forward(
```

### Comparing `nkululeko-0.84.1/nkululeko/models/model.py` & `nkululeko-0.85.0/nkululeko/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.logo = self.util.config_val("MODEL", "logo", False)
         self.xfoldx = self.util.config_val("MODEL", "k_fold_cross", False)
 
     def set_model_type(self, type):
         self.model_type = type
 
     def is_ann(self):
-        if self.model_type == "ann":
+        if (self.model_type == "ann") or (self.model_type == "finetuned"):
             return True
         else:
             return False
 
     def set_testdata(self, data_df, feats_df):
         self.df_test, self.feats_test = data_df, feats_df
```

### Comparing `nkululeko-0.84.1/nkululeko/models/model_cnn.py` & `nkululeko-0.85.0/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/models/model_gmm.py` & `nkululeko-0.85.0/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/models/model_knn.py` & `nkululeko-0.85.0/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/models/model_knn_reg.py` & `nkululeko-0.85.0/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/models/model_mlp.py` & `nkululeko-0.85.0/nkululeko/models/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.85.0/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/models/model_svm.py` & `nkululeko-0.85.0/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/models/model_svr.py` & `nkululeko-0.85.0/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/multidb.py` & `nkululeko-0.85.0/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/nkuluflag.py` & `nkululeko-0.85.0/nkululeko/nkuluflag.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/nkululeko.py` & `nkululeko-0.85.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/plots.py` & `nkululeko-0.85.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/predict.py` & `nkululeko-0.85.0/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/reporting/defines.py` & `nkululeko-0.85.0/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/reporting/latex_writer.py` & `nkululeko-0.85.0/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/reporting/report.py` & `nkululeko-0.85.0/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/reporting/report_item.py` & `nkululeko-0.85.0/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/reporting/reporter.py` & `nkululeko-0.85.0/nkululeko/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/reporting/result.py` & `nkululeko-0.85.0/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/resample.py` & `nkululeko-0.85.0/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/runmanager.py` & `nkululeko-0.85.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/scaler.py` & `nkululeko-0.85.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/segment.py` & `nkululeko-0.85.0/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.85.0/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.85.0/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/syllable_nuclei.py` & `nkululeko-0.85.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/test.py` & `nkululeko-0.85.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/test_predictor.py` & `nkululeko-0.85.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/test_pretrain.py` & `nkululeko-0.85.0/nkululeko/test_pretrain.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,31 +49,31 @@
     # load the data
     expr.load_datasets()
 
     # split into train and test
     expr.fill_train_and_tests()
     util.debug(f"train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}")
 
+    model_root = util.get_path("model_dir")
     log_root = audeer.mkdir("log")
-    model_root = audeer.mkdir("model")
     torch_root = audeer.path(model_root, "torch")
 
     metrics_gender = {
         "UAR": audmetric.unweighted_average_recall,
         "ACC": audmetric.accuracy,
     }
 
     sampling_rate = 16000
     max_duration_sec = 8.0
 
     model_path = "facebook/wav2vec2-large-robust-ft-swbd-300h"
     num_layers = None
 
     os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
-    os.environ["CUDA_VISIBLE_DEVICES"] = "3"
+    os.environ["CUDA_VISIBLE_DEVICES"] = "0"
 
     batch_size = 16
     accumulation_steps = 4
     # create dataset
 
     dataset = {}
     target_name = glob_conf.target
@@ -255,29 +255,41 @@
         logging_steps=num_steps,
         learning_rate=1e-4,
         save_total_limit=2,
         metric_for_best_model="combined",
         greater_is_better=True,
         load_best_model_at_end=True,
         remove_unused_columns=False,
+        report_to="none",
     )
 
     trainer = Trainer(
         model=model,
         data_collator=data_collator,
         args=training_args,
         compute_metrics=compute_metrics,
         train_dataset=dataset["train"],
         eval_dataset=dataset["dev"],
         tokenizer=processor.feature_extractor,
         callbacks=[transformers.integrations.TensorBoardCallback()],
     )
+    if False:
+        trainer.train()
+        trainer.save_model(torch_root)
 
-    trainer.train()
-    trainer.save_model(torch_root)
+    modelnew = fm.Model.from_pretrained(
+        torch_root,
+        config=config,
+    )
+    print(f"loaded new model type{type(modelnew)}")
+    import audiofile
+
+    signal, _ = audiofile.read("./test.wav", always_2d=True)
+    result = modelnew.predict(signal)
+    print(result)
 
     print("DONE")
 
 
 def main(src_dir):
     parser = argparse.ArgumentParser(description="Call the nkululeko framework.")
     parser.add_argument("--config", default="exp.ini", help="The base configuration")
```

### Comparing `nkululeko-0.84.1/nkululeko/utils/files.py` & `nkululeko-0.85.0/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/utils/stats.py` & `nkululeko-0.85.0/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko/utils/util.py` & `nkululeko-0.85.0/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.85.0/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.84.1
+Version: 0.85.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.85.0
+--------------
+* first version with finetuning wav2vec2 layers
+
 Version 0.84.1
 --------------
 * made resample independent of config file
 
 Version 0.84.0
 --------------
 * added SHAP analysis
```

### Comparing `nkululeko-0.84.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.85.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 nkululeko/models/model_lin_reg.py
 nkululeko/models/model_mlp.py
 nkululeko/models/model_mlp_regression.py
 nkululeko/models/model_svm.py
 nkululeko/models/model_svr.py
 nkululeko/models/model_tree.py
 nkululeko/models/model_tree_reg.py
+nkululeko/models/model_tuned.py
 nkululeko/models/model_xgb.py
 nkululeko/models/model_xgr.py
 nkululeko/reporting/__init__.py
 nkululeko/reporting/defines.py
 nkululeko/reporting/latex_writer.py
 nkululeko/reporting/report.py
 nkululeko/reporting/report_item.py
```

### Comparing `nkululeko-0.84.1/setup.cfg` & `nkululeko-0.85.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.1/venv/bin/activate_this.py` & `nkululeko-0.85.0/venv/bin/activate_this.py`

 * *Files identical despite different names*

