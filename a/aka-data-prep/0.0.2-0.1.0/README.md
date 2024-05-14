# Comparing `tmp/aka-data-prep-0.0.2.tar.gz` & `tmp/aka-data-prep-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka-data-prep-0.0.2.tar", last modified: Tue May 14 18:19:50 2024, max compression
+gzip compressed data, was "aka-data-prep-0.1.0.tar", last modified: Tue May 14 21:37:52 2024, max compression
```

## Comparing `aka-data-prep-0.0.2.tar` & `aka-data-prep-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/
--rw-rw-rw-   0        0        0      190 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/aka_data_prep/
--rw-rw-rw-   0        0        0      107 2024-05-14 08:17:52.000000 aka-data-prep-0.0.2/aka_data_prep/__init__.py
--rw-rw-rw-   0        0        0    18734 2024-05-14 18:03:42.000000 aka-data-prep-0.0.2/aka_data_prep/aka_data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/
--rw-rw-rw-   0        0        0      190 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-05-14 18:17:44.000000 aka-data-prep-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/
+-rw-rw-rw-   0        0        0      190 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/aka_data_prep/
+-rw-rw-rw-   0        0        0      124 2024-05-14 20:45:06.000000 aka-data-prep-0.1.0/aka_data_prep/__init__.py
+-rw-rw-rw-   0        0        0    28453 2024-05-14 21:33:14.000000 aka-data-prep-0.1.0/aka_data_prep/aka_data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/
+-rw-rw-rw-   0        0        0      190 2024-05-14 21:37:52.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:37:52.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-14 21:37:52.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 21:37:52.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-05-14 21:37:28.000000 aka-data-prep-0.1.0/setup.py
```

