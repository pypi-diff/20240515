# Comparing `tmp/config-cobra-0.1.0.tar.gz` & `tmp/config-cobra-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config-cobra-0.1.0.tar", last modified: Wed May 15 13:51:33 2024, max compression
+gzip compressed data, was "config-cobra-0.1.1.tar", last modified: Wed May 15 14:12:56 2024, max compression
```

## Comparing `config-cobra-0.1.0.tar` & `config-cobra-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 13:51:33.078806 config-cobra-0.1.0/
--rw-rw-r--   0 james     (1000) james     (1000)     1062 2024-05-14 18:17:06.000000 config-cobra-0.1.0/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)      159 2024-05-15 13:51:33.078806 config-cobra-0.1.0/PKG-INFO
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 13:51:33.078806 config-cobra-0.1.0/config_cobra.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)      159 2024-05-15 13:51:33.000000 config-cobra-0.1.0/config_cobra.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      492 2024-05-15 13:51:33.000000 config-cobra-0.1.0/config_cobra.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2024-05-15 13:51:33.000000 config-cobra-0.1.0/config_cobra.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)       47 2024-05-15 13:51:33.000000 config-cobra-0.1.0/config_cobra.egg-info/entry_points.txt
--rw-rw-r--   0 james     (1000) james     (1000)      215 2024-05-15 13:51:33.000000 config-cobra-0.1.0/config_cobra.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)       10 2024-05-15 13:51:33.000000 config-cobra-0.1.0/config_cobra.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)       38 2024-05-15 13:51:33.078806 config-cobra-0.1.0/setup.cfg
--rw-rw-r--   0 james     (1000) james     (1000)      405 2024-05-14 18:06:47.000000 config-cobra-0.1.0/setup.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 13:51:33.078806 config-cobra-0.1.0/src/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 12:14:48.000000 config-cobra-0.1.0/src/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     1107 2024-05-14 18:08:03.000000 config-cobra-0.1.0/src/app.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 13:51:33.078806 config-cobra-0.1.0/src/db/
--rw-rw-r--   0 james     (1000) james     (1000)       93 2024-05-14 18:00:13.000000 config-cobra-0.1.0/src/db/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     1259 2024-05-14 16:49:00.000000 config-cobra-0.1.0/src/db/database_instance.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 13:51:33.078806 config-cobra-0.1.0/src/runner/
--rw-rw-r--   0 james     (1000) james     (1000)       39 2024-05-14 13:20:33.000000 config-cobra-0.1.0/src/runner/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     5140 2024-05-14 18:08:55.000000 config-cobra-0.1.0/src/runner/update_runner.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 13:51:33.078806 config-cobra-0.1.0/src/settings/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 13:11:52.000000 config-cobra-0.1.0/src/settings/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)      301 2024-05-14 18:12:45.000000 config-cobra-0.1.0/src/settings/settings.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 13:51:33.078806 config-cobra-0.1.0/tests/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 12:30:51.000000 config-cobra-0.1.0/tests/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 13:51:33.078806 config-cobra-0.1.0/tests/runner/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 16:29:23.000000 config-cobra-0.1.0/tests/runner/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     2174 2024-05-14 18:03:12.000000 config-cobra-0.1.0/tests/runner/update_runner_unit_test.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:12:56.370673 config-cobra-0.1.1/
+-rw-rw-r--   0 james     (1000) james     (1000)     1062 2024-05-14 18:17:06.000000 config-cobra-0.1.1/LICENSE
+-rw-rw-r--   0 james     (1000) james     (1000)      181 2024-05-15 14:12:56.370673 config-cobra-0.1.1/PKG-INFO
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:12:56.370673 config-cobra-0.1.1/config_cobra.egg-info/
+-rw-rw-r--   0 james     (1000) james     (1000)      181 2024-05-15 14:12:56.000000 config-cobra-0.1.1/config_cobra.egg-info/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      492 2024-05-15 14:12:56.000000 config-cobra-0.1.1/config_cobra.egg-info/SOURCES.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        1 2024-05-15 14:12:56.000000 config-cobra-0.1.1/config_cobra.egg-info/dependency_links.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       47 2024-05-15 14:12:56.000000 config-cobra-0.1.1/config_cobra.egg-info/entry_points.txt
+-rw-rw-r--   0 james     (1000) james     (1000)      215 2024-05-15 14:12:56.000000 config-cobra-0.1.1/config_cobra.egg-info/requires.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       10 2024-05-15 14:12:56.000000 config-cobra-0.1.1/config_cobra.egg-info/top_level.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       38 2024-05-15 14:12:56.370673 config-cobra-0.1.1/setup.cfg
+-rw-rw-r--   0 james     (1000) james     (1000)      477 2024-05-15 14:12:27.000000 config-cobra-0.1.1/setup.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:12:56.370673 config-cobra-0.1.1/src/
+-rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 12:14:48.000000 config-cobra-0.1.1/src/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1107 2024-05-14 18:08:03.000000 config-cobra-0.1.1/src/app.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:12:56.370673 config-cobra-0.1.1/src/db/
+-rw-rw-r--   0 james     (1000) james     (1000)       93 2024-05-14 18:00:13.000000 config-cobra-0.1.1/src/db/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1259 2024-05-14 16:49:00.000000 config-cobra-0.1.1/src/db/database_instance.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:12:56.370673 config-cobra-0.1.1/src/runner/
+-rw-rw-r--   0 james     (1000) james     (1000)       39 2024-05-14 13:20:33.000000 config-cobra-0.1.1/src/runner/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     5140 2024-05-14 18:08:55.000000 config-cobra-0.1.1/src/runner/update_runner.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:12:56.370673 config-cobra-0.1.1/src/settings/
+-rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 13:11:52.000000 config-cobra-0.1.1/src/settings/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)      301 2024-05-14 18:12:45.000000 config-cobra-0.1.1/src/settings/settings.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:12:56.370673 config-cobra-0.1.1/tests/
+-rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 12:30:51.000000 config-cobra-0.1.1/tests/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:12:56.370673 config-cobra-0.1.1/tests/runner/
+-rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 16:29:23.000000 config-cobra-0.1.1/tests/runner/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     2174 2024-05-14 18:03:12.000000 config-cobra-0.1.1/tests/runner/update_runner_unit_test.py
```

### Comparing `config-cobra-0.1.0/LICENSE` & `config-cobra-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `config-cobra-0.1.0/src/app.py` & `config-cobra-0.1.1/src/app.py`

 * *Files identical despite different names*

### Comparing `config-cobra-0.1.0/src/db/database_instance.py` & `config-cobra-0.1.1/src/db/database_instance.py`

 * *Files identical despite different names*

### Comparing `config-cobra-0.1.0/src/runner/update_runner.py` & `config-cobra-0.1.1/src/runner/update_runner.py`

 * *Files identical despite different names*

### Comparing `config-cobra-0.1.0/tests/runner/update_runner_unit_test.py` & `config-cobra-0.1.1/tests/runner/update_runner_unit_test.py`

 * *Files identical despite different names*

