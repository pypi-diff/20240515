# Comparing `tmp/opencvv-0.1.tar.gz` & `tmp/opencvv-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencvv-0.1.tar", last modified: Mon May 13 08:49:43 2024, max compression
+gzip compressed data, was "opencvv-0.2.tar", last modified: Wed May 15 07:51:40 2024, max compression
```

## Comparing `opencvv-0.1.tar` & `opencvv-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 savioratharv   (501) staff       (20)        0 2024-05-13 08:49:43.225069 opencvv-0.1/
--rw-r--r--   0 savioratharv   (501) staff       (20)      254 2024-05-13 08:49:43.224938 opencvv-0.1/PKG-INFO
--rw-rw-r--   0 savioratharv   (501) staff       (20)        0 2023-12-10 01:56:46.000000 opencvv-0.1/README.md
-drwxr-xr-x   0 savioratharv   (501) staff       (20)        0 2024-05-13 08:49:43.224271 opencvv-0.1/opencvv/
--rw-rw-r--   0 savioratharv   (501) staff       (20)        0 2023-12-10 01:58:10.000000 opencvv-0.1/opencvv/__init__.py
--rw-rw-r--   0 savioratharv   (501) staff       (20)      208 2023-12-10 01:58:02.000000 opencvv-0.1/opencvv/text_reader.py
-drwxr-xr-x   0 savioratharv   (501) staff       (20)        0 2024-05-13 08:49:43.224758 opencvv-0.1/opencvv.egg-info/
--rw-r--r--   0 savioratharv   (501) staff       (20)      254 2024-05-13 08:49:43.000000 opencvv-0.1/opencvv.egg-info/PKG-INFO
--rw-r--r--   0 savioratharv   (501) staff       (20)      185 2024-05-13 08:49:43.000000 opencvv-0.1/opencvv.egg-info/SOURCES.txt
--rw-r--r--   0 savioratharv   (501) staff       (20)        1 2024-05-13 08:49:43.000000 opencvv-0.1/opencvv.egg-info/dependency_links.txt
--rw-r--r--   0 savioratharv   (501) staff       (20)        8 2024-05-13 08:49:43.000000 opencvv-0.1/opencvv.egg-info/top_level.txt
--rw-r--r--   0 savioratharv   (501) staff       (20)       38 2024-05-13 08:49:43.225122 opencvv-0.1/setup.cfg
--rw-rw-r--   0 savioratharv   (501) staff       (20)      449 2024-05-13 08:48:55.000000 opencvv-0.1/setup.py
+drwxr-xr-x   0 savioratharv   (501) staff       (20)        0 2024-05-15 07:51:40.594204 opencvv-0.2/
+-rw-r--r--   0 savioratharv   (501) staff       (20)      254 2024-05-15 07:51:40.594056 opencvv-0.2/PKG-INFO
+-rw-rw-r--   0 savioratharv   (501) staff       (20)        0 2023-12-10 01:56:46.000000 opencvv-0.2/README.md
+drwxr-xr-x   0 savioratharv   (501) staff       (20)        0 2024-05-15 07:51:40.593132 opencvv-0.2/opencvv/
+-rw-rw-r--   0 savioratharv   (501) staff       (20)        0 2023-12-10 01:58:10.000000 opencvv-0.2/opencvv/__init__.py
+-rw-rw-r--   0 savioratharv   (501) staff       (20)      208 2023-12-10 01:58:02.000000 opencvv-0.2/opencvv/text_reader.py
+drwxr-xr-x   0 savioratharv   (501) staff       (20)        0 2024-05-15 07:51:40.593855 opencvv-0.2/opencvv.egg-info/
+-rw-r--r--   0 savioratharv   (501) staff       (20)      254 2024-05-15 07:51:40.000000 opencvv-0.2/opencvv.egg-info/PKG-INFO
+-rw-r--r--   0 savioratharv   (501) staff       (20)      185 2024-05-15 07:51:40.000000 opencvv-0.2/opencvv.egg-info/SOURCES.txt
+-rw-r--r--   0 savioratharv   (501) staff       (20)        1 2024-05-15 07:51:40.000000 opencvv-0.2/opencvv.egg-info/dependency_links.txt
+-rw-r--r--   0 savioratharv   (501) staff       (20)        8 2024-05-15 07:51:40.000000 opencvv-0.2/opencvv.egg-info/top_level.txt
+-rw-r--r--   0 savioratharv   (501) staff       (20)       38 2024-05-15 07:51:40.594263 opencvv-0.2/setup.cfg
+-rw-rw-r--   0 savioratharv   (501) staff       (20)      449 2024-05-15 07:51:26.000000 opencvv-0.2/setup.py
```

