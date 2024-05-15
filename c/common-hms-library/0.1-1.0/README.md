# Comparing `tmp/common_hms_library-0.1.tar.gz` & `tmp/common_hms_library-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_hms_library-0.1.tar", last modified: Mon May 13 14:29:08 2024, max compression
+gzip compressed data, was "common_hms_library-1.0.tar", last modified: Wed May 15 05:05:00 2024, max compression
```

## Comparing `common_hms_library-0.1.tar` & `common_hms_library-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 softprime  (1000) softprime  (1000)        0 2024-05-13 14:29:08.803676 common_hms_library-0.1/
--rw-r--r--   0 softprime  (1000) softprime  (1000)       60 2024-05-13 14:29:08.803676 common_hms_library-0.1/PKG-INFO
-drwxrwxr-x   0 softprime  (1000) softprime  (1000)        0 2024-05-13 14:29:08.799676 common_hms_library-0.1/common_hms_library/
--rw-rw-r--   0 softprime  (1000) softprime  (1000)       43 2024-05-13 14:22:30.000000 common_hms_library-0.1/common_hms_library/__init__.py
--rw-rw-r--   0 softprime  (1000) softprime  (1000)      480 2024-05-13 14:22:30.000000 common_hms_library-0.1/common_hms_library/age_calculation.py
-drwxrwxr-x   0 softprime  (1000) softprime  (1000)        0 2024-05-13 14:29:08.803676 common_hms_library-0.1/common_hms_library.egg-info/
--rw-r--r--   0 softprime  (1000) softprime  (1000)       60 2024-05-13 14:29:08.000000 common_hms_library-0.1/common_hms_library.egg-info/PKG-INFO
--rw-rw-r--   0 softprime  (1000) softprime  (1000)      245 2024-05-13 14:29:08.000000 common_hms_library-0.1/common_hms_library.egg-info/SOURCES.txt
--rw-rw-r--   0 softprime  (1000) softprime  (1000)        1 2024-05-13 14:29:08.000000 common_hms_library-0.1/common_hms_library.egg-info/dependency_links.txt
--rw-rw-r--   0 softprime  (1000) softprime  (1000)       19 2024-05-13 14:29:08.000000 common_hms_library-0.1/common_hms_library.egg-info/top_level.txt
--rw-rw-r--   0 softprime  (1000) softprime  (1000)       38 2024-05-13 14:29:08.803676 common_hms_library-0.1/setup.cfg
--rw-rw-r--   0 softprime  (1000) softprime  (1000)      160 2024-05-13 14:22:30.000000 common_hms_library-0.1/setup.py
+drwxrwxr-x   0 softprime  (1000) softprime  (1000)        0 2024-05-15 05:05:00.225481 common_hms_library-1.0/
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)      222 2024-05-15 05:05:00.225481 common_hms_library-1.0/PKG-INFO
+drwxrwxr-x   0 softprime  (1000) softprime  (1000)        0 2024-05-15 05:05:00.225481 common_hms_library-1.0/common_hms_library/
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)       43 2024-05-13 14:22:30.000000 common_hms_library-1.0/common_hms_library/__init__.py
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)      480 2024-05-13 14:22:30.000000 common_hms_library-1.0/common_hms_library/age_calculation.py
+drwxrwxr-x   0 softprime  (1000) softprime  (1000)        0 2024-05-15 05:05:00.225481 common_hms_library-1.0/common_hms_library.egg-info/
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)      222 2024-05-15 05:05:00.000000 common_hms_library-1.0/common_hms_library.egg-info/PKG-INFO
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)      245 2024-05-15 05:05:00.000000 common_hms_library-1.0/common_hms_library.egg-info/SOURCES.txt
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)        1 2024-05-15 05:05:00.000000 common_hms_library-1.0/common_hms_library.egg-info/dependency_links.txt
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)       19 2024-05-15 05:05:00.000000 common_hms_library-1.0/common_hms_library.egg-info/top_level.txt
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)       38 2024-05-15 05:05:00.225481 common_hms_library-1.0/setup.cfg
+-rw-rw-r--   0 softprime  (1000) softprime  (1000)      268 2024-05-15 05:03:31.000000 common_hms_library-1.0/setup.py
```

