# Comparing `tmp/tc66c2mqtt-0.0.1rc0.tar.gz` & `tmp/tc66c2mqtt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc66c2mqtt-0.0.1rc0.tar", last modified: Mon Apr 29 15:32:43 2024, max compression
+gzip compressed data, was "tc66c2mqtt-0.1.0.tar", last modified: Wed May 15 20:16:49 2024, max compression
```

## Comparing `tc66c2mqtt-0.0.1rc0.tar` & `tc66c2mqtt-0.1.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-29 15:32:43.965533 tc66c2mqtt-0.0.1rc0/
--rw-rw-r--   0 jens      (1000) users      (100)      310 2024-04-26 06:29:23.000000 tc66c2mqtt-0.0.1rc0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2024-04-26 06:29:23.000000 tc66c2mqtt-0.0.1rc0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-29 15:32:43.961533 tc66c2mqtt-0.0.1rc0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-29 15:32:43.961533 tc66c2mqtt-0.0.1rc0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1677 2024-04-26 06:29:23.000000 tc66c2mqtt-0.0.1rc0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      116 2024-04-26 06:29:23.000000 tc66c2mqtt-0.0.1rc0/.gitignore
--rw-r--r--   0 jens      (1000) users      (100)     2287 2024-04-29 15:32:43.965533 tc66c2mqtt-0.0.1rc0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)      952 2024-04-29 15:27:40.000000 tc66c2mqtt-0.0.1rc0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3082 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3082 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/dev-cli.py
--rw-rw-r--   0 jens      (1000) users      (100)     4837 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    80959 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    17213 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2024-04-29 15:32:43.965533 tc66c2mqtt-0.0.1rc0/setup.cfg
--rw-rw-r--   0 jens      (1000) users      (100)      192 2024-04-29 13:33:31.000000 tc66c2mqtt-0.0.1rc0/tc66.dat
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-29 15:32:43.961533 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/
--rw-rw-r--   0 jens      (1000) users      (100)      137 2024-04-29 15:29:25.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      160 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-29 15:32:43.965533 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/
--rw-rw-r--   0 jens      (1000) users      (100)     1062 2024-04-29 15:30:25.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3532 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/print_data.py
--rw-rw-r--   0 jens      (1000) users      (100)     2324 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/scan.py
--rw-rw-r--   0 jens      (1000) users      (100)     1371 2024-04-29 15:24:16.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     2468 2024-04-29 15:24:16.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/systemd.py
--rw-rw-r--   0 jens      (1000) users      (100)      800 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/update_readme_history.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-29 15:32:43.965533 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/
--rw-rw-r--   0 jens      (1000) users      (100)     2139 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      962 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/code_style.py
--rw-rw-r--   0 jens      (1000) users      (100)     2307 2024-04-29 15:32:13.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/packaging.py
--rw-rw-r--   0 jens      (1000) users      (100)     1514 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/testing.py
--rw-rw-r--   0 jens      (1000) users      (100)      187 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)      581 2024-04-29 15:06:38.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     2586 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tc66.py
--rw-rw-r--   0 jens      (1000) users      (100)      718 2024-04-29 13:40:29.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tc66_decryptor.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-29 15:32:43.965533 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/
--rw-rw-r--   0 jens      (1000) users      (100)     1197 2024-04-26 06:29:23.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1057 2024-04-29 14:05:44.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)      215 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     1454 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)      428 2024-04-29 15:21:02.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/test_tc66.py
--rw-rw-r--   0 jens      (1000) users      (100)      356 2024-04-29 15:30:55.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/test_tc66_decryptor.py
--rw-rw-r--   0 jens      (1000) users      (100)     1120 2024-04-29 15:26:01.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt/user_settings.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-29 15:32:43.965533 tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/
--rw-r--r--   0 jens      (1000) users      (100)     2287 2024-04-29 15:32:43.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1052 2024-04-29 15:32:43.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2024-04-29 15:32:43.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      101 2024-04-29 15:32:43.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      284 2024-04-29 15:32:43.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       11 2024-04-29 15:32:43.000000 tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/top_level.txt
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-15 20:16:49.196575 tc66c2mqtt-0.1.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      310 2024-04-26 06:29:23.000000 tc66c2mqtt-0.1.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2024-04-26 06:29:23.000000 tc66c2mqtt-0.1.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-15 20:16:49.192574 tc66c2mqtt-0.1.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-15 20:16:49.192574 tc66c2mqtt-0.1.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1677 2024-04-26 06:29:23.000000 tc66c2mqtt-0.1.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      116 2024-04-26 06:29:23.000000 tc66c2mqtt-0.1.0/.gitignore
+-rw-r--r--   0 jens      (1000) users      (100)     2490 2024-05-15 20:16:49.196575 tc66c2mqtt-0.1.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1158 2024-05-15 15:05:32.000000 tc66c2mqtt-0.1.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3082 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3082 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/dev-cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4837 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    80534 2024-05-15 16:01:46.000000 tc66c2mqtt-0.1.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    16788 2024-05-15 16:01:21.000000 tc66c2mqtt-0.1.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2024-05-15 20:16:49.196575 tc66c2mqtt-0.1.0/setup.cfg
+-rw-rw-r--   0 jens      (1000) users      (100)      192 2024-04-29 13:33:31.000000 tc66c2mqtt-0.1.0/tc66.dat
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-15 20:16:49.192574 tc66c2mqtt-0.1.0/tc66c2mqtt/
+-rw-rw-r--   0 jens      (1000) users      (100)      134 2024-05-15 20:15:47.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      160 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-15 20:16:49.192574 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/
+-rw-rw-r--   0 jens      (1000) users      (100)     1062 2024-04-29 15:30:25.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4472 2024-05-15 15:58:13.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/print_data.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1207 2024-05-15 15:24:00.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/publish.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2324 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/scan.py
+-rw-rw-r--   0 jens      (1000) users      (100)      972 2024-04-29 19:26:37.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2429 2024-04-29 19:29:21.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/systemd.py
+-rw-rw-r--   0 jens      (1000) users      (100)      800 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/update_readme_history.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-15 20:16:49.192574 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/
+-rw-rw-r--   0 jens      (1000) users      (100)     2139 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      962 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/code_style.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2307 2024-04-29 15:32:13.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/packaging.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1514 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/testing.py
+-rw-rw-r--   0 jens      (1000) users      (100)      419 2024-04-29 19:28:54.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)      583 2024-05-15 15:05:32.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4491 2024-05-15 15:09:39.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/mqtt_handler.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2797 2024-05-15 15:05:32.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tc66.py
+-rw-rw-r--   0 jens      (1000) users      (100)      718 2024-04-29 13:40:29.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tc66_decryptor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3058 2024-05-15 15:05:32.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tc66c_bluetooth.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-15 20:16:49.196575 tc66c2mqtt-0.1.0/tc66c2mqtt/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)     1197 2024-04-26 06:29:23.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1057 2024-04-29 14:05:44.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)      215 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1454 2024-04-29 15:21:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1123 2024-05-15 15:05:32.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tests/test_tc66.py
+-rw-rw-r--   0 jens      (1000) users      (100)      356 2024-04-29 15:30:55.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/tests/test_tc66_decryptor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1759 2024-04-29 19:29:02.000000 tc66c2mqtt-0.1.0/tc66c2mqtt/user_settings.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-15 20:16:49.196575 tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/
+-rw-r--r--   0 jens      (1000) users      (100)     2490 2024-05-15 20:16:49.000000 tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1139 2024-05-15 20:16:49.000000 tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2024-05-15 20:16:49.000000 tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      101 2024-05-15 20:16:49.000000 tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      284 2024-05-15 20:16:49.000000 tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       11 2024-05-15 20:16:49.000000 tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/top_level.txt
```

### Comparing `tc66c2mqtt-0.0.1rc0/.github/workflows/tests.yml` & `tc66c2mqtt-0.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/PKG-INFO` & `tc66c2mqtt-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc66c2mqtt
-Version: 0.0.1rc0
+Version: 0.1.0
 Summary: Sen MQTT events from TC66C device
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/tc66c2mqtt
 Project-URL: Source, https://github.com/jedie/tc66c2mqtt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -42,17 +42,20 @@
 [![codecov](https://codecov.io/github/jedie/tc66c2mqtt/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/tc66c2mqtt)
 [![tc66c2mqtt @ PyPi](https://img.shields.io/pypi/v/tc66c2mqtt?label=tc66c2mqtt%20%40%20PyPi)](https://pypi.org/project/tc66c2mqtt/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/tc66c2mqtt)](https://github.com/jedie/tc66c2mqtt/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/tc66c2mqtt)](https://github.com/jedie/tc66c2mqtt/blob/main/LICENSE)
 
 Send MQTT events from RDTech TC66C device
 
-**under development and not really useable, yet!**
+**under heavy development**
 
 
 Tested with [Joy-IT TC66C](https://joy-it.net/de/products/JT-TC66C).
 
 
 RDTech TC66C hardware info at sigrok:
 
  * https://sigrok.org/wiki/RDTech_TC66C
 
+test print data in terminal looks like:
+
+![2024-05-07_20-08_print_data.png](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/tc66c2mqtt/2024-05-07_20-08_print_data.png "2024-05-07_20-08_print_data.png")
```

### Comparing `tc66c2mqtt-0.0.1rc0/README.md` & `tc66c2mqtt-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 [![codecov](https://codecov.io/github/jedie/tc66c2mqtt/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/tc66c2mqtt)
 [![tc66c2mqtt @ PyPi](https://img.shields.io/pypi/v/tc66c2mqtt?label=tc66c2mqtt%20%40%20PyPi)](https://pypi.org/project/tc66c2mqtt/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/tc66c2mqtt)](https://github.com/jedie/tc66c2mqtt/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/tc66c2mqtt)](https://github.com/jedie/tc66c2mqtt/blob/main/LICENSE)
 
 Send MQTT events from RDTech TC66C device
 
-**under development and not really useable, yet!**
+**under heavy development**
 
 
 Tested with [Joy-IT TC66C](https://joy-it.net/de/products/JT-TC66C).
 
 
 RDTech TC66C hardware info at sigrok:
 
  * https://sigrok.org/wiki/RDTech_TC66C
 
+test print data in terminal looks like:
+
+![2024-05-07_20-08_print_data.png](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/tc66c2mqtt/2024-05-07_20-08_print_data.png "2024-05-07_20-08_print_data.png")
```

### Comparing `tc66c2mqtt-0.0.1rc0/cli.py` & `tc66c2mqtt-0.1.0/cli.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/dev-cli.py` & `tc66c2mqtt-0.1.0/dev-cli.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/pyproject.toml` & `tc66c2mqtt-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/requirements.dev.txt` & `tc66c2mqtt-0.1.0/requirements.dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -66,17 +66,17 @@
     --hash=sha256:d36ed1124bb81b32f8614555b34cc4259c3fbc7eec17870e8ff8ded335b58d8c \
     --hash=sha256:da33a1a5e49c4122ccdfd56cd021ff1ebc4a1ec4e2d01594fef9b6f267a9e741 \
     --hash=sha256:dd1b5a14e417189db4c7b64a6540f31730713d173f0b63e55fabd52d61d8fdce \
     --hash=sha256:e151054aa00bad1f4e1f04919542885f89f5f7d086b8a59e5000e6c616896ffb \
     --hash=sha256:eaea3008c281f1038edb473c1aa8ed8143a5535ff18f978a318f10302b254063 \
     --hash=sha256:ef703f83fc32e131e9bcc0a5094cfe85599e7109f896fe8bc96cc402f3eb4b6e
     # via darker
-bleak==0.21.1 \
-    --hash=sha256:ccec260a0f5ec02dd133d68b0351c0151b2ecf3ddd0bcabc4c04a1cdd7f33256 \
-    --hash=sha256:ec4a1a2772fb315b992cbaa1153070c7e26968a52b0e2727035f443a1af5c18f
+bleak==0.22.1 \
+    --hash=sha256:4afb5420847713535381ed2f04e7a70a1d1459153bb76e396a311964fde4aa4f \
+    --hash=sha256:73c2e774c22345e170d36a55a9dd06f6633c88b4184d5f86140a8224f12282d4
     # via tc66c2mqtt (pyproject.toml)
 build==1.2.1 \
     --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
     --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
     # via pip-tools
 bx-py-utils==92 \
     --hash=sha256:38641b2e1a09ed0c64cd6ba0e03c97fea347302439db0234a0492c365ae32719 \
@@ -275,101 +275,101 @@
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via tox
 cookiecutter==2.6.0 \
     --hash=sha256:a54a8e37995e4ed963b3e82831072d1ad4b005af736bb17b99c2cbd9d41b6e2d \
     --hash=sha256:db21f8169ea4f4fdc2408d48ca44859349de2647fbe494a9d6c3edfc0542c21c
     # via manageprojects
-coverage==7.5.0 \
-    --hash=sha256:075299460948cd12722a970c7eae43d25d37989da682997687b34ae6b87c0ef0 \
-    --hash=sha256:07dfdd492d645eea1bd70fb1d6febdcf47db178b0d99161d8e4eed18e7f62fe7 \
-    --hash=sha256:0cbdf2cae14a06827bec50bd58e49249452d211d9caddd8bd80e35b53cb04631 \
-    --hash=sha256:2055c4fb9a6ff624253d432aa471a37202cd8f458c033d6d989be4499aed037b \
-    --hash=sha256:262fffc1f6c1a26125d5d573e1ec379285a3723363f3bd9c83923c9593a2ac25 \
-    --hash=sha256:280132aada3bc2f0fac939a5771db4fbb84f245cb35b94fae4994d4c1f80dae7 \
-    --hash=sha256:2b57780b51084d5223eee7b59f0d4911c31c16ee5aa12737c7a02455829ff067 \
-    --hash=sha256:2bd7065249703cbeb6d4ce679c734bef0ee69baa7bff9724361ada04a15b7e3b \
-    --hash=sha256:3235d7c781232e525b0761730e052388a01548bd7f67d0067a253887c6e8df46 \
-    --hash=sha256:33c020d3322662e74bc507fb11488773a96894aa82a622c35a5a28673c0c26f5 \
-    --hash=sha256:357754dcdfd811462a725e7501a9b4556388e8ecf66e79df6f4b988fa3d0b39a \
-    --hash=sha256:39793731182c4be939b4be0cdecde074b833f6171313cf53481f869937129ed3 \
-    --hash=sha256:3c2b77f295edb9fcdb6a250f83e6481c679335ca7e6e4a955e4290350f2d22a4 \
-    --hash=sha256:41327143c5b1d715f5f98a397608f90ab9ebba606ae4e6f3389c2145410c52b1 \
-    --hash=sha256:427e1e627b0963ac02d7c8730ca6d935df10280d230508c0ba059505e9233475 \
-    --hash=sha256:432949a32c3e3f820af808db1833d6d1631664d53dd3ce487aa25d574e18ad1c \
-    --hash=sha256:4ba01d9ba112b55bfa4b24808ec431197bb34f09f66f7cb4fd0258ff9d3711b1 \
-    --hash=sha256:4d0e206259b73af35c4ec1319fd04003776e11e859936658cb6ceffdeba0f5be \
-    --hash=sha256:51431d0abbed3a868e967f8257c5faf283d41ec882f58413cf295a389bb22e58 \
-    --hash=sha256:565b2e82d0968c977e0b0f7cbf25fd06d78d4856289abc79694c8edcce6eb2de \
-    --hash=sha256:6782cd6216fab5a83216cc39f13ebe30adfac2fa72688c5a4d8d180cd52e8f6a \
-    --hash=sha256:6afd2e84e7da40fe23ca588379f815fb6dbbb1b757c883935ed11647205111cb \
-    --hash=sha256:710c62b6e35a9a766b99b15cdc56d5aeda0914edae8bb467e9c355f75d14ee95 \
-    --hash=sha256:84921b10aeb2dd453247fd10de22907984eaf80901b578a5cf0bb1e279a587cb \
-    --hash=sha256:85a5dbe1ba1bf38d6c63b6d2c42132d45cbee6d9f0c51b52c59aa4afba057517 \
-    --hash=sha256:9c6384cc90e37cfb60435bbbe0488444e54b98700f727f16f64d8bfda0b84656 \
-    --hash=sha256:9dd88fce54abbdbf4c42fb1fea0e498973d07816f24c0e27a1ecaf91883ce69e \
-    --hash=sha256:a81eb64feded34f40c8986869a2f764f0fe2db58c0530d3a4afbcde50f314880 \
-    --hash=sha256:a898c11dca8f8c97b467138004a30133974aacd572818c383596f8d5b2eb04a9 \
-    --hash=sha256:a9960dd1891b2ddf13a7fe45339cd59ecee3abb6b8326d8b932d0c5da208104f \
-    --hash=sha256:a9a7ef30a1b02547c1b23fa9a5564f03c9982fc71eb2ecb7f98c96d7a0db5cf2 \
-    --hash=sha256:ad97ec0da94b378e593ef532b980c15e377df9b9608c7c6da3506953182398af \
-    --hash=sha256:adf032b6c105881f9d77fa17d9eebe0ad1f9bfb2ad25777811f97c5362aa07f2 \
-    --hash=sha256:bbfe6389c5522b99768a93d89aca52ef92310a96b99782973b9d11e80511f932 \
-    --hash=sha256:bd4bacd62aa2f1a1627352fe68885d6ee694bdaebb16038b6e680f2924a9b2cc \
-    --hash=sha256:bf0b4b8d9caa8d64df838e0f8dcf68fb570c5733b726d1494b87f3da85db3a2d \
-    --hash=sha256:c379cdd3efc0658e652a14112d51a7668f6bfca7445c5a10dee7eabecabba19d \
-    --hash=sha256:c58536f6892559e030e6924896a44098bc1290663ea12532c78cef71d0df8493 \
-    --hash=sha256:cbe6581fcff7c8e262eb574244f81f5faaea539e712a058e6707a9d272fe5b64 \
-    --hash=sha256:ced268e82af993d7801a9db2dbc1d2322e786c5dc76295d8e89473d46c6b84d4 \
-    --hash=sha256:cf3539007202ebfe03923128fedfdd245db5860a36810136ad95a564a2fdffff \
-    --hash=sha256:cf62d17310f34084c59c01e027259076479128d11e4661bb6c9acb38c5e19bb8 \
-    --hash=sha256:d0194d654e360b3e6cc9b774e83235bae6b9b2cac3be09040880bb0e8a88f4a1 \
-    --hash=sha256:d3d117890b6eee85887b1eed41eefe2e598ad6e40523d9f94c4c4b213258e4a4 \
-    --hash=sha256:db2de4e546f0ec4b2787d625e0b16b78e99c3e21bc1722b4977c0dddf11ca84e \
-    --hash=sha256:e768d870801f68c74c2b669fc909839660180c366501d4cc4b87efd6b0eee375 \
-    --hash=sha256:e7c211f25777746d468d76f11719e64acb40eed410d81c26cefac641975beb88 \
-    --hash=sha256:eed462b4541c540d63ab57b3fc69e7d8c84d5957668854ee4e408b50e92ce26a \
-    --hash=sha256:f0bfe42523893c188e9616d853c47685e1c575fe25f737adf473d0405dcfa7eb \
-    --hash=sha256:f609ebcb0242d84b7adeee2b06c11a2ddaec5464d21888b2c8255f5fd6a98ae4 \
-    --hash=sha256:fea9d3ca80bcf17edb2c08a4704259dadac196fe5e9274067e7a20511fad1743 \
-    --hash=sha256:fed7a72d54bd52f4aeb6c6e951f363903bd7d70bc1cad64dd1f087980d309ab9
+coverage==7.5.1 \
+    --hash=sha256:0646599e9b139988b63704d704af8e8df7fa4cbc4a1f33df69d97f36cb0a38de \
+    --hash=sha256:0cdcbc320b14c3e5877ee79e649677cb7d89ef588852e9583e6b24c2e5072661 \
+    --hash=sha256:0d0a0f5e06881ecedfe6f3dd2f56dcb057b6dbeb3327fd32d4b12854df36bf26 \
+    --hash=sha256:1434e088b41594baa71188a17533083eabf5609e8e72f16ce8c186001e6b8c41 \
+    --hash=sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d \
+    --hash=sha256:1cc0fe9b0b3a8364093c53b0b4c0c2dd4bb23acbec4c9240b5f284095ccf7981 \
+    --hash=sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2 \
+    --hash=sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34 \
+    --hash=sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f \
+    --hash=sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a \
+    --hash=sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35 \
+    --hash=sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223 \
+    --hash=sha256:4cc37def103a2725bc672f84bd939a6fe4522310503207aae4d56351644682f1 \
+    --hash=sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746 \
+    --hash=sha256:5037f8fcc2a95b1f0e80585bd9d1ec31068a9bcb157d9750a172836e98bc7a90 \
+    --hash=sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c \
+    --hash=sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca \
+    --hash=sha256:57e0204b5b745594e5bc14b9b50006da722827f0b8c776949f1135677e88d0b8 \
+    --hash=sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596 \
+    --hash=sha256:5c3721c2c9e4c4953a41a26c14f4cef64330392a6d2d675c8b1db3b645e31f0e \
+    --hash=sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd \
+    --hash=sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e \
+    --hash=sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3 \
+    --hash=sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e \
+    --hash=sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312 \
+    --hash=sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7 \
+    --hash=sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572 \
+    --hash=sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428 \
+    --hash=sha256:79afb6197e2f7f60c4824dd4b2d4c2ec5801ceb6ba9ce5d2c3080e5660d51a4f \
+    --hash=sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07 \
+    --hash=sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e \
+    --hash=sha256:8fe7502616b67b234482c3ce276ff26f39ffe88adca2acf0261df4b8454668b4 \
+    --hash=sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136 \
+    --hash=sha256:9735317685ba6ec7e3754798c8871c2f49aa5e687cc794a0b1d284b2389d1bd5 \
+    --hash=sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8 \
+    --hash=sha256:9e78295f4144f9dacfed4f92935fbe1780021247c2fabf73a819b17f0ccfff8d \
+    --hash=sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228 \
+    --hash=sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206 \
+    --hash=sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa \
+    --hash=sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e \
+    --hash=sha256:c3e757949f268364b96ca894b4c342b41dc6f8f8b66c37878aacef5930db61be \
+    --hash=sha256:ca498687ca46a62ae590253fba634a1fe9836bc56f626852fb2720f334c9e4e5 \
+    --hash=sha256:d1d0d98d95dd18fe29dc66808e1accf59f037d5716f86a501fc0256455219668 \
+    --hash=sha256:d21918e9ef11edf36764b93101e2ae8cc82aa5efdc7c5a4e9c6c35a48496d601 \
+    --hash=sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057 \
+    --hash=sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146 \
+    --hash=sha256:dde0070c40ea8bb3641e811c1cfbf18e265d024deff6de52c5950677a8fb1e0f \
+    --hash=sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8 \
+    --hash=sha256:e2213def81a50519d7cc56ed643c9e93e0247f5bbe0d1247d15fa520814a7cd7 \
+    --hash=sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987 \
+    --hash=sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19 \
+    --hash=sha256:fc0b4d8bfeabd25ea75e94632f5b6e047eef8adaed0c2161ada1e922e7f7cece
     # via tc66c2mqtt (pyproject.toml)
-cryptography==42.0.5 \
-    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
-    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
-    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
-    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
-    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
-    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
-    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
-    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
-    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
-    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
-    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
-    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
-    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
-    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
-    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
-    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
-    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
-    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
-    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
-    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
-    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
-    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
-    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
-    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
-    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
-    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
-    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
-    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
-    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
-    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
-    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
-    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
+cryptography==42.0.7 \
+    --hash=sha256:02c0eee2d7133bdbbc5e24441258d5d2244beb31da5ed19fbb80315f4bbbff55 \
+    --hash=sha256:0d563795db98b4cd57742a78a288cdbdc9daedac29f2239793071fe114f13785 \
+    --hash=sha256:16268d46086bb8ad5bf0a2b5544d8a9ed87a0e33f5e77dd3c3301e63d941a83b \
+    --hash=sha256:1a58839984d9cb34c855197043eaae2c187d930ca6d644612843b4fe8513c886 \
+    --hash=sha256:2954fccea107026512b15afb4aa664a5640cd0af630e2ee3962f2602693f0c82 \
+    --hash=sha256:2e47577f9b18723fa294b0ea9a17d5e53a227867a0a4904a1a076d1646d45ca1 \
+    --hash=sha256:31adb7d06fe4383226c3e963471f6837742889b3c4caa55aac20ad951bc8ffda \
+    --hash=sha256:3577d029bc3f4827dd5bf8bf7710cac13527b470bbf1820a3f394adb38ed7d5f \
+    --hash=sha256:36017400817987670037fbb0324d71489b6ead6231c9604f8fc1f7d008087c68 \
+    --hash=sha256:362e7197754c231797ec45ee081f3088a27a47c6c01eff2ac83f60f85a50fe60 \
+    --hash=sha256:3de9a45d3b2b7d8088c3fbf1ed4395dfeff79d07842217b38df14ef09ce1d8d7 \
+    --hash=sha256:4f698edacf9c9e0371112792558d2f705b5645076cc0aaae02f816a0171770fd \
+    --hash=sha256:5482e789294854c28237bba77c4c83be698be740e31a3ae5e879ee5444166582 \
+    --hash=sha256:5e44507bf8d14b36b8389b226665d597bc0f18ea035d75b4e53c7b1ea84583cc \
+    --hash=sha256:779245e13b9a6638df14641d029add5dc17edbef6ec915688f3acb9e720a5858 \
+    --hash=sha256:789caea816c6704f63f6241a519bfa347f72fbd67ba28d04636b7c6b7da94b0b \
+    --hash=sha256:7f8b25fa616d8b846aef64b15c606bb0828dbc35faf90566eb139aa9cff67af2 \
+    --hash=sha256:8cb8ce7c3347fcf9446f201dc30e2d5a3c898d009126010cbd1f443f28b52678 \
+    --hash=sha256:93a3209f6bb2b33e725ed08ee0991b92976dfdcf4e8b38646540674fc7508e13 \
+    --hash=sha256:a3a5ac8b56fe37f3125e5b72b61dcde43283e5370827f5233893d461b7360cd4 \
+    --hash=sha256:a47787a5e3649008a1102d3df55424e86606c9bae6fb77ac59afe06d234605f8 \
+    --hash=sha256:a79165431551042cc9d1d90e6145d5d0d3ab0f2d66326c201d9b0e7f5bf43604 \
+    --hash=sha256:a987f840718078212fdf4504d0fd4c6effe34a7e4740378e59d47696e8dfb477 \
+    --hash=sha256:a9bc127cdc4ecf87a5ea22a2556cab6c7eda2923f84e4f3cc588e8470ce4e42e \
+    --hash=sha256:bd13b5e9b543532453de08bcdc3cc7cebec6f9883e886fd20a92f26940fd3e7a \
+    --hash=sha256:c65f96dad14f8528a447414125e1fc8feb2ad5a272b8f68477abbcc1ea7d94b9 \
+    --hash=sha256:d8e3098721b84392ee45af2dd554c947c32cc52f862b6a3ae982dbb90f577f14 \
+    --hash=sha256:e6b79d0adb01aae87e8a44c2b64bc3f3fe59515280e00fb6d57a7267a2583cda \
+    --hash=sha256:e6b8f1881dac458c34778d0a424ae5769de30544fc678eac51c1c8bb2183e9da \
+    --hash=sha256:e9b2a6309f14c0497f348d08a065d52f3020656f675819fc405fb63bbcd26562 \
+    --hash=sha256:ecbfbc00bf55888edda9868a4cf927205de8499e7fabe6c050322298382953f2 \
+    --hash=sha256:efd0bf5205240182e0f13bcaea41be4fdf5c22c5129fc7ced4a0282ac86998c9
     # via
     #   authlib
     #   secretstorage
 darker[color,flynt,isort]==2.1.1 \
     --hash=sha256:a6e6a682c0604e76fe9aec7650e96a944f517563c69b28fcc076db9d957d98ea \
     --hash=sha256:ead701414c45359fc0312bc285614d3285fc135476d43f3bc08d989ee19d9020
     # via
@@ -377,49 +377,49 @@
     #   tc66c2mqtt (pyproject.toml)
 darkgraylib==1.2.1 \
     --hash=sha256:60c59de69842367ce0c78c32c451fa8e9d29500e681312d9864a7416bcdb7792 \
     --hash=sha256:a5dd6a2015a470d9047278cdd01a91ccb1d746675f8fd4562b3b5f6b8cbda930
     # via
     #   darker
     #   graylint
-dbus-fast==2.21.1 \
-    --hash=sha256:0ff6c72bcd6539d798015bda33c7ce35c7de76276b9bd45e48db13672713521a \
-    --hash=sha256:13ab6a0f64d345cb42c489239962261f724bd441458bef245b39828ed94ea6f4 \
-    --hash=sha256:15d62adfab7c6f4a491085f53f9634d24745ca5a2772549945b7e2de27c0d534 \
-    --hash=sha256:237db4ab0b90e5284ea7659264630d693273cdbda323a40368f320869bf6470f \
-    --hash=sha256:2db4d0d60a891a8b20a4c6de68a088efe73b29ab4a5949fe6aad2713c131e174 \
-    --hash=sha256:36d8cd43b3799e766158f1bb0b27cc4eef685fd892417b0382b7fdfdd94f1e6c \
-    --hash=sha256:39a3f3662391b49553bf9d9d2e9a6cb31e0d7d337557ee0c0be5c558a3c7d230 \
-    --hash=sha256:4591e0962c272d42d305ab3fb8889f13d47255e412fd3b9839620836662c91fe \
-    --hash=sha256:47aa28520fe274414b655c74cbe2e91d8b76e22f40cd41a758bb6975e526827b \
-    --hash=sha256:52641305461660c8969c6bb12364206a108c5c9e014c9220c70b99c4f48b6750 \
-    --hash=sha256:54e8771e31ee1deb01feef2475c12123cab770c371ecc97af98eb6ca10a2858e \
-    --hash=sha256:62331ee3871f6881f517ca65ae185fb2462a0bf2fe78acc4a4d621fc4da08396 \
-    --hash=sha256:65e76b20099c33352d5e7734a219982858873cf66fe510951d9bd27cb690190f \
-    --hash=sha256:66e160f496ac79248feb09a0acf4aab5d139d823330cbd9377f6e19ae007330a \
-    --hash=sha256:670b5c4d78c9c2d25e7ba650d212d98bf24d40292f91fe4e2f3ad4f80dc6d7e5 \
-    --hash=sha256:7333896544a4d0a3d708bd092f8c05eb3599dc2b34ae6e4c4b44d04d5514b0ec \
-    --hash=sha256:78c84ecf19459571784fd6a8ad8b3e9006cf96c3282e8220bc49098866ef4cc7 \
-    --hash=sha256:85be33bb04e918833ac6f28f68f83a1e83425eb6e08b9c482cc3318820dfd55f \
-    --hash=sha256:87b852d2005f1d59399ca51c5f3538f28a4742d739d7abe82b7ae8d01d8a5d02 \
-    --hash=sha256:8fae9609d972f0c2b72017796a8140b8a6fb842426f0aed4f43f0fa7d780a16f \
-    --hash=sha256:927f294b1dc7cea9372ef8c7c46ebeb5c7e6c1c7345358f952e7499bdbdf7eb4 \
-    --hash=sha256:999fed45cb391126107b804be0e344e75556fceaee4cc30a0ca06d77309bdf3c \
-    --hash=sha256:9cae9a6b9bb54f3f89424fdd960b60ac53239b9e5d4a5d9a598d222fbf8d3173 \
-    --hash=sha256:9e9a43ea42b8a9f2c62ca50ce05582de7b4f1f7eb27091f904578c29124af246 \
-    --hash=sha256:a5b3895ea12c4e636dfaacf75fa5bd1e8450b2ffb97507520991eaf1989d102e \
-    --hash=sha256:a999e35628988ad4f81af36192cd592b8fd1e72e1bbc76a64d80808e6f4b9540 \
-    --hash=sha256:b04b88be594dad81b33f6770283eed2125763632515c5112f8aa30f259cd334c \
-    --hash=sha256:b7d1f35218549762e52a782c0b548e0681332beee773d3dfffe2efc38b2ee960 \
-    --hash=sha256:c585e7a94bb723a70b4966677b882be8bda324cc41bd129765e3ceab428889bb \
-    --hash=sha256:c938eb7130067ca3b74b248ee376228776d8f013a206ae78e6fc644c9db0f4f5 \
-    --hash=sha256:cbfd6892fa092cbd6f52edcb24797af62fba8baa50995db856b0a342184c850d \
-    --hash=sha256:d4da8d58064f0a3dd07bfc283ba912b9d5a4cb38f1c0fcd9ecb2b9d43111243c \
-    --hash=sha256:e2309b9cafba799e9d343fdfdd5ae46276adf3929fef60f296f23b97ed1aa2f6 \
-    --hash=sha256:ffc2b6beb212d0d231816dcb7bd8bcdafccd04750ba8f5e915f40ad312f5adf2
+dbus-fast==2.21.2 \
+    --hash=sha256:044eec5d0668d3229480094f5b2aefafb336afa6976d686bd0cd8770eee1bb2c \
+    --hash=sha256:0b78f2116fb745a7623c8e18d9c435bfe4732e4f9284a923c4b9a44ef68ae2d4 \
+    --hash=sha256:194899057b8382c1902c32e1a565a2d47bcc99e06aafe9d660348394532a4bf6 \
+    --hash=sha256:29f07ef89e35b93afa87dea86abec2aff68802572944485250f50def15dc5ef8 \
+    --hash=sha256:2fd1be6967a92957f517dbd3755ee7cddc128ec840af2ef4ad6fb023a0dac74d \
+    --hash=sha256:32efcbe276a4fdf6946450c512355e7ae22836cf3595d48c59330687cda52117 \
+    --hash=sha256:37e6f717dedc299fc15ab8f5ec5b180725d2b896ba1aaef07c1921df0b7113a0 \
+    --hash=sha256:38138fc5a24797cc443c6894d25497271ccf3399c8aa8cdba228a7bdda2d2921 \
+    --hash=sha256:3b96a645cbd035f47f3b934130cd0ae977c043480ad7fe9838f78fdcb480c189 \
+    --hash=sha256:40aa9068759bbf7e062f074c965b391b95f18f897cc9be6eb906ee48a6f77724 \
+    --hash=sha256:51279b69ac6b872208f3aa1b00b910dd9ef9c3d625b79eb378405dbd72a29cab \
+    --hash=sha256:601c3c8796e7edd23bce0432e44ca8f0b85c48a17ab5258f57cd8fe815f9c07a \
+    --hash=sha256:60d989030403cc1611105bec6a90df22967e523ae28486dee5f9bd644e37f797 \
+    --hash=sha256:6c6f1fda6f318061a023d6da96ee50ad2d30c04557012a60a0f1abd39c2a8704 \
+    --hash=sha256:6edec4f92d32b9a288b38457a114086a0d5f5fdec9c3e9b7ff6052fd45963c1d \
+    --hash=sha256:6f056f2bfee24e87a4184202d3b108a56176344303bb1278988f13f5e90777da \
+    --hash=sha256:81ac390d4e26711b3ac46b3dd81a29bcbc1eddd4a408b336c67f0c94eb6d7ff0 \
+    --hash=sha256:8645187b2e86c5141217adcb462d6dbecd37fb2ab8705f66b3773a66206ef83d \
+    --hash=sha256:886ce5750d4e64636bd933f22513e9ba06b7ee9650f28699c553c162b52db666 \
+    --hash=sha256:90f09498ac91f0e6ddc7fa569e851a2b258a70917cd07ae8412ad5725ef1d411 \
+    --hash=sha256:9ba884d102e069e105f22986fccf1d21776e6ced11f4b75aeddcc37e728a80fd \
+    --hash=sha256:a3159f1cecd4b86f565c01da787ad6eaa57e8ba210d355836fa849e4c0b1ee57 \
+    --hash=sha256:aabe539f0e9961a1beb6e8c0078112a1a60de18958335678edb3f26021951ff9 \
+    --hash=sha256:afde99d085a330e8aed59535d808636f1f563cb08d12900d0e415508e6270a1d \
+    --hash=sha256:b17f1eafeaa825e8933a5394157db9e0a24e65eac188a244dbbbc01dc23fde7a \
+    --hash=sha256:b5e2015a385f0b364eff1827b151313429d3148d2718d679bec8a9c67b78721a \
+    --hash=sha256:b5f79edcb0dd48e98b1a1e3e4a655fd0ecc2ba72275f9e8379e8655b4411edcc \
+    --hash=sha256:bc696304ce0f5da374ddfb3e83273e9d89602a8f20e7fab57b079378f2cb5789 \
+    --hash=sha256:c2bb0fd813bf3cafc6796d86d42cc8a9d37c2633d973dd963c3ad4c080d7061d \
+    --hash=sha256:d2406b838ccbda9bd49dda4a7620ce228da306cd8f9a3f8c9f42b2d792a491fb \
+    --hash=sha256:d9f4191f7108f9433e5c017915e60ec57231aaf58c82fde6e20bd497998ebc97 \
+    --hash=sha256:eade5ed18327bf306b75e525ded98c08921e1b21d42e715b7f0a1371a7669168 \
+    --hash=sha256:ed431895630135da9cec736326304f0833ac31919043efdbecf8f6c7bed40d05 \
+    --hash=sha256:f5db0737471e60228c1a6aabecbf883c972f0b9e50bf7fc0878a8b35ebdf1d1e
     # via bleak
 distlib==0.3.8 \
     --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
     --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
     # via virtualenv
 docutils==0.21.2 \
     --hash=sha256:3a6b18732edf182daa3cd12775bbb338cf5691468f91eeeb109deff6ebfa986f \
@@ -432,17 +432,17 @@
     #   safety
     #   safety-schemas
 editorconfig==0.12.4 \
     --hash=sha256:24857fa1793917dd9ccf0c7810a07e05404ce9b823521c7dce22a4fb5d125f80
     # via
     #   manageprojects
     #   tc66c2mqtt (pyproject.toml)
-filelock==3.13.4 \
-    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
-    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
+filelock==3.14.0 \
+    --hash=sha256:43339835842f110ca7ae60f1e1c160714c5a6afd15a2873419ab185334975c0f \
+    --hash=sha256:6ea72da3be9b8c82afd3edcf99f2fffbb5076335a5ae4d03248bb5b6c3eae78a
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0 \
     --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
     --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
     # via
@@ -455,51 +455,46 @@
     # via
     #   manageprojects
     #   tc66c2mqtt (pyproject.toml)
 flynt==1.0.1 \
     --hash=sha256:65d1c546434827275123222a98408e9561bcd67db832dd58f530ff17b8329ec1 \
     --hash=sha256:988aac00672a5469726cc0a17cef7d1178c284a9fe8563458db2475d0aaed965
     # via darker
-frozendict==2.4.2 \
-    --hash=sha256:07153e6d2720fa1131bb180ce388c7042affb29561d8bcd1c0d6e683a8beaea2 \
-    --hash=sha256:1412aeb325e4a28cfe32106c66c046372bb7fd5a9af1748193549c5d01a9e9c1 \
-    --hash=sha256:146129502cd9d96de64e0c8f7dc4c66422da3d4bfccf891dd80a3821b358a926 \
-    --hash=sha256:19743495b1e92a7e4db56fcd6a5d36ea1d1b0f550822d6fd780e44d58f0b8c18 \
-    --hash=sha256:19e64630e164a297f83e9a1c69f1cd36fa4b3d1196c1f9fc006a0385aa198ea4 \
-    --hash=sha256:20a6f741c92fdeb3766924cde42b8ee445cf568e3be8aa983cb83e9fe5b61e63 \
-    --hash=sha256:34704f9ffb21448d4b5c0f9239f8f058c0efab4bfdbe2956c5be978fef0b929c \
-    --hash=sha256:3fc6e3158107b5431255978b954758b1041cc70a3b8e7657373110512eb528e3 \
-    --hash=sha256:476e4857e1d87b05c9102dd5409216ce4716cb7df619e6657429bc99279303cc \
-    --hash=sha256:4a5841681e70d2862ca153543f2912e0bab034bf29e2d3610e86ea42506121c2 \
-    --hash=sha256:4a8b298f39242d25770d029588ce9d4f524e9f4edc60d2d34b6178fb07c8a93e \
-    --hash=sha256:4ca09a376114172e4d9918e6d576f58244c45e21f5af1245085699fd3a171c47 \
-    --hash=sha256:4db1d6cc412bd865cab36723995208b82166a97bc6c724753bcd2b90cf24f164 \
-    --hash=sha256:5280d685cd1659883a3010dec843afe3065416ae92e453498997d4474a898a39 \
-    --hash=sha256:55953aa2acf5bf183c664f3d0f540f8c8ac8f5fa97170f2098d413414318eb2b \
-    --hash=sha256:741779e1d1a2e6bb2c623f78423bd5d14aad35dc0c57e6ccc89e54eaab5f1b8a \
-    --hash=sha256:79e1c94ad2a925ad5723d82a4134c6d851d5a7bc72b7e9da8b2087c42758a512 \
-    --hash=sha256:7a8d2ea4f10505ad15f53ce3742420682d916d0c4d566edb8e1019756e7cea30 \
-    --hash=sha256:7d13ffe649e9db6f4bb5e107d9be7dfd23e13101bc69f97aa5fa6cbf6aecaadd \
-    --hash=sha256:81efb4ea854a1c93d954a67389eaf78c508acb2d4768321a835cda2754ec5c01 \
-    --hash=sha256:83cc9d063131fd8adbeb18a473d222b5dc8301cac9505cfe578158f9a9bf55a9 \
-    --hash=sha256:84c36bfa819cd8442f6e0bdb86413c7678b2822a46b1a22cfa0f0dd30d9e5c45 \
-    --hash=sha256:92c46b155ea9eb9ecabc66ba2d9030f2634319f55c6448688965ece094f14b51 \
-    --hash=sha256:9ac1f74ccf818977abbc1868090c06436b8f06534d306f808f15cffc304ae046 \
-    --hash=sha256:ac954be447a907face9b652207fbd943b9b552212890db959ba653e8f1dc3f56 \
-    --hash=sha256:bedb0a6587bae53bd53727b92a87c4cf90ad7a7e0bd2db562d439beb6982712e \
-    --hash=sha256:c157b8a92743a7905b341edb0663044fecdc7780f96c59a2843d3da68d694b90 \
-    --hash=sha256:c5f1a4d9662b854dce52b560b60f51349905dc871826b8c6be20141a13067a53 \
-    --hash=sha256:cbab325c0a98b2f3ee291b36710623781b4977a3057f9103a7b0f11bcc23b177 \
-    --hash=sha256:cead3bfe70c90c634a9b76807c9d7e75e6c5666ec96fa2cea8e7412ccf22a1f8 \
-    --hash=sha256:d4a10119f17552cbeab48d4ae830ba091c6d47616589618adc31f251184579a7 \
-    --hash=sha256:f7a90ea6d5248617a1222daef07d22fb146ff07635a36db327e1ce114bf3e304 \
-    --hash=sha256:f7ce0535f02eba9746e4e2cf0abef0f0f2051d20fdccf4af31bc3d1adecf5a71 \
-    --hash=sha256:f7e0ff5e84742604a1b42c2de4f1e67630c0868cf52a5c585b54a99e06f6b453 \
-    --hash=sha256:f958d40637e0440bce2453019821c94fe86cfc5f3847ae11cd4f02c3548b1d1b \
-    --hash=sha256:ff6fb5831539fffb09d71cc0cc0462b1f27c0160cb6c6fa2d1f4c1bc7fffe52a
+frozendict==2.4.4 \
+    --hash=sha256:07c3a5dee8bbb84cba770e273cdbf2c87c8e035903af8f781292d72583416801 \
+    --hash=sha256:12a342e439aef28ccec533f0253ea53d75fe9102bd6ea928ff530e76eac38906 \
+    --hash=sha256:1697793b5f62b416c0fc1d94638ec91ed3aa4ab277f6affa3a95216ecb3af170 \
+    --hash=sha256:199a4d32194f3afed6258de7e317054155bc9519252b568d9cfffde7e4d834e5 \
+    --hash=sha256:259528ba6b56fa051bc996f1c4d8b57e30d6dd3bc2f27441891b04babc4b5e73 \
+    --hash=sha256:2b70b431e3a72d410a2cdf1497b3aba2f553635e0c0f657ce311d841bf8273b6 \
+    --hash=sha256:2bd009cf4fc47972838a91e9b83654dc9a095dc4f2bb3a37c3f3124c8a364543 \
+    --hash=sha256:2d8536e068d6bf281f23fa835ac07747fb0f8851879dd189e9709f9567408b4d \
+    --hash=sha256:3148062675536724502c6344d7c485dd4667fdf7980ca9bd05e338ccc0c4471e \
+    --hash=sha256:3f7c031b26e4ee6a3f786ceb5e3abf1181c4ade92dce1f847da26ea2c96008c7 \
+    --hash=sha256:4297d694eb600efa429769125a6f910ec02b85606f22f178bafbee309e7d3ec7 \
+    --hash=sha256:4a59578d47b3949437519b5c39a016a6116b9e787bb19289e333faae81462e59 \
+    --hash=sha256:4ae8d05c8d0b6134bfb6bfb369d5fa0c4df21eabb5ca7f645af95fdc6689678e \
+    --hash=sha256:5d58d9a8d9e49662c6dafbea5e641f97decdb3d6ccd76e55e79818415362ba25 \
+    --hash=sha256:63aa49f1919af7d45fb8fd5dec4c0859bc09f46880bd6297c79bb2db2969b63d \
+    --hash=sha256:6874fec816b37b6eb5795b00e0574cba261bf59723e2de607a195d5edaff0786 \
+    --hash=sha256:6eb716e6a6d693c03b1d53280a1947716129f5ef9bcdd061db5c17dea44b80fe \
+    --hash=sha256:78c94991944dd33c5376f720228e5b252ee67faf3bac50ef381adc9e51e90d9d \
+    --hash=sha256:7f79c26dff10ce11dad3b3627c89bb2e87b9dd5958c2b24325f16a23019b8b94 \
+    --hash=sha256:7fee9420475bb6ff357000092aa9990c2f6182b2bab15764330f4ad7de2eae49 \
+    --hash=sha256:812ab17522ba13637826e65454115a914c2da538356e85f43ecea069813e4b33 \
+    --hash=sha256:85375ec6e979e6373bffb4f54576a68bf7497c350861d20686ccae38aab69c0a \
+    --hash=sha256:87ebcde21565a14fe039672c25550060d6f6d88cf1f339beac094c3b10004eb0 \
+    --hash=sha256:93a7b19afb429cbf99d56faf436b45ef2fa8fe9aca89c49eb1610c3bd85f1760 \
+    --hash=sha256:b3b967d5065872e27b06f785a80c0ed0a45d1f7c9b85223da05358e734d858ca \
+    --hash=sha256:c6bf9260018d653f3cab9bd147bd8592bf98a5c6e338be0491ced3c196c034a3 \
+    --hash=sha256:c8f92425686323a950337da4b75b4c17a3327b831df8c881df24038d560640d4 \
+    --hash=sha256:d13b4310db337f4d2103867c5a05090b22bc4d50ca842093779ef541ea9c9eea \
+    --hash=sha256:dc2228874eacae390e63fd4f2bb513b3144066a977dc192163c9f6c7f6de6474 \
+    --hash=sha256:e1b941132d79ce72d562a13341d38fc217bc1ee24d8c35a20d754e79ff99e038 \
+    --hash=sha256:fefeb700bc7eb8b4c2dc48704e4221860d254c8989fb53488540bc44e44a1ac2
     # via ha-services
 graylint==1.1.1 \
     --hash=sha256:0fd8e02972ca03d0ef2bf0adea76b5343efcd492d7afb5f658f3e3a724f55a36 \
     --hash=sha256:b7e0eab6c159684dbf5ef84e942c3340f6a6549b02a3d11b1a1763cc4f8f0593
     # via darker
 ha-services==2.6.0 \
     --hash=sha256:55468ad8454e0b87a1f0ec5b934b1c98d864a1ae200faf4bdc3efd5c8c61c963 \
@@ -533,23 +528,23 @@
     # via keyring
 jeepney==0.8.0 \
     --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
     --hash=sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755
     # via
     #   keyring
     #   secretstorage
-jinja2==3.1.3 \
-    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
-    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+jinja2==3.1.4 \
+    --hash=sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369 \
+    --hash=sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d
     # via
     #   cookiecutter
     #   safety
-keyring==25.2.0 \
-    --hash=sha256:19f17d40335444aab84b19a0d16a77ec0758a9c384e3446ae2ed8bd6d53b67a5 \
-    --hash=sha256:7045f367268ce42dba44745050164b431e46f6e92f99ef2937dfadaef368d8cf
+keyring==25.2.1 \
+    --hash=sha256:2458681cdefc0dbc0b7eb6cf75d0b98e59f9ad9b2d4edd319d18f68bdca95e50 \
+    --hash=sha256:daaffd42dbda25ddafb1ad5fec4024e5bbcfe424597ca1ca452b299861e49f1b
     # via twine
 manageprojects==0.17.1 \
     --hash=sha256:355d970261f14b53b574d102e7e82462fe6769baa06c479f00f07a0bcfcb8e4d \
     --hash=sha256:4662ff7f0e64ea9b420b67c270594c88542858a1434ebe8b5f93b7bf2ae2e706
     # via tc66c2mqtt (pyproject.toml)
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
@@ -613,17 +608,17 @@
     --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
     --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
     --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
     --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
     --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
     --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
     # via jinja2
-marshmallow==3.21.1 \
-    --hash=sha256:4e65e9e0d80fc9e609574b9983cf32579f305c718afb30d7233ab818571768c3 \
-    --hash=sha256:f085493f79efb0644f270a9bf2892843142d80d7174bbbd2f3713f2a589dc633
+marshmallow==3.21.2 \
+    --hash=sha256:70b54a6282f4704d12c0a41599682c5c5450e843b9ec406308653b47c59648a1 \
+    --hash=sha256:82408deadd8b33d56338d2182d455db632c6313aa2af61916672146bb32edc56
     # via safety
 mccabe==0.7.0 \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
     # via flake8
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
@@ -737,33 +732,33 @@
     #   cli-base-utilities
     #   dparse
     #   marshmallow
     #   pyproject-api
     #   safety
     #   safety-schemas
     #   tox
-paho-mqtt==2.0.0 \
-    --hash=sha256:13b205f29251e4f2c66a6c923c31fc4fd780561e03b2d775cff8e4f2915cf947 \
-    --hash=sha256:2ef745073dfc9aa68bfec30d0b9b6f0304ea75182bae85a7c77a80cefce1eff5
+paho-mqtt==2.1.0 \
+    --hash=sha256:12d6e7511d4137555a3f6ea167ae846af2c7357b10bc6fa4f7c3968fc1723834 \
+    --hash=sha256:6db9ba9b34ed5bc6b6e3812718c7e06e2fd7444540df2455d2c51bd58808feee
     # via ha-services
 pathspec==0.12.1 \
     --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
     --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
     # via black
 pip-tools==7.4.1 \
     --hash=sha256:4c690e5fbae2f21e87843e89c26191f0d9454f362d8acdbd695716493ec8b3a9 \
     --hash=sha256:864826f5073864450e24dbeeb85ce3920cdfb09848a3d69ebf537b521f14bcc9
     # via tc66c2mqtt (pyproject.toml)
 pkginfo==1.10.0 \
     --hash=sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297 \
     --hash=sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097
     # via twine
-platformdirs==4.2.1 \
-    --hash=sha256:031cd18d4ec63ec53e82dceaac0417d218a6863f7745dfcc9efe7793b7039bdf \
-    --hash=sha256:17d5a1161b3fd67b390023cb2d3b026bbd40abde6fdb052dfbd3a29c3ba22ee1
+platformdirs==4.2.2 \
+    --hash=sha256:2d7a1657e36a80ea911db832a8a6ece5ee53d8de21edd5cc5879af6530b1bfee \
+    --hash=sha256:38b7b51f512eed9e84a22788b4bce1de17c0adb134d6becb09836e37d8654cd3
     # via
     #   black
     #   tox
     #   virtualenv
 pluggy==1.5.0 \
     --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
     --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
@@ -921,17 +916,17 @@
     --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
     --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
     # via
     #   autoflake
     #   flake8
     #   manageprojects
     #   tc66c2mqtt (pyproject.toml)
-pygments==2.17.2 \
-    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
-    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
+pygments==2.18.0 \
+    --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
+    --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
     # via
     #   darker
     #   readme-renderer
     #   rich
 pyproject-api==1.6.1 \
     --hash=sha256:1817dc018adc0d1ff9ca1ed8c60e1623d5aaca40814b953af14a9cf9a5cae538 \
     --hash=sha256:4c0116d60476b0786c88692cf4e325a9814965e2469c5998b830bba16b183675
@@ -1038,17 +1033,17 @@
     #   ha-services
     #   manageprojects
     #   rich-click
     #   safety
     #   tc66c2mqtt (pyproject.toml)
     #   twine
     #   typer
-rich-click==1.7.4 \
-    --hash=sha256:7ce5de8e4dc0333aec946113529b3eeb349f2e5d2fafee96b9edf8ee36a01395 \
-    --hash=sha256:e363655475c60fec5a3e16a1eb618118ed79e666c365a36006b107c17c93ac4e
+rich-click==1.8.2 \
+    --hash=sha256:8e29bdede858b59aa2859a1ab1c4ccbd39ed7ed5870262dae756fba6b5dc72e8 \
+    --hash=sha256:b57856f304e4fe0394b82d7ce0784450758f8c8b4e201ccc4320501cc201806b
     # via
     #   cli-base-utilities
     #   ha-services
     #   manageprojects
     #   tc66c2mqtt (pyproject.toml)
 ruamel-yaml==0.18.6 \
     --hash=sha256:57b53ba33def16c4f3d807c0ccbc00f8a6081827e81ba2491691b76882d0c636 \
@@ -1104,17 +1099,17 @@
     --hash=sha256:e2b4c44b60eadec492926a7270abb100ef9f72798e18743939bdbf037aab8c28 \
     --hash=sha256:e79e5db08739731b0ce4850bed599235d601701d5694c36570a99a0c5ca41a9d \
     --hash=sha256:ebc06178e8821efc9692ea7544aa5644217358490145629914d8020042c24aa1 \
     --hash=sha256:edaef1c1200c4b4cb914583150dcaa3bc30e592e907c01117c08b13a07255ec2 \
     --hash=sha256:f481f16baec5290e45aebdc2a5168ebc6d35189ae6fea7a58787613a25f6e875 \
     --hash=sha256:fff3573c2db359f091e1589c3d7c5fc2f86f5bdb6f24252c2d8e539d4e45f412
     # via ruamel-yaml
-safety==3.1.0 \
-    --hash=sha256:71f47b82ece153ec2f240e277f7cbfa70d5da2e0d143162c67f63b2f7459a1aa \
-    --hash=sha256:f2ba2d36f15ac1e24751547a73b854509a7d6db31efd30b57f64ffdf9d021934
+safety==3.2.0 \
+    --hash=sha256:8bd5cab5f3d8a61ce0ea6e98f267c1006d056097c45c644fee7afeff7d5949c1 \
+    --hash=sha256:a432fc9d17e79a4386c4f093656b617c56f839cde022649cfa796d72c7a544de
     # via tc66c2mqtt (pyproject.toml)
 safety-schemas==0.0.2 \
     --hash=sha256:277c077ce6e53221874a87c29515ffdd2f3773a6db4d035a9f67cc98db3b8c7f \
     --hash=sha256:7d1b040ec06480f05cff6b45ea7a93e09c8942df864fb0d01ddeb67c323cfa8c
     # via safety
 secretstorage==3.3.3 \
     --hash=sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77 \
@@ -1144,17 +1139,17 @@
     #   darkgraylib
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   cli-base-utilities
     #   tc66c2mqtt (pyproject.toml)
-tomlkit==0.12.4 \
-    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
-    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
+tomlkit==0.12.5 \
+    --hash=sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f \
+    --hash=sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c
     # via
     #   cli-base-utilities
     #   ha-services
     #   manageprojects
 tox==4.15.0 \
     --hash=sha256:300055f335d855b2ab1b12c5802de7f62a36d4fd53f30bd2835f6a201dda46ea \
     --hash=sha256:7a0beeef166fbe566f54f795b4906c31b428eddafc0102ac00d20998dd1933f6
@@ -1192,17 +1187,17 @@
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via
     #   requests
     #   safety
     #   tc66c2mqtt (pyproject.toml)
     #   twine
-virtualenv==20.26.0 \
-    --hash=sha256:0846377ea76e818daaa3e00a4365c018bc3ac9760cbb3544de542885aad61fb3 \
-    --hash=sha256:ec25a9671a5102c8d2657f62792a27b48f016664c6873f6beed3800008577210
+virtualenv==20.26.2 \
+    --hash=sha256:82bf0f4eebbb78d36ddaee0283d43fe5736b53880b8a8cdcd37390a07ac3741c \
+    --hash=sha256:a624db5e94f01ad993d476b9ee5346fdf7b9de43ccaee0e0197012dc838a0e9b
     # via tox
 wheel==0.43.0 \
     --hash=sha256:465ef92c69fa5c5da2d1cf8ac40559a8c940886afcef87dcf14b9470862f1d85 \
     --hash=sha256:55c570405f142630c6b9f72fe09d9b67cf1477fcf543ae5b8dcb1f5b7377da81
     # via pip-tools
 zipp==3.18.1 \
     --hash=sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b \
```

### Comparing `tc66c2mqtt-0.0.1rc0/requirements.txt` & `tc66c2mqtt-0.1.0/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #
 #    ./dev-cli.py update
 #
 async-timeout==4.0.3 \
     --hash=sha256:4640d96be84d82d02ed59ea2b7105a0f7b33abe8703703cd0ab0bf87c427522f \
     --hash=sha256:7405140ff1230c310e51dc27b3145b9092d659ce68ff733fb0cefe3ee42be028
     # via cli-base-utilities
-bleak==0.21.1 \
-    --hash=sha256:ccec260a0f5ec02dd133d68b0351c0151b2ecf3ddd0bcabc4c04a1cdd7f33256 \
-    --hash=sha256:ec4a1a2772fb315b992cbaa1153070c7e26968a52b0e2727035f443a1af5c18f
+bleak==0.22.1 \
+    --hash=sha256:4afb5420847713535381ed2f04e7a70a1d1459153bb76e396a311964fde4aa4f \
+    --hash=sha256:73c2e774c22345e170d36a55a9dd06f6633c88b4184d5f86140a8224f12282d4
     # via tc66c2mqtt (pyproject.toml)
 bx-py-utils==92 \
     --hash=sha256:38641b2e1a09ed0c64cd6ba0e03c97fea347302439db0234a0492c365ae32719 \
     --hash=sha256:849c59429af6ca0bf35265569884193c60be578285a66b533146e5782a10637b
     # via
     #   cli-base-utilities
     #   tc66c2mqtt (pyproject.toml)
@@ -28,87 +28,82 @@
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
     # via
     #   cli-base-utilities
     #   ha-services
     #   rich-click
     #   tc66c2mqtt (pyproject.toml)
-dbus-fast==2.21.1 \
-    --hash=sha256:0ff6c72bcd6539d798015bda33c7ce35c7de76276b9bd45e48db13672713521a \
-    --hash=sha256:13ab6a0f64d345cb42c489239962261f724bd441458bef245b39828ed94ea6f4 \
-    --hash=sha256:15d62adfab7c6f4a491085f53f9634d24745ca5a2772549945b7e2de27c0d534 \
-    --hash=sha256:237db4ab0b90e5284ea7659264630d693273cdbda323a40368f320869bf6470f \
-    --hash=sha256:2db4d0d60a891a8b20a4c6de68a088efe73b29ab4a5949fe6aad2713c131e174 \
-    --hash=sha256:36d8cd43b3799e766158f1bb0b27cc4eef685fd892417b0382b7fdfdd94f1e6c \
-    --hash=sha256:39a3f3662391b49553bf9d9d2e9a6cb31e0d7d337557ee0c0be5c558a3c7d230 \
-    --hash=sha256:4591e0962c272d42d305ab3fb8889f13d47255e412fd3b9839620836662c91fe \
-    --hash=sha256:47aa28520fe274414b655c74cbe2e91d8b76e22f40cd41a758bb6975e526827b \
-    --hash=sha256:52641305461660c8969c6bb12364206a108c5c9e014c9220c70b99c4f48b6750 \
-    --hash=sha256:54e8771e31ee1deb01feef2475c12123cab770c371ecc97af98eb6ca10a2858e \
-    --hash=sha256:62331ee3871f6881f517ca65ae185fb2462a0bf2fe78acc4a4d621fc4da08396 \
-    --hash=sha256:65e76b20099c33352d5e7734a219982858873cf66fe510951d9bd27cb690190f \
-    --hash=sha256:66e160f496ac79248feb09a0acf4aab5d139d823330cbd9377f6e19ae007330a \
-    --hash=sha256:670b5c4d78c9c2d25e7ba650d212d98bf24d40292f91fe4e2f3ad4f80dc6d7e5 \
-    --hash=sha256:7333896544a4d0a3d708bd092f8c05eb3599dc2b34ae6e4c4b44d04d5514b0ec \
-    --hash=sha256:78c84ecf19459571784fd6a8ad8b3e9006cf96c3282e8220bc49098866ef4cc7 \
-    --hash=sha256:85be33bb04e918833ac6f28f68f83a1e83425eb6e08b9c482cc3318820dfd55f \
-    --hash=sha256:87b852d2005f1d59399ca51c5f3538f28a4742d739d7abe82b7ae8d01d8a5d02 \
-    --hash=sha256:8fae9609d972f0c2b72017796a8140b8a6fb842426f0aed4f43f0fa7d780a16f \
-    --hash=sha256:927f294b1dc7cea9372ef8c7c46ebeb5c7e6c1c7345358f952e7499bdbdf7eb4 \
-    --hash=sha256:999fed45cb391126107b804be0e344e75556fceaee4cc30a0ca06d77309bdf3c \
-    --hash=sha256:9cae9a6b9bb54f3f89424fdd960b60ac53239b9e5d4a5d9a598d222fbf8d3173 \
-    --hash=sha256:9e9a43ea42b8a9f2c62ca50ce05582de7b4f1f7eb27091f904578c29124af246 \
-    --hash=sha256:a5b3895ea12c4e636dfaacf75fa5bd1e8450b2ffb97507520991eaf1989d102e \
-    --hash=sha256:a999e35628988ad4f81af36192cd592b8fd1e72e1bbc76a64d80808e6f4b9540 \
-    --hash=sha256:b04b88be594dad81b33f6770283eed2125763632515c5112f8aa30f259cd334c \
-    --hash=sha256:b7d1f35218549762e52a782c0b548e0681332beee773d3dfffe2efc38b2ee960 \
-    --hash=sha256:c585e7a94bb723a70b4966677b882be8bda324cc41bd129765e3ceab428889bb \
-    --hash=sha256:c938eb7130067ca3b74b248ee376228776d8f013a206ae78e6fc644c9db0f4f5 \
-    --hash=sha256:cbfd6892fa092cbd6f52edcb24797af62fba8baa50995db856b0a342184c850d \
-    --hash=sha256:d4da8d58064f0a3dd07bfc283ba912b9d5a4cb38f1c0fcd9ecb2b9d43111243c \
-    --hash=sha256:e2309b9cafba799e9d343fdfdd5ae46276adf3929fef60f296f23b97ed1aa2f6 \
-    --hash=sha256:ffc2b6beb212d0d231816dcb7bd8bcdafccd04750ba8f5e915f40ad312f5adf2
+dbus-fast==2.21.2 \
+    --hash=sha256:044eec5d0668d3229480094f5b2aefafb336afa6976d686bd0cd8770eee1bb2c \
+    --hash=sha256:0b78f2116fb745a7623c8e18d9c435bfe4732e4f9284a923c4b9a44ef68ae2d4 \
+    --hash=sha256:194899057b8382c1902c32e1a565a2d47bcc99e06aafe9d660348394532a4bf6 \
+    --hash=sha256:29f07ef89e35b93afa87dea86abec2aff68802572944485250f50def15dc5ef8 \
+    --hash=sha256:2fd1be6967a92957f517dbd3755ee7cddc128ec840af2ef4ad6fb023a0dac74d \
+    --hash=sha256:32efcbe276a4fdf6946450c512355e7ae22836cf3595d48c59330687cda52117 \
+    --hash=sha256:37e6f717dedc299fc15ab8f5ec5b180725d2b896ba1aaef07c1921df0b7113a0 \
+    --hash=sha256:38138fc5a24797cc443c6894d25497271ccf3399c8aa8cdba228a7bdda2d2921 \
+    --hash=sha256:3b96a645cbd035f47f3b934130cd0ae977c043480ad7fe9838f78fdcb480c189 \
+    --hash=sha256:40aa9068759bbf7e062f074c965b391b95f18f897cc9be6eb906ee48a6f77724 \
+    --hash=sha256:51279b69ac6b872208f3aa1b00b910dd9ef9c3d625b79eb378405dbd72a29cab \
+    --hash=sha256:601c3c8796e7edd23bce0432e44ca8f0b85c48a17ab5258f57cd8fe815f9c07a \
+    --hash=sha256:60d989030403cc1611105bec6a90df22967e523ae28486dee5f9bd644e37f797 \
+    --hash=sha256:6c6f1fda6f318061a023d6da96ee50ad2d30c04557012a60a0f1abd39c2a8704 \
+    --hash=sha256:6edec4f92d32b9a288b38457a114086a0d5f5fdec9c3e9b7ff6052fd45963c1d \
+    --hash=sha256:6f056f2bfee24e87a4184202d3b108a56176344303bb1278988f13f5e90777da \
+    --hash=sha256:81ac390d4e26711b3ac46b3dd81a29bcbc1eddd4a408b336c67f0c94eb6d7ff0 \
+    --hash=sha256:8645187b2e86c5141217adcb462d6dbecd37fb2ab8705f66b3773a66206ef83d \
+    --hash=sha256:886ce5750d4e64636bd933f22513e9ba06b7ee9650f28699c553c162b52db666 \
+    --hash=sha256:90f09498ac91f0e6ddc7fa569e851a2b258a70917cd07ae8412ad5725ef1d411 \
+    --hash=sha256:9ba884d102e069e105f22986fccf1d21776e6ced11f4b75aeddcc37e728a80fd \
+    --hash=sha256:a3159f1cecd4b86f565c01da787ad6eaa57e8ba210d355836fa849e4c0b1ee57 \
+    --hash=sha256:aabe539f0e9961a1beb6e8c0078112a1a60de18958335678edb3f26021951ff9 \
+    --hash=sha256:afde99d085a330e8aed59535d808636f1f563cb08d12900d0e415508e6270a1d \
+    --hash=sha256:b17f1eafeaa825e8933a5394157db9e0a24e65eac188a244dbbbc01dc23fde7a \
+    --hash=sha256:b5e2015a385f0b364eff1827b151313429d3148d2718d679bec8a9c67b78721a \
+    --hash=sha256:b5f79edcb0dd48e98b1a1e3e4a655fd0ecc2ba72275f9e8379e8655b4411edcc \
+    --hash=sha256:bc696304ce0f5da374ddfb3e83273e9d89602a8f20e7fab57b079378f2cb5789 \
+    --hash=sha256:c2bb0fd813bf3cafc6796d86d42cc8a9d37c2633d973dd963c3ad4c080d7061d \
+    --hash=sha256:d2406b838ccbda9bd49dda4a7620ce228da306cd8f9a3f8c9f42b2d792a491fb \
+    --hash=sha256:d9f4191f7108f9433e5c017915e60ec57231aaf58c82fde6e20bd497998ebc97 \
+    --hash=sha256:eade5ed18327bf306b75e525ded98c08921e1b21d42e715b7f0a1371a7669168 \
+    --hash=sha256:ed431895630135da9cec736326304f0833ac31919043efdbecf8f6c7bed40d05 \
+    --hash=sha256:f5db0737471e60228c1a6aabecbf883c972f0b9e50bf7fc0878a8b35ebdf1d1e
     # via bleak
-frozendict==2.4.2 \
-    --hash=sha256:07153e6d2720fa1131bb180ce388c7042affb29561d8bcd1c0d6e683a8beaea2 \
-    --hash=sha256:1412aeb325e4a28cfe32106c66c046372bb7fd5a9af1748193549c5d01a9e9c1 \
-    --hash=sha256:146129502cd9d96de64e0c8f7dc4c66422da3d4bfccf891dd80a3821b358a926 \
-    --hash=sha256:19743495b1e92a7e4db56fcd6a5d36ea1d1b0f550822d6fd780e44d58f0b8c18 \
-    --hash=sha256:19e64630e164a297f83e9a1c69f1cd36fa4b3d1196c1f9fc006a0385aa198ea4 \
-    --hash=sha256:20a6f741c92fdeb3766924cde42b8ee445cf568e3be8aa983cb83e9fe5b61e63 \
-    --hash=sha256:34704f9ffb21448d4b5c0f9239f8f058c0efab4bfdbe2956c5be978fef0b929c \
-    --hash=sha256:3fc6e3158107b5431255978b954758b1041cc70a3b8e7657373110512eb528e3 \
-    --hash=sha256:476e4857e1d87b05c9102dd5409216ce4716cb7df619e6657429bc99279303cc \
-    --hash=sha256:4a5841681e70d2862ca153543f2912e0bab034bf29e2d3610e86ea42506121c2 \
-    --hash=sha256:4a8b298f39242d25770d029588ce9d4f524e9f4edc60d2d34b6178fb07c8a93e \
-    --hash=sha256:4ca09a376114172e4d9918e6d576f58244c45e21f5af1245085699fd3a171c47 \
-    --hash=sha256:4db1d6cc412bd865cab36723995208b82166a97bc6c724753bcd2b90cf24f164 \
-    --hash=sha256:5280d685cd1659883a3010dec843afe3065416ae92e453498997d4474a898a39 \
-    --hash=sha256:55953aa2acf5bf183c664f3d0f540f8c8ac8f5fa97170f2098d413414318eb2b \
-    --hash=sha256:741779e1d1a2e6bb2c623f78423bd5d14aad35dc0c57e6ccc89e54eaab5f1b8a \
-    --hash=sha256:79e1c94ad2a925ad5723d82a4134c6d851d5a7bc72b7e9da8b2087c42758a512 \
-    --hash=sha256:7a8d2ea4f10505ad15f53ce3742420682d916d0c4d566edb8e1019756e7cea30 \
-    --hash=sha256:7d13ffe649e9db6f4bb5e107d9be7dfd23e13101bc69f97aa5fa6cbf6aecaadd \
-    --hash=sha256:81efb4ea854a1c93d954a67389eaf78c508acb2d4768321a835cda2754ec5c01 \
-    --hash=sha256:83cc9d063131fd8adbeb18a473d222b5dc8301cac9505cfe578158f9a9bf55a9 \
-    --hash=sha256:84c36bfa819cd8442f6e0bdb86413c7678b2822a46b1a22cfa0f0dd30d9e5c45 \
-    --hash=sha256:92c46b155ea9eb9ecabc66ba2d9030f2634319f55c6448688965ece094f14b51 \
-    --hash=sha256:9ac1f74ccf818977abbc1868090c06436b8f06534d306f808f15cffc304ae046 \
-    --hash=sha256:ac954be447a907face9b652207fbd943b9b552212890db959ba653e8f1dc3f56 \
-    --hash=sha256:bedb0a6587bae53bd53727b92a87c4cf90ad7a7e0bd2db562d439beb6982712e \
-    --hash=sha256:c157b8a92743a7905b341edb0663044fecdc7780f96c59a2843d3da68d694b90 \
-    --hash=sha256:c5f1a4d9662b854dce52b560b60f51349905dc871826b8c6be20141a13067a53 \
-    --hash=sha256:cbab325c0a98b2f3ee291b36710623781b4977a3057f9103a7b0f11bcc23b177 \
-    --hash=sha256:cead3bfe70c90c634a9b76807c9d7e75e6c5666ec96fa2cea8e7412ccf22a1f8 \
-    --hash=sha256:d4a10119f17552cbeab48d4ae830ba091c6d47616589618adc31f251184579a7 \
-    --hash=sha256:f7a90ea6d5248617a1222daef07d22fb146ff07635a36db327e1ce114bf3e304 \
-    --hash=sha256:f7ce0535f02eba9746e4e2cf0abef0f0f2051d20fdccf4af31bc3d1adecf5a71 \
-    --hash=sha256:f7e0ff5e84742604a1b42c2de4f1e67630c0868cf52a5c585b54a99e06f6b453 \
-    --hash=sha256:f958d40637e0440bce2453019821c94fe86cfc5f3847ae11cd4f02c3548b1d1b \
-    --hash=sha256:ff6fb5831539fffb09d71cc0cc0462b1f27c0160cb6c6fa2d1f4c1bc7fffe52a
+frozendict==2.4.4 \
+    --hash=sha256:07c3a5dee8bbb84cba770e273cdbf2c87c8e035903af8f781292d72583416801 \
+    --hash=sha256:12a342e439aef28ccec533f0253ea53d75fe9102bd6ea928ff530e76eac38906 \
+    --hash=sha256:1697793b5f62b416c0fc1d94638ec91ed3aa4ab277f6affa3a95216ecb3af170 \
+    --hash=sha256:199a4d32194f3afed6258de7e317054155bc9519252b568d9cfffde7e4d834e5 \
+    --hash=sha256:259528ba6b56fa051bc996f1c4d8b57e30d6dd3bc2f27441891b04babc4b5e73 \
+    --hash=sha256:2b70b431e3a72d410a2cdf1497b3aba2f553635e0c0f657ce311d841bf8273b6 \
+    --hash=sha256:2bd009cf4fc47972838a91e9b83654dc9a095dc4f2bb3a37c3f3124c8a364543 \
+    --hash=sha256:2d8536e068d6bf281f23fa835ac07747fb0f8851879dd189e9709f9567408b4d \
+    --hash=sha256:3148062675536724502c6344d7c485dd4667fdf7980ca9bd05e338ccc0c4471e \
+    --hash=sha256:3f7c031b26e4ee6a3f786ceb5e3abf1181c4ade92dce1f847da26ea2c96008c7 \
+    --hash=sha256:4297d694eb600efa429769125a6f910ec02b85606f22f178bafbee309e7d3ec7 \
+    --hash=sha256:4a59578d47b3949437519b5c39a016a6116b9e787bb19289e333faae81462e59 \
+    --hash=sha256:4ae8d05c8d0b6134bfb6bfb369d5fa0c4df21eabb5ca7f645af95fdc6689678e \
+    --hash=sha256:5d58d9a8d9e49662c6dafbea5e641f97decdb3d6ccd76e55e79818415362ba25 \
+    --hash=sha256:63aa49f1919af7d45fb8fd5dec4c0859bc09f46880bd6297c79bb2db2969b63d \
+    --hash=sha256:6874fec816b37b6eb5795b00e0574cba261bf59723e2de607a195d5edaff0786 \
+    --hash=sha256:6eb716e6a6d693c03b1d53280a1947716129f5ef9bcdd061db5c17dea44b80fe \
+    --hash=sha256:78c94991944dd33c5376f720228e5b252ee67faf3bac50ef381adc9e51e90d9d \
+    --hash=sha256:7f79c26dff10ce11dad3b3627c89bb2e87b9dd5958c2b24325f16a23019b8b94 \
+    --hash=sha256:7fee9420475bb6ff357000092aa9990c2f6182b2bab15764330f4ad7de2eae49 \
+    --hash=sha256:812ab17522ba13637826e65454115a914c2da538356e85f43ecea069813e4b33 \
+    --hash=sha256:85375ec6e979e6373bffb4f54576a68bf7497c350861d20686ccae38aab69c0a \
+    --hash=sha256:87ebcde21565a14fe039672c25550060d6f6d88cf1f339beac094c3b10004eb0 \
+    --hash=sha256:93a7b19afb429cbf99d56faf436b45ef2fa8fe9aca89c49eb1610c3bd85f1760 \
+    --hash=sha256:b3b967d5065872e27b06f785a80c0ed0a45d1f7c9b85223da05358e734d858ca \
+    --hash=sha256:c6bf9260018d653f3cab9bd147bd8592bf98a5c6e338be0491ced3c196c034a3 \
+    --hash=sha256:c8f92425686323a950337da4b75b4c17a3327b831df8c881df24038d560640d4 \
+    --hash=sha256:d13b4310db337f4d2103867c5a05090b22bc4d50ca842093779ef541ea9c9eea \
+    --hash=sha256:dc2228874eacae390e63fd4f2bb513b3144066a977dc192163c9f6c7f6de6474 \
+    --hash=sha256:e1b941132d79ce72d562a13341d38fc217bc1ee24d8c35a20d754e79ff99e038 \
+    --hash=sha256:fefeb700bc7eb8b4c2dc48704e4221860d254c8989fb53488540bc44e44a1ac2
     # via ha-services
 ha-services==2.6.0 \
     --hash=sha256:55468ad8454e0b87a1f0ec5b934b1c98d864a1ae200faf4bdc3efd5c8c61c963 \
     --hash=sha256:d6887bdfda0a014ca4cf77fa08897604db0692d680fe1a7cc7c72644fdd288db
     # via tc66c2mqtt (pyproject.toml)
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
@@ -156,17 +151,17 @@
     --hash=sha256:fd62e5818731a66aaa8e9b0a1e5543dc979a46278da01e85c3c9a1a4f047ef7e \
     --hash=sha256:fda4c357145cf0b760000c4ad597e19b53adf01382b711f281720a10a0fe72b7
     # via ha-services
 packaging==24.0 \
     --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
     --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
     # via cli-base-utilities
-paho-mqtt==2.0.0 \
-    --hash=sha256:13b205f29251e4f2c66a6c923c31fc4fd780561e03b2d775cff8e4f2915cf947 \
-    --hash=sha256:2ef745073dfc9aa68bfec30d0b9b6f0304ea75182bae85a7c77a80cefce1eff5
+paho-mqtt==2.1.0 \
+    --hash=sha256:12d6e7511d4137555a3f6ea167ae846af2c7357b10bc6fa4f7c3968fc1723834 \
+    --hash=sha256:6db9ba9b34ed5bc6b6e3812718c7e06e2fd7444540df2455d2c51bd58808feee
     # via ha-services
 psutil==5.9.8 \
     --hash=sha256:02615ed8c5ea222323408ceba16c60e99c3f91639b07da6373fb7e6539abc56d \
     --hash=sha256:05806de88103b25903dff19bb6692bd2e714ccf9e668d050d144012055cbca73 \
     --hash=sha256:26bd09967ae00920df88e0352a91cff1a78f8d69b3ecabbfe733610c0af486c8 \
     --hash=sha256:27cc40c3493bb10de1be4b3f07cae4c010ce715290a5be22b98493509c6299e2 \
     --hash=sha256:36f435891adb138ed3c9e58c6af3e2e6ca9ac2f365efe1f9cfef2794e6c93b4e \
@@ -212,40 +207,40 @@
     --hash=sha256:ec0bb1188c1d13426039af8ffcb4dbe3aad1d7680c35a62d8eaf2a529b5d3d4f \
     --hash=sha256:ec1f93feb3bb93380ab0ebf8b859e8e5678c0f010d2d78367cf6bc30bfeb148e \
     --hash=sha256:f0e6d631bae3f231d3634f91ae4da7a960f7ff87f2865b2d2b831af1dfb04e9a \
     --hash=sha256:f35d6cee81fa145333137009d9c8ba90951d7d77b67c79cbe5f03c7eb74d8fe2 \
     --hash=sha256:f47888542a0633baff535a04726948e876bf1ed880fddb7c10a736fa99146ab3 \
     --hash=sha256:fb3b87461fa35afa19c971b0a2b7456a7b1db7b4eba9a8424666104925b78128
     # via tc66c2mqtt (pyproject.toml)
-pygments==2.17.2 \
-    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
-    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
+pygments==2.18.0 \
+    --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
+    --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
     # via rich
 rich==13.7.1 \
     --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
     --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
     # via
     #   cli-base-utilities
     #   ha-services
     #   rich-click
     #   tc66c2mqtt (pyproject.toml)
-rich-click==1.7.4 \
-    --hash=sha256:7ce5de8e4dc0333aec946113529b3eeb349f2e5d2fafee96b9edf8ee36a01395 \
-    --hash=sha256:e363655475c60fec5a3e16a1eb618118ed79e666c365a36006b107c17c93ac4e
+rich-click==1.8.2 \
+    --hash=sha256:8e29bdede858b59aa2859a1ab1c4ccbd39ed7ed5870262dae756fba6b5dc72e8 \
+    --hash=sha256:b57856f304e4fe0394b82d7ce0784450758f8c8b4e201ccc4320501cc201806b
     # via
     #   cli-base-utilities
     #   ha-services
     #   tc66c2mqtt (pyproject.toml)
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via cli-base-utilities
-tomlkit==0.12.4 \
-    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
-    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
+tomlkit==0.12.5 \
+    --hash=sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f \
+    --hash=sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c
     # via
     #   cli-base-utilities
     #   ha-services
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
```

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/__init__.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/__init__.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/scan.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/scan.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/settings.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,19 @@
 
 import rich_click as click
 from cli_base.cli_tools.verbosity import OPTION_KWARGS_VERBOSE, setup_logging
 from cli_base.toml_settings.api import TomlSettings
 from rich import print  # noqa
 
 from tc66c2mqtt.cli_app import cli
-from tc66c2mqtt.user_settings import UserSettings
-
+from tc66c2mqtt.user_settings import get_toml_settings
 
 logger = logging.getLogger(__name__)
 
 
-def get_toml_settings() -> TomlSettings:
-    return TomlSettings(
-        dir_name='tc66c2mqtt',
-        file_name='tc66c2mqtt',
-        settings_dataclass=UserSettings(),
-    )
-
-
-def get_user_settings(verbosity: int) -> UserSettings:
-    toml_settings: TomlSettings = get_toml_settings()
-    user_settings: UserSettings = toml_settings.get_user_settings(debug=verbosity > 0)
-    return user_settings
-
-
 @cli.command()
 @click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
 def edit_settings(verbosity: int):
     """
     Edit the settings file. On first call: Create the default one.
     """
     setup_logging(verbosity=verbosity)
```

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/systemd.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/systemd.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import rich_click as click
 from cli_base.cli_tools.verbosity import OPTION_KWARGS_VERBOSE, setup_logging
 from cli_base.systemd.api import ServiceControl
 from rich import print  # noqa
 
 from tc66c2mqtt.cli_app import cli
-from tc66c2mqtt.cli_app.settings import get_user_settings
-from tc66c2mqtt.user_settings import SystemdServiceInfo, UserSettings
+from tc66c2mqtt.user_settings import SystemdServiceInfo, UserSettings, get_user_settings
 
 
 logger = logging.getLogger(__name__)
 
 
 def get_systemd_settings(verbosity: int) -> SystemdServiceInfo:
     user_settings: UserSettings = get_user_settings(verbosity=verbosity)
```

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_app/update_readme_history.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_app/update_readme_history.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/__init__.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/__init__.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/code_style.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/code_style.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/packaging.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/packaging.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/cli_dev/testing.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/cli_dev/testing.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/data_classes.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/data_classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     group0Ah: float  # in Ampere-hours
     group0Wh: float  # in Watt-hours
     group1Ah: float  # in Ampere-hours
     group1Wh: float  # in Watt-hours
     #
     temperature: int  # in Celsius
     #
-    dataPlus: float  # in Volts
-    dataMinus: float  # in Volts
+    data_plus: float  # in Volts
+    data_minus: float  # in Volts
```

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tc66.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/tc66.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 
     number_of_runs = int.from_bytes(pac1[44:48], 'little')
 
     voltage = float(int.from_bytes(pac1[48:52], 'little')) / 10_000
     current = float(int.from_bytes(pac1[52:56], 'little')) / 100_000
     power = float(int.from_bytes(pac1[56:60], 'little')) / 10_000
 
+    # Compare V * A = W ;)
+    power_calc = voltage * current
+    diff = abs(power - power_calc)
+    if diff > 0.0002:
+        logger.warning(f'Power calculation diff: {power=}, {power_calc=} ({diff=})')
+
     # CRC16: pac1[60:64]
 
     pac2 = data[64:128]
     logging.debug(f'{pac2=}')
     pac2prefix = pac2[:4]
     if pac2prefix != b'pac2':
         logger.error(f'Invalid prefix {pac2prefix=}')
@@ -44,16 +50,16 @@
     group1Wh = float(int.from_bytes(pac2[20:24], 'little')) / 1_000
 
     temperature_sign = int.from_bytes(pac2[24:28], 'little')
     temperature = int.from_bytes(pac2[28:32], 'little')
     if temperature_sign:
         temperature = -temperature
 
-    dataPlus = float(int.from_bytes(pac2[32:36], 'little')) / 100
-    dataMinus = float(int.from_bytes(pac2[36:40], 'little')) / 100
+    data_plus = float(int.from_bytes(pac2[32:36], 'little')) / 100
+    data_minus = float(int.from_bytes(pac2[36:40], 'little')) / 100
 
     # pac2[40:60] contains unknown data -> ignore
     # CRC16: pac2[60:64]
     # pac3 = data[128:192] -> All data are unknown
     pac3: bytes = data[128:192]
     logging.debug(f'{pac3=}')
     pac3prefix = pac3[:4]
@@ -76,10 +82,10 @@
         group0Ah=group0Ah,
         group0Wh=group0Wh,
         group1Ah=group1Ah,
         group1Wh=group1Wh,
         #
         temperature=temperature,
         #
-        dataPlus=dataPlus,
-        dataMinus=dataMinus,
+        data_plus=data_plus,
+        data_minus=data_minus,
     )
```

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tc66_decryptor.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/tc66_decryptor.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/__init__.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/fixtures.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt/tests/test_project_setup.py` & `tc66c2mqtt-0.1.0/tc66c2mqtt/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/PKG-INFO` & `tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc66c2mqtt
-Version: 0.0.1rc0
+Version: 0.1.0
 Summary: Sen MQTT events from TC66C device
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/tc66c2mqtt
 Project-URL: Source, https://github.com/jedie/tc66c2mqtt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -42,17 +42,20 @@
 [![codecov](https://codecov.io/github/jedie/tc66c2mqtt/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/tc66c2mqtt)
 [![tc66c2mqtt @ PyPi](https://img.shields.io/pypi/v/tc66c2mqtt?label=tc66c2mqtt%20%40%20PyPi)](https://pypi.org/project/tc66c2mqtt/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/tc66c2mqtt)](https://github.com/jedie/tc66c2mqtt/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/tc66c2mqtt)](https://github.com/jedie/tc66c2mqtt/blob/main/LICENSE)
 
 Send MQTT events from RDTech TC66C device
 
-**under development and not really useable, yet!**
+**under heavy development**
 
 
 Tested with [Joy-IT TC66C](https://joy-it.net/de/products/JT-TC66C).
 
 
 RDTech TC66C hardware info at sigrok:
 
  * https://sigrok.org/wiki/RDTech_TC66C
 
+test print data in terminal looks like:
+
+![2024-05-07_20-08_print_data.png](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/tc66c2mqtt/2024-05-07_20-08_print_data.png "2024-05-07_20-08_print_data.png")
```

### Comparing `tc66c2mqtt-0.0.1rc0/tc66c2mqtt.egg-info/SOURCES.txt` & `tc66c2mqtt-0.1.0/tc66c2mqtt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 requirements.txt
 tc66.dat
 .github/workflows/tests.yml
 tc66c2mqtt/__init__.py
 tc66c2mqtt/__main__.py
 tc66c2mqtt/constants.py
 tc66c2mqtt/data_classes.py
+tc66c2mqtt/mqtt_handler.py
 tc66c2mqtt/tc66.py
 tc66c2mqtt/tc66_decryptor.py
+tc66c2mqtt/tc66c_bluetooth.py
 tc66c2mqtt/user_settings.py
 tc66c2mqtt.egg-info/PKG-INFO
 tc66c2mqtt.egg-info/SOURCES.txt
 tc66c2mqtt.egg-info/dependency_links.txt
 tc66c2mqtt.egg-info/entry_points.txt
 tc66c2mqtt.egg-info/requires.txt
 tc66c2mqtt.egg-info/top_level.txt
 tc66c2mqtt/cli_app/__init__.py
 tc66c2mqtt/cli_app/print_data.py
+tc66c2mqtt/cli_app/publish.py
 tc66c2mqtt/cli_app/scan.py
 tc66c2mqtt/cli_app/settings.py
 tc66c2mqtt/cli_app/systemd.py
 tc66c2mqtt/cli_app/update_readme_history.py
 tc66c2mqtt/cli_dev/__init__.py
 tc66c2mqtt/cli_dev/code_style.py
 tc66c2mqtt/cli_dev/packaging.py
```

