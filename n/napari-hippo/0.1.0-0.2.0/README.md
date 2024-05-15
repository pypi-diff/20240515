# Comparing `tmp/napari-hippo-0.1.0.tar.gz` & `tmp/napari_hippo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-hippo-0.1.0.tar", last modified: Wed Jan 31 18:49:11 2024, max compression
+gzip compressed data, was "napari_hippo-0.2.0.tar", last modified: Wed May 15 15:25:29 2024, max compression
```

## Comparing `napari-hippo-0.1.0.tar` & `napari_hippo-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 thiele67   (503) staff       (20)        0 2024-01-31 18:49:11.061825 napari-hippo-0.1.0/
--rw-r--r--   0 thiele67   (503) staff       (20)     1067 2024-01-29 15:00:10.000000 napari-hippo-0.1.0/LICENSE
--rw-r--r--   0 thiele67   (503) staff       (20)      216 2023-08-02 07:27:09.000000 napari-hippo-0.1.0/MANIFEST.in
--rw-r--r--   0 thiele67   (503) staff       (20)     2306 2024-01-31 18:49:11.061637 napari-hippo-0.1.0/PKG-INFO
--rw-r--r--   0 thiele67   (503) staff       (20)     1025 2024-01-29 16:40:54.000000 napari-hippo-0.1.0/README.md
--rw-r--r--   0 thiele67   (503) staff       (20)     1177 2023-06-20 12:44:31.000000 napari-hippo-0.1.0/pyproject.toml
--rw-r--r--   0 thiele67   (503) staff       (20)     1373 2024-01-31 18:49:11.062587 napari-hippo-0.1.0/setup.cfg
-drwxr-xr-x   0 thiele67   (503) staff       (20)        0 2024-01-31 18:49:11.017159 napari-hippo-0.1.0/src/
-drwxr-xr-x   0 thiele67   (503) staff       (20)        0 2024-01-31 18:49:11.033247 napari-hippo-0.1.0/src/napari_hippo/
--rw-r--r--   0 thiele67   (503) staff       (20)     1775 2024-01-30 12:54:31.000000 napari-hippo-0.1.0/src/napari_hippo/__init__.py
--rw-r--r--   0 thiele67   (503) staff       (20)     5664 2023-08-04 12:14:47.000000 napari-hippo-0.1.0/src/napari_hippo/_caterpillarWidget.py
--rw-r--r--   0 thiele67   (503) staff       (20)    12829 2023-10-10 18:38:51.000000 napari-hippo-0.1.0/src/napari_hippo/_crunchyTools.py
--rw-r--r--   0 thiele67   (503) staff       (20)     2959 2023-10-20 11:14:58.000000 napari-hippo-0.1.0/src/napari_hippo/_fieldTools.py
--rw-r--r--   0 thiele67   (503) staff       (20)      692 2023-06-28 15:26:49.000000 napari-hippo-0.1.0/src/napari_hippo/_guiBase.py
--rw-r--r--   0 thiele67   (503) staff       (20)     9709 2023-08-04 12:13:05.000000 napari-hippo-0.1.0/src/napari_hippo/_hyliteTools.py
--rw-r--r--   0 thiele67   (503) staff       (20)    27000 2024-01-29 08:32:11.000000 napari-hippo-0.1.0/src/napari_hippo/_ioTools.py
--rw-r--r--   0 thiele67   (503) staff       (20)     8125 2024-01-24 14:44:14.000000 napari-hippo-0.1.0/src/napari_hippo/_reader.py
--rw-r--r--   0 thiele67   (503) staff       (20)      402 2023-07-04 19:23:10.000000 napari-hippo-0.1.0/src/napari_hippo/_sample_data.py
-drwxr-xr-x   0 thiele67   (503) staff       (20)        0 2024-01-31 18:49:11.045916 napari-hippo-0.1.0/src/napari_hippo/_tests/
--rw-------   0 thiele67   (503) staff       (20)        0 2023-06-20 12:44:31.000000 napari-hippo-0.1.0/src/napari_hippo/_tests/__init__.py
--rw-r--r--   0 thiele67   (503) staff       (20)     1173 2023-07-04 19:52:26.000000 napari-hippo-0.1.0/src/napari_hippo/_tests/test_Caterpillar.py
--rw-r--r--   0 thiele67   (503) staff       (20)     3103 2023-08-02 07:15:40.000000 napari-hippo-0.1.0/src/napari_hippo/_tests/test_CrunchyTools.py
--rw-r--r--   0 thiele67   (503) staff       (20)     1305 2023-08-02 09:52:06.000000 napari-hippo-0.1.0/src/napari_hippo/_tests/test_HyliteTools.py
--rw-r--r--   0 thiele67   (503) staff       (20)     1649 2023-10-09 07:00:15.000000 napari-hippo-0.1.0/src/napari_hippo/_tests/test_IOTools.py
--rw-r--r--   0 thiele67   (503) staff       (20)     2709 2023-07-04 20:53:01.000000 napari-hippo-0.1.0/src/napari_hippo/_tests/test_reader.py
--rw-r--r--   0 thiele67   (503) staff       (20)      721 2023-07-04 19:42:04.000000 napari-hippo-0.1.0/src/napari_hippo/_tests/test_sample_data.py
--rw-r--r--   0 thiele67   (503) staff       (20)     1385 2023-07-04 19:46:46.000000 napari-hippo-0.1.0/src/napari_hippo/_tests/test_writer.py
--rw-r--r--   0 thiele67   (503) staff       (20)     3271 2023-07-05 06:52:02.000000 napari-hippo-0.1.0/src/napari_hippo/_util.py
--rw-r--r--   0 thiele67   (503) staff       (20)     1895 2023-07-04 19:15:11.000000 napari-hippo-0.1.0/src/napari_hippo/_writer.py
--rw-r--r--   0 thiele67   (503) staff       (20)     2567 2023-10-20 09:59:50.000000 napari-hippo-0.1.0/src/napari_hippo/napari.yaml
-drwxr-xr-x   0 thiele67   (503) staff       (20)        0 2024-01-31 18:49:11.058941 napari-hippo-0.1.0/src/napari_hippo/testdata/
--rw-r--r--   0 thiele67   (503) staff       (20)      260 2023-07-04 19:19:05.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/__init__.py
--rw-r--r--   0 thiele67   (503) staff       (20)     1296 2023-10-09 10:06:43.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/block1.dat
--rwxr-xr-x   0 thiele67   (503) staff       (20)     1131 2023-10-10 07:42:24.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/block1.hdr
--rw-r--r--   0 thiele67   (503) staff       (20)     4421 2023-10-09 18:39:40.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/block1.png
--rw-r--r--   0 thiele67   (503) staff       (20)     1222 2023-10-09 10:06:43.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/block2.dat
--rwxr-xr-x   0 thiele67   (503) staff       (20)     1170 2023-10-10 07:42:24.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/block2.hdr
--rw-r--r--   0 thiele67   (503) staff       (20)     4712 2023-07-04 20:52:38.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/block2.png
--rwx------   0 thiele67   (503) staff       (20)   786600 2022-04-25 11:50:05.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/image.dat
--rwx------   0 thiele67   (503) staff       (20)    11740 2023-06-26 19:37:28.000000 napari-hippo-0.1.0/src/napari_hippo/testdata/image.hdr
-drwxr-xr-x   0 thiele67   (503) staff       (20)        0 2024-01-31 18:49:11.059842 napari-hippo-0.1.0/src/napari_hippo.egg-info/
--rw-r--r--   0 thiele67   (503) staff       (20)     2306 2024-01-31 18:49:11.000000 napari-hippo-0.1.0/src/napari_hippo.egg-info/PKG-INFO
--rw-r--r--   0 thiele67   (503) staff       (20)     1328 2024-01-31 18:49:11.000000 napari-hippo-0.1.0/src/napari_hippo.egg-info/SOURCES.txt
--rw-r--r--   0 thiele67   (503) staff       (20)        1 2024-01-31 18:49:11.000000 napari-hippo-0.1.0/src/napari_hippo.egg-info/dependency_links.txt
--rw-r--r--   0 thiele67   (503) staff       (20)       58 2024-01-31 18:49:11.000000 napari-hippo-0.1.0/src/napari_hippo.egg-info/entry_points.txt
--rw-r--r--   0 thiele67   (503) staff       (20)       98 2024-01-31 18:49:11.000000 napari-hippo-0.1.0/src/napari_hippo.egg-info/requires.txt
--rw-r--r--   0 thiele67   (503) staff       (20)       13 2024-01-31 18:49:11.000000 napari-hippo-0.1.0/src/napari_hippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:25:29.485244 napari_hippo-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-15 15:25:29.485244 napari_hippo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-15 15:25:29.485244 napari_hippo-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:25:29.473245 napari_hippo-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:25:29.477244 napari_hippo-0.2.0/src/napari_hippo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_caterpillarWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16156 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_crunchyTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_fieldTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_guiBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_hyliteTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31891 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_ioTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:25:29.481244 napari_hippo-0.2.0/src/napari_hippo/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_tests/test_Caterpillar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_tests/test_CrunchyTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_tests/test_HyliteTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_tests/test_IOTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:25:29.481244 napari_hippo-0.2.0/src/napari_hippo/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/block1.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/block1.hdr
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/block1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/block2.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1170 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/block2.hdr
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/block2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   786600 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/image.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11550 2024-05-15 15:25:25.000000 napari_hippo-0.2.0/src/napari_hippo/testdata/image.hdr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:25:29.481244 napari_hippo-0.2.0/src/napari_hippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-15 15:25:29.000000 napari_hippo-0.2.0/src/napari_hippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-15 15:25:29.000000 napari_hippo-0.2.0/src/napari_hippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:25:29.000000 napari_hippo-0.2.0/src/napari_hippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 15:25:29.000000 napari_hippo-0.2.0/src/napari_hippo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 15:25:29.000000 napari_hippo-0.2.0/src/napari_hippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 15:25:29.000000 napari_hippo-0.2.0/src/napari_hippo.egg-info/top_level.txt
```

### Comparing `napari-hippo-0.1.0/LICENSE` & `napari_hippo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/README.md` & `napari_hippo-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,117 @@
 00000000: 2320 6e61 7061 7269 2d68 6970 706f 0a0a  # napari-hippo..
-00000010: 5b21 5b4c 6963 656e 7365 204d 4954 5d28  [![License MIT](
-00000020: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000030: 6c64 732e 696f 2f70 7970 692f 6c2f 6e61  lds.io/pypi/l/na
-00000040: 7061 7269 2d68 6970 706f 2e73 7667 3f63  pari-hippo.svg?c
-00000050: 6f6c 6f72 3d67 7265 656e 295d 2868 7474  olor=green)](htt
-00000060: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000070: 7361 6d74 6869 656c 652f 6e61 7061 7269  samthiele/napari
-00000080: 2d68 6970 706f 2f62 6c6f 622f 6d61 696e  -hippo/blob/main
-00000090: 2f4c 4943 454e 5345 290a 5b21 5b50 7950  /LICENSE).[![PyP
-000000a0: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
-000000b0: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-000000c0: 2f6e 6170 6172 692d 6869 7070 6f2e 7376  /napari-hippo.sv
-000000d0: 673f 636f 6c6f 723d 6772 6565 6e29 5d28  g?color=green)](
-000000e0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-000000f0: 2f70 726f 6a65 6374 2f6e 6170 6172 692d  /project/napari-
-00000100: 6869 7070 6f29 0a5b 215b 6e61 7061 7269  hippo).[![napari
-00000110: 2068 7562 5d28 6874 7470 733a 2f2f 696d   hub](https://im
-00000120: 672e 7368 6965 6c64 732e 696f 2f65 6e64  g.shields.io/end
-00000130: 706f 696e 743f 7572 6c3d 6874 7470 733a  point?url=https:
-00000140: 2f2f 6170 692e 6e61 7061 7269 2d68 7562  //api.napari-hub
-00000150: 2e6f 7267 2f73 6869 656c 6473 2f6e 6170  .org/shields/nap
-00000160: 6172 692d 6869 7070 6f29 5d28 6874 7470  ari-hippo)](http
-00000170: 733a 2f2f 6e61 7061 7269 2d68 7562 2e6f  s://napari-hub.o
-00000180: 7267 2f70 6c75 6769 6e73 2f6e 6170 6172  rg/plugins/napar
-00000190: 692d 6869 7070 6f29 0a0a 4120 6c61 7267  i-hippo)..A larg
-000001a0: 6520 616e 6420 736c 6967 6874 6c79 2063  e and slightly c
-000001b0: 6c75 6d73 7920 706c 7567 696e 2066 6f72  lumsy plugin for
-000001c0: 2076 6965 7769 6e67 2061 6e64 2061 6e61   viewing and ana
-000001d0: 6c79 7369 6e67 2068 7970 6572 7370 6563  lysing hyperspec
-000001e0: 7472 616c 2064 6174 6120 696e 204e 6170  tral data in Nap
-000001f0: 6172 692e 0a0a 215b 4675 6e6b 7920 7363  ari...![Funky sc
-00000200: 7265 656e 7368 6f74 206f 6620 7468 6520  reenshot of the 
-00000210: 6e61 7061 7269 2d68 6970 706f 2047 5549  napari-hippo GUI
-00000220: 5d28 7363 7265 656e 7368 6f74 2e70 6e67  ](screenshot.png
-00000230: 290a 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  )..-------------
+00000010: 0a7c 203c 6120 6872 6566 3d22 6874 7470  .| <a href="http
+00000020: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000030: 616d 7468 6965 6c65 2f6e 6170 6172 692d  amthiele/napari-
+00000040: 6869 7070 6f2f 7769 6b69 223e 3c69 6d67  hippo/wiki"><img
+00000050: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000060: 7468 7562 2e63 6f6d 2f73 616d 7468 6965  thub.com/samthie
+00000070: 6c65 2f6e 6170 6172 692d 6869 7070 6f2f  le/napari-hippo/
+00000080: 626c 6f62 2f6d 6169 6e2f 6c6f 676f 2e70  blob/main/logo.p
+00000090: 6e67 2220 6865 6967 6874 3d22 3332 222f  ng" height="32"/
+000000a0: 3e3c 2f61 3e7c 205b 215b 4c69 6365 6e73  ></a>| [![Licens
+000000b0: 6520 4d49 545d 2868 7474 7073 3a2f 2f69  e MIT](https://i
+000000c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000000d0: 7069 2f6c 2f6e 6170 6172 692d 6869 7070  pi/l/napari-hipp
+000000e0: 6f2e 7376 673f 636f 6c6f 723d 6772 6565  o.svg?color=gree
+000000f0: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
+00000100: 7562 2e63 6f6d 2f73 616d 7468 6965 6c65  ub.com/samthiele
+00000110: 2f6e 6170 6172 692d 6869 7070 6f2f 626c  /napari-hippo/bl
+00000120: 6f62 2f6d 6169 6e2f 4c49 4345 4e53 4529  ob/main/LICENSE)
+00000130: 207c 205b 215b 5079 5049 5d28 6874 7470   | [![PyPI](http
+00000140: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000150: 696f 2f70 7970 692f 762f 6e61 7061 7269  io/pypi/v/napari
+00000160: 2d68 6970 706f 2e73 7667 3f63 6f6c 6f72  -hippo.svg?color
+00000170: 3d67 7265 656e 295d 2868 7474 7073 3a2f  =green)](https:/
+00000180: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000190: 742f 6e61 7061 7269 2d68 6970 706f 2920  t/napari-hippo) 
+000001a0: 7c20 5b21 5b6e 6170 6172 6920 6875 625d  | [![napari hub]
+000001b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000001c0: 656c 6473 2e69 6f2f 656e 6470 6f69 6e74  elds.io/endpoint
+000001d0: 3f75 726c 3d68 7474 7073 3a2f 2f61 7069  ?url=https://api
+000001e0: 2e6e 6170 6172 692d 6875 622e 6f72 672f  .napari-hub.org/
+000001f0: 7368 6965 6c64 732f 6e61 7061 7269 2d68  shields/napari-h
+00000200: 6970 706f 295d 2868 7474 7073 3a2f 2f6e  ippo)](https://n
+00000210: 6170 6172 692d 6875 622e 6f72 672f 706c  apari-hub.org/pl
+00000220: 7567 696e 732f 6e61 7061 7269 2d68 6970  ugins/napari-hip
+00000230: 706f 290a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  po).| ----------
 00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000250: 2d2d 2d2d 2d0a 0a23 2320 496e 7374 616c  -----..## Instal
-00000260: 6c61 7469 6f6e 0a0a 596f 7520 6361 6e20  lation..You can 
-00000270: 696e 7374 616c 6c20 606e 6170 6172 692d  install `napari-
-00000280: 6869 7070 6f60 2076 6961 205b 7069 705d  hippo` via [pip]
-00000290: 3a0a 0a20 2020 2070 6970 2069 6e73 7461  :..    pip insta
-000002a0: 6c6c 206e 6170 6172 692d 6869 7070 6f0a  ll napari-hippo.
-000002b0: 0a0a 2323 2043 6f6e 7472 6962 7574 696e  ..## Contributin
-000002c0: 670a 0a43 6f6e 7472 6962 7574 696f 6e73  g..Contributions
-000002d0: 2061 7265 2076 6572 7920 7765 6c63 6f6d   are very welcom
-000002e0: 6520 3a62 6c75 7368 3a0a 0a23 2320 4c69  e :blush:..## Li
-000002f0: 6365 6e73 650a 0a44 6973 7472 6962 7574  cense..Distribut
-00000300: 6564 2075 6e64 6572 2074 6865 2074 6572  ed under the ter
-00000310: 6d73 206f 6620 7468 6520 5b4d 4954 5d20  ms of the [MIT] 
-00000320: 6c69 6365 6e73 652c 0a22 6e61 7061 7269  license,."napari
-00000330: 2d68 6970 706f 2220 6973 2066 7265 6520  -hippo" is free 
-00000340: 616e 6420 6f70 656e 2073 6f75 7263 6520  and open source 
-00000350: 736f 6674 7761 7265 0a0a 2323 2049 7373  software..## Iss
-00000360: 7565 730a 0a49 6620 796f 7520 656e 636f  ues..If you enco
-00000370: 756e 7465 7220 616e 7920 7072 6f62 6c65  unter any proble
-00000380: 6d73 2c20 706c 6561 7365 205b 6669 6c65  ms, please [file
-00000390: 2061 6e20 6973 7375 655d 2061 6c6f 6e67   an issue] along
-000003a0: 2077 6974 6820 6120 6465 7461 696c 6564   with a detailed
-000003b0: 2064 6573 6372 6970 7469 6f6e 2e0a 0a23   description...#
-000003c0: 2320 4369 7461 7469 6f6e 0a0a 4120 6369  # Citation..A ci
-000003d0: 7461 7469 6f6e 2066 6f72 2074 6869 7320  tation for this 
-000003e0: 706c 7567 696e 2077 696c 6c20 6265 2061  plugin will be a
-000003f0: 6e6e 6f75 6e63 6564 2073 686f 7274 6c79  nnounced shortly
-00000400: 2e                                       .
+00000250: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00000260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000270: 2d2d 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -- |------------
+00000280: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+00000290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 0a20  ------------|.. 
+000002a0: 2020 200a 4120 6c61 7267 6520 616e 6420     .A large and 
+000002b0: 736c 6967 6874 6c79 2063 6c75 6d73 7920  slightly clumsy 
+000002c0: 706c 7567 696e 2066 6f72 2076 6965 7769  plugin for viewi
+000002d0: 6e67 2061 6e64 2061 6e61 6c79 7369 6e67  ng and analysing
+000002e0: 2068 7970 6572 7370 6563 7472 616c 2064   hyperspectral d
+000002f0: 6174 6120 696e 204e 6170 6172 692e 0a0a  ata in Napari...
+00000300: 215b 4675 6e6b 7920 7363 7265 656e 7368  ![Funky screensh
+00000310: 6f74 206f 6620 7468 6520 6e61 7061 7269  ot of the napari
+00000320: 2d68 6970 706f 2047 5549 5d28 7363 7265  -hippo GUI](scre
+00000330: 656e 7368 6f74 2e70 6e67 290a 0a0a 2d2d  enshot.png)...--
+00000340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000360: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000370: 6e0a 0a46 6f6c 6c6f 7720 5b74 6865 7365  n..Follow [these
+00000380: 2069 6e73 7472 7563 7469 6f6e 735d 2868   instructions](h
+00000390: 7474 7073 3a2f 2f6e 6170 6172 692e 6f72  ttps://napari.or
+000003a0: 672f 7374 6162 6c65 2f74 7574 6f72 6961  g/stable/tutoria
+000003b0: 6c73 2f66 756e 6461 6d65 6e74 616c 732f  ls/fundamentals/
+000003c0: 696e 7374 616c 6c61 7469 6f6e 2920 746f  installation) to
+000003d0: 2066 6972 7374 2069 6e73 7461 6c6c 206e   first install n
+000003e0: 6170 6172 692e 2054 6865 6e20 796f 7520  apari. Then you 
+000003f0: 6361 6e20 696e 7374 616c 6c20 606e 6170  can install `nap
+00000400: 6172 692d 6869 7070 6f60 2076 6961 205b  ari-hippo` via [
+00000410: 7069 705d 2868 7474 7073 3a2f 2f70 7970  pip](https://pyp
+00000420: 692e 6f72 672f 7072 6f6a 6563 742f 6e61  i.org/project/na
+00000430: 7061 7269 2d68 6970 706f 293a 0a0a 2020  pari-hippo):..  
+00000440: 2020 7069 7020 696e 7374 616c 6c20 6e61    pip install na
+00000450: 7061 7269 2d68 6970 706f 0a0a 2323 2044  pari-hippo..## D
+00000460: 6f63 756d 656e 7461 7469 6f6e 0a0a 5765  ocumentation..We
+00000470: 2061 7265 2069 6e20 7468 6520 7072 6f63   are in the proc
+00000480: 6573 7320 6f66 2062 7569 6c64 696e 6720  ess of building 
+00000490: 6120 646f 6375 6d65 6e74 6174 696f 6e20  a documentation 
+000004a0: 7769 6b69 2066 6f72 2074 6869 7320 706c  wiki for this pl
+000004b0: 7567 696e 205b 6865 7265 5d28 6874 7470  ugin [here](http
+000004c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+000004d0: 616d 7468 6965 6c65 2f6e 6170 6172 692d  amthiele/napari-
+000004e0: 6869 7070 6f2f 7769 6b69 292e 0a0a 2323  hippo/wiki)...##
+000004f0: 2043 6f6e 7472 6962 7574 696e 670a 0a43   Contributing..C
+00000500: 6f6e 7472 6962 7574 696f 6e73 2061 7265  ontributions are
+00000510: 2076 6572 7920 7765 6c63 6f6d 6521 2050   very welcome! P
+00000520: 6c65 6173 6520 6665 656c 2066 7265 6520  lease feel free 
+00000530: 746f 2073 7562 6d69 7420 7075 6c6c 2072  to submit pull r
+00000540: 6571 7565 7374 7320 6f72 2074 656c 6c20  equests or tell 
+00000550: 7573 2061 626f 7574 2079 6f75 7220 6964  us about your id
+00000560: 6561 7320 286f 7220 7072 6f62 6c65 6d73  eas (or problems
+00000570: 2920 6f6e 2074 6865 205b 6469 7363 7573  ) on the [discus
+00000580: 7369 6f6e 735d 2868 7474 7073 3a2f 2f70  sions](https://p
+00000590: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000005a0: 6e61 7061 7269 2d68 6970 706f 2920 7061  napari-hippo) pa
+000005b0: 6765 2e0a 0a23 2320 4c69 6365 6e73 650a  ge...## License.
+000005c0: 0a44 6973 7472 6962 7574 6564 2075 6e64  .Distributed und
+000005d0: 6572 2074 6865 2074 6572 6d73 206f 6620  er the terms of 
+000005e0: 7468 6520 5b4d 4954 5d28 6874 7470 733a  the [MIT](https:
+000005f0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 616d  //github.com/sam
+00000600: 7468 6965 6c65 2f6e 6170 6172 692d 6869  thiele/napari-hi
+00000610: 7070 6f2f 626c 6f62 2f6d 6169 6e2f 4c49  ppo/blob/main/LI
+00000620: 4345 4e53 4529 206c 6963 656e 7365 2c0a  CENSE) license,.
+00000630: 606e 6170 6172 692d 6869 7070 6f60 2069  `napari-hippo` i
+00000640: 7320 6672 6565 2061 6e64 206f 7065 6e20  s free and open 
+00000650: 736f 7572 6365 2073 6f66 7477 6172 652e  source software.
+00000660: 0a0a 2323 2049 7373 7565 730a 0a49 6620  ..## Issues..If 
+00000670: 796f 7520 656e 636f 756e 7465 7220 616e  you encounter an
+00000680: 7920 7072 6f62 6c65 6d73 2c20 706c 6561  y problems, plea
+00000690: 7365 205b 6669 6c65 2061 6e20 6973 7375  se [file an issu
+000006a0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+000006b0: 622e 636f 6d2f 7361 6d74 6869 656c 652f  b.com/samthiele/
+000006c0: 6e61 7061 7269 2d68 6970 706f 2f69 7373  napari-hippo/iss
+000006d0: 7565 732f 6e65 772f 6368 6f6f 7365 2920  ues/new/choose) 
+000006e0: 616c 6f6e 6720 7769 7468 2061 2064 6574  along with a det
+000006f0: 6169 6c65 6420 6465 7363 7269 7074 696f  ailed descriptio
+00000700: 6e2e 0a0a 2323 2043 6974 6174 696f 6e0a  n...## Citation.
+00000710: 0a41 2063 6974 6174 696f 6e20 666f 7220  .A citation for 
+00000720: 606e 6170 6172 692d 6869 7070 6f60 2077  `napari-hippo` w
+00000730: 696c 6c20 6265 2061 6e6e 6f75 6e63 6564  ill be announced
+00000740: 2073 686f 7274 6c79 2e0a                  shortly..
```

### Comparing `napari-hippo-0.1.0/pyproject.toml` & `napari_hippo-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/setup.cfg` & `napari_hippo-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/__init__.py` & `napari_hippo-0.2.0/src/napari_hippo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 from ._util import n2h, h2n, getHyImage
 from ._reader import napari_get_ENVI_reader, napari_get_specim_reader
 from ._sample_data import make_sample_data
 from ._ioTools import IOWidget
 from ._crunchyTools import CrunchyToolsWidget
 from ._hyliteTools import HyliteToolsWidget
```

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_fieldTools.py` & `napari_hippo-0.2.0/src/napari_hippo/_fieldTools.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_guiBase.py` & `napari_hippo-0.2.0/src/napari_hippo/_guiBase.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_hyliteTools.py` & `napari_hippo-0.2.0/src/napari_hippo/_hyliteTools.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,16 +91,21 @@
     elif stretch == 'Absolute':
         result.data = np.clip( (result.data - vmin) / (vmax-vmin), 0, 1 )
 
     # add to napari
     # todo - we should copy the affine matrix here?
     # (but have to deal with the different dimensionality of hypercubes vs rgb images)
     meta = dict(path=layer.metadata['path'], type='HSIp', wav=result.get_wavelengths())
+    if ']' in layer.name:
+        name = '[slice]'+layer.name.split(']')[1] + " [%s]"%(bands)
+    else:
+        name = '[slice] ' + layer.name + " [%s]"%(bands)
+    
     return viewer.add_image( h2n( result.data ), rgb=True,
-                       name=layer.name + " [%s]"%(bands),
+                       name=name,
                        metadata=meta )
 
 def hullCorrect(wmin : float = 2000.,
                 wmax : float = 2500.,
                 upper : bool = True):
     viewer = napari.current_viewer()  # get viewer
     image, layer  = getHyImage(viewer)
@@ -132,17 +137,15 @@
         R = PCA
     else:
         napari.utils.notifications.show_warning(
             "Warning: Unknown dimension reduction method %s."%method)
         return
 
     brange = ( image.get_band_index(wmin), image.get_band_index(wmax) )
-    result, _ = R( image, bands= ndim, band_range=brange )
-
-    print(np.isfinite(result.data).any() )
+    result = R( image, bands= ndim, band_range=brange )[0]
 
     meta = dict(path=layer.metadata['path'],
                 type='HSIf',
                 wav=np.arange(result.band_count()))
     data = h2n(result.data)
     if (result.band_count() == 3) or (result.band_count() == 4):
         data = np.transpose(data, (2, 0, 1 ) ) # bands should be in first axis...
@@ -191,16 +194,20 @@
             "Warning: Could not find valid HSI data.")
         return
 
     result = calculate( image, operation )
     meta = dict(path=layer.metadata['path'],
                 type='HSIp',
                 wav=np.array(result.get_wavelengths()))
+    if ']' in layer.name:
+        name = '[calc]'+layer.name.split(']')[1]
+    else:
+        name = '[calc] ' + layer.name
     return viewer.add_image(h2n(result.data), rgb=False, colormap='gist_earth',
-                            name=layer.name + " [calc]", metadata=meta )
+                            name=name, metadata=meta )
 
 
 def calculate(image, op: str = "1000. + $2 * 2190:2210 / (2150+2230)"):
     """
 
     Args:
         image: A HyImage instance to run a calculation on.
@@ -242,8 +249,8 @@
         op = op.replace(s, 'a[..., %d]' % ix)
 
     # finally, remove any $ from constants
     const = re.findall('[$][0-9]+', op)
     for s in const:
         op = op.replace(s, s[1:])
 
-    return hylite.HyImage(eval(op, {'np': np, 'a': image.data}))
+    return hylite.HyImage(eval(op, {'np': np, 'a': image.data}))
```

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_ioTools.py` & `napari_hippo-0.2.0/src/napari_hippo/_ioTools.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,20 @@
     def __init__(self, napari_viewer):
         super().__init__(napari_viewer)
 
         #btn = QPushButton("Load with query")
         #btn.clicked.connect(self._query)
 
         self.query_widget = magicgui(search, call_button='Search', root={'mode': 'd'}, auto_call=False)
-        self.info_widget = magicgui(info, call_button="Show Layer Info")
-        self._add([self.query_widget, self.info_widget], 'Import')
+        #self.info_widget = magicgui(info, call_button="Show Layer Info")
+        #self._add([self.query_widget, self.info_widget], 'Import')
+        self._add([self.query_widget], 'Import')
 
-        self.load_mask_widget = magicgui(loadMasks, call_button='Load Masks', mode={"choices": ['filename', 'directory']})
-        self.save_mask_widget = magicgui(saveMasks, call_button='Save Masks')
+        self.load_mask_widget = magicgui(loadMasks, call_button='Load/Init Masks', mode={"choices": ['filename', 'directory']})
+        self.save_mask_widget = magicgui(saveMasks, call_button='Save/Apply Masks', mode={"choices": ['Save to disk', 'Set as nan', 'Nan and crop']})
         self.update_mask_widget = magicgui(updateMasks, call_button='Update')
         self._add( [self.load_mask_widget, self.save_mask_widget,
                      self.update_mask_widget], 'Mask' )
 
         self.updateGeometry_widget = magicgui(updateGeometry, call_button="Save/Load")
         self.exportPatch_widget = magicgui(exportPatches, call_button='Export Patches',
                                              filename={"mode": "w", "filter":"*.hyc"})
@@ -120,49 +121,49 @@
 
         viewer.reset_view()
         viewer.dims.set_point(0, 0)
         napari.utils.notifications.show_info("Loaded %d images." % len(images))
 
         return out
 
-def info():
-    """
-    Displays metadata on the selected image as a notification.
-    """
-    viewer = napari.current_viewer()  # get viewer
-    layers = list(viewer.layers.selection)
-    if len(layers) > 0:
-        l = layers[0]
-
-        # get data
-        path = l.metadata.get('path', 'undefined')
-        if isinstance(path, list):
-            path = path[viewer.dims.current_step[0]]
-        name = os.path.basename( os.path.dirname(path) ) + '/' + os.path.basename(path)
-
-        # create message
-        msg = '%s (%s)\n'%(name, l.metadata.get('type', 'undefined'))
-        for k,v in l.metadata.items():
-            if k not in ['type']: # add other metadata if it exists
-                print(k, ': ', v ) # print metadata to console for reference too
-                line = ''
-                if isinstance(v, list) or isinstance(v, np.ndarray):
-                    line="%s: %s"%(k, str(v[viewer.dims.current_step[0]]))
-                else:
-                    line="%s: %s"%(k, str(v))
+# def info():
+#     """
+#     Displays metadata on the selected image as a notification.
+#     """
+#     viewer = napari.current_viewer()  # get viewer
+#     layers = list(viewer.layers.selection)
+#     if len(layers) > 0:
+#         l = layers[0]
+
+#         # get data
+#         path = l.metadata.get('path', 'undefined')
+#         if isinstance(path, list):
+#             path = path[viewer.dims.current_step[0]]
+#         name = os.path.basename( os.path.dirname(path) ) + '/' + os.path.basename(path)
+
+#         # create message
+#         msg = '%s (%s)\n'%(name, l.metadata.get('type', 'undefined'))
+#         for k,v in l.metadata.items():
+#             if k not in ['type']: # add other metadata if it exists
+#                 print(k, ': ', v ) # print metadata to console for reference too
+#                 line = ''
+#                 if isinstance(v, list) or isinstance(v, np.ndarray):
+#                     line="%s: %s"%(k, str(v[viewer.dims.current_step[0]]))
+#                 else:
+#                     line="%s: %s"%(k, str(v))
+
+#                 # clip for clarity
+#                 if len(line) > 30:
+#                     line = line[:30] + "..." + line[-15:]
+#                 msg+=line+"\n"
 
-                # clip for clarity
-                if len(line) > 30:
-                    line = line[:30] + "..." + line[-15:]
-                msg+=line+"\n"
+#         # show message
+#         napari.utils.notifications.show_info(msg)
 
-        # show message
-        napari.utils.notifications.show_info(msg)
-
-def loadMasks( mode : str = 'filename' ):
+def loadMasks( mode : str = 'directory' ):
     """
     Load mask files associated with an cube, slice or image stack.
 
     Args:
         mode = the matching mode to identify mask files. Options are:
                 - filename: masks will be envi files (.hdr extension) with the same filename
                             as the source image (must be .png, .jpg or similar).
@@ -207,96 +208,187 @@
                         shape = np.array(l.data[0].shape)
                     else:  # conventional RGB or greyscale (x,y,band)
                         shape = np.array([l.data.shape[0], l.data.shape[1]])
 
                     print("Creating mask for %s with shape %s." % (p,shape))
                     data.append( np.zeros( (shape[0], shape[1]), dtype=int) )
 
-            # build dask array
-            try:
-                import dask
-            except:
-                assert False, "Error - please install dask before building image stacks!"
-            shape = np.max([d.shape for d in data], axis=0)
-            for i in range(len(data)):
-                if data[i] is None:
-                    data[i] = np.zeros(shape, dtype=int)
-            stack = dask.array.stack([dask.array.from_delayed(dask.delayed(d), shape=shape, dtype=int,
-                                                              ) for d in data])
-            viewer.add_labels(stack, name='mask', metadata=dict(type='MASK', path=maskpaths))
-
-
-    # add polygon layers
-    for n, c in zip(['include', 'exclude'], [(0, 1, 1), (1, 0, 0)]):
-        l = viewer.add_shapes(None, ndim=3,
-                          name=n,
-                          edge_color=np.array(c),
-                          face_color=np.array((1, 1, 1, 0)),  # transparent
-                          edge_width=2, opacity=0.5)
-        l.mode = 'add_polygon'
-
-def saveMasks():
+            # single image mask; easy
+            if len(maskpaths) == 1:
+                viewer.add_labels(data[0], name='mask', metadata=dict(type='MASK', path=maskpaths))
+            else:
+                # build dask array for multi-mask stack
+                try:
+                    import dask
+                except:
+                    assert False, "Error - please install dask before building image stacks!"
+                shape = np.max([d.shape for d in data], axis=0)
+                for i in range(len(data)):
+                    if data[i] is None:
+                        data[i] = np.zeros(shape, dtype=int)
+                stack = dask.array.stack([dask.array.from_delayed(dask.delayed(d), shape=shape, dtype=int,
+                                                                ) for d in data])
+                viewer.add_labels(stack, name='mask', metadata=dict(type='MASK', path=maskpaths))
+
+    if len(layers) > 0: # add polygon layers
+        for n, c in zip(['include', 'exclude'], [(0, 1, 1), (1, 0, 0)]):
+            if len(maskpaths) > 1: # we're working on a stack
+                l = viewer.add_shapes(None, ndim=3,
+                                name=n,
+                                edge_color=np.array(c),
+                                face_color=np.array((1, 1, 1, 0)),  # transparent
+                                edge_width=2, opacity=0.5)
+            else: # this is a single layer
+                l = viewer.add_shapes(None, ndim=2,
+                                name=n,
+                                edge_color=np.array(c),
+                                face_color=np.array((1, 1, 1, 0)),  # transparent
+                                edge_width=2, opacity=0.5)
+            l.mode = 'add_polygon'
+
+def saveMasks(mode='Save to disk'):
+    """
+    Apply or save masks. Depending on the mode, these will be saved to disk or 
+    applied (to nan masked pixels in the selected image), with the option to also
+    crop the masked image to the mask region.
+    """
     viewer = napari.current_viewer()  # get viewer
 
-    # update selected layers
-    for l in viewer.layers:
+    # save masks to disk
+    if 'save' in mode.lower():
+        for l in viewer.layers:
+            if l.metadata.get('type', '') == 'MASK':
+                ndim = l.ndim
+                for i,p in enumerate(l.metadata.get('path',[])):
+                    if ndim == 2: # single 2D mask
+                        mask = hylite.HyImage( np.array( l.data ).T[...,None] )
+                    else: # slice from a stack of masks
+                        mask = hylite.HyImage( np.array( l.data[i] ).T[...,None] )
+                    mask.data = mask.data.astype(np.uint16) # N.B. cannot be uint8 otherwise we over-write our PNG files!!
+                    print("Saving mask to %s" % p )
+                    io.save(p, mask )
+        return
+    
+    # get mask
+    if 'mask' in viewer.layers:
+        l = viewer.layers['mask']
         if l.metadata.get('type', '') == 'MASK':
+            ndim = l.ndim
             for i,p in enumerate(l.metadata.get('path',[])):
-                mask = hylite.HyImage( np.array( l.data[i] ).T[...,None] )
-                mask.data = mask.data.astype(np.uint8)
-                print("Saving mask to %s" % p )
-                io.save(p, mask )
-
+                if ndim == 2: # single 2D mask
+                    mask = hylite.HyImage( np.array( l.data ).T[...,None] )
+                else:
+                    napari.utils.notifications.show_warning("Only [cube] data can be masked in this way.")
+                    return
+                break
+        else:
+            napari.utils.notifications.show_warning("Invalid mask - please create it using 'Load/Init Masks'")
+            return
+    
+    if 'nan' in mode.lower(): # 'Set as nan'
+        # apply mask
+        if mask is not None:
+            msk = (mask.data[...,0] == 0).T
+            for l in viewer.layers:
+                if isinstance(l, napari.layers.Image ):
+                    if l.metadata.get('type', '') == 'HSIf':
+                        l.data = l.data.astype(np.float32) # nans are float
+                        l.data[ :, 
+                            msk[:l.data.shape[1], :l.data.shape[2]] ] = np.nan
+                        l.refresh()
+                    elif l.rgb or l.metadata.get('type','') == 'HSIp':
+                        l.data = l.data.astype(np.float32) # nans are float
+                        l.data[ msk[:l.data.shape[0], :l.data.shape[1]] , : ] = np.nan
+                        l.refresh()
+
+    if 'crop' in mode.lower(): # 'Nan and crop'
+        xmn = np.argmin( msk.all(axis=1) )
+        xmx = msk.shape[0] - np.argmin( msk.all(axis=1)[::-1] )
+        ymn = np.argmin( msk.all(axis=0) )
+        ymx = msk.shape[1] - np.argmin( msk.all(axis=0)[::-1] )
+        
+        for l in viewer.layers:
+            if isinstance(l, napari.layers.Image ):
+                if l.metadata.get('type', '') == 'HSIf':
+                    l.data = l.data[:,
+                                    xmn:min(xmx,l.data.shape[1]),
+                                    ymn:min(ymx,l.data.shape[2])] 
+                    l.refresh()
+                elif l.rgb or l.metadata.get('type','') == 'HSIp':
+                    l.data = l.data[xmn:min(xmx, l.data.shape[0]), 
+                                    ymn:min(ymx, l.data.shape[1]), :]
+                    l.refresh()
+            
+        # our mask is no longer the correct shape; remove!
+        for l in ['mask', 'exclude', 'include']:
+            if l in viewer.layers:
+                viewer.layers.remove(l)
 def updateMasks():
     """
-    Update masks based on include and exclude polygons.
+    Update masks based on include and exclude polygons. These are then saved to disk
+    or 
     """
     viewer = napari.current_viewer()  # get viewer
 
     # update selected layers
     for l in viewer.layers:
         if l.metadata.get('type', '') == 'MASK':
 
             # get masks for include and exclude
             eMask = None
             iMask = None
             if 'exclude' in viewer.layers:
+                ndim = viewer.layers['exclude'].ndim
                 eMask = viewer.layers['exclude'].to_masks(l.data.shape)
             if 'include' in viewer.layers:
+                ndim = viewer.layers['exclude'].ndim
                 iMask = viewer.layers['include'].to_masks(l.data.shape)
-
-            stack=[]
-            for i in range(l.data.shape[0]):
-                mask = np.array( l.data[i] )
-                if (eMask is not None) and (len(eMask) > 0):
-                    sub = eMask[:,i, :mask.shape[0], :mask.shape[1]].any(axis=0)
-                    if sub.any():
-                        mask[sub] = 0
-                if (iMask is not None) and (len(iMask) > 0):
-                    add = iMask[:,i, :mask.shape[0], :mask.shape[1]].any(axis=0)
+            
+            if ndim == 2: # mask single image (easy)
+                mask = np.array( l.data )
+                if (eMask is not None) & len(eMask) > 0:
+                    sub = eMask[:,:mask.shape[0], :mask.shape[1]].any(axis=0)
+                    mask[sub] = 0
+                if (iMask is not None) & len(iMask) > 0:
+                    add = iMask[:,:mask.shape[0], :mask.shape[1]].any(axis=0)
                     if add.any():
                         mask[add] = 1
-                stack.append(mask)
+                l.data = mask
+                l.refresh()
 
-            # rebuild dask stack
-            try:
-                import dask.array
-                import dask.delayed
-            except:
-                napari.utils.notifications.show_warning(
-                    "Warning: stacked masks cannot be edited without dask installed.")
-                return
-
-            shape = np.max([i.shape for i in stack], axis=0)
-            stack = dask.array.stack([dask.array.from_delayed(dask.delayed(i), shape=shape, dtype=i.dtype,
-                                                              ) for i in stack])
-
-            # update layer data
-            l.data = stack
-            l.refresh()
+            else: # mask image stack
+                stack=[]
+                for i in range(l.data.shape[0]):
+                    mask = np.array( l.data[i] )
+                    if (eMask is not None) and (len(eMask) > 0):
+                        sub = eMask[:,i, :mask.shape[0], :mask.shape[1]].any(axis=0)
+                        if sub.any():
+                            mask[sub] = 0
+                    if (iMask is not None) and (len(iMask) > 0):
+                        add = iMask[:,i, :mask.shape[0], :mask.shape[1]].any(axis=0)
+                        if add.any():
+                            mask[add] = 1
+                    stack.append(mask)
+
+                # rebuild dask stack
+                try:
+                    import dask.array
+                    import dask.delayed
+                except:
+                    napari.utils.notifications.show_warning(
+                        "Warning: stacked masks cannot be edited without dask installed.")
+                    return
+
+                shape = np.max([i.shape for i in stack], axis=0)
+                stack = dask.array.stack([dask.array.from_delayed(dask.delayed(i), shape=shape, dtype=i.dtype,
+                                                                ) for i in stack])
+
+                # update layer data
+                l.data = stack
+                l.refresh()
 
     # clear exclude and include polygons
     viewer.layers['exclude'].data = []
     viewer.layers['include'].data = []
 
     print("--")
 
@@ -575,19 +667,20 @@
                 else:
                     try: # look for an ENVI file with the same name
                         image = io.load(os.path.splitext(l.metadata['path'])[0] + ".hdr" )
                     except:
                         continue # skip this one
 
                 img_name = os.path.splitext( os.path.basename( l.metadata['path'] ) )[0]
-                labels = points.text.values
+
                 # extract points
-                if points is not None:
+                if (points is not None) and (len(points.data) > 0):
                     spectra = []
                     names = []
+                    labels = points.text.values
                     for i,(py,px) in enumerate(points.data):
                         print("Extracting spectra from pixel (%d,%d) in image %s with %d bands"%(px,py,img_name, image.band_count()))
                         if (px > 0) and (py > 0):
                             if (px < image.xdim()) and (py < image.ydim()):
                                 spectra.append(image.data[int(px),int(py),:])
                                 if i < len(labels):
                                     names.append("P%d_%s"%(i,labels[i]))
@@ -603,15 +696,15 @@
                         fig.canvas.manager.set_window_title(img_name+"_points")
                         fig.show()
                     O.set(img_name+"_points", lib)
                     O.save()
                     O.free()
 
                 # extract ROIs 
-                if roi is not None:
+                if (roi is not None) and (len(roi.data) > 0):
                     labels = roi.text.values
                     masks = roi.to_masks((image.ydim(), image.xdim()))
                     spectra = [] # for average spectra library
                     names = [] 
                     for i,m in enumerate(masks):
                         m = np.array( m ).T # convert mask to hylite layout
```

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_reader.py` & `napari_hippo-0.2.0/src/napari_hippo/_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,30 +87,38 @@
             print(meta)
             if len(meta) > 0:
                 image = None
                 sensor = ''
                 with open(meta[0], 'r') as f:
                     for l in f.readlines():
                         if 'sensor type' in l.lower():
+                            if 'fenix1k' in l.lower():
+                                sensor = 'fenix1k'
                             if 'fenix' in l.lower():
                                 sensor = 'fenix'
                             elif 'fx50' in l.lower():
                                 sensor = 'fx50'
                             elif 'lwir' in l.lower():
                                 sensor = 'lwir'
                             elif 'rgb' in l.lower():
                                 sensor = 'rgb'
                             break
                 if 'fenix' in sensor: # Fenix
                     from hylite.reference.spectra import R90 as ref
                     from hylite.sensors import Fenix
-                    image = Fenix.correct_folder( root, calib=ref,
-                                                        flip=True,
+                    if '1k' in sensor:
+                        image = Fenix.correct_folder( root, calib=ref,
+                                                        flip=True, # no lense flip for 1k
                                                         shift=False,
                                                         verbose=True)
+                    else:
+                        image = Fenix.correct_folder( root, calib=ref,
+                                                            flip=True,
+                                                            shift=False,
+                                                            verbose=True)
                 elif 'fx50' in sensor: # FX50
                     from hylite.sensors import FX50
                     image = FX50.correct_folder(root, bpr=True, flip=True,
                                                       verbose=True)
                 elif 'lwir' in sensor: # OWL
                     from hylite.sensors import OWL
                     image = OWL.correct_folder(root, bpr=True, flip=True,
```

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_tests/test_Caterpillar.py` & `napari_hippo-0.2.0/src/napari_hippo/_tests/test_Caterpillar.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_tests/test_CrunchyTools.py` & `napari_hippo-0.2.0/src/napari_hippo/_tests/test_CrunchyTools.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_tests/test_HyliteTools.py` & `napari_hippo-0.2.0/src/napari_hippo/_tests/test_HyliteTools.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_tests/test_IOTools.py` & `napari_hippo-0.2.0/src/napari_hippo/_tests/test_IOTools.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_tests/test_reader.py` & `napari_hippo-0.2.0/src/napari_hippo/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_tests/test_sample_data.py` & `napari_hippo-0.2.0/src/napari_hippo/_tests/test_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_tests/test_writer.py` & `napari_hippo-0.2.0/src/napari_hippo/_tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_util.py` & `napari_hippo-0.2.0/src/napari_hippo/_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -62,11 +62,16 @@
                                 return hylite.HyImage(n2h(l.data), wav=w), l
                             elif pixels is not None:
                                 d = hylite.HyData( np.array( [l.data[x,y,:] for x,y in pixels] ) )
                                 d.set_wavelengths( w )
                                 return d
                             else:
                                 return hylite.HyImage( n2h( l.data ), wav=w).export_bands(bands), l
+                elif l.rgb:
+                    if bands is None:
+                        return hylite.HyImage( n2h( l.data )), l
+                    else:
+                        return hylite.HyImage( n2h( l.data )).export_bands(bands), l
 
     # if we got here, there are not appropriate images in the selection
     napari.utils.notifications.show_warning("Please select an HSI image.")
     return None, None
```

### Comparing `napari-hippo-0.1.0/src/napari_hippo/_writer.py` & `napari_hippo-0.2.0/src/napari_hippo/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/napari.yaml` & `napari_hippo-0.2.0/src/napari_hippo/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/testdata/block1.hdr` & `napari_hippo-0.2.0/src/napari_hippo/testdata/block1.hdr`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/testdata/block1.png` & `napari_hippo-0.2.0/src/napari_hippo/testdata/block1.png`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/testdata/block2.hdr` & `napari_hippo-0.2.0/src/napari_hippo/testdata/block2.hdr`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/testdata/block2.png` & `napari_hippo-0.2.0/src/napari_hippo/testdata/block2.png`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/testdata/image.dat` & `napari_hippo-0.2.0/src/napari_hippo/testdata/image.dat`

 * *Files identical despite different names*

### Comparing `napari-hippo-0.1.0/src/napari_hippo/testdata/image.hdr` & `napari_hippo-0.2.0/src/napari_hippo/testdata/image.hdr`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-ENVI
-description = {
-  File Resize Result, x resize factor: 1.000000, y resize factor: 1.000000.}
-samples = 23
-lines   = 38
-bands   = 450
-header offset = 0
-file type = ENVI Standard
-data type = 12
-interleave = bsq
-sensor type = Fenix
-byte order = 0
-x start = 247
-y start = 425
-default bands = {287,262,244}
-wavelength units = Nanometers
-reflectance scale factor = 65535.000000
-data ignore value = 0
-fwhm = {
- 3.360000, 3.360000, 3.360000, 3.360000, 3.360000, 3.370000, 3.370000,
- 3.370000, 3.370000, 3.370000, 3.370000, 3.370000, 3.380000, 3.380000,
- 3.380000, 3.380000, 3.380000, 3.380000, 3.380000, 3.380000, 3.390000,
- 3.390000, 3.390000, 3.390000, 3.390000, 3.390000, 3.390000, 3.390000,
- 3.400000, 3.400000, 3.400000, 3.400000, 3.400000, 3.400000, 3.400000,
- 3.400000, 3.410000, 3.410000, 3.410000, 3.410000, 3.410000, 3.410000,
- 3.410000, 3.410000, 3.410000, 3.410000, 3.420000, 3.420000, 3.420000,
- 3.420000, 3.420000, 3.420000, 3.420000, 3.420000, 3.420000, 3.420000,
- 3.420000, 3.420000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000,
- 3.430000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000,
- 3.430000, 3.430000, 3.430000, 3.430000, 3.440000, 3.440000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
- 3.450000, 3.450000, 3.450000, 3.450000, 3.450000, 3.450000, 3.450000,
- 3.450000, 3.450000, 3.450000, 3.450000, 3.450000, 3.450000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
- 3.440000, 3.440000, 3.440000, 3.430000, 3.430000, 3.430000, 3.430000,
- 3.430000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000,
- 3.430000, 3.430000, 3.430000, 3.430000, 3.420000, 3.420000, 3.420000,
- 3.420000, 3.420000, 3.420000, 3.420000, 3.420000, 3.420000, 5.630000,
- 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000,
- 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000,
- 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000,
- 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000,
- 5.630000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000,
- 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000,
- 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000,
- 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000,
- 5.620000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000,
- 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000,
- 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000,
- 5.610000, 5.600000, 5.600000, 5.600000, 5.600000, 5.600000, 5.600000,
- 5.600000, 5.600000, 5.600000, 5.600000, 5.600000, 5.600000, 5.600000,
- 5.600000, 5.600000, 5.600000, 5.600000, 5.600000, 5.590000, 5.590000,
- 5.590000, 5.590000, 5.590000, 5.590000, 5.590000, 5.590000, 5.590000,
- 5.590000, 5.590000, 5.590000, 5.590000, 5.590000, 5.590000, 5.590000,
- 5.580000, 5.580000, 5.580000, 5.580000, 5.580000, 5.580000, 5.580000,
- 5.580000, 5.580000, 5.580000, 5.580000, 5.580000, 5.580000, 5.580000,
- 5.580000, 5.570000, 5.570000, 5.570000, 5.570000, 5.570000, 5.570000,
- 5.570000, 5.570000, 5.570000, 5.570000, 5.570000, 5.570000, 5.570000,
- 5.560000, 5.560000, 5.560000, 5.560000, 5.560000, 5.560000, 5.560000,
- 5.560000, 5.560000, 5.560000, 5.560000, 5.560000, 5.560000, 5.550000,
- 5.550000, 5.550000, 5.550000, 5.550000, 5.550000, 5.550000, 5.550000,
- 5.550000, 5.550000, 5.550000, 5.550000, 5.540000, 5.540000, 5.540000,
- 5.540000, 5.540000, 5.540000, 5.540000, 5.540000, 5.540000, 5.540000,
- 5.540000, 5.530000, 5.530000, 5.530000, 5.530000, 5.530000, 5.530000,
- 5.530000, 5.530000, 5.530000, 5.530000, 5.520000, 5.520000, 5.520000,
- 5.520000, 5.520000, 5.520000, 5.520000, 5.520000, 5.520000, 5.520000,
- 5.510000, 5.510000, 5.510000, 5.510000, 5.510000, 5.510000, 5.510000,
- 5.510000, 5.510000, 5.510000, 5.500000, 5.500000, 5.500000, 5.500000,
- 5.500000, 5.500000, 5.500000, 5.500000, 5.500000, 5.490000, 5.490000,
- 5.490000, 5.490000, 5.490000, 5.490000, 5.490000, 5.490000, 5.490000,
- 5.480000, 5.480000, 5.480000, 5.480000, 5.480000, 5.480000, 5.480000,
- 5.480000, 5.480000, 5.470000, 5.470000, 5.470000, 5.470000, 5.470000,
- 5.470000, 5.470000, 5.470000, 5.460000, 5.460000, 5.460000, 5.460000,
- 5.460000, 5.460000, 5.460000, 5.460000, 5.460000, 5.450000, 5.450000,
- 5.450000, 5.450000, 5.450000, 5.450000, 5.450000, 5.450000, 5.440000,
- 5.440000, 5.440000, 5.440000, 5.440000, 5.440000, 5.440000, 5.430000,
- 5.430000, 5.430000, 5.430000, 5.430000, 5.430000, 5.430000, 5.430000,
- 5.420000, 5.420000}
- wavelength = {
-  378.190002,  381.549988,  384.910004,  388.269989,  391.640015,  395.000000,
-  398.369995,  401.739990,  405.109985,  408.480011,  411.850006,  415.220001,
-  418.600006,  421.980011,  425.350006,  428.730011,  432.109985,  435.500000,
-  438.880005,  442.260010,  445.649994,  449.040009,  452.429993,  455.820007,
-  459.209991,  462.600006,  465.989990,  469.390015,  472.779999,  476.179993,
-  479.579987,  482.980011,  486.380005,  489.779999,  493.179993,  496.589996,
-  499.989990,  503.399994,  506.809998,  510.220001,  513.619995,  517.030029,
-  520.450012,  523.859985,  527.270020,  530.690002,  534.099976,  537.520020,
-  540.929993,  544.349976,  547.770020,  551.190002,  554.609985,  558.030029,
-  561.450012,  564.880005,  568.299988,  571.719971,  575.150024,  578.570007,
-  582.000000,  585.429993,  588.859985,  592.289978,  595.710022,  599.140015,
-  602.580017,  606.010010,  609.440002,  612.869995,  616.299988,  619.739990,
-  623.169983,  626.609985,  630.039978,  633.479980,  636.919983,  640.349976,
-  643.789978,  647.229980,  650.669983,  654.109985,  657.539978,  660.979980,
-  664.419983,  667.859985,  671.309998,  674.750000,  678.190002,  681.630005,
-  685.070007,  688.510010,  691.960022,  695.400024,  698.840027,  702.289978,
-  705.729980,  709.169983,  712.619995,  716.059998,  719.510010,  722.950012,
-  726.400024,  729.840027,  733.289978,  736.729980,  740.179993,  743.619995,
-  747.070007,  750.510010,  753.960022,  757.400024,  760.849976,  764.289978,
-  767.739990,  771.179993,  774.630005,  778.070007,  781.520020,  784.960022,
-  788.409973,  791.849976,  795.299988,  798.739990,  802.179993,  805.630005,
-  809.070007,  812.520020,  815.960022,  819.400024,  822.840027,  826.289978,
-  829.729980,  833.169983,  836.609985,  840.049988,  843.489990,  846.940002,
-  850.380005,  853.820007,  857.250000,  860.690002,  864.130005,  867.570007,
-  871.010010,  874.440002,  877.880005,  881.320007,  884.750000,  888.190002,
-  891.619995,  895.059998,  898.489990,  901.919983,  905.359985,  908.789978,
-  912.219971,  915.650024,  919.080017,  922.510010,  925.940002,  929.359985,
-  932.789978,  936.219971,  939.640015,  943.070007,  946.489990,  949.909973,
-  953.340027,  956.760010,  960.179993,  963.599976,  967.020020,  970.429993,
-  976.440002,  982.080017,  987.710022,  993.340027,  998.969971, 1004.599976,
- 1010.229980, 1015.859985, 1021.489990, 1027.119995, 1032.750000, 1038.380005,
- 1044.010010, 1049.640015, 1055.270020, 1060.900024, 1066.530029, 1072.160034,
- 1077.780029, 1083.410034, 1089.040039, 1094.670044, 1100.290039, 1105.920044,
- 1111.550049, 1117.170044, 1122.800049, 1128.430054, 1134.050049, 1139.680054,
- 1145.300049, 1150.930054, 1156.550049, 1162.170044, 1167.800049, 1173.420044,
- 1179.040039, 1184.670044, 1190.290039, 1195.910034, 1201.530029, 1207.150024,
- 1212.770020, 1218.390015, 1224.010010, 1229.630005, 1235.250000, 1240.869995,
- 1246.489990, 1252.109985, 1257.729980, 1263.339966, 1268.959961, 1274.579956,
- 1280.189941, 1285.810059, 1291.420044, 1297.040039, 1302.650024, 1308.270020,
- 1313.880005, 1319.500000, 1325.109985, 1330.719971, 1336.329956, 1341.939941,
- 1347.560059, 1353.170044, 1358.780029, 1364.390015, 1370.000000, 1375.599976,
- 1381.209961, 1386.819946, 1392.430054, 1398.030029, 1403.640015, 1409.250000,
- 1414.849976, 1420.459961, 1426.060059, 1431.660034, 1437.270020, 1442.869995,
- 1448.469971, 1454.069946, 1459.670044, 1465.280029, 1470.880005, 1476.469971,
- 1482.069946, 1487.670044, 1493.270020, 1498.869995, 1504.459961, 1510.060059,
- 1515.650024, 1521.250000, 1526.839966, 1532.439941, 1538.030029, 1543.619995,
- 1549.209961, 1554.810059, 1560.400024, 1565.989990, 1571.579956, 1577.170044,
- 1582.750000, 1588.339966, 1593.930054, 1599.510010, 1605.099976, 1610.680054,
- 1616.270020, 1621.849976, 1627.430054, 1633.020020, 1638.599976, 1644.180054,
- 1649.760010, 1655.339966, 1660.920044, 1666.500000, 1672.069946, 1677.650024,
- 1683.229980, 1688.800049, 1694.380005, 1699.949951, 1705.520020, 1711.099976,
- 1716.670044, 1722.239990, 1727.810059, 1733.380005, 1738.949951, 1744.510010,
- 1750.079956, 1755.650024, 1761.209961, 1766.780029, 1772.339966, 1777.910034,
- 1783.469971, 1789.030029, 1794.589966, 1800.150024, 1805.709961, 1811.270020,
- 1816.829956, 1822.380005, 1827.939941, 1833.489990, 1839.050049, 1844.599976,
- 1850.160034, 1855.709961, 1861.260010, 1866.810059, 1872.359985, 1877.910034,
- 1883.449951, 1889.000000, 1894.550049, 1900.089966, 1905.640015, 1911.180054,
- 1916.719971, 1922.260010, 1927.800049, 1933.339966, 1938.880005, 1944.420044,
- 1949.959961, 1955.489990, 1961.030029, 1966.560059, 1972.089966, 1977.630005,
- 1983.160034, 1988.689941, 1994.219971, 1999.750000, 2005.270020, 2010.800049,
- 2016.329956, 2021.849976, 2027.380005, 2032.900024, 2038.420044, 2043.939941,
- 2049.459961, 2054.979980, 2060.500000, 2066.010010, 2071.530029, 2077.040039,
- 2082.560059, 2088.070068, 2093.580078, 2099.090088, 2104.600098, 2110.110107,
- 2115.620117, 2121.120117, 2126.629883, 2132.129883, 2137.639893, 2143.139893,
- 2148.639893, 2154.139893, 2159.639893, 2165.139893, 2170.639893, 2176.129883,
- 2181.629883, 2187.120117, 2192.610107, 2198.100098, 2203.590088, 2209.080078,
- 2214.570068, 2220.060059, 2225.540039, 2231.030029, 2236.510010, 2241.989990,
- 2247.479980, 2252.959961, 2258.439941, 2263.909912, 2269.389893, 2274.870117,
- 2280.340088, 2285.810059, 2291.280029, 2296.760010, 2302.229980, 2307.689941,
- 2313.159912, 2318.629883, 2324.090088, 2329.560059, 2335.020020, 2340.479980,
- 2345.939941, 2351.399902, 2356.860107, 2362.310059, 2367.770020, 2373.219971,
- 2378.669922, 2384.120117, 2389.570068, 2395.020020, 2400.469971, 2405.919922,
- 2411.360107, 2416.810059, 2422.250000, 2427.689941, 2433.129883, 2438.570068,
- 2444.010010, 2449.439941, 2454.879883, 2460.310059, 2465.739990, 2471.169922,
- 2476.600098, 2482.030029, 2487.459961, 2492.879883, 2498.310059, 2503.729980}
-acquisitionwindow1 left = 652
-acquisitionwindow1 top = 696
-acquisitionwindow2 left = 0
-acquisitionwindow2 top = 0
-acquisition date = DATE(yyyy-mm-dd): 2022-03-22
-binning = {
- 4, 2}
-binning2 = {
- 1, 1}
-scb temperature channel1 = 33.14
-scb temperature channel2 = 27.23
-scb temperature channel3 = 30.64
-scb temperature channel4 = 28.01
-start time = UTC TIME: 15:41:28
-stop time = UTC TIME: 15:42:00
-swir temperature = 147.00
-temperature = {
- 147.00, 33.14, 27.23, 30.64, 28.01}
-tint1 = 18.000000
-tint2 = 4.455800
-trigger mode1 = External
-trigger mode2 = External
-vimg = {
- 1, 450}
-vimg1 = {
- 1, 174}
-vimg2 = {
- 175, 450}
-vroi = {
- 1, 450}
+ENVI
+description = {
+  File Resize Result, x resize factor: 1.000000, y resize factor: 1.000000.}
+samples = 23
+lines   = 38
+bands   = 450
+header offset = 0
+file type = ENVI Standard
+data type = 12
+interleave = bsq
+sensor type = Fenix
+byte order = 0
+x start = 247
+y start = 425
+default bands = {287,262,244}
+wavelength units = Nanometers
+reflectance scale factor = 65535.000000
+data ignore value = 0
+fwhm = {
+ 3.360000, 3.360000, 3.360000, 3.360000, 3.360000, 3.370000, 3.370000,
+ 3.370000, 3.370000, 3.370000, 3.370000, 3.370000, 3.380000, 3.380000,
+ 3.380000, 3.380000, 3.380000, 3.380000, 3.380000, 3.380000, 3.390000,
+ 3.390000, 3.390000, 3.390000, 3.390000, 3.390000, 3.390000, 3.390000,
+ 3.400000, 3.400000, 3.400000, 3.400000, 3.400000, 3.400000, 3.400000,
+ 3.400000, 3.410000, 3.410000, 3.410000, 3.410000, 3.410000, 3.410000,
+ 3.410000, 3.410000, 3.410000, 3.410000, 3.420000, 3.420000, 3.420000,
+ 3.420000, 3.420000, 3.420000, 3.420000, 3.420000, 3.420000, 3.420000,
+ 3.420000, 3.420000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000,
+ 3.430000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000,
+ 3.430000, 3.430000, 3.430000, 3.430000, 3.440000, 3.440000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
+ 3.450000, 3.450000, 3.450000, 3.450000, 3.450000, 3.450000, 3.450000,
+ 3.450000, 3.450000, 3.450000, 3.450000, 3.450000, 3.450000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000, 3.440000,
+ 3.440000, 3.440000, 3.440000, 3.430000, 3.430000, 3.430000, 3.430000,
+ 3.430000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000, 3.430000,
+ 3.430000, 3.430000, 3.430000, 3.430000, 3.420000, 3.420000, 3.420000,
+ 3.420000, 3.420000, 3.420000, 3.420000, 3.420000, 3.420000, 5.630000,
+ 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000,
+ 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000,
+ 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000,
+ 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000, 5.630000,
+ 5.630000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000,
+ 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000,
+ 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000,
+ 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000, 5.620000,
+ 5.620000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000,
+ 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000,
+ 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000, 5.610000,
+ 5.610000, 5.600000, 5.600000, 5.600000, 5.600000, 5.600000, 5.600000,
+ 5.600000, 5.600000, 5.600000, 5.600000, 5.600000, 5.600000, 5.600000,
+ 5.600000, 5.600000, 5.600000, 5.600000, 5.600000, 5.590000, 5.590000,
+ 5.590000, 5.590000, 5.590000, 5.590000, 5.590000, 5.590000, 5.590000,
+ 5.590000, 5.590000, 5.590000, 5.590000, 5.590000, 5.590000, 5.590000,
+ 5.580000, 5.580000, 5.580000, 5.580000, 5.580000, 5.580000, 5.580000,
+ 5.580000, 5.580000, 5.580000, 5.580000, 5.580000, 5.580000, 5.580000,
+ 5.580000, 5.570000, 5.570000, 5.570000, 5.570000, 5.570000, 5.570000,
+ 5.570000, 5.570000, 5.570000, 5.570000, 5.570000, 5.570000, 5.570000,
+ 5.560000, 5.560000, 5.560000, 5.560000, 5.560000, 5.560000, 5.560000,
+ 5.560000, 5.560000, 5.560000, 5.560000, 5.560000, 5.560000, 5.550000,
+ 5.550000, 5.550000, 5.550000, 5.550000, 5.550000, 5.550000, 5.550000,
+ 5.550000, 5.550000, 5.550000, 5.550000, 5.540000, 5.540000, 5.540000,
+ 5.540000, 5.540000, 5.540000, 5.540000, 5.540000, 5.540000, 5.540000,
+ 5.540000, 5.530000, 5.530000, 5.530000, 5.530000, 5.530000, 5.530000,
+ 5.530000, 5.530000, 5.530000, 5.530000, 5.520000, 5.520000, 5.520000,
+ 5.520000, 5.520000, 5.520000, 5.520000, 5.520000, 5.520000, 5.520000,
+ 5.510000, 5.510000, 5.510000, 5.510000, 5.510000, 5.510000, 5.510000,
+ 5.510000, 5.510000, 5.510000, 5.500000, 5.500000, 5.500000, 5.500000,
+ 5.500000, 5.500000, 5.500000, 5.500000, 5.500000, 5.490000, 5.490000,
+ 5.490000, 5.490000, 5.490000, 5.490000, 5.490000, 5.490000, 5.490000,
+ 5.480000, 5.480000, 5.480000, 5.480000, 5.480000, 5.480000, 5.480000,
+ 5.480000, 5.480000, 5.470000, 5.470000, 5.470000, 5.470000, 5.470000,
+ 5.470000, 5.470000, 5.470000, 5.460000, 5.460000, 5.460000, 5.460000,
+ 5.460000, 5.460000, 5.460000, 5.460000, 5.460000, 5.450000, 5.450000,
+ 5.450000, 5.450000, 5.450000, 5.450000, 5.450000, 5.450000, 5.440000,
+ 5.440000, 5.440000, 5.440000, 5.440000, 5.440000, 5.440000, 5.430000,
+ 5.430000, 5.430000, 5.430000, 5.430000, 5.430000, 5.430000, 5.430000,
+ 5.420000, 5.420000}
+ wavelength = {
+  378.190002,  381.549988,  384.910004,  388.269989,  391.640015,  395.000000,
+  398.369995,  401.739990,  405.109985,  408.480011,  411.850006,  415.220001,
+  418.600006,  421.980011,  425.350006,  428.730011,  432.109985,  435.500000,
+  438.880005,  442.260010,  445.649994,  449.040009,  452.429993,  455.820007,
+  459.209991,  462.600006,  465.989990,  469.390015,  472.779999,  476.179993,
+  479.579987,  482.980011,  486.380005,  489.779999,  493.179993,  496.589996,
+  499.989990,  503.399994,  506.809998,  510.220001,  513.619995,  517.030029,
+  520.450012,  523.859985,  527.270020,  530.690002,  534.099976,  537.520020,
+  540.929993,  544.349976,  547.770020,  551.190002,  554.609985,  558.030029,
+  561.450012,  564.880005,  568.299988,  571.719971,  575.150024,  578.570007,
+  582.000000,  585.429993,  588.859985,  592.289978,  595.710022,  599.140015,
+  602.580017,  606.010010,  609.440002,  612.869995,  616.299988,  619.739990,
+  623.169983,  626.609985,  630.039978,  633.479980,  636.919983,  640.349976,
+  643.789978,  647.229980,  650.669983,  654.109985,  657.539978,  660.979980,
+  664.419983,  667.859985,  671.309998,  674.750000,  678.190002,  681.630005,
+  685.070007,  688.510010,  691.960022,  695.400024,  698.840027,  702.289978,
+  705.729980,  709.169983,  712.619995,  716.059998,  719.510010,  722.950012,
+  726.400024,  729.840027,  733.289978,  736.729980,  740.179993,  743.619995,
+  747.070007,  750.510010,  753.960022,  757.400024,  760.849976,  764.289978,
+  767.739990,  771.179993,  774.630005,  778.070007,  781.520020,  784.960022,
+  788.409973,  791.849976,  795.299988,  798.739990,  802.179993,  805.630005,
+  809.070007,  812.520020,  815.960022,  819.400024,  822.840027,  826.289978,
+  829.729980,  833.169983,  836.609985,  840.049988,  843.489990,  846.940002,
+  850.380005,  853.820007,  857.250000,  860.690002,  864.130005,  867.570007,
+  871.010010,  874.440002,  877.880005,  881.320007,  884.750000,  888.190002,
+  891.619995,  895.059998,  898.489990,  901.919983,  905.359985,  908.789978,
+  912.219971,  915.650024,  919.080017,  922.510010,  925.940002,  929.359985,
+  932.789978,  936.219971,  939.640015,  943.070007,  946.489990,  949.909973,
+  953.340027,  956.760010,  960.179993,  963.599976,  967.020020,  970.429993,
+  976.440002,  982.080017,  987.710022,  993.340027,  998.969971, 1004.599976,
+ 1010.229980, 1015.859985, 1021.489990, 1027.119995, 1032.750000, 1038.380005,
+ 1044.010010, 1049.640015, 1055.270020, 1060.900024, 1066.530029, 1072.160034,
+ 1077.780029, 1083.410034, 1089.040039, 1094.670044, 1100.290039, 1105.920044,
+ 1111.550049, 1117.170044, 1122.800049, 1128.430054, 1134.050049, 1139.680054,
+ 1145.300049, 1150.930054, 1156.550049, 1162.170044, 1167.800049, 1173.420044,
+ 1179.040039, 1184.670044, 1190.290039, 1195.910034, 1201.530029, 1207.150024,
+ 1212.770020, 1218.390015, 1224.010010, 1229.630005, 1235.250000, 1240.869995,
+ 1246.489990, 1252.109985, 1257.729980, 1263.339966, 1268.959961, 1274.579956,
+ 1280.189941, 1285.810059, 1291.420044, 1297.040039, 1302.650024, 1308.270020,
+ 1313.880005, 1319.500000, 1325.109985, 1330.719971, 1336.329956, 1341.939941,
+ 1347.560059, 1353.170044, 1358.780029, 1364.390015, 1370.000000, 1375.599976,
+ 1381.209961, 1386.819946, 1392.430054, 1398.030029, 1403.640015, 1409.250000,
+ 1414.849976, 1420.459961, 1426.060059, 1431.660034, 1437.270020, 1442.869995,
+ 1448.469971, 1454.069946, 1459.670044, 1465.280029, 1470.880005, 1476.469971,
+ 1482.069946, 1487.670044, 1493.270020, 1498.869995, 1504.459961, 1510.060059,
+ 1515.650024, 1521.250000, 1526.839966, 1532.439941, 1538.030029, 1543.619995,
+ 1549.209961, 1554.810059, 1560.400024, 1565.989990, 1571.579956, 1577.170044,
+ 1582.750000, 1588.339966, 1593.930054, 1599.510010, 1605.099976, 1610.680054,
+ 1616.270020, 1621.849976, 1627.430054, 1633.020020, 1638.599976, 1644.180054,
+ 1649.760010, 1655.339966, 1660.920044, 1666.500000, 1672.069946, 1677.650024,
+ 1683.229980, 1688.800049, 1694.380005, 1699.949951, 1705.520020, 1711.099976,
+ 1716.670044, 1722.239990, 1727.810059, 1733.380005, 1738.949951, 1744.510010,
+ 1750.079956, 1755.650024, 1761.209961, 1766.780029, 1772.339966, 1777.910034,
+ 1783.469971, 1789.030029, 1794.589966, 1800.150024, 1805.709961, 1811.270020,
+ 1816.829956, 1822.380005, 1827.939941, 1833.489990, 1839.050049, 1844.599976,
+ 1850.160034, 1855.709961, 1861.260010, 1866.810059, 1872.359985, 1877.910034,
+ 1883.449951, 1889.000000, 1894.550049, 1900.089966, 1905.640015, 1911.180054,
+ 1916.719971, 1922.260010, 1927.800049, 1933.339966, 1938.880005, 1944.420044,
+ 1949.959961, 1955.489990, 1961.030029, 1966.560059, 1972.089966, 1977.630005,
+ 1983.160034, 1988.689941, 1994.219971, 1999.750000, 2005.270020, 2010.800049,
+ 2016.329956, 2021.849976, 2027.380005, 2032.900024, 2038.420044, 2043.939941,
+ 2049.459961, 2054.979980, 2060.500000, 2066.010010, 2071.530029, 2077.040039,
+ 2082.560059, 2088.070068, 2093.580078, 2099.090088, 2104.600098, 2110.110107,
+ 2115.620117, 2121.120117, 2126.629883, 2132.129883, 2137.639893, 2143.139893,
+ 2148.639893, 2154.139893, 2159.639893, 2165.139893, 2170.639893, 2176.129883,
+ 2181.629883, 2187.120117, 2192.610107, 2198.100098, 2203.590088, 2209.080078,
+ 2214.570068, 2220.060059, 2225.540039, 2231.030029, 2236.510010, 2241.989990,
+ 2247.479980, 2252.959961, 2258.439941, 2263.909912, 2269.389893, 2274.870117,
+ 2280.340088, 2285.810059, 2291.280029, 2296.760010, 2302.229980, 2307.689941,
+ 2313.159912, 2318.629883, 2324.090088, 2329.560059, 2335.020020, 2340.479980,
+ 2345.939941, 2351.399902, 2356.860107, 2362.310059, 2367.770020, 2373.219971,
+ 2378.669922, 2384.120117, 2389.570068, 2395.020020, 2400.469971, 2405.919922,
+ 2411.360107, 2416.810059, 2422.250000, 2427.689941, 2433.129883, 2438.570068,
+ 2444.010010, 2449.439941, 2454.879883, 2460.310059, 2465.739990, 2471.169922,
+ 2476.600098, 2482.030029, 2487.459961, 2492.879883, 2498.310059, 2503.729980}
+acquisitionwindow1 left = 652
+acquisitionwindow1 top = 696
+acquisitionwindow2 left = 0
+acquisitionwindow2 top = 0
+acquisition date = DATE(yyyy-mm-dd): 2022-03-22
+binning = {
+ 4, 2}
+binning2 = {
+ 1, 1}
+scb temperature channel1 = 33.14
+scb temperature channel2 = 27.23
+scb temperature channel3 = 30.64
+scb temperature channel4 = 28.01
+start time = UTC TIME: 15:41:28
+stop time = UTC TIME: 15:42:00
+swir temperature = 147.00
+temperature = {
+ 147.00, 33.14, 27.23, 30.64, 28.01}
+tint1 = 18.000000
+tint2 = 4.455800
+trigger mode1 = External
+trigger mode2 = External
+vimg = {
+ 1, 450}
+vimg1 = {
+ 1, 174}
+vimg2 = {
+ 175, 450}
+vroi = {
+ 1, 450}
```

### Comparing `napari-hippo-0.1.0/src/napari_hippo.egg-info/SOURCES.txt` & `napari_hippo-0.2.0/src/napari_hippo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

