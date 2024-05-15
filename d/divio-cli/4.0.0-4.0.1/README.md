# Comparing `tmp/divio-cli-4.0.0.tar.gz` & `tmp/divio_cli-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio-cli-4.0.0.tar", last modified: Tue Feb 13 14:16:00 2024, max compression
+gzip compressed data, was "divio_cli-4.0.1.tar", last modified: Wed May 15 10:52:32 2024, max compression
```

## Comparing `divio-cli-4.0.0.tar` & `divio_cli-4.0.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 14:16:00.304294 divio-cli-4.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-02-13 14:15:41.000000 divio-cli-4.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2224 2024-02-13 14:15:41.000000 divio-cli-4.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    13223 2024-02-13 14:15:41.000000 divio-cli-4.0.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-02-13 14:15:41.000000 divio-cli-4.0.0/DESCRIPTION.md
--rw-rw-rw-   0 root         (0) root         (0)     1476 2024-02-13 14:15:41.000000 divio-cli-4.0.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-02-13 14:15:41.000000 divio-cli-4.0.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-02-13 14:15:41.000000 divio-cli-4.0.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     3608 2024-02-13 14:16:00.300294 divio-cli-4.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3420 2024-02-13 14:15:41.000000 divio-cli-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 14:16:00.300294 divio-cli-4.0.0/divio_cli/
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13298 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/api_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     8731 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/check_system.py
--rw-rw-rw-   0 root         (0) root         (0)    45500 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5511 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/client.py
--rw-rw-rw-   0 root         (0) root         (0)    43050 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/cloud.py
--rw-rw-rw-   0 root         (0) root         (0)     5291 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 14:16:00.300294 divio-cli-4.0.0/divio_cli/domain_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/domain_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/domain_models/app_template.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/excepthook.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 14:16:00.300294 divio-cli-4.0.0/divio_cli/localdev/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/localdev/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7171 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/localdev/backups.py
--rw-rw-rw-   0 root         (0) root         (0)    34767 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/localdev/main.py
--rw-rw-rw-   0 root         (0) root         (0)     9474 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/localdev/push.py
--rw-rw-rw-   0 root         (0) root         (0)    13951 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/localdev/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/messages.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 14:16:00.300294 divio-cli-4.0.0/divio_cli/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3265 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2374 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/test_deployments_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/test_environment_variables_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1967 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/test_localdev_backups.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/test_localdev_push.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/test_localdev_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/test/test_project_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 14:16:00.300294 divio-cli-4.0.0/divio_cli/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2288 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/upload/addon.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/upload/common.py
--rw-rw-rw-   0 root         (0) root         (0)    15293 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 14:16:00.300294 divio-cli-4.0.0/divio_cli/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/validators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/validators/addon.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/validators/common.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-02-13 14:16:00.000000 divio-cli-4.0.0/divio_cli/version.py
--rw-rw-rw-   0 root         (0) root         (0)    12534 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/widgets.py
--rw-rw-rw-   0 root         (0) root         (0)    34002 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/wizards.py
--rw-rw-rw-   0 root         (0) root         (0)     9777 2024-02-13 14:15:41.000000 divio-cli-4.0.0/divio_cli/wizards_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 14:16:00.300294 divio-cli-4.0.0/divio_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3608 2024-02-13 14:16:00.000000 divio-cli-4.0.0/divio_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1471 2024-02-13 14:16:00.000000 divio-cli-4.0.0/divio_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-13 14:16:00.000000 divio-cli-4.0.0/divio_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-13 14:16:00.000000 divio-cli-4.0.0/divio_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-13 14:16:00.000000 divio-cli-4.0.0/divio_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      250 2024-02-13 14:16:00.000000 divio-cli-4.0.0/divio_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-02-13 14:16:00.000000 divio-cli-4.0.0/divio_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2459 2024-02-13 14:15:41.000000 divio-cli-4.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-13 14:16:00.304294 divio-cli-4.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      332 2024-02-13 14:15:41.000000 divio-cli-4.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:52:32.824605 divio_cli-4.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-15 10:01:21.000000 divio_cli-4.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2024-05-15 10:01:21.000000 divio_cli-4.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13408 2024-05-15 10:35:15.000000 divio_cli-4.0.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-15 10:01:21.000000 divio_cli-4.0.1/DESCRIPTION.md
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2024-05-15 10:01:21.000000 divio_cli-4.0.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-15 10:01:21.000000 divio_cli-4.0.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-05-15 10:01:21.000000 divio_cli-4.0.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3608 2024-05-15 10:52:32.820604 divio_cli-4.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3420 2024-05-15 10:01:21.000000 divio_cli-4.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:52:32.820604 divio_cli-4.0.1/divio_cli/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13298 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/api_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8731 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/check_system.py
+-rw-rw-rw-   0 root         (0) root         (0)    45500 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5511 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    43087 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/cloud.py
+-rw-rw-rw-   0 root         (0) root         (0)     5291 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:52:32.820604 divio_cli-4.0.1/divio_cli/domain_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 10:52:15.000000 divio_cli-4.0.1/divio_cli/domain_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/domain_models/app_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/excepthook.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:52:32.820604 divio_cli-4.0.1/divio_cli/localdev/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/localdev/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7171 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/localdev/backups.py
+-rw-rw-rw-   0 root         (0) root         (0)    34767 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/localdev/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     9474 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/localdev/push.py
+-rw-rw-rw-   0 root         (0) root         (0)    13951 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/localdev/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/messages.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:52:32.820604 divio_cli-4.0.1/divio_cli/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 10:52:15.000000 divio_cli-4.0.1/divio_cli/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3265 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/test_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/test_deployments_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/test_environment_variables_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/test_localdev_backups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/test_localdev_push.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/test_localdev_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/test/test_project_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:52:32.820604 divio_cli-4.0.1/divio_cli/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 10:52:15.000000 divio_cli-4.0.1/divio_cli/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2288 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/upload/addon.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/upload/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    15293 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:52:32.820604 divio_cli-4.0.1/divio_cli/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 10:52:15.000000 divio_cli-4.0.1/divio_cli/validators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/validators/addon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/validators/common.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-15 10:52:32.000000 divio_cli-4.0.1/divio_cli/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12534 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/widgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    34002 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/wizards.py
+-rw-rw-rw-   0 root         (0) root         (0)    10418 2024-05-15 10:01:21.000000 divio_cli-4.0.1/divio_cli/wizards_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:52:32.820604 divio_cli-4.0.1/divio_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3608 2024-05-15 10:52:32.000000 divio_cli-4.0.1/divio_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1471 2024-05-15 10:52:32.000000 divio_cli-4.0.1/divio_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:52:32.000000 divio_cli-4.0.1/divio_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-15 10:52:32.000000 divio_cli-4.0.1/divio_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:52:32.000000 divio_cli-4.0.1/divio_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-15 10:52:32.000000 divio_cli-4.0.1/divio_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 10:52:32.000000 divio_cli-4.0.1/divio_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2024-05-15 10:01:21.000000 divio_cli-4.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 10:52:32.824605 divio_cli-4.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      332 2024-05-15 10:01:21.000000 divio_cli-4.0.1/tox.ini
```

### Comparing `divio-cli-4.0.0/.gitlab-ci.yml` & `divio_cli-4.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/CHANGELOG.rst` & `divio_cli-4.0.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+4.0.1 (2024-05-15)
+-------------------
+
+* Fixed SSH verification for external repositories during app creation.
+* Fixed `divio app push db` validation for local postgres binary files.
+
 4.0.0 (2024-02-13)
 -------------------
 
 * Added tests for environment variables and deployments commands.
 * Added application creation functionality based on the new application creation approach.
 * Added support to list and add services to an application.
 * Added support to list regions.
```

### Comparing `divio-cli-4.0.0/LICENSE.txt` & `divio_cli-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/Makefile` & `divio_cli-4.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/PKG-INFO` & `divio_cli-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio-cli
-Version: 4.0.0
+Version: 4.0.1
 Summary: The command-line client for the Divio Cloud
 Author-email: Divio AG <info@divio.com>
 License: Copyright (c) 2015, Divio AG
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `divio-cli-4.0.0/README.md` & `divio_cli-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/api_requests.py` & `divio_cli-4.0.1/divio_cli/api_requests.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/check_system.py` & `divio_cli-4.0.1/divio_cli/check_system.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/cli.py` & `divio_cli-4.0.1/divio_cli/cli.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/client.py` & `divio_cli-4.0.1/divio_cli/client.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/cloud.py` & `divio_cli-4.0.1/divio_cli/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1039,14 +1039,15 @@
             return api_requests.CheckRepositoryRequest(
                 self.session,
                 url_kwargs={"repository_uuid": repository_uuid},
                 data={
                     "branch": branch,
                     "migrate": migrate,
                 },
+                proceed_on_4xx=True,
             )()
         except (KeyError, json.decoder.JSONDecodeError):
             click.secho(
                 "Error establishing connection while authenticating repository.",
                 fg="red",
                 err=True,
             )
```

### Comparing `divio-cli-4.0.0/divio_cli/config.py` & `divio_cli-4.0.1/divio_cli/config.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/domain_models/app_template.py` & `divio_cli-4.0.1/divio_cli/domain_models/app_template.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/excepthook.py` & `divio_cli-4.0.1/divio_cli/excepthook.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/exceptions.py` & `divio_cli-4.0.1/divio_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/localdev/backups.py` & `divio_cli-4.0.1/divio_cli/localdev/backups.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/localdev/main.py` & `divio_cli-4.0.1/divio_cli/localdev/main.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/localdev/push.py` & `divio_cli-4.0.1/divio_cli/localdev/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         return os.path.join(self.project_home, local_file)
 
 
 def is_db_dump(local_file: str, db_type: str):
     """Test if a file looks like a database dump"""
     start_bytes = open(local_file, "rb").read(1024)
     if db_type == "fsm-postgres":
-        if start_bytes.startswith(b"\x50\x47\x44\x42"):
+        if start_bytes.startswith(b"\x50\x47\x44\x4d"):
             return True  # postgres binary dump
     if start_bytes.startswith(b"--") and b"dump" in start_bytes.lower():
         return True  # plaintext dump
     return False
 
 
 def dump_database(
```

### Comparing `divio-cli-4.0.0/divio_cli/localdev/utils.py` & `divio_cli-4.0.1/divio_cli/localdev/utils.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/messages.py` & `divio_cli-4.0.1/divio_cli/messages.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/settings.py` & `divio_cli-4.0.1/divio_cli/settings.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/test/conftest.py` & `divio_cli-4.0.1/divio_cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/test/test_commands.py` & `divio_cli-4.0.1/divio_cli/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/test/test_deployments_commands.py` & `divio_cli-4.0.1/divio_cli/test/test_deployments_commands.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/test/test_environment_variables_commands.py` & `divio_cli-4.0.1/divio_cli/test/test_environment_variables_commands.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/test/test_exceptions.py` & `divio_cli-4.0.1/divio_cli/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/test/test_localdev_backups.py` & `divio_cli-4.0.1/divio_cli/test/test_localdev_backups.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/test/test_localdev_push.py` & `divio_cli-4.0.1/divio_cli/test/test_localdev_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             pusher.restore_step()
         assert str(exinfo.value) == " error!\nBackup restore failed."
 
 
 @pytest.mark.parametrize(
     ("content", "postgres_res", "mysql_res"),
     [
-        (b"\x50\x47\x44\x42\x44\x34\x34", True, False),
+        (b"\x50\x47\x44\x4d\x44\x34\x34", True, False),
         (b"\x50\x47\x42\x44", False, False),
         (b"-- MariaDB dump 10.19  Distrib 10.5.17-MariaDB\n--", True, True),
         (b"-- MySQL DUMP with some distrib", True, True),
         (b"--\n-- PostgreSQL database dUmp\n--", True, True),
         (b"MySQL dump", False, False),
         (b"-- d u m p", False, False),
     ],
```

### Comparing `divio-cli-4.0.0/divio_cli/test/test_localdev_utils.py` & `divio_cli-4.0.1/divio_cli/test/test_localdev_utils.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/test/test_project_settings.py` & `divio_cli-4.0.1/divio_cli/test/test_project_settings.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/upload/addon.py` & `divio_cli-4.0.1/divio_cli/upload/addon.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/upload/common.py` & `divio_cli-4.0.1/divio_cli/upload/common.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/utils.py` & `divio_cli-4.0.1/divio_cli/utils.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/validators/addon.py` & `divio_cli-4.0.1/divio_cli/validators/addon.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/validators/common.py` & `divio_cli-4.0.1/divio_cli/validators/common.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/widgets.py` & `divio_cli-4.0.1/divio_cli/widgets.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/wizards.py` & `divio_cli-4.0.1/divio_cli/wizards.py`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/divio_cli/wizards_utils.py` & `divio_cli-4.0.1/divio_cli/wizards_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,19 +70,23 @@
     "enter_release_command_label": "Enter the label of your release command",
     "enter_release_command": "Enter your release command",
     "add_another_release_command": "Want to add another release command?",
     # External repository
     "repo_connect": "Want to connect an external repository to your application?",
     "repo_url_enter": "Enter the URL of your external repository",
     "repo_branch_enter": "Enter the name of your target branch",
-    "repo_ssh_key_type_select": "Select the type of your deploy key",
+    "repo_ssh_key_type_select": (
+        "SSH verification requires a specific key type. Please select one"
+    ),
     "repo_host_username_enter": "Enter the username of your repository host",
     "repo_host_password_enter": "Enter the password of your repository host (your input is not displayed)",
     "create_deploy_key": (
-        "Please register this ssh key with your repository provider. Ready to continue?"
+        "Please register this ssh key with your repository provider. See "
+        "https://docs.divio.com/how-to/resources-configure-git/#add-your-application-s-public-key-to-the-git-host "
+        "for more information. Ready to continue?"
     ),
     "repository_verification_skipped": "Repository verification skipped. No repository connected.",
     "repo_verification_timeout": "Repository verification timeout.",
     "repo_verification_failed": "Repository verification failed.",
     "confirm_app_creation": "Confirm application creation to proceed.",
     # Deploy
     "deployment_triggered": "Deployment of 'test' environment triggered.",
@@ -245,14 +249,28 @@
         else:
             break
 
     return repo_url
 
 
 def verify_app_repo(client, uuid, branch):
+    choices = [
+        ("Retry repository verification", "retry"),
+        ("Restart repository connection", "restart"),
+        ("Skip this step (no repository)", "skip"),
+    ]
+    options = [
+        inquirer.List(
+            "choice",
+            message="How would you like to proceed?",
+            choices=choices,
+            carousel=True,
+        )
+    ]
+
     # Initiating the celery task to verify the repository.
     client.check_repository(uuid, branch)
 
     c = 0
     while True:
         repo_state = client.get_repository(uuid)["state"]
         if repo_state in ["INVALID", "CLONED"] or c > 14:
@@ -265,28 +283,25 @@
             status_print(
                 APP_WIZARD_MESSAGES["repo_verification_timeout"], "error"
             )
         else:
             status_print(
                 APP_WIZARD_MESSAGES["repo_verification_failed"], "error"
             )
-
-        choices = [
-            ("Retry repository verification", "retry"),
-            ("Restart repository connection", "restart"),
-            ("Skip this step (no repository)", "skip"),
-        ]
-        options = [
-            inquirer.List(
-                "choice",
-                message="How would you like to proceed?",
-                choices=choices,
-                carousel=True,
-            )
-        ]
         verification_status = inquirer.prompt(
             options, raise_keyboard_interrupt=True
         )["choice"]
     else:
-        verification_status = "success"
+        # Cloned repository successfully, pull access confirmed.
+        # A second check is required to also verify push access.
+        response = client.check_repository(uuid, branch)
+        if response.get("code") == "success":
+            verification_status = "success"
+        else:
+            status_print(
+                APP_WIZARD_MESSAGES["repo_verification_failed"], "error"
+            )
+            verification_status = inquirer.prompt(
+                options, raise_keyboard_interrupt=True
+            )["choice"]
 
     return verification_status
```

### Comparing `divio-cli-4.0.0/divio_cli.egg-info/PKG-INFO` & `divio_cli-4.0.1/divio_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio-cli
-Version: 4.0.0
+Version: 4.0.1
 Summary: The command-line client for the Divio Cloud
 Author-email: Divio AG <info@divio.com>
 License: Copyright (c) 2015, Divio AG
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `divio-cli-4.0.0/divio_cli.egg-info/SOURCES.txt` & `divio_cli-4.0.1/divio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `divio-cli-4.0.0/pyproject.toml` & `divio_cli-4.0.1/pyproject.toml`

 * *Files identical despite different names*

