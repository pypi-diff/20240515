# Comparing `tmp/hexkit-3.0.2.tar.gz` & `tmp/hexkit-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexkit-3.0.2.tar", last modified: Fri May 10 13:41:08 2024, max compression
+gzip compressed data, was "hexkit-3.1.0.tar", last modified: Wed May 15 11:26:50 2024, max compression
```

## Comparing `hexkit-3.0.2.tar` & `hexkit-3.1.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.899418 hexkit-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-10 13:41:02.000000 hexkit-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 13:41:02.000000 hexkit-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-10 13:41:08.895418 hexkit-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-10 13:41:02.000000 hexkit-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-10 13:41:02.000000 hexkit-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:41:08.899418 hexkit-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.883418 hexkit-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.887418 hexkit-3.0.2/src/hexkit/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16932 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/daopub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/daosub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/objstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/akafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/akafka/provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/daosub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongodb/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongodb/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/mongokafka/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongokafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16534 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongokafka/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.895418 hexkit-3.0.2/src/hexkit/providers/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.895418 hexkit-3.0.2/src/hexkit/providers/s3/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/test_file1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/test_file2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/test_file3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/test_file4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.895418 hexkit-3.0.2/src/hexkit/providers/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/testing/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.895418 hexkit-3.0.2/src/hexkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.581028 hexkit-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-15 11:26:43.000000 hexkit-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 11:26:43.000000 hexkit-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-15 11:26:50.581028 hexkit-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-15 11:26:43.000000 hexkit-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-15 11:26:43.000000 hexkit-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:26:50.581028 hexkit-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.565028 hexkit-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.569028 hexkit-3.1.0/src/hexkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.573028 hexkit-3.1.0/src/hexkit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16932 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/protocols/dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/protocols/daopub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/protocols/daosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/protocols/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/protocols/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24753 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/protocols/objstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.573028 hexkit-3.1.0/src/hexkit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.573028 hexkit-3.1.0/src/hexkit/providers/akafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.573028 hexkit-3.1.0/src/hexkit/providers/akafka/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/provider/daosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/provider/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/provider/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/provider/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21924 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/akafka/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.573028 hexkit-3.1.0/src/hexkit/providers/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/mongodb/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/mongodb/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.577028 hexkit-3.1.0/src/hexkit/providers/mongokafka/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/mongokafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16534 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/mongokafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/mongokafka/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.577028 hexkit-3.1.0/src/hexkit/providers/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/s3/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.577028 hexkit-3.1.0/src/hexkit/providers/s3/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/s3/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/s3/test_files/test_file1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/s3/test_files/test_file2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/s3/test_files/test_file3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/s3/test_files/test_file4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18811 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/s3/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.577028 hexkit-3.1.0/src/hexkit/providers/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/providers/testing/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-15 11:26:43.000000 hexkit-3.1.0/src/hexkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:26:50.577028 hexkit-3.1.0/src/hexkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-15 11:26:50.000000 hexkit-3.1.0/src/hexkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 11:26:50.000000 hexkit-3.1.0/src/hexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:26:50.000000 hexkit-3.1.0/src/hexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-15 11:26:50.000000 hexkit-3.1.0/src/hexkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 11:26:50.000000 hexkit-3.1.0/src/hexkit.egg-info/top_level.txt
```

### Comparing `hexkit-3.0.2/LICENSE` & `hexkit-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/PKG-INFO` & `hexkit-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 3.0.2
+Version: 3.1.0
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -19,29 +19,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic_settings<3,>=2
 Requires-Dist: PyYAML<7,>=6.0
 Provides-Extra: akafka
 Requires-Dist: aiokafka~=0.10.0; extra == "akafka"
-Requires-Dist: jsonschema<5,>=4.21; extra == "akafka"
+Requires-Dist: jsonschema<5,>=4.22; extra == "akafka"
 Provides-Extra: s3
-Requires-Dist: boto3<2,>=1.26.50; extra == "s3"
-Requires-Dist: botocore<2,>=1.29.50; extra == "s3"
+Requires-Dist: boto3<2,>=1.34.104; extra == "s3"
+Requires-Dist: botocore<2,>=1.34.104; extra == "s3"
 Provides-Extra: mongodb
-Requires-Dist: motor<4,>=3.1.1; extra == "mongodb"
+Requires-Dist: motor<4,>=3.4.0; extra == "mongodb"
 Provides-Extra: test-akafka
 Requires-Dist: hexkit[akafka]; extra == "test-akafka"
-Requires-Dist: testcontainers[kafka]<5,>=4.3.3; extra == "test-akafka"
+Requires-Dist: testcontainers[kafka]<5,>=4.4.1; extra == "test-akafka"
 Provides-Extra: test-s3
 Requires-Dist: hexkit[s3]; extra == "test-s3"
-Requires-Dist: testcontainers<5,>=4.3.3; extra == "test-s3"
+Requires-Dist: testcontainers<5,>=4.4.1; extra == "test-s3"
 Provides-Extra: test-mongodb
 Requires-Dist: hexkit[mongodb]; extra == "test-mongodb"
-Requires-Dist: testcontainers[mongo]<5,>=4.3.3; extra == "test-mongodb"
+Requires-Dist: testcontainers[mongo]<5,>=4.4.1; extra == "test-mongodb"
 Provides-Extra: test
 Requires-Dist: hexkit[test-akafka,test-mongodb,test-s3]; extra == "test"
 Provides-Extra: all
 Requires-Dist: hexkit[test]; extra == "all"
 
 ![tests](https://github.com/ghga-de/hexkit/actions/workflows/tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/hexkit.svg)](https://pypi.python.org/pypi/hexkit/)
```

### Comparing `hexkit-3.0.2/README.md` & `hexkit-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/pyproject.toml` & `hexkit-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,48 +19,48 @@
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "hexkit"
-version = "3.0.2"
+version = "3.1.0"
 description = "A Toolkit for Building Microservices using the Hexagonal Architecture"
 dependencies = [
     "pydantic >=2, <3",
     "pydantic_settings >=2, <3",
     "PyYAML >=6.0, <7",
 ]
 
 [project.license]
 text = "Apache 2.0"
 
 [project.optional-dependencies]
 akafka = [
     "aiokafka~=0.10.0",
-    "jsonschema >=4.21, <5",
+    "jsonschema >=4.22, <5",
 ]
 s3 = [
-    "boto3 >=1.26.50, <2",
-    "botocore >=1.29.50, <2",
+    "boto3 >=1.34.104, <2",
+    "botocore >=1.34.104, <2",
 ]
 mongodb = [
-    "motor >=3.1.1, <4",
+    "motor >=3.4.0, <4",
 ]
 test-akafka = [
     "hexkit[akafka]",
-    "testcontainers[kafka] >=4.3.3, <5",
+    "testcontainers[kafka] >=4.4.1, <5",
 ]
 test-s3 = [
     "hexkit[s3]",
-    "testcontainers >=4.3.3, <5",
+    "testcontainers >=4.4.1, <5",
 ]
 test-mongodb = [
     "hexkit[mongodb]",
-    "testcontainers[mongo] >=4.3.3, <5",
+    "testcontainers[mongo] >=4.4.1, <5",
 ]
 test = [
     "hexkit[test-akafka,test-s3,test-mongodb]",
 ]
 all = [
     "hexkit[test]",
 ]
```

### Comparing `hexkit-3.0.2/src/hexkit/__init__.py` & `hexkit-3.1.0/src/hexkit/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/__main__.py` & `hexkit-3.1.0/src/hexkit/__main__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/base.py` & `hexkit-3.1.0/src/hexkit/base.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/config.py` & `hexkit-3.1.0/src/hexkit/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/correlation.py` & `hexkit-3.1.0/src/hexkit/correlation.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/custom_types.py` & `hexkit-3.1.0/src/hexkit/custom_types.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/log.py` & `hexkit-3.1.0/src/hexkit/log.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/protocols/__init__.py` & `hexkit-3.1.0/src/hexkit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/protocols/dao.py` & `hexkit-3.1.0/src/hexkit/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/protocols/daopub.py` & `hexkit-3.1.0/src/hexkit/protocols/daopub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/protocols/daosub.py` & `hexkit-3.1.0/src/hexkit/protocols/daosub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/protocols/eventpub.py` & `hexkit-3.1.0/src/hexkit/protocols/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/protocols/eventsub.py` & `hexkit-3.1.0/src/hexkit/protocols/eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/protocols/objstorage.py` & `hexkit-3.1.0/src/hexkit/protocols/objstorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,24 +513,24 @@
     class BucketError(ObjectStorageProtocolError):
         """Generic base exception for error that occur while handling buckets."""
 
     class BucketNotFoundError(BucketError):
         """Thrown when trying to access a bucket with an ID that doesn't exist."""
 
         def __init__(self, bucket_id: Optional[str]):
-            in_bucket = f" in bucket with ID '{bucket_id}'" if bucket_id else ""
-            message = f"The bucket{in_bucket} does not exist."
+            with_id = f" with ID '{bucket_id}'" if bucket_id else ""
+            message = f"The bucket{with_id} does not exist."
             super().__init__(message)
 
     class BucketAlreadyExistsError(BucketError):
         """Thrown when trying to create a bucket with an ID that already exists."""
 
         def __init__(self, bucket_id: Optional[str]):
-            in_bucket = f" in bucket with ID '{bucket_id}'" if bucket_id else ""
-            message = f"The bucket{in_bucket} already exists."
+            with_id = f" with ID '{bucket_id}'" if bucket_id else ""
+            message = f"The bucket{with_id} already exists."
             super().__init__(message)
 
     class BucketNotEmptyError(BucketError):
         """Thrown when trying to delete a bucket that is not empty."""
 
         def __init__(self, bucket_id: Optional[str]):
             with_id = f" with ID '{bucket_id}'" if bucket_id else ""
```

### Comparing `hexkit-3.0.2/src/hexkit/providers/__init__.py` & `hexkit-3.1.0/src/hexkit/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/__init__.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/config.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/provider/__init__.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/provider/daosub.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/provider/daosub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/provider/eventpub.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/provider/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/provider/eventsub.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/provider/eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/provider/utils.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/provider/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/testcontainer.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/testcontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing import Literal, Optional
 
 from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_for_logs
 
 __all__ = ["KafkaSSLContainer"]
 
-DEFAULT_IMAGE = "confluentinc/cp-kafka:7.6.0"
+DEFAULT_IMAGE = "confluentinc/cp-kafka:7.6.1"
 
 DEFAULT_PORT = 9093  # default port for the Kafka container
 BROKER_PORT = 9092  # auxiliary port for inter broker listener
 
 
 class KafkaSSLContainer(DockerContainer):
     """Kafka container that supports SSL (or actually TLS)."""
```

### Comparing `hexkit-3.0.2/src/hexkit/providers/akafka/testutils.py` & `hexkit-3.1.0/src/hexkit/providers/akafka/testutils.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,20 +16,27 @@
 
 """Utilities for testing code that uses Kafka-based provider.
 
 Please note, only use for testing purposes.
 """
 
 import json
-from collections.abc import AsyncGenerator, Sequence
+from collections.abc import AsyncGenerator, Generator, Sequence
 from contextlib import asynccontextmanager
 from dataclasses import dataclass
 from functools import partial
-from typing import Callable, Optional, Union
+from typing import Any, Callable, Optional, Union
 
+try:
+    from typing import Self
+except ImportError:  # Python < 3.11
+    from typing_extensions import Self
+
+
+import pytest
 import pytest_asyncio
 from aiokafka import AIOKafkaConsumer, TopicPartition
 from aiokafka.admin import AIOKafkaAdminClient
 from testcontainers.kafka import KafkaContainer
 
 from hexkit.custom_types import Ascii, JsonObject, PytestScope
 from hexkit.providers.akafka import KafkaConfig
@@ -37,14 +44,34 @@
     ConsumerEvent,
     KafkaEventPublisher,
     get_header_value,
     headers_as_dict,
 )
 from hexkit.providers.akafka.testcontainer import DEFAULT_IMAGE as KAFKA_IMAGE
 
+__all__ = [
+    "KAFKA_IMAGE",
+    "EventBase",
+    "EventRecorder",
+    "ExpectedEvent",
+    "RecordedEvent",
+    "ValidationError",
+    "KafkaConfig",
+    "KafkaContainerFixture",
+    "KafkaEventPublisher",
+    "KafkaFixture",
+    "get_kafka_container_fixture",
+    "get_clean_kafka_fixture",
+    "get_persistent_kafka_fixture",
+    "kafka_container_fixture",
+    "clean_kafka_fixture",
+    "persistent_kafka_fixture",
+    "kafka_fixture",
+]
+
 
 @dataclass(frozen=True)
 class EventBase:
     """Base for describing events expected and recorded by the EventRecorder class."""
 
     payload: JsonObject
     type_: Ascii
@@ -335,15 +362,15 @@
         """Stop recording and check the recorded events against the expectation when
         exiting the context block.
         """
         await self.stop_recording()
 
 
 class KafkaFixture:
-    """Yielded by the `kafka_fixture` function"""
+    """A fixture with utility methods for tests that use Apache Kafka."""
 
     def __init__(
         self,
         *,
         config: KafkaConfig,
         kafka_servers: list[str],
         publisher: KafkaEventPublisher,
@@ -464,53 +491,119 @@
             yield event_recorder
 
         check_recorded_events(
             recorded_events=event_recorder.recorded_events, expected_events=events
         )
 
 
-async def kafka_fixture_function() -> AsyncGenerator[KafkaFixture, None]:
-    """Pytest fixture for tests depending on the Kafka-base providers.
+class KafkaContainerFixture(KafkaContainer):
+    """Kafka test container with configuration and command execution."""
 
-    **Do not call directly** Instead, use get_kafka_fixture()
-    """
-    with KafkaContainer(image=KAFKA_IMAGE) as kafka:
-        kafka_servers = [kafka.get_bootstrap_server()]
-        config = KafkaConfig(
+    kafka_config: KafkaConfig
+
+    def __init__(self, port: int = 9093, **kwargs: Any) -> None:
+        """Initialize the container."""
+        super().__init__(image=KAFKA_IMAGE, port=port, **kwargs)
+
+    def __enter__(self) -> Self:
+        """Enter the container context."""
+        super().__enter__()
+        kafka_servers = [self.get_bootstrap_server()]
+        self.kafka_config = KafkaConfig(
             service_name="test_publisher",
             service_instance_id="001",
             kafka_servers=kafka_servers,
         )
+        return self
 
-        def wrapped_exec_run(command: str, run_in_shell: bool):
-            """Run the given command in the kafka testcontainer.
+    def wrapped_exec_run(self, command: str, run_in_shell: bool):
+        """Run the given command in the kafka testcontainer.
 
-            Args:
-              - `command`: The full command to run.
-              - `run_in_shell`: If True, will run the command in a shell.
-
-            Raises:
-              - `RuntimeError`: when the exit code returned by the command is not zero.
-            """
-            cmd = ["sh", "-c", command] if run_in_shell else command
-            exit_code, output = kafka.get_wrapped_container().exec_run(cmd)
-
-            if exit_code != 0:
-                raise RuntimeError(
-                    f"result: {exit_code}, output: {output.decode('utf-8')}"
-                )
+        Args:
+            - `command`: The full command to run.
+            - `run_in_shell`: If True, will run the command in a shell.
 
-        async with KafkaEventPublisher.construct(config=config) as publisher:
-            yield KafkaFixture(
-                config=config,
-                kafka_servers=kafka_servers,
-                publisher=publisher,
-                cmd_exec_func=wrapped_exec_run,
-            )
+        Raises:
+            - `RuntimeError`: when the exit code returned by the command is not zero.
+        """
+        cmd = ["sh", "-c", command] if run_in_shell else command
+        exit_code, output = self.get_wrapped_container().exec_run(cmd)
+
+        if exit_code != 0:
+            raise RuntimeError(f"result: {exit_code}, output: {output.decode('utf-8')}")
+
+
+def _kafka_container_fixture() -> Generator[KafkaContainerFixture, None, None]:
+    """Fixture function for getting a running Kafka test container."""
+    with KafkaContainerFixture() as kafka_container:
+        yield kafka_container
+
+
+def get_kafka_container_fixture(
+    scope: PytestScope = "session", name: str = "kafka_container"
+):
+    """Get a Kafka test container fixture with desired scope and name.
+
+    By default, the session scope is used for Kafka test containers.
+    """
+    return pytest.fixture(_kafka_container_fixture, scope=scope, name=name)
+
+
+kafka_container_fixture = get_kafka_container_fixture()
 
 
-def get_kafka_fixture(scope: PytestScope = "function"):
-    """Produce a kafka fixture with desired scope. Default is the function scope."""
-    return pytest_asyncio.fixture(kafka_fixture_function, scope=scope)
+async def _persistent_kafka_fixture(
+    kafka_container: KafkaContainerFixture,
+) -> AsyncGenerator[KafkaFixture, None]:
+    """Fixture function that gets a persistent Kafka fixture.
+
+    The state of Kafka is not cleaned up by this function.
+    """
+    config = kafka_container.kafka_config
+    async with KafkaEventPublisher.construct(config=config) as publisher:
+        kafka_fixture = KafkaFixture(
+            config=config,
+            kafka_servers=config.kafka_servers,
+            cmd_exec_func=kafka_container.wrapped_exec_run,
+            publisher=publisher,
+        )
+        yield kafka_fixture
+
+
+def get_persistent_kafka_fixture(scope: PytestScope = "function", name: str = "kafka"):
+    """Get a Kafka fixture with desired scope and name.
+
+    The state of the Kafka test container is persisted across tests.
+
+    By default, the function scope is used for this fixture,
+    while the session scope is used for the underlying Kafka test container.
+    """
+    return pytest_asyncio.fixture(_persistent_kafka_fixture, scope=scope, name=name)
+
+
+persistent_kafka_fixture = get_persistent_kafka_fixture()
+
+
+async def _clean_kafka_fixture(
+    kafka_container: KafkaContainerFixture,
+) -> AsyncGenerator[KafkaFixture, None]:
+    """Fixture function that gets a clean Kafka fixture.
+
+    The clean state is achieved by clearing all Kafka topics upfront.
+    """
+    async for kafka_fixture in _persistent_kafka_fixture(kafka_container):
+        await kafka_fixture.clear_topics()
+        yield kafka_fixture
+
+
+def get_clean_kafka_fixture(scope: PytestScope = "function", name: str = "kafka"):
+    """Get a Kafka fixture with desired scope and name.
+
+    The state of Kafka is reset by clearing all topics before running tests.
+
+    By default, the function scope is used for this fixture,
+    while the session scope is used for the underlying Kafka test container.
+    """
+    return pytest_asyncio.fixture(_clean_kafka_fixture, scope=scope, name=name)
 
 
-kafka_fixture = get_kafka_fixture()
+kafka_fixture = clean_kafka_fixture = get_clean_kafka_fixture()
```

### Comparing `hexkit-3.0.2/src/hexkit/providers/mongodb/__init__.py` & `hexkit-3.1.0/src/hexkit/providers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/mongodb/provider.py` & `hexkit-3.1.0/src/hexkit/providers/mongodb/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/mongokafka/__init__.py` & `hexkit-3.1.0/src/hexkit/providers/mongokafka/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/mongokafka/provider.py` & `hexkit-3.1.0/src/hexkit/providers/mongokafka/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/s3/__init__.py` & `hexkit-3.1.0/src/hexkit/providers/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/s3/provider.py` & `hexkit-3.1.0/src/hexkit/providers/s3/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/s3/test_files/__init__.py` & `hexkit-3.1.0/src/hexkit/providers/s3/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/s3/testutils.py` & `hexkit-3.1.0/src/hexkit/providers/s3/testutils.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,30 +19,50 @@
 Please note, only use for testing purposes.
 """
 
 # ruff: noqa: PLR0913
 
 import hashlib
 import os
-from collections.abc import Generator
+from collections.abc import AsyncGenerator, Generator
 from contextlib import contextmanager
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Optional
 
 import pytest
+import pytest_asyncio
 import requests
 from pydantic import BaseModel, SecretStr, computed_field
 from testcontainers.localstack import LocalStackContainer
 
 from hexkit.custom_types import PytestScope
 from hexkit.protocols.objstorage import ObjectStorageProtocol, PresignedPostURL
 from hexkit.providers.s3.provider import S3Config, S3ObjectStorage
 
-LOCALSTACK_IMAGE = "localstack/localstack:0.14.5"
+__all__ = [
+    "LOCALSTACK_IMAGE",
+    "MEBIBYTE",
+    "TEST_FILE_DIR",
+    "TEST_FILE_PATHS",
+    "calc_md5",
+    "FileObject",
+    "S3Fixture",
+    "S3ContainerFixture",
+    "get_s3_container_fixture",
+    "get_clean_s3_fixture",
+    "get_persistent_s3_fixture",
+    "clean_s3_fixture",
+    "persistent_s3_fixture",
+    "s3_fixture",
+    "file_fixture",
+]
+
+
+LOCALSTACK_IMAGE = "localstack/localstack:3.4.0"
 
 TEST_FILE_DIR = Path(__file__).parent.resolve() / "test_files"
 
 TEST_FILE_PATHS = [
     TEST_FILE_DIR / filename
     for filename in os.listdir(TEST_FILE_DIR)
     if filename.startswith("test_") and filename.endswith(".yaml")
@@ -77,15 +97,15 @@
     @property
     def md5(self) -> str:
         """Calculate the md5 hash of the content"""
         return calc_md5(self.content)
 
 
 class S3Fixture:
-    """Yielded by the `s3_fixture` function"""
+    """A fixture with utility methods for tests that use S3 file storage"""
 
     def __init__(self, config: S3Config, storage: S3ObjectStorage):
         """Initialize with config."""
         self.config = config
         self.storage = storage
         self._buckets: set[str] = set()
 
@@ -116,41 +136,117 @@
         """Delete the populated buckets."""
         buckets = self._buckets
         for bucket in list(buckets.difference(buckets_to_exclude or [])):
             await self.storage.delete_bucket(bucket, delete_content=True)
             buckets.discard(bucket)
 
 
-def s3_fixture_function() -> Generator[S3Fixture, None, None]:
-    """Pytest fixture for tests depending on the S3ObjectStorage DAO.
+class S3ContainerFixture(LocalStackContainer):
+    """LocalStack test container with S3 configuration."""
+
+    s3_config: S3Config
+
+    _created_buckets: set[str]
+
+
+def _s3_container_fixture() -> Generator[S3ContainerFixture, None, None]:
+    """Fixture function for getting a running S3 test container."""
+    with S3ContainerFixture(image=LOCALSTACK_IMAGE) as s3_container:
+        s3_endpoint_url = s3_container.get_url()
+        s3_config = S3Config(  # type: ignore [call-arg]
+            s3_endpoint_url=s3_endpoint_url,
+            s3_access_key_id="test",
+            s3_secret_access_key=SecretStr("test"),
+        )
+        s3_container.s3_config = s3_config
+        s3_container._created_buckets = set()
+        yield s3_container
+
+
+def get_s3_container_fixture(
+    scope: PytestScope = "session", name: str = "s3_container"
+):
+    """Get a LocalStack test container fixture with desired scope and name.
+
+    By default, the session scope is used for LocalStack test containers.
+    """
+    return pytest.fixture(_s3_container_fixture, scope=scope, name=name)
+
+
+s3_container_fixture = get_s3_container_fixture()
+
+
+def _persistent_s3_fixture(
+    s3_container: S3ContainerFixture,
+) -> Generator[S3Fixture, None, None]:
+    """Fixture function that gets a persistent S3 storage fixture.
 
-    **Do not call directly** Instead, use get_s3_fixture()
+    The state of the S3 storage is not cleaned up by the function.
     """
-    with LocalStackContainer(image=LOCALSTACK_IMAGE).with_services("s3") as localstack:
-        config = config_from_localstack_container(localstack)
+    config = s3_container.s3_config
+    storage = S3ObjectStorage(config=config)
+    yield S3Fixture(config=config, storage=storage)
 
-        storage = S3ObjectStorage(config=config)
-        yield S3Fixture(config=config, storage=storage)
 
+def get_persistent_s3_fixture(scope: PytestScope = "function", name: str = "s3"):
+    """Get an S3 fixture with desired scope and name.
 
-def get_s3_fixture(scope: PytestScope = "function"):
-    """Produce an S3 fixture with desired scope. Default is the function scope."""
-    return pytest.fixture(s3_fixture_function, scope=scope)
+    The state of the LocalStack test container is persisted across tests.
+
+    By default, the function scope is used for this fixture,
+    while the session scope is used for the underlying LocalStack test container.
+    """
+    return pytest.fixture(_persistent_s3_fixture, scope=scope, name=name)
+
+
+persistent_s3_fixture = get_persistent_s3_fixture()
+
+
+async def _clean_s3_fixture(
+    s3_container: S3ContainerFixture,
+) -> AsyncGenerator[S3Fixture, None]:
+    """Async fixture function that gets a clean S3 storage fixture.
+
+    The clean state is achieved by deleting all S3 buckets upfront.
+    """
+    for s3_fixture in _persistent_s3_fixture(s3_container):
+        container_buckets = s3_container._created_buckets
+        fixture_buckets = s3_fixture.storage._created_buckets
+        fixture_buckets.update(container_buckets)
+        fixture_buckets_before = fixture_buckets.copy()
+        await s3_fixture.storage.delete_created_buckets()
+        deleted_buckets = fixture_buckets_before - fixture_buckets
+        container_buckets.difference_update(deleted_buckets)
+
+        yield s3_fixture
+
+    container_buckets.update(fixture_buckets)
+
+
+def get_clean_s3_fixture(scope: PytestScope = "function", name: str = "s3"):
+    """Get an S3 storage fixture with desired scope and name.
+
+    The state of the S3 storage is reset by deleting all buckets before running tests.
+
+    By default, the function scope is used for this fixture,
+    while the session scope is used for the underlying LocalStack test container.
+    """
+    return pytest_asyncio.fixture(_clean_s3_fixture, scope=scope, name=name)
 
 
-s3_fixture = get_s3_fixture()
+s3_fixture = clean_s3_fixture = get_clean_s3_fixture()
 
 
 @contextmanager
 def temp_file_object(
     bucket_id: str = "default-test-bucket",
     object_id: str = "default-test-object",
     size: int = 5 * MEBIBYTE,
 ) -> Generator[FileObject, None, None]:
-    """Generates a file object with the specified size in bytes."""
+    """Generate a file object with the specified size in bytes."""
     chunk_size = 1024
     chunk = b"\0" * chunk_size
     current_size = 0
     with NamedTemporaryFile("w+b") as temp_file:
         while True:
             if current_size + chunk_size >= size:
                 temp_file.write(chunk[: size - current_size])
```

### Comparing `hexkit-3.0.2/src/hexkit/providers/testing/__init__.py` & `hexkit-3.1.0/src/hexkit/providers/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/providers/testing/eventpub.py` & `hexkit-3.1.0/src/hexkit/providers/testing/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit/utils.py` & `hexkit-3.1.0/src/hexkit/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.2/src/hexkit.egg-info/PKG-INFO` & `hexkit-3.1.0/src/hexkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 3.0.2
+Version: 3.1.0
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -19,29 +19,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic_settings<3,>=2
 Requires-Dist: PyYAML<7,>=6.0
 Provides-Extra: akafka
 Requires-Dist: aiokafka~=0.10.0; extra == "akafka"
-Requires-Dist: jsonschema<5,>=4.21; extra == "akafka"
+Requires-Dist: jsonschema<5,>=4.22; extra == "akafka"
 Provides-Extra: s3
-Requires-Dist: boto3<2,>=1.26.50; extra == "s3"
-Requires-Dist: botocore<2,>=1.29.50; extra == "s3"
+Requires-Dist: boto3<2,>=1.34.104; extra == "s3"
+Requires-Dist: botocore<2,>=1.34.104; extra == "s3"
 Provides-Extra: mongodb
-Requires-Dist: motor<4,>=3.1.1; extra == "mongodb"
+Requires-Dist: motor<4,>=3.4.0; extra == "mongodb"
 Provides-Extra: test-akafka
 Requires-Dist: hexkit[akafka]; extra == "test-akafka"
-Requires-Dist: testcontainers[kafka]<5,>=4.3.3; extra == "test-akafka"
+Requires-Dist: testcontainers[kafka]<5,>=4.4.1; extra == "test-akafka"
 Provides-Extra: test-s3
 Requires-Dist: hexkit[s3]; extra == "test-s3"
-Requires-Dist: testcontainers<5,>=4.3.3; extra == "test-s3"
+Requires-Dist: testcontainers<5,>=4.4.1; extra == "test-s3"
 Provides-Extra: test-mongodb
 Requires-Dist: hexkit[mongodb]; extra == "test-mongodb"
-Requires-Dist: testcontainers[mongo]<5,>=4.3.3; extra == "test-mongodb"
+Requires-Dist: testcontainers[mongo]<5,>=4.4.1; extra == "test-mongodb"
 Provides-Extra: test
 Requires-Dist: hexkit[test-akafka,test-mongodb,test-s3]; extra == "test"
 Provides-Extra: all
 Requires-Dist: hexkit[test]; extra == "all"
 
 ![tests](https://github.com/ghga-de/hexkit/actions/workflows/tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/hexkit.svg)](https://pypi.python.org/pypi/hexkit/)
```

### Comparing `hexkit-3.0.2/src/hexkit.egg-info/SOURCES.txt` & `hexkit-3.1.0/src/hexkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/hexkit/providers/akafka/provider/eventsub.py
 src/hexkit/providers/akafka/provider/utils.py
 src/hexkit/providers/mongodb/__init__.py
 src/hexkit/providers/mongodb/provider.py
 src/hexkit/providers/mongodb/testutils.py
 src/hexkit/providers/mongokafka/__init__.py
 src/hexkit/providers/mongokafka/provider.py
+src/hexkit/providers/mongokafka/testutils.py
 src/hexkit/providers/s3/__init__.py
 src/hexkit/providers/s3/provider.py
 src/hexkit/providers/s3/testutils.py
 src/hexkit/providers/s3/test_files/__init__.py
 src/hexkit/providers/s3/test_files/test_file1.yaml
 src/hexkit/providers/s3/test_files/test_file2.yaml
 src/hexkit/providers/s3/test_files/test_file3.yaml
```

