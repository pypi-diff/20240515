# Comparing `tmp/crc_bonfire-5.7.2.tar.gz` & `tmp/crc_bonfire-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc_bonfire-5.7.2.tar", last modified: Thu May  2 18:50:23 2024, max compression
+gzip compressed data, was "crc_bonfire-5.8.0.tar", last modified: Wed May 15 13:42:13 2024, max compression
```

## Comparing `crc_bonfire-5.7.2.tar` & `crc_bonfire-5.8.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.958171 crc_bonfire-5.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.962171 crc_bonfire-5.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.962171 crc_bonfire-5.7.2/bonfire/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47966 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/bonfire.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/elastic_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/openshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    29373 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/qontract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.962171 crc_bonfire-5.7.2/bonfire/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/default-iqe-cji.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/local-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/reservation-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/build_deploy.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/cicd/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/cicd/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/cicd/bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/crc_bonfire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2975380 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/entry_points.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/data/namespace_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/data/reservation_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_app_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_bonfire.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_get_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/utils/search_replace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.259021 crc_bonfire-5.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.267021 crc_bonfire-5.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.267021 crc_bonfire-5.8.0/bonfire/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48982 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/configmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/elastic_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29373 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/qontract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.267021 crc_bonfire-5.8.0/bonfire/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/default-iqe-cji.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/local-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/resources/reservation-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/bonfire/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/build_deploy.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.267021 crc_bonfire-5.8.0/cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/cicd/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/cicd/bootstrap.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/crc_bonfire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 13:42:13.000000 crc_bonfire-5.8.0/crc_bonfire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2975380 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/entry_points.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/data/namespace_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/data/reservation_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_app_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:42:13.271021 crc_bonfire-5.8.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-15 13:42:02.000000 crc_bonfire-5.8.0/utils/search_replace.py
```

### Comparing `crc_bonfire-5.7.2/.github/workflows/release.yml` & `crc_bonfire-5.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/.github/workflows/tests.yml` & `crc_bonfire-5.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/.gitignore` & `crc_bonfire-5.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/CONTRIBUTING.md` & `crc_bonfire-5.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/Dockerfile` & `crc_bonfire-5.8.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/PKG-INFO` & `crc_bonfire-5.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 5.7.2
+Version: 5.8.0
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
 Home-page: https://www.github.com/RedHatInsights/bonfire
 Author: Brandon Squizzato
 Author-email: bsquizza@redhat.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crc_bonfire-5.7.2/README.md` & `crc_bonfire-5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/bonfire.py` & `crc_bonfire-5.8.0/bonfire/bonfire.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     get_console_url,
     get_pool_size_limit,
     get_reserved_namespace_quantity,
 )
 from bonfire.processor import TemplateProcessor, process_clowd_env, process_iqe_cji
 from bonfire.qontract import get_apps_for_env, sub_refs
 from bonfire.secrets import import_secrets_from_dir
+from bonfire.configmaps import import_configmaps_from_dir
 from bonfire.utils import (
     FatalError,
     check_pypi,
     find_what_depends_on,
     get_version,
     split_equals,
     validate_time_string,
@@ -901,19 +902,19 @@
         log.error("Hit timeout error: %s", err)
         _error("namespace wait timed out")
 
 
 @namespace.command("describe")
 @click.argument("namespace", required=False, type=str)
 @click.option(
-        "--output",
-        "-o",
-        default="cli",
-        help="which output format to return the data in",
-        type=click.Choice(["cli", "json"], case_sensitive=False),
+    "--output",
+    "-o",
+    default="cli",
+    help="which output format to return the data in",
+    type=click.Choice(["cli", "json"], case_sensitive=False),
 )
 def _describe_namespace(namespace, output):
     """Get current namespace info"""
     if not namespace:
         namespace = current_namespace_or_error()
 
     click.echo(describe_namespace(namespace, output))
@@ -1249,20 +1250,34 @@
 @click.option(
     "--import-secrets",
     is_flag=True,
     help="Import secrets from local directory at deploy time",
     default=False,
 )
 @click.option(
+    "--import-configmaps",
+    is_flag=True,
+    help="Import configmaps from local directory at deploy time",
+    default=False,
+)
+@click.option(
     "--secrets-dir",
     type=str,
-    help="Directory to use for secrets import (default: " "$XDG_CONFIG_HOME/bonfire/secrets/)",
+    help="Directory to use for secrets import (default: $XDG_CONFIG_HOME/bonfire/secrets/)",
     default=conf.DEFAULT_SECRETS_DIR,
 )
 @click.option(
+    "--configmaps-dir",
+    type=str,
+    help=(
+        "Directory to use for configmaps import (default: $XDG_CONFIG_HOME/bonfire/configmaps/)"
+    ),
+    default=conf.DEFAULT_CONFIGMAPS_DIR,
+)
+@click.option(
     "--no-release-on-fail",
     is_flag=True,
     help="Do not release namespace reservation if deployment fails",
 )
 @options(_ns_reserve_options)
 @options(_timeout_option)
 def _cmd_config_deploy(
@@ -1289,15 +1304,17 @@
     name,
     requester,
     duration,
     timeout,
     no_release_on_fail,
     component_filter,
     import_secrets,
+    import_configmaps,
     secrets_dir,
+    configmaps_dir,
     local,
     frontends,
     pool,
     force,
     preferred_params,
 ):
     """Process app templates and deploy them to a cluster"""
@@ -1322,14 +1339,17 @@
         force,
         using_current=using_current,
     )
 
     if import_secrets:
         import_secrets_from_dir(secrets_dir)
 
+    if import_configmaps:
+        import_configmaps_from_dir(configmaps_dir)
+
     clowd_env = _get_env_name(ns, clowd_env)
 
     def _err_handler(err):
         try:
             if not no_release_on_fail and reserved_new_ns and not reserve:
                 # if we auto-reserved this ns, auto-release it on failure unless
                 # --no-release-on-fail was requested
@@ -1419,30 +1439,48 @@
 @click.option(
     "--import-secrets",
     is_flag=True,
     help="Import secrets from local directory at deploy time",
     default=False,
 )
 @click.option(
+    "--import-configmaps",
+    is_flag=True,
+    help="Import configmaps from local directory at deploy time",
+    default=False,
+)
+@click.option(
     "--secrets-dir",
     type=str,
     help=("Import secrets from this directory (default: " "$XDG_CONFIG_HOME/bonfire/secrets/)"),
     default=conf.DEFAULT_SECRETS_DIR,
 )
+@click.option(
+    "--configmaps-dir",
+    type=str,
+    help=(
+        "Import configmaps from this directory \
+           (default: "
+        "$XDG_CONFIG_HOME/bonfire/configmaps/)"
+    ),
+    default=conf.DEFAULT_CONFIGMAPS_DIR,
+)
 @options(_ns_reserve_options)
 @options(_timeout_option)
 @click_exception_wrapper("deploy-env")
 def _cmd_deploy_clowdenv(
     namespace,
     quay_user,
     clowd_env,
     template_file,
     timeout,
     import_secrets,
+    import_configmaps,
     secrets_dir,
+    configmaps_dir,
     name,
     requester,
     duration,
     local,
     pool,
     force,
 ):
@@ -1451,14 +1489,17 @@
         _error("cluster does not have clowder operator installed")
 
     namespace, _ = _get_namespace(namespace, name, requester, duration, pool, timeout, local, force)
 
     if import_secrets:
         import_secrets_from_dir(secrets_dir)
 
+    if import_configmaps:
+        import_configmaps_from_dir(configmaps_dir)
+
     clowd_env_config = _process_clowdenv(namespace, quay_user, clowd_env, template_file, local)
 
     log.debug("ClowdEnvironment config:\n%s", clowd_env_config)
 
     apply_config(None, clowd_env_config)
 
     if not namespace:
```

### Comparing `crc_bonfire-5.7.2/bonfire/config.py` & `crc_bonfire-5.8.0/bonfire/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 log = logging.getLogger(__name__)
 
 
 DEFAULT_CONFIG_PATH = get_config_path().joinpath("config.yaml")
 DEFAULT_ENV_PATH = get_config_path().joinpath("env")
 DEFAULT_SECRETS_DIR = get_config_path().joinpath("secrets")
+DEFAULT_CONFIGMAPS_DIR = get_config_path().joinpath("configmaps")
 
 DEFAULT_NAMESPACE_POOL = "default"
 
 DEFAULT_CLOWDENV_TEMPLATE = resource_filename(
     "bonfire", "resources/local-cluster-clowdenvironment.yaml"
 )
 EPHEMERAL_CLUSTER_CLOWDENV_TEMPLATE = resource_filename(
@@ -80,15 +81,15 @@
 if os.getenv("BONFIRE_TRUSTED_COMPONENTS"):
     TRUSTED_COMPONENTS = os.getenv("BONFIRE_TRUSTED_COMPONENTS").split(",")
 
 ELASTICSEARCH_HOST = os.getenv("ELASTICSEARCH_HOST", DEFAULT_ELASTICSEARCH_HOST)
 ELASTICSEARCH_INDEX = os.getenv("ELASTICSEARCH_INDEX", DEFAULT_ELASTICSEARCH_INDEX)
 ELASTICSEARCH_APIKEY = os.getenv("ELASTICSEARCH_APIKEY")
 if ELASTICSEARCH_APIKEY:
-    ELASTICSEARCH_APIKEY = f'ApiKey {ELASTICSEARCH_APIKEY}'
+    ELASTICSEARCH_APIKEY = f"ApiKey {ELASTICSEARCH_APIKEY}"
 ENABLE_TELEMETRY = os.getenv("ENABLE_TELEMETRY", DEFAULT_ENABLE_TELEMETRY).lower() == "true"
 
 CLIENT_ID = os.getenv("CLIENT_ID", DEFAULT_CLIENT_ID)
 
 DEFAULT_FRONTEND_DEPENDENCIES = (
     "chrome-service",
     "landing-page-frontend",
@@ -96,15 +97,15 @@
     "insights-dashboard",
     "rbac",
     "rbac-frontend",
     "settings-frontend",
     "host-inventory",
     "host-inventory-frontend",
     "unleash-proxy",
-    "service-accounts"
+    "service-accounts",
 )
 
 
 def _get_auto_added_frontend_dependencies():
     env_var = os.getenv("BONFIRE_FRONTEND_DEPENDENCIES")
 
     if env_var is None:
```

### Comparing `crc_bonfire-5.7.2/bonfire/elastic_logging.py` & `crc_bonfire-5.8.0/bonfire/elastic_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
         # prevent duplicate handlers
         self.es_handler = next(
             (h for h in self.es_telemetry.handlers if type(h) is AsyncElasticsearchHandler), None
         )
         if not self.es_handler:
             self.es_handler = AsyncElasticsearchHandler(
-                f'{conf.ELASTICSEARCH_HOST}/{conf.ELASTICSEARCH_INDEX}/_doc/')
+                f"{conf.ELASTICSEARCH_HOST}/{conf.ELASTICSEARCH_INDEX}/_doc/"
+            )
             self.es_telemetry.addHandler(self.es_handler)
 
     def send_telemetry(self, log_message, success=True):
         self.es_handler.set_success_status(success)
 
         self.es_telemetry.info(log_message)
```

### Comparing `crc_bonfire-5.7.2/bonfire/local.py` & `crc_bonfire-5.8.0/bonfire/local.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/namespaces.py` & `crc_bonfire-5.8.0/bonfire/namespaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,24 +397,24 @@
     data += f"Keycloak admin route: {keycloak_url}\n"
     data += f"Keycloak admin login: {kc_creds['username']} | {kc_creds['password']}\n"
     data += f"{num_clowdapps} ClowdApp(s), " f"{num_frontends} Frontend(s) deployed\n"
     data += f"Gateway route: https://{fe_host}\n"
     data += f"Default user login: {kc_creds['defaultUsername']} | {kc_creds['defaultPassword']}\n"
     if output == "json":
         data = {
-                "namespace": project_name,
-                "keycloak_admin_route": keycloak_url,
-                "keycloak_admin_username": kc_creds['username'],
-                "keycloak_admin_password": kc_creds['password'],
-                "clowdapps_deployed": num_clowdapps,
-                "frontends_deployed": num_frontends,
-                "default_username": kc_creds['defaultUsername'],
-                "default_password": kc_creds['defaultPassword'],
-                "gateway_route": f"https://{fe_host}",
-            }
+            "namespace": project_name,
+            "keycloak_admin_route": keycloak_url,
+            "keycloak_admin_username": kc_creds["username"],
+            "keycloak_admin_password": kc_creds["password"],
+            "clowdapps_deployed": num_clowdapps,
+            "frontends_deployed": num_frontends,
+            "default_username": kc_creds["defaultUsername"],
+            "default_password": kc_creds["defaultPassword"],
+            "gateway_route": f"https://{fe_host}",
+        }
         data = json.dumps(data, indent=2)
 
     return data
 
 
 def parse_fe_env(project_name):
     fe_env = get_json("frontendenvironment", f"env-{project_name}")
```

### Comparing `crc_bonfire-5.7.2/bonfire/openshift.py` & `crc_bonfire-5.8.0/bonfire/openshift.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/processor.py` & `crc_bonfire-5.8.0/bonfire/processor.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/qontract.py` & `crc_bonfire-5.8.0/bonfire/qontract.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/resources/default-iqe-cji.yaml` & `crc_bonfire-5.8.0/bonfire/resources/default-iqe-cji.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/resources/default_config.yaml` & `crc_bonfire-5.8.0/bonfire/resources/default_config.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml` & `crc_bonfire-5.8.0/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/resources/local-cluster-clowdenvironment.yaml` & `crc_bonfire-5.8.0/bonfire/resources/local-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/secrets.py` & `crc_bonfire-5.8.0/bonfire/secrets.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/bonfire/utils.py` & `crc_bonfire-5.8.0/bonfire/utils.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/cicd/README.md` & `crc_bonfire-5.8.0/cicd/README.md`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/crc_bonfire.egg-info/PKG-INFO` & `crc_bonfire-5.8.0/crc_bonfire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 5.7.2
+Version: 5.8.0
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
 Home-page: https://www.github.com/RedHatInsights/bonfire
 Author: Brandon Squizzato
 Author-email: bsquizza@redhat.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crc_bonfire-5.7.2/crc_bonfire.egg-info/SOURCES.txt` & `crc_bonfire-5.8.0/crc_bonfire.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pytest.ini
 setup.cfg
 .github/workflows/release.yml
 .github/workflows/tests.yml
 bonfire/__init__.py
 bonfire/bonfire.py
 bonfire/config.py
+bonfire/configmaps.py
 bonfire/elastic_logging.py
 bonfire/local.py
 bonfire/namespaces.py
 bonfire/openshift.py
 bonfire/processor.py
 bonfire/qontract.py
 bonfire/secrets.py
```

### Comparing `crc_bonfire-5.7.2/demo.gif` & `crc_bonfire-5.8.0/demo.gif`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/entrypoint.sh` & `crc_bonfire-5.8.0/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/setup.cfg` & `crc_bonfire-5.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/tests/data/namespace_data.json` & `crc_bonfire-5.8.0/tests/data/namespace_data.json`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/tests/data/reservation_data.json` & `crc_bonfire-5.8.0/tests/data/reservation_data.json`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/tests/test_app_configs.py` & `crc_bonfire-5.8.0/tests/test_app_configs.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/tests/test_bonfire.py` & `crc_bonfire-5.8.0/tests/test_bonfire.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/tests/test_get_apps.py` & `crc_bonfire-5.8.0/tests/test_get_apps.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/tests/test_processor.py` & `crc_bonfire-5.8.0/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/tests/test_utils.py` & `crc_bonfire-5.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `crc_bonfire-5.7.2/utils/search_replace.py` & `crc_bonfire-5.8.0/utils/search_replace.py`

 * *Files identical despite different names*

