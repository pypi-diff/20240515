# Comparing `tmp/ddeutil_io-0.1.2.tar.gz` & `tmp/ddeutil_io-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_io-0.1.2.tar", last modified: Tue May 14 15:55:47 2024, max compression
+gzip compressed data, was "ddeutil_io-0.1.3.tar", last modified: Tue May 14 16:24:30 2024, max compression
```

## Comparing `ddeutil_io-0.1.2.tar` & `ddeutil_io-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.179581 ddeutil_io-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.179581 ddeutil_io-0.1.2/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.179581 ddeutil_io-0.1.2/src/ddeutil/io/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__about__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.183581 ddeutil_io-0.1.2/src/ddeutil/io/__base/
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__base/__regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__base/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    17049 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.183581 ddeutil_io-0.1.2/src/ddeutil/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9315 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.183581 ddeutil_io-0.1.2/src/ddeutil/node/base/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/base/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/base/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/base/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/datasets_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/src/ddeutil/node/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/vendors/boto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/vendors/sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/src/ddeutil/node/vendors/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:55:47.000000 ddeutil_io-0.1.2/src/ddeutil_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:55:47.187581 ddeutil_io-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_base_file_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_config_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-14 15:55:42.000000 ddeutil_io-0.1.2/tests/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.386695 ddeutil_io-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-14 16:24:30.386695 ddeutil_io-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:24:30.386695 ddeutil_io-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.378695 ddeutil_io-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.378695 ddeutil_io-0.1.3/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.382695 ddeutil_io-0.1.3/src/ddeutil/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__about__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.382695 ddeutil_io-0.1.3/src/ddeutil/io/__base/
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__base/__regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__base/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17049 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.382695 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.382695 ddeutil_io-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_file_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_config_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_register.py
```

### Comparing `ddeutil_io-0.1.2/LICENSE` & `ddeutil_io-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/pyproject.toml` & `ddeutil_io-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/__base/__init__.py` & `ddeutil_io-0.1.3/src/ddeutil/io/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/__base/__regex.py` & `ddeutil_io-0.1.3/src/ddeutil/io/__base/__regex.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/__base/files.py` & `ddeutil_io-0.1.3/src/ddeutil/io/__base/files.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/__base/utils.py` & `ddeutil_io-0.1.3/src/ddeutil/io/__base/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/config.py` & `ddeutil_io-0.1.3/src/ddeutil/io/config.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/exceptions.py` & `ddeutil_io-0.1.3/src/ddeutil/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/models.py` & `ddeutil_io-0.1.3/src/ddeutil/io/models.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/register.py` & `ddeutil_io-0.1.3/src/ddeutil/io/register.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil/io/utils.py` & `ddeutil_io-0.1.3/src/ddeutil/io/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/src/ddeutil_io.egg-info/SOURCES.txt` & `ddeutil_io-0.1.3/src/ddeutil_io.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -8,33 +8,14 @@
 src/ddeutil/io/models.py
 src/ddeutil/io/register.py
 src/ddeutil/io/utils.py
 src/ddeutil/io/__base/__init__.py
 src/ddeutil/io/__base/__regex.py
 src/ddeutil/io/__base/files.py
 src/ddeutil/io/__base/utils.py
-src/ddeutil/node/__init__.py
-src/ddeutil/node/action.py
-src/ddeutil/node/apps.py
-src/ddeutil/node/connection.py
-src/ddeutil/node/datasets.py
-src/ddeutil/node/datasets_legacy.py
-src/ddeutil/node/exceptions.py
-src/ddeutil/node/loader.py
-src/ddeutil/node/node.py
-src/ddeutil/node/schedule.py
-src/ddeutil/node/schema.py
-src/ddeutil/node/base/__init__.py
-src/ddeutil/node/base/converter.py
-src/ddeutil/node/base/loader.py
-src/ddeutil/node/base/models.py
-src/ddeutil/node/vendors/__init__.py
-src/ddeutil/node/vendors/boto.py
-src/ddeutil/node/vendors/sftp.py
-src/ddeutil/node/vendors/vpn.py
 src/ddeutil_io.egg-info/PKG-INFO
 src/ddeutil_io.egg-info/SOURCES.txt
 src/ddeutil_io.egg-info/dependency_links.txt
 src/ddeutil_io.egg-info/requires.txt
 src/ddeutil_io.egg-info/top_level.txt
 tests/test_base_csv.py
 tests/test_base_dir.py
```

### Comparing `ddeutil_io-0.1.2/tests/test_base_csv.py` & `ddeutil_io-0.1.3/tests/test_base_csv.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/tests/test_base_dir.py` & `ddeutil_io-0.1.3/tests/test_base_dir.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/tests/test_base_env.py` & `ddeutil_io-0.1.3/tests/test_base_env.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/tests/test_base_file.py` & `ddeutil_io-0.1.3/tests/test_base_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/tests/test_base_file_yaml.py` & `ddeutil_io-0.1.3/tests/test_base_file_yaml.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/tests/test_config_file.py` & `ddeutil_io-0.1.3/tests/test_config_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/tests/test_config_sqlite.py` & `ddeutil_io-0.1.3/tests/test_config_sqlite.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/tests/test_models.py` & `ddeutil_io-0.1.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.2/tests/test_register.py` & `ddeutil_io-0.1.3/tests/test_register.py`

 * *Files identical despite different names*

