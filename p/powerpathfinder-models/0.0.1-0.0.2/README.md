# Comparing `tmp/powerpathfinder_models-0.0.1.tar.gz` & `tmp/powerpathfinder_models-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpathfinder_models-0.0.1.tar", last modified: Sun May 12 16:28:34 2024, max compression
+gzip compressed data, was "powerpathfinder_models-0.0.2.tar", last modified: Tue May 14 22:16:58 2024, max compression
```

## Comparing `powerpathfinder_models-0.0.1.tar` & `powerpathfinder_models-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:34.516845 powerpathfinder_models-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-12 16:28:34.516845 powerpathfinder_models-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:34.512845 powerpathfinder_models-0.0.1/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:34.512845 powerpathfinder_models-0.0.1/common/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:34.512845 powerpathfinder_models-0.0.1/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/models/charger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/models/route.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/common/models/valuation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:34.516845 powerpathfinder_models-0.0.1/powerpathfinder_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-12 16:28:34.000000 powerpathfinder_models-0.0.1/powerpathfinder_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-12 16:28:34.000000 powerpathfinder_models-0.0.1/powerpathfinder_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:28:34.000000 powerpathfinder_models-0.0.1/powerpathfinder_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 16:28:34.000000 powerpathfinder_models-0.0.1/powerpathfinder_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 16:28:34.000000 powerpathfinder_models-0.0.1/powerpathfinder_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 16:28:30.000000 powerpathfinder_models-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 16:28:34.516845 powerpathfinder_models-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.795967 powerpathfinder_models-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 22:16:58.795967 powerpathfinder_models-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.791967 powerpathfinder_models-0.0.2/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.791967 powerpathfinder_models-0.0.2/common/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.791967 powerpathfinder_models-0.0.2/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/charger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/valuation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.795967 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 22:16:58.795967 powerpathfinder_models-0.0.2/setup.cfg
```

### Comparing `powerpathfinder_models-0.0.1/common/models/charger.py` & `powerpathfinder_models-0.0.2/common/models/charger.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-0.0.1/common/models/payment.py` & `powerpathfinder_models-0.0.2/common/models/payment.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-0.0.1/common/models/route.py` & `powerpathfinder_models-0.0.2/common/models/route.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-0.0.1/common/models/user.py` & `powerpathfinder_models-0.0.2/common/models/user.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-0.0.1/common/models/valuation.py` & `powerpathfinder_models-0.0.2/common/models/valuation.py`

 * *Files identical despite different names*

