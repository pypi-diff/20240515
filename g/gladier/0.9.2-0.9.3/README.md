# Comparing `tmp/gladier-0.9.2.tar.gz` & `tmp/gladier-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gladier-0.9.2.tar", last modified: Mon Nov 13 18:54:57 2023, max compression
+gzip compressed data, was "gladier-0.9.3.tar", last modified: Mon Feb 19 17:33:35 2024, max compression
```

## Comparing `gladier-0.9.2.tar` & `gladier-0.9.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.182047 gladier-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-13 18:54:49.000000 gladier-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-11-13 18:54:49.000000 gladier-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-11-13 18:54:57.182047 gladier-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-11-13 18:54:49.000000 gladier-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.174046 gladier-0.9.2/gladier/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23105 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.174046 gladier-0.9.2/gladier/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/managers/compute_login_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/managers/compute_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19916 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/managers/flows_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/managers/login_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/managers/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/state_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.174046 gladier-0.9.2/gladier/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/storage/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/storage/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.178047 gladier-0.9.2/gladier/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.178047 gladier-0.9.2/gladier/tools/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/builtins/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/builtins/choice_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/builtins/expression_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/builtins/fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/builtins/pass_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/builtins/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.178047 gladier-0.9.2/gladier/tools/globus/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/globus/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/globus/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/globus/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.178047 gladier-0.9.2/gladier/tools/posix/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/posix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/tools/posix/shell_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.178047 gladier-0.9.2/gladier/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/automate.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/dynamic_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/flow_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/flow_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/flow_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/name_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/tool_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/utils/tool_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-13 18:54:49.000000 gladier-0.9.2/gladier/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 18:54:57.174046 gladier-0.9.2/gladier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-11-13 18:54:57.000000 gladier-0.9.2/gladier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2023-11-13 18:54:57.000000 gladier-0.9.2/gladier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 18:54:57.000000 gladier-0.9.2/gladier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-13 18:54:57.000000 gladier-0.9.2/gladier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-13 18:54:57.000000 gladier-0.9.2/gladier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-13 18:54:49.000000 gladier-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-13 18:54:57.182047 gladier-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-11-13 18:54:49.000000 gladier-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.676385 gladier-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-19 17:33:27.000000 gladier-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-19 17:33:27.000000 gladier-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-02-19 17:33:35.676385 gladier-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-19 17:33:27.000000 gladier-0.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.672385 gladier-0.9.3/gladier/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23436 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.672385 gladier-0.9.3/gladier/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/managers/compute_login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/managers/compute_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20639 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/managers/flows_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/managers/login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/managers/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/state_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.672385 gladier-0.9.3/gladier/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/storage/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/storage/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.672385 gladier-0.9.3/gladier/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.676385 gladier-0.9.3/gladier/tools/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/builtins/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/builtins/choice_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/builtins/expression_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/builtins/fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/builtins/pass_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/builtins/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.676385 gladier-0.9.3/gladier/tools/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/globus/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/globus/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/globus/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.676385 gladier-0.9.3/gladier/tools/posix/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/tools/posix/shell_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.676385 gladier-0.9.3/gladier/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/automate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/dynamic_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/flow_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/flow_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/flow_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/name_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/tool_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/utils/tool_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-19 17:33:27.000000 gladier-0.9.3/gladier/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:33:35.676385 gladier-0.9.3/gladier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-02-19 17:33:35.000000 gladier-0.9.3/gladier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-19 17:33:35.000000 gladier-0.9.3/gladier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 17:33:35.000000 gladier-0.9.3/gladier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-19 17:33:35.000000 gladier-0.9.3/gladier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-19 17:33:35.000000 gladier-0.9.3/gladier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-19 17:33:27.000000 gladier-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-19 17:33:35.680385 gladier-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-19 17:33:27.000000 gladier-0.9.3/setup.py
```

### Comparing `gladier-0.9.2/LICENSE` & `gladier-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/PKG-INFO` & `gladier-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: globus-sdk<4,>=3.23.0
 Requires-Dist: globus-compute-sdk<3.0.0,>=2.0.1
 Requires-Dist: packaging>=21.3
 Requires-Dist: fair-research-login>=0.2.6
```

### Comparing `gladier-0.9.2/README.rst` & `gladier-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/__init__.py` & `gladier-0.9.3/gladier/__init__.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/base.py` & `gladier-0.9.3/gladier/base.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/client.py` & `gladier-0.9.3/gladier/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,18 @@
        * An explicit flow definition to use for this client. Cannot be used with
          @generate_flow_definition. Changes are tracked on each run, and will result
          in a flow re-deploy on any change.
     * flow_schema (default: {})
        * A flow schema to accompany the flow definition. Schema is checked on each
          run and are re-deployed if it changes. Overrides any existing schema set
          on a given flow_manager instance unless unset.
+    * subscription_id (default: None)
+       * A subscription ID to associate with a flow. This typically is automatically
+         determined and does not need to be supplied, but may be required if the user
+         has more than one subscription
     * secret_config_filename (default: ``~/.gladier-secrets.cfg``)
        * Storage are for Globus Tokens and general storage
     * app_name (default: 'Gladier Client')
        * The app name used during a login flow
     * client_id
        * The Globus Client ID used for native logins
     * globus_group (default: None)
@@ -99,14 +103,15 @@
     :raises gladier.exc.AuthException: if authorizers given are insufficient
 
     """
 
     secret_config_filename: t.Optional[str] = None
     app_name: t.Optional[str] = "Gladier Client"
     client_id: str = "f1631610-d9e4-4db2-81ba-7f93ad4414e3"
+    subscription_id: t.Optional[str] = None
     globus_group: t.Optional[str] = None
     alias_class = gladier.utils.tool_alias.StateSuffixVariablePrefix
 
     def __init__(
         self,
         auto_registration: bool = True,
         login_manager: t.Optional[BaseLoginManager] = None,
@@ -115,15 +120,15 @@
         self._tools = None
         self.storage = self._determine_storage()
         self.login_manager = login_manager or self._determine_login_manager(
             self.storage
         )
 
         self.flows_manager = flows_manager or FlowsManager(
-            auto_registration=auto_registration
+            auto_registration=auto_registration, subscription_id=self.subscription_id
         )
         if self.globus_group:
             self.flows_manager.globus_group = self.globus_group
         if not self.flows_manager.flow_title:
             self.flows_manager.flow_title = f"{self.__class__.__name__} flow"
 
         self.compute_manager = ComputeManager(auto_registration=auto_registration)
```

### Comparing `gladier-0.9.2/gladier/decorators.py` & `gladier-0.9.3/gladier/decorators.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/exc.py` & `gladier-0.9.3/gladier/exc.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/helpers.py` & `gladier-0.9.3/gladier/helpers.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/managers/compute_login_manager.py` & `gladier-0.9.3/gladier/managers/compute_login_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/managers/compute_manager.py` & `gladier-0.9.3/gladier/managers/compute_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/managers/flows_manager.py` & `gladier-0.9.3/gladier/managers/flows_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,17 @@
                                exc: gladier.exc.RegistrationException) -> None:
 
     :param flow_id: Explicit flow id to use. None will result in deploying a new flow
     :param flow_definition: Flow definiton that should be used. Usually set dynamically
                             at runtime when used with a Gladier Client
     :param flow_schema: The schema to be used alongside the flow definition
     :param flow_title: The title for the Globus Flow
+    :param subscription_id: A subscription ID to associate with a flow. This typically is automatically
+                            determined and does not need to be supplied, but may be required if the user
+                            has more than one subscription
     :param globus_group: A Globus Group UUID. Used to grant all flow and run permissions
     :param on_change: callback on checksum mismatch or missing flow id. Default registers/deploys
                       flow, ``None`` takes no action and attempts to run "obselete" flows.
     :param redeploy_on_404: Deploy a new flow if attempting to run the current flow ID results
                             in 404. Behavior is disabled if an explicit flow_id is specified.
 
     When used with a Gladier Client, following items will be auto-configured and should not be
@@ -79,23 +82,25 @@
 
     def __init__(
         self,
         flow_id: t.Optional[str] = None,
         flow_definition: t.Optional[dict] = None,
         flow_schema: t.Optional[dict] = None,
         flow_title: t.Optional[str] = None,
+        subscription_id: t.Optional[str] = None,
         globus_group: t.Optional[str] = None,
         on_change: t.Optional[t.Callable] = ensure_flow_registered,
         redeploy_on_404: bool = True,
         **kwargs,
     ):
         self.flow_id = flow_id
         self.flow_definition = flow_definition
         self.flow_schema = flow_schema
         self.flow_title = flow_title
+        self.subscription_id = subscription_id
         self.globus_group = globus_group
         self.on_change = on_change or (lambda self, exc: None)
         self.redeploy_on_404 = redeploy_on_404
 
         if self.flow_id is not None:
             self.redeploy_on_404 = False
             log.info("Custom Flow ID set, redeploy_on_404 disabled.")
@@ -318,14 +323,18 @@
             for p_type in ["flow_viewers", "flow_starters", "flow_administrators"]
             if self.get_flow_permission(p_type)
         }
         log.debug(f'Flow permissions set to: {flow_permissions or "Flows defaults"}')
         flow_kwargs = flow_permissions
         # Input schema is a required field and must be part of all flows.
         flow_kwargs["input_schema"] = self.flow_schema
+        # TODO: The globus sdk does not currently support subscription id on UPDATE.
+        # This should change eventually, but right now cannot be supplied or it will raise errors
+        # It is added only on CREATE for now.
+        # flow_kwargs["subscription_id"] = self.subscription_id
         if flow_id:
             try:
                 log.info(f"Flow checksum failed, updating flow {flow_id}...")
                 self.flows_client.update_flow(
                     flow_id,
                     title=self.flow_title,
                     definition=self.flow_definition,
@@ -338,14 +347,15 @@
             except globus_sdk.exc.GlobusAPIError as gapie:
                 if gapie.http_status == 404 and self.redeploy_on_404:
                     flow_id = None
                 else:
                     raise
         if flow_id is None:
             log.info("No flow detected, deploying new flow...")
+            flow_kwargs["subscription_id"] = self.subscription_id
             flow = self.flows_client.create_flow(
                 self.flow_title, self.flow_definition, **flow_kwargs
             ).data
             log.debug(f'Flow deployed with id {flow["id"]}')
             self.storage.set_value("flow_id", flow["id"])
             self.storage.set_value(
                 "flow_checksum",
```

### Comparing `gladier-0.9.2/gladier/managers/login_manager.py` & `gladier-0.9.3/gladier/managers/login_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/managers/service_manager.py` & `gladier-0.9.3/gladier/managers/service_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/state_models.py` & `gladier-0.9.3/gladier/state_models.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/storage/config.py` & `gladier-0.9.3/gladier/storage/config.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/storage/migrations.py` & `gladier-0.9.3/gladier/storage/migrations.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/storage/tokens.py` & `gladier-0.9.3/gladier/storage/tokens.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/__init__.py` & `gladier-0.9.3/gladier/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/builtins/__init__.py` & `gladier-0.9.3/gladier/tools/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/builtins/action.py` & `gladier-0.9.3/gladier/tools/builtins/action.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/builtins/choice_state.py` & `gladier-0.9.3/gladier/tools/builtins/choice_state.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/builtins/expression_eval.py` & `gladier-0.9.3/gladier/tools/builtins/expression_eval.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/builtins/fail.py` & `gladier-0.9.3/gladier/tools/builtins/fail.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/builtins/pass_state.py` & `gladier-0.9.3/gladier/tools/builtins/pass_state.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/builtins/wait.py` & `gladier-0.9.3/gladier/tools/builtins/wait.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/globus/__init__.py` & `gladier-0.9.3/gladier/tools/globus/__init__.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/globus/compute.py` & `gladier-0.9.3/gladier/tools/globus/compute.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/globus/search.py` & `gladier-0.9.3/gladier/tools/globus/search.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/globus/transfer.py` & `gladier-0.9.3/gladier/tools/globus/transfer.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/helpers.py` & `gladier-0.9.3/gladier/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/tools/posix/shell_cmd.py` & `gladier-0.9.3/gladier/tools/posix/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/utils/automate.py` & `gladier-0.9.3/gladier/utils/automate.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/utils/dynamic_imports.py` & `gladier-0.9.3/gladier/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/utils/flow_generation.py` & `gladier-0.9.3/gladier/utils/flow_generation.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/utils/flow_modifiers.py` & `gladier-0.9.3/gladier/utils/flow_modifiers.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/utils/flow_traversal.py` & `gladier-0.9.3/gladier/utils/flow_traversal.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/utils/name_generation.py` & `gladier-0.9.3/gladier/utils/name_generation.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/utils/tool_alias.py` & `gladier-0.9.3/gladier/utils/tool_alias.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier/utils/tool_chain.py` & `gladier-0.9.3/gladier/utils/tool_chain.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/gladier.egg-info/PKG-INFO` & `gladier-0.9.3/gladier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: globus-sdk<4,>=3.23.0
 Requires-Dist: globus-compute-sdk<3.0.0,>=2.0.1
 Requires-Dist: packaging>=21.3
 Requires-Dist: fair-research-login>=0.2.6
```

### Comparing `gladier-0.9.2/gladier.egg-info/SOURCES.txt` & `gladier-0.9.3/gladier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gladier-0.9.2/setup.py` & `gladier-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,9 +40,10 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

