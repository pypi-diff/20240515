# Comparing `tmp/config-cobra-0.1.4.tar.gz` & `tmp/config-cobra-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config-cobra-0.1.4.tar", last modified: Wed May 15 14:48:39 2024, max compression
+gzip compressed data, was "config-cobra-0.1.5.tar", last modified: Wed May 15 16:52:16 2024, max compression
```

## Comparing `config-cobra-0.1.4.tar` & `config-cobra-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:48:39.540789 config-cobra-0.1.4/
--rw-rw-r--   0 james     (1000) james     (1000)     1062 2024-05-14 18:17:06.000000 config-cobra-0.1.4/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)     3353 2024-05-15 14:48:39.540789 config-cobra-0.1.4/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)     3110 2024-05-15 14:48:15.000000 config-cobra-0.1.4/README.md
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:48:39.540789 config-cobra-0.1.4/config_cobra.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)     3353 2024-05-15 14:48:39.000000 config-cobra-0.1.4/config_cobra.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      502 2024-05-15 14:48:39.000000 config-cobra-0.1.4/config_cobra.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2024-05-15 14:48:39.000000 config-cobra-0.1.4/config_cobra.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)       47 2024-05-15 14:48:39.000000 config-cobra-0.1.4/config_cobra.egg-info/entry_points.txt
--rw-rw-r--   0 james     (1000) james     (1000)      215 2024-05-15 14:48:39.000000 config-cobra-0.1.4/config_cobra.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)       10 2024-05-15 14:48:39.000000 config-cobra-0.1.4/config_cobra.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)       38 2024-05-15 14:48:39.540789 config-cobra-0.1.4/setup.cfg
--rw-rw-r--   0 james     (1000) james     (1000)      702 2024-05-15 14:48:10.000000 config-cobra-0.1.4/setup.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:48:39.540789 config-cobra-0.1.4/src/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 12:14:48.000000 config-cobra-0.1.4/src/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     1107 2024-05-14 18:08:03.000000 config-cobra-0.1.4/src/app.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:48:39.540789 config-cobra-0.1.4/src/db/
--rw-rw-r--   0 james     (1000) james     (1000)       93 2024-05-14 18:00:13.000000 config-cobra-0.1.4/src/db/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     1259 2024-05-14 16:49:00.000000 config-cobra-0.1.4/src/db/database_instance.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:48:39.540789 config-cobra-0.1.4/src/runner/
--rw-rw-r--   0 james     (1000) james     (1000)       39 2024-05-14 13:20:33.000000 config-cobra-0.1.4/src/runner/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     5140 2024-05-14 18:08:55.000000 config-cobra-0.1.4/src/runner/update_runner.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:48:39.540789 config-cobra-0.1.4/src/settings/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 13:11:52.000000 config-cobra-0.1.4/src/settings/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)      301 2024-05-15 14:47:58.000000 config-cobra-0.1.4/src/settings/settings.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:48:39.540789 config-cobra-0.1.4/tests/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 12:30:51.000000 config-cobra-0.1.4/tests/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 14:48:39.540789 config-cobra-0.1.4/tests/runner/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 16:29:23.000000 config-cobra-0.1.4/tests/runner/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     2174 2024-05-14 18:03:12.000000 config-cobra-0.1.4/tests/runner/update_runner_unit_test.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 16:52:16.533653 config-cobra-0.1.5/
+-rw-rw-r--   0 james     (1000) james     (1000)     1062 2024-05-14 18:17:06.000000 config-cobra-0.1.5/LICENSE
+-rw-rw-r--   0 james     (1000) james     (1000)     3353 2024-05-15 16:52:16.533653 config-cobra-0.1.5/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)     3110 2024-05-15 16:52:09.000000 config-cobra-0.1.5/README.md
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 16:52:16.533653 config-cobra-0.1.5/config_cobra.egg-info/
+-rw-rw-r--   0 james     (1000) james     (1000)     3353 2024-05-15 16:52:16.000000 config-cobra-0.1.5/config_cobra.egg-info/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      502 2024-05-15 16:52:16.000000 config-cobra-0.1.5/config_cobra.egg-info/SOURCES.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        1 2024-05-15 16:52:16.000000 config-cobra-0.1.5/config_cobra.egg-info/dependency_links.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       47 2024-05-15 16:52:16.000000 config-cobra-0.1.5/config_cobra.egg-info/entry_points.txt
+-rw-rw-r--   0 james     (1000) james     (1000)      215 2024-05-15 16:52:16.000000 config-cobra-0.1.5/config_cobra.egg-info/requires.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       10 2024-05-15 16:52:16.000000 config-cobra-0.1.5/config_cobra.egg-info/top_level.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       38 2024-05-15 16:52:16.533653 config-cobra-0.1.5/setup.cfg
+-rw-rw-r--   0 james     (1000) james     (1000)      702 2024-05-15 16:52:03.000000 config-cobra-0.1.5/setup.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 16:52:16.533653 config-cobra-0.1.5/src/
+-rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 12:14:48.000000 config-cobra-0.1.5/src/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1107 2024-05-14 18:08:03.000000 config-cobra-0.1.5/src/app.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 16:52:16.533653 config-cobra-0.1.5/src/db/
+-rw-rw-r--   0 james     (1000) james     (1000)       93 2024-05-14 18:00:13.000000 config-cobra-0.1.5/src/db/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1259 2024-05-14 16:49:00.000000 config-cobra-0.1.5/src/db/database_instance.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 16:52:16.533653 config-cobra-0.1.5/src/runner/
+-rw-rw-r--   0 james     (1000) james     (1000)       39 2024-05-14 13:20:33.000000 config-cobra-0.1.5/src/runner/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     5140 2024-05-14 18:08:55.000000 config-cobra-0.1.5/src/runner/update_runner.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 16:52:16.533653 config-cobra-0.1.5/src/settings/
+-rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 13:11:52.000000 config-cobra-0.1.5/src/settings/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)      301 2024-05-15 15:11:03.000000 config-cobra-0.1.5/src/settings/settings.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 16:52:16.533653 config-cobra-0.1.5/tests/
+-rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 12:30:51.000000 config-cobra-0.1.5/tests/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-15 16:52:16.533653 config-cobra-0.1.5/tests/runner/
+-rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-14 16:29:23.000000 config-cobra-0.1.5/tests/runner/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     2174 2024-05-14 18:03:12.000000 config-cobra-0.1.5/tests/runner/update_runner_unit_test.py
```

### Comparing `config-cobra-0.1.4/LICENSE` & `config-cobra-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `config-cobra-0.1.4/PKG-INFO` & `config-cobra-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: config-cobra
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple yaml to database updater
 Home-page: https://github.com/JTSG1/configCobra
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ConfigCobra v0.1.4
+# ConfigCobra v0.1.5
 
 This is a basic project to provide a way to deploy database configuration to remote databases via pipelines. The basic premise is that we can control the config via yaml file declarations.  These yaml files provide instructions on what operation should be performed on data and the fields associated with it.
 
 This is the initial version and the feature set is somewhat limited but useful for my purposes.
 
 ----
 
 ## features
 
-Features in v0.1.4 of ConfigCobra
+Features in v0.1.5 of ConfigCobra
 
 - postgres data deployments
 - Supports standard CRUD operations
 - basic local validation of fields supplied against a list of columns
 - flexible pk field names
 
 Database connection is controlled by environment variables since the intended use case for this is inside a container
```

### Comparing `config-cobra-0.1.4/README.md` & `config-cobra-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# ConfigCobra v0.1.4
+# ConfigCobra v0.1.5
 
 This is a basic project to provide a way to deploy database configuration to remote databases via pipelines. The basic premise is that we can control the config via yaml file declarations.  These yaml files provide instructions on what operation should be performed on data and the fields associated with it.
 
 This is the initial version and the feature set is somewhat limited but useful for my purposes.
 
 ----
 
 ## features
 
-Features in v0.1.4 of ConfigCobra
+Features in v0.1.5 of ConfigCobra
 
 - postgres data deployments
 - Supports standard CRUD operations
 - basic local validation of fields supplied against a list of columns
 - flexible pk field names
 
 Database connection is controlled by environment variables since the intended use case for this is inside a container
```

### Comparing `config-cobra-0.1.4/config_cobra.egg-info/PKG-INFO` & `config-cobra-0.1.5/config_cobra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: config-cobra
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple yaml to database updater
 Home-page: https://github.com/JTSG1/configCobra
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ConfigCobra v0.1.4
+# ConfigCobra v0.1.5
 
 This is a basic project to provide a way to deploy database configuration to remote databases via pipelines. The basic premise is that we can control the config via yaml file declarations.  These yaml files provide instructions on what operation should be performed on data and the fields associated with it.
 
 This is the initial version and the feature set is somewhat limited but useful for my purposes.
 
 ----
 
 ## features
 
-Features in v0.1.4 of ConfigCobra
+Features in v0.1.5 of ConfigCobra
 
 - postgres data deployments
 - Supports standard CRUD operations
 - basic local validation of fields supplied against a list of columns
 - flexible pk field names
 
 Database connection is controlled by environment variables since the intended use case for this is inside a container
```

### Comparing `config-cobra-0.1.4/setup.py` & `config-cobra-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='config-cobra',
-    version='0.1.4',
+    version='0.1.5',
     description='A simple yaml to database updater',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/JTSG1/configCobra',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `config-cobra-0.1.4/src/app.py` & `config-cobra-0.1.5/src/app.py`

 * *Files identical despite different names*

### Comparing `config-cobra-0.1.4/src/db/database_instance.py` & `config-cobra-0.1.5/src/db/database_instance.py`

 * *Files identical despite different names*

### Comparing `config-cobra-0.1.4/src/runner/update_runner.py` & `config-cobra-0.1.5/src/runner/update_runner.py`

 * *Files identical despite different names*

### Comparing `config-cobra-0.1.4/tests/runner/update_runner_unit_test.py` & `config-cobra-0.1.5/tests/runner/update_runner_unit_test.py`

 * *Files identical despite different names*

