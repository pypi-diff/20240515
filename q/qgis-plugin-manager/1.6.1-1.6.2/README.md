# Comparing `tmp/qgis-plugin-manager-1.6.1.tar.gz` & `tmp/qgis-plugin-manager-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgis-plugin-manager-1.6.1.tar", last modified: Thu Jul  6 12:10:26 2023, max compression
+gzip compressed data, was "qgis-plugin-manager-1.6.2.tar", last modified: Wed May 15 08:48:59 2024, max compression
```

## Comparing `qgis-plugin-manager-1.6.1.tar` & `qgis-plugin-manager-1.6.2.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (122)    10902 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9507 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/qgis_plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-07-06 12:10:24.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6664 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/definitions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11958 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (122)    18787 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10902 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-07-06 12:10:24.000000 qgis-plugin-manager-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/test/test_full_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/test/test_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/test/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:48:59.836010 qgis-plugin-manager-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-15 08:48:59.832010 qgis-plugin-manager-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-15 08:48:57.000000 qgis-plugin-manager-1.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:48:59.832010 qgis-plugin-manager-1.6.2/qgis_plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-15 08:48:57.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6653 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19417 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:48:59.832010 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:48:59.836010 qgis-plugin-manager-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-15 08:48:57.000000 qgis-plugin-manager-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:48:59.832010 qgis-plugin-manager-1.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/test/test_full_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/test/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/test/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/test/test_utils.py
```

### Comparing `qgis-plugin-manager-1.6.1/PKG-INFO` & `qgis-plugin-manager-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-manager
-Version: 1.6.1
+Version: 1.6.2
 Summary: Tool for downloading/managing QGIS plugins from CLI.
 Home-page: https://github.com/3liz/qgis-plugin-manager
-Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.1.tar.gz
+Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.2.tar.gz
 Author: Étienne Trimaille
 Author-email: etrimaille@3liz.com
 Project-URL: Docs, https://github.com/3liz/qgis-plugin-manager/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/3liz/qgis-plugin-manager/issues/
 Project-URL: Source, https://github.com/3liz/qgis-plugin-manager
 Keywords: QGIS
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,32 +18,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # QGIS-Plugin-Manager
 
 [![Tests](https://github.com/3liz/qgis-plugin-manager/actions/workflows/release.yml/badge.svg)](https://github.com/3liz/qgis-plugin-manager/actions/workflows/release.yml)
 [![PyPi version badge](https://badgen.net/pypi/v/qgis-plugin-manager)](https://pypi.org/project/qgis-plugin-manager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/qgis-plugin-manager)](https://pypi.org/project/qgis-plugin-manager/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qgis-plugin-manager)](https://pypi.org/project/qgis-plugin-manager/)
 
 Mainly designed for QGIS Server plugins, but it works also for desktop.
 
 Not tested on Windows.
 
-The **CLI** API is not stable yet.
-
 ## Installation
 
 Python 3.7 **minimum**, you can make a Python venv if needed.
 ```bash
 python3 --version
 ```
 
@@ -63,15 +63,15 @@
   Read [the documentation](README.md#notify-upstream-if-a-restart-is-needed).
 * `QGIS_PLUGINPATH` for storing plugins, from [QGIS Server documentation](https://docs.qgis.org/latest/en/docs/server_manual/config.html#environment-variables)
 * `PYTHONPATH` for importing QGIS libraries
 
 ## Utilisation
 
 **Either** you need to go in the directory where you are storing plugins, **or** you can use the environment variable `QGIS_PLUGINPATH`.
-You can read the [documentation](https://docs.qgis.org/3.22/en/docs/server_manual/config.html#environment-variables)
+You can read the [documentation](https://docs.qgis.org/latest/en/docs/server_manual/config.html#environment-variables)
 on QGIS Server about this variable.
 
 ```bash
 cd /path/where/you/have/plugins
 # usually on a server
 cd /usr/lib/qgis/plugins
 # on unix desktop with the default QGIS profile
@@ -105,26 +105,26 @@
 
 ### Init
 
 To create the first `sources.list` in the directory with at least the default repository https://plugins.qgis.org :
 ```bash
 $ qgis-plugin-manager init
 $ cat sources.list 
-https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19
+https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34
 ```
 
 You can have one or many servers, one on each line.
 
 ### List
 
 List all plugins installed :
 
 ```bash
 $ qgis-plugin-manager list
-QGIS server version 3.19.0
+QGIS server version 3.34.2
 List all plugins in /home/etienne/dev/qgis/server_plugin
 
 ------------------------------------------------------------------------------------------------------------------------------------
 |  Name            |  Version  | Flags           |  QGIS min  |  QGIS max  |  Author         | Folder owner     | Action ⚠         |
 ------------------------------------------------------------------------------------------------------------------------------------
 |Lizmap            |master     |                 |3.4         |3.99        |3Liz             | root : 0o755     | Unkown version   |
 |wfsOutputExtension|1.5.3      |Server           |3.0         |            |3Liz             | etienne : 0o755  |                  |
@@ -144,21 +144,21 @@
 
 ### Remote
 
 ```bash
 $ qgis-plugin-manager remote
 List of remotes :
 
-https://plugins.qgis.org/plugins/plugins.xml?qgis=3.22
+https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34
 
 $ cat sources.list 
 https://plugins.qgis.org/plugins/plugins.xml?qgis=[VERSION]
 ```
 
-`[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.22`.
+`[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.34`.
 If QGIS is upgraded, the XML file will be updated as well.
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
 #### Basic authentication
@@ -174,18 +174,18 @@
 
 ### Update
 
 To fetch the XML files from each repository :
 
 ```bash
 $ qgis-plugin-manager update
-Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19...
+Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34...
 	Ok
 $ ls .cache_qgis_plugin_manager/
-https-plugins-qgis-org-plugins-plugins-xml-qgis-3-19.xml
+https-plugins-qgis-org-plugins-plugins-xml-qgis-3-34.xml
 ```
 
 ### Cache
 
 Check if a plugin is available :
 
 ```bash
@@ -286,14 +286,16 @@
 ```
 
 ### Notify upstream if a restart is needed
 
 When a plugin is installed or removed and if the environment variable `QGIS_PLUGIN_MANAGER_RESTART_FILE` is set,
 an empty file will be created or touched. It can notify you if QGIS Server needs to be restarted for instance.
 
+This is useful for a deployment with [Ansible](https://www.ansible.com/) for instance.
+
 Note that you must manually remove this file.
 
 ## Run tests
 
 ```bash
 export PYTHONPATH=/home/etienne/dev/app/qgis-master/share/qgis/python/:/usr/lib/python3/dist-packages/
 cd test
```

### Comparing `qgis-plugin-manager-1.6.1/README.md` & `qgis-plugin-manager-1.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/qgis-plugin-manager)](https://pypi.org/project/qgis-plugin-manager/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qgis-plugin-manager)](https://pypi.org/project/qgis-plugin-manager/)
 
 Mainly designed for QGIS Server plugins, but it works also for desktop.
 
 Not tested on Windows.
 
-The **CLI** API is not stable yet.
-
 ## Installation
 
 Python 3.7 **minimum**, you can make a Python venv if needed.
 ```bash
 python3 --version
 ```
 
@@ -34,15 +32,15 @@
   Read [the documentation](README.md#notify-upstream-if-a-restart-is-needed).
 * `QGIS_PLUGINPATH` for storing plugins, from [QGIS Server documentation](https://docs.qgis.org/latest/en/docs/server_manual/config.html#environment-variables)
 * `PYTHONPATH` for importing QGIS libraries
 
 ## Utilisation
 
 **Either** you need to go in the directory where you are storing plugins, **or** you can use the environment variable `QGIS_PLUGINPATH`.
-You can read the [documentation](https://docs.qgis.org/3.22/en/docs/server_manual/config.html#environment-variables)
+You can read the [documentation](https://docs.qgis.org/latest/en/docs/server_manual/config.html#environment-variables)
 on QGIS Server about this variable.
 
 ```bash
 cd /path/where/you/have/plugins
 # usually on a server
 cd /usr/lib/qgis/plugins
 # on unix desktop with the default QGIS profile
@@ -76,26 +74,26 @@
 
 ### Init
 
 To create the first `sources.list` in the directory with at least the default repository https://plugins.qgis.org :
 ```bash
 $ qgis-plugin-manager init
 $ cat sources.list 
-https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19
+https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34
 ```
 
 You can have one or many servers, one on each line.
 
 ### List
 
 List all plugins installed :
 
 ```bash
 $ qgis-plugin-manager list
-QGIS server version 3.19.0
+QGIS server version 3.34.2
 List all plugins in /home/etienne/dev/qgis/server_plugin
 
 ------------------------------------------------------------------------------------------------------------------------------------
 |  Name            |  Version  | Flags           |  QGIS min  |  QGIS max  |  Author         | Folder owner     | Action ⚠         |
 ------------------------------------------------------------------------------------------------------------------------------------
 |Lizmap            |master     |                 |3.4         |3.99        |3Liz             | root : 0o755     | Unkown version   |
 |wfsOutputExtension|1.5.3      |Server           |3.0         |            |3Liz             | etienne : 0o755  |                  |
@@ -115,21 +113,21 @@
 
 ### Remote
 
 ```bash
 $ qgis-plugin-manager remote
 List of remotes :
 
-https://plugins.qgis.org/plugins/plugins.xml?qgis=3.22
+https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34
 
 $ cat sources.list 
 https://plugins.qgis.org/plugins/plugins.xml?qgis=[VERSION]
 ```
 
-`[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.22`.
+`[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.34`.
 If QGIS is upgraded, the XML file will be updated as well.
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
 #### Basic authentication
@@ -145,18 +143,18 @@
 
 ### Update
 
 To fetch the XML files from each repository :
 
 ```bash
 $ qgis-plugin-manager update
-Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19...
+Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34...
 	Ok
 $ ls .cache_qgis_plugin_manager/
-https-plugins-qgis-org-plugins-plugins-xml-qgis-3-19.xml
+https-plugins-qgis-org-plugins-plugins-xml-qgis-3-34.xml
 ```
 
 ### Cache
 
 Check if a plugin is available :
 
 ```bash
@@ -257,14 +255,16 @@
 ```
 
 ### Notify upstream if a restart is needed
 
 When a plugin is installed or removed and if the environment variable `QGIS_PLUGIN_MANAGER_RESTART_FILE` is set,
 an empty file will be created or touched. It can notify you if QGIS Server needs to be restarted for instance.
 
+This is useful for a deployment with [Ansible](https://www.ansible.com/) for instance.
+
 Note that you must manually remove this file.
 
 ## Run tests
 
 ```bash
 export PYTHONPATH=/home/etienne/dev/app/qgis-master/share/qgis/python/:/usr/lib/python3/dist-packages/
 cd test
```

### Comparing `qgis-plugin-manager-1.6.1/qgis_plugin_manager/__about__.py` & `qgis-plugin-manager-1.6.2/qgis_plugin_manager/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 __license__ = "GNU General Public License v3.0"
 __summary__ = "Tool for downloading/managing QGIS plugins from CLI."
 __title__ = "QGIS Plugin Manager"
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri__ = "https://github.com/3liz/qgis-plugin-manager"
 
 # This string might be updated on CI on runtime with a proper semantic version name with X.Y.Z
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 if "." not in __version__:
     # If __version__ is still not a proper semantic versioning with X.Y.Z
     # let's hardcode 0.0.0
     __version__ = "0.0.0"
 
 __version_info__ = tuple(
     [
         int(num) if num.isdigit() else num
         for num in __version__.replace("-", ".", 1).split(".")
-    ]
+    ],
 )
```

### Comparing `qgis-plugin-manager-1.6.1/qgis_plugin_manager/__main__.py` & `qgis-plugin-manager-1.6.2/qgis_plugin_manager/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 from qgis_plugin_manager.__about__ import __version__
 from qgis_plugin_manager.definitions import Level
 from qgis_plugin_manager.local_directory import LocalDirectory
 from qgis_plugin_manager.remote import Remote
 from qgis_plugin_manager.utils import qgis_server_version
 
 
-def main() -> int:  # noqa: C901
+def main() -> int:
     """ Main function for the CLI menu. """
     parser = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("-v", "--version", action="version", version=__version__)
 
     subparsers = parser.add_subparsers(
-        title="commands", description="qgis-plugin-manager command", dest="command"
+        title="commands", description="qgis-plugin-manager command", dest="command",
     )
 
     subparsers.add_parser("init", help="Create the `sources.list` with plugins.qgis.org as remote")
 
     subparsers.add_parser("list", help="List all plugins in the directory")
 
     subparsers.add_parser("remote", help="List all remote server")
@@ -163,15 +163,15 @@
                 plugin_object = plugins.plugin_info(folder)
 
                 if plugin_object.name in ignored_plugins:
                     print(
                         f"{Level.Alert}"
                         f"Plugin {plugin_object.name} skipped from the upgrade command, because the plugin "
                         f"is in the ignored list."
-                        f"{Level.End}"
+                        f"{Level.End}",
                     )
                     continue
 
                 # Need to check version
                 result = remote.install(
                     plugin_name=plugin_object.name,
                     current_version=plugin_object.version,
```

### Comparing `qgis-plugin-manager-1.6.1/qgis_plugin_manager/definitions.py` & `qgis-plugin-manager-1.6.2/qgis_plugin_manager/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import NamedTuple
+from typing import List, NamedTuple
 
 __copyright__ = 'Copyright 2021, 3Liz'
 __license__ = 'GPL version 3'
 __email__ = 'info@3liz.org'
 
 
 class Plugin(NamedTuple):
     """ Definition of a plugin in the XML file. """
     name: str = None
     description: str = None
     version: str = None
-    search: list = []
+    search: List = None
     qgis_minimum_version: str = None
     qgis_maximum_version: str = None
     homepage: str = None
     pre_release: str = None
     file_name: str = None
     icon: str = None
     author_name: str = None
```

### Comparing `qgis-plugin-manager-1.6.1/qgis_plugin_manager/local_directory.py` & `qgis-plugin-manager-1.6.2/qgis_plugin_manager/local_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import configparser
 import os
 import shutil
 import stat
 
 from pathlib import Path
-from typing import Dict, Union
+from typing import Dict, Optional, Union
 
 from qgis_plugin_manager.definitions import Level, Plugin
 from qgis_plugin_manager.remote import Remote
 from qgis_plugin_manager.utils import (
     DEFAULT_QGIS_VERSION,
     parse_version,
     pretty_table,
@@ -21,15 +21,15 @@
     sources_file,
     to_bool,
 )
 
 
 class LocalDirectory:
 
-    def __init__(self, folder: Path, qgis_version: str = None):
+    def __init__(self, folder: Path, qgis_version: Optional[str] = None):
         """ Constructor"""
         self.folder = folder
         # Dictionary : folder : plugin name
         self._plugins = None
         self._invalid = []
 
         self.qgis_version_str = qgis_version
@@ -51,15 +51,15 @@
         if self.qgis_version:
             version = "[VERSION]"
             print("Init https://plugins.qgis.org")
         else:
             print(
                 f"{Level.Alert}"
                 f"QGIS version is unknown, creating with a default {DEFAULT_QGIS_VERSION}"
-                f"{Level.End}"
+                f"{Level.End}",
             )
             version = DEFAULT_QGIS_VERSION
 
         server = f"https://plugins.qgis.org/plugins/plugins.xml?qgis={version}\n"
 
         try:
             with open(source_file, 'w', encoding='utf8') as f:
@@ -148,15 +148,15 @@
                 plugin_folder, "server") in ('True', 'true', '1', 'yes', True),
             has_processing=self.plugin_metadata(
                 plugin_folder, "hasProcessingProvider") in ('True', 'true', '1', 'yes', True),
             has_wps=self.plugin_metadata(plugin_folder, "wps") in ('True', 'true', '1', 'yes', True),
         )
         return data
 
-    def plugin_installed_version(self, plugin_name) -> Union[str, None]:
+    def plugin_installed_version(self, plugin_name: str) -> Union[str, None]:
         """ If a plugin is installed or not. """
         if self._plugins is None:
             self.plugin_list()
 
         for plugin_folder in self.plugin_list():
             info = self.plugin_info(plugin_folder)
             if info.name == plugin_name:
@@ -178,38 +178,38 @@
             all_names.append(info.name)
 
             if info.name == plugin_name:
                 plugin_path = self.folder.joinpath(plugin_folder)
                 try:
                     shutil.rmtree(plugin_path)
                 except Exception as e:
-                    print(f"{Level.Critical}Plugin {plugin_name} could not be removed : {str(e)}")
+                    print(f"{Level.Critical}Plugin {plugin_name} could not be removed : {e!s}")
 
                 if not Path(self.folder.joinpath(plugin_folder)).exists():
                     print(f"{Level.Success}Plugin {plugin_name} removed")
                     restart_qgis_server()
                     return True
                 else:
                     print(
                         f"{Level.Alert}"
                         f"Plugin {plugin_name} using folder {plugin_folder} could not be removed "
                         f"for unknown reason"
-                        f"{Level.End}"
+                        f"{Level.End}",
                     )
                 break
         print(f"{Level.Alert}Plugin name '{plugin_name}' not found{Level.End}")
 
         all_names = list(set(all_names))
         similarity = similar_names(plugin_name.lower(), all_names)
         for plugin in similarity:
             print(f"Do you mean maybe '{plugin}' ?")
 
         return False
 
-    def print_table(self, current_directory: bool = True):  # noqa: C901
+    def print_table(self, current_directory: bool = True):
         """ Print all plugins installed as a table. """
         if self._plugins is None:
             self.plugin_list()
 
         remote = Remote(self.folder, qgis_version=self.qgis_version_str)
 
         if current_directory:
@@ -318,21 +318,21 @@
             plugin_data.append(Level.Alert + ';'.join(extra_info) + Level.End)
             data.append(plugin_data)
 
         if len(data):
             print(pretty_table(data, headers))
         else:
             print(
-                f"{Level.Alert}No plugin found in the current directory {self.folder.absolute()}{Level.End}"
+                f"{Level.Alert}No plugin found in the current directory {self.folder.absolute()}{Level.End}",
             )
 
         if len(list_of_owners) > 1:
             list_of_owners = [f"'{i}'" for i in list_of_owners]
             print(
                 f"{Level.Alert}"
                 f"Different rights have been detected : {','.join(list_of_owners)}"
                 f"{Level.End}. "
-                f"Please check user-rights."
+                f"Please check user-rights.",
             )
 
         if len(self._invalid) >= 1:
             print(pretty_table(self._invalid, ['Invalid']))
```

### Comparing `qgis-plugin-manager-1.6.1/qgis_plugin_manager/remote.py` & `qgis-plugin-manager-1.6.2/qgis_plugin_manager/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 __copyright__ = 'Copyright 2022, 3Liz'
 __license__ = 'GPL version 3'
 __email__ = 'info@3liz.org'
 
 import base64
 import os
+import platform
 import re
 import shutil
 import urllib
 import urllib.request
 import zipfile
 
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union
-from urllib.parse import unquote, urlencode, urlparse, urlunparse, parse_qs
+from typing import Dict, Iterator, List, Optional, Tuple, Union
+from urllib.parse import parse_qs, unquote, urlencode, urlparse, urlunparse
 from xml.etree.ElementTree import parse
 
 from qgis_plugin_manager.definitions import Level, Plugin
 from qgis_plugin_manager.utils import (
+    DEFAULT_QGIS_VERSION,
     current_user,
     restart_qgis_server,
     similar_names,
     sources_file,
     to_bool,
 )
 
 
 class Remote:
 
-    def __init__(self, folder: Path, qgis_version: str = None):
+    def __init__(self, folder: Path, qgis_version: Optional[str] = None):
         """ Constructor. """
         self.folder = folder
         self.list = None
         self.list_plugins = None
         self.setting_error = False
         self.qgis_version = qgis_version
 
+    def user_agent(self) -> str:
+        """ User agent. """
+        # https://github.com/3liz/qgis-plugin-manager/issues/66
+        # https://lists.osgeo.org/pipermail/qgis-user/2024-May/054439.html
+        if not self.qgis_version:
+            qgis_version = f"{DEFAULT_QGIS_VERSION}00"
+        else:
+            qgis_version = self.qgis_version
+
+        qgis_version = qgis_version.replace(".", "")
+        return f"Mozilla/5.0 QGIS/{qgis_version}/{platform.system()}"
+
     def remote_is_ready(self) -> bool:
         """ Return if the remote is ready to be parsed. """
         if to_bool(os.getenv("QGIS_PLUGIN_MANAGER_SKIP_SOURCES_FILE"), False):
             return True
 
         source_list = sources_file(self.folder)
         if not source_list.exists():
@@ -57,15 +71,15 @@
 
             if not filename.exists():
                 if not self.setting_error:
                     print(
                         f"{Level.Critical}"
                         f"The 'update' command has not been done before. "
                         f"The repository {server} has not been fetched before."
-                        f"{Level.End}"
+                        f"{Level.End}",
                     )
                     self.setting_error = True
                     return False
 
         return True
 
     def remote_list(self) -> list:
@@ -92,36 +106,36 @@
                     # Commented line
                     continue
 
                 if raw_line.startswith("https://plugins.qgis.org") and "[VERSION]" not in raw_line:
                     print(
                         f"{Level.Alert}"
                         f"Your https://plugins.qgis.org remote is not using a dynamic QGIS version."
-                        f"{Level.End}"
+                        f"{Level.End}",
                     )
                     print(
                         f"Instead of\n'{raw_line}'"
                         f"\nin your 'sources.list' file, you should have"
                         f"\n"
                         f"'https://plugins.qgis.org/plugins/plugins.xml?qgis=[VERSION]'"
                         f"\n\n"
                         f"Can you remove the file sources.list ? 'qgis-plugin-manager init' will "
                         f"regenerate it using dynamic QGIS version if QGIS is well configured.\n"
                         f"This is only a warning, the process will continue with the hardcoded QGIS "
                         f"version in your 'sources.list' file."
-                        f"\n\n"
+                        f"\n\n",
                     )
 
                 if "[VERSION]" in raw_line:
                     if not qgis_version:
                         print(
                             f"{Level.Alert}"
                             f"Skipping line '{raw_line}' because it has a token [VERSION] but "
                             f"no QGIS version could be detected."
-                            f"{Level.End}"
+                            f"{Level.End}",
                         )
                         continue
 
                     raw_line = raw_line.replace("[VERSION]", f"{qgis_version[0]}.{qgis_version[1]}")
 
                 self.list.append(raw_line)
 
@@ -170,15 +184,15 @@
         cache.mkdir()
 
         flag = False
         for server in self.list:
             print(f"Downloading {self.public_remote_name(server)}…")
             url, login, password = self.credentials(server)
             headers = {
-                'User-Agent': 'Mozilla/5.0',
+                'User-Agent': self.user_agent(),
             }
             if login:
                 token = base64.b64encode(f"{login}:{password}".encode())
                 headers["Authorization"] = b"Basic %s" % token
             request = urllib.request.Request(url, headers=headers)
             try:
                 f = urllib.request.urlopen(request)
@@ -294,15 +308,15 @@
             # Remove duplicates
             data['search'] = list(dict.fromkeys(search_text))
 
             plugin_obj = Plugin(**data)
             self.list_plugins[xml_plugin_name] = plugin_obj
         return plugins
 
-    def search(self, search_string: str, strict=True) -> List:
+    def search(self, search_string: str, strict: bool = True) -> List:
         """ Search in plugin names and tags."""
         # strict is used in tests to not check if the remote is ready
         if strict and not self.remote_is_ready():
             return []
 
         if self.list is None:
             self.remote_list()
@@ -315,16 +329,16 @@
             if plugin_name not in results:
                 if similar_names(search_string, plugin.search):
                     results.append(plugin_name)
 
         return results
 
     def install(
-            self, plugin_name, version="latest", current_version: str = "", force: bool = False,
-            remove_zip=True
+            self, plugin_name: str, version: str = "latest", current_version: str = "", force: bool = False,
+            remove_zip: bool = True,
     ) -> bool:
         """ Install the plugin with a specific version.
 
         Default version is latest.
         """
         if not self.remote_is_ready():
             return False
@@ -345,15 +359,15 @@
         url = self.list_plugins[plugin_name].download_url
         file_name = self.list_plugins[plugin_name].file_name
         actual = self.list_plugins[plugin_name].version
 
         if current_version == actual:
             if not force:
                 print(
-                    f"\t{Level.Alert}Same version detected on the remote, skipping {plugin_name}{Level.End}"
+                    f"\t{Level.Alert}Same version detected on the remote, skipping {plugin_name}{Level.End}",
                 )
                 # Plugin is installed and correct version, it's exit code 0
                 return True
 
             # print(f"Same plugin version detected {plugin_name} {current_version}, forcing…")
 
         if version != 'latest':
@@ -401,24 +415,24 @@
             print(f"Installed with user '{user}'")
         print("Please check file permissions and owner according to the user running QGIS Server.")
 
         restart_qgis_server()
         return True
 
     def _download_zip(
-            self, url: str, version: str, plugin_name: str, file_name: str, user: str
+            self, url: str, version: str, plugin_name: str, file_name: str, user: str,
     ) -> Tuple[bool, Union[None, Path]]:
         """ Download the ZIP
         """
         if url.startswith('file:'):
             zip_file = Path(unquote(urlparse(url).path))
 
         else:
             headers = {
-                'User-Agent': 'Mozilla/5.0',
+                'User-Agent': self.user_agent(),
             }
             request = urllib.request.Request(url, headers=headers)
             result = False
             try:
                 f = urllib.request.urlopen(request)
                 result = True
             except urllib.error.HTTPError as e:
@@ -453,36 +467,36 @@
                 print(f"\t{Level.Critical}Current user {user} can not write in {file_path}{Level.End}")
                 print("Check file permissions for the folder.")
                 return False, None
 
         return True, zip_file
 
     @staticmethod
-    def check_qgis_dev_version(qgis_version) -> Optional[List[str]]:
+    def check_qgis_dev_version(qgis_version: str) -> Optional[List[str]]:
         """ Check if the QGIS current version is odd number. """
         if not qgis_version:
             return None
 
         qgis_version = qgis_version.split('.')
         if int(qgis_version[1]) % 2 != 0:
             print(
                 f"{Level.Alert}"
                 f"A QGIS development version is detected : {qgis_version[0]}.{qgis_version[1]}."
-                f"{Level.End}"
+                f"{Level.End}",
             )
             qgis_version[1] = str(int(qgis_version[1]) + 1)
             print(
                 f"{Level.Alert}"
                 f"If needed, it will use {qgis_version[0]}.{qgis_version[1]} instead."
-                f"{Level.End}"
+                f"{Level.End}",
             )
         return qgis_version
 
     @staticmethod
-    def server_cache_filename(cache_folder, server) -> Path:
+    def server_cache_filename(cache_folder: str, server: str) -> Path:
         """ Return the path for XML file. """
         server, login, _ = Remote.credentials(server)
         filename = ""
         for x in server:
             if x.isalnum():
                 filename += x
             else:
@@ -506,25 +520,25 @@
 
         u = u._replace(query=urlencode(query, True))
         if login and password:
             return urlunparse(u), login[0], password[0]
 
         return urlunparse(u), '', ''
 
-    def all_credentials(self):
+    def all_credentials(self) -> Iterator[Tuple[str, str, str]]:
         """ Dirty hack to get all credentials for now… """
         if self.list is None:
             self.remote_list()
 
         for server in self.list:
             url, login, password = self.credentials(server)
             yield url, login, password
 
     @classmethod
     def public_remote_name(cls, server: str) -> str:
         """ Clean a URL from a password if needed. """
         u = urlparse(server)
         query = parse_qs(u.query, keep_blank_values=True)
         if 'password' in query.keys():
-            query['password'] = 'XXXXX'
+            query['password'] = '******'
         u = u._replace(query=urlencode(query, True))
         return urlunparse(u)
```

### Comparing `qgis-plugin-manager-1.6.1/qgis_plugin_manager/utils.py` & `qgis-plugin-manager-1.6.2/qgis_plugin_manager/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-__copyright__ = 'Copyright 2022, 3Liz'
+__copyright__ = 'Copyright 2024, 3Liz'
 __license__ = 'GPL version 3'
 __email__ = 'info@3liz.org'
 
 import os
 
 from difflib import SequenceMatcher
 from pathlib import Path
 from typing import Union
 
 from qgis_plugin_manager.definitions import Level
 
-DEFAULT_QGIS_VERSION = "3.22"
+DEFAULT_QGIS_VERSION = "3.34"
 
 
-def pretty_table(iterable, header) -> str:
+def pretty_table(iterable: list, header: list) -> str:
     """ Copy/paste from http://stackoverflow.com/a/40426743/2395485 """
     max_len = [len(x) for x in header]
     for row in iterable:
         row = [row] if type(row) not in (list, tuple) else row
         for index, col in enumerate(row):
             if max_len[index] < len(str(col)):
                 max_len[index] = len(str(col))
     output = '-' * (sum(max_len) + 1) + '\n'
     output += '|' + ''.join(
-        [h + ' ' * (l - len(h)) + '|' for h, l in zip(header, max_len)]) + '\n'
+        [a_header + ' ' * (a_line - len(a_header)) + '|' for a_header, a_line in zip(header, max_len)]) + '\n'
     output += '-' * (sum(max_len) + 1) + '\n'
     for row in iterable:
         row = [row] if type(row) not in (list, tuple) else row
         output += '|' + ''.join(
             [
                 str(c) + ' ' * (
-                    l - len(str(c))) + '|' for c, l in zip(
+                    a_line - len(str(c))) + '|' for c, a_line in zip(
                     row, max_len)
-            ]
+            ],
         ) + '\n'
     output += '-' * (sum(max_len) + 1) + '\n'
     return output
 
 
 def restart_qgis_server():
     """ Restart QGIS Server tip. """
@@ -118,27 +118,29 @@
     """ Try to guess the QGIS Server version.
 
         On linux distro, qgis python packages are installed at standard location
         in /usr/lib/python3/dist-packages
     """
     try:
         from qgis.core import Qgis
+
+        # 3.34.6
         return Qgis.QGIS_VERSION.split('-')[0]
     except ImportError:
         print(
             f"{Level.Alert}"
             f"Cannot check version with PyQGIS, check your QGIS installation or your PYTHONPATH"
-            f"{Level.End}"
+            f"{Level.End}",
         )
         print(f"Current user : {current_user()}")
         print(f'PYTHONPATH={os.getenv("PYTHONPATH")}')
         return ''
 
 
-def sources_file(current_folder) -> Path:
+def sources_file(current_folder: Path) -> Path:
     """ Return the default path to the "sources.list" file.
 
     The path by default or if it's defined with the environment variable.
     """
     env_path = os.getenv("QGIS_PLUGIN_MANAGER_SOURCES_FILE")
     if env_path:
         return Path(env_path)
```

### Comparing `qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/PKG-INFO` & `qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-manager
-Version: 1.6.1
+Version: 1.6.2
 Summary: Tool for downloading/managing QGIS plugins from CLI.
 Home-page: https://github.com/3liz/qgis-plugin-manager
-Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.1.tar.gz
+Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.2.tar.gz
 Author: Étienne Trimaille
 Author-email: etrimaille@3liz.com
 Project-URL: Docs, https://github.com/3liz/qgis-plugin-manager/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/3liz/qgis-plugin-manager/issues/
 Project-URL: Source, https://github.com/3liz/qgis-plugin-manager
 Keywords: QGIS
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,32 +18,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # QGIS-Plugin-Manager
 
 [![Tests](https://github.com/3liz/qgis-plugin-manager/actions/workflows/release.yml/badge.svg)](https://github.com/3liz/qgis-plugin-manager/actions/workflows/release.yml)
 [![PyPi version badge](https://badgen.net/pypi/v/qgis-plugin-manager)](https://pypi.org/project/qgis-plugin-manager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/qgis-plugin-manager)](https://pypi.org/project/qgis-plugin-manager/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qgis-plugin-manager)](https://pypi.org/project/qgis-plugin-manager/)
 
 Mainly designed for QGIS Server plugins, but it works also for desktop.
 
 Not tested on Windows.
 
-The **CLI** API is not stable yet.
-
 ## Installation
 
 Python 3.7 **minimum**, you can make a Python venv if needed.
 ```bash
 python3 --version
 ```
 
@@ -63,15 +63,15 @@
   Read [the documentation](README.md#notify-upstream-if-a-restart-is-needed).
 * `QGIS_PLUGINPATH` for storing plugins, from [QGIS Server documentation](https://docs.qgis.org/latest/en/docs/server_manual/config.html#environment-variables)
 * `PYTHONPATH` for importing QGIS libraries
 
 ## Utilisation
 
 **Either** you need to go in the directory where you are storing plugins, **or** you can use the environment variable `QGIS_PLUGINPATH`.
-You can read the [documentation](https://docs.qgis.org/3.22/en/docs/server_manual/config.html#environment-variables)
+You can read the [documentation](https://docs.qgis.org/latest/en/docs/server_manual/config.html#environment-variables)
 on QGIS Server about this variable.
 
 ```bash
 cd /path/where/you/have/plugins
 # usually on a server
 cd /usr/lib/qgis/plugins
 # on unix desktop with the default QGIS profile
@@ -105,26 +105,26 @@
 
 ### Init
 
 To create the first `sources.list` in the directory with at least the default repository https://plugins.qgis.org :
 ```bash
 $ qgis-plugin-manager init
 $ cat sources.list 
-https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19
+https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34
 ```
 
 You can have one or many servers, one on each line.
 
 ### List
 
 List all plugins installed :
 
 ```bash
 $ qgis-plugin-manager list
-QGIS server version 3.19.0
+QGIS server version 3.34.2
 List all plugins in /home/etienne/dev/qgis/server_plugin
 
 ------------------------------------------------------------------------------------------------------------------------------------
 |  Name            |  Version  | Flags           |  QGIS min  |  QGIS max  |  Author         | Folder owner     | Action ⚠         |
 ------------------------------------------------------------------------------------------------------------------------------------
 |Lizmap            |master     |                 |3.4         |3.99        |3Liz             | root : 0o755     | Unkown version   |
 |wfsOutputExtension|1.5.3      |Server           |3.0         |            |3Liz             | etienne : 0o755  |                  |
@@ -144,21 +144,21 @@
 
 ### Remote
 
 ```bash
 $ qgis-plugin-manager remote
 List of remotes :
 
-https://plugins.qgis.org/plugins/plugins.xml?qgis=3.22
+https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34
 
 $ cat sources.list 
 https://plugins.qgis.org/plugins/plugins.xml?qgis=[VERSION]
 ```
 
-`[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.22`.
+`[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.34`.
 If QGIS is upgraded, the XML file will be updated as well.
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
 #### Basic authentication
@@ -174,18 +174,18 @@
 
 ### Update
 
 To fetch the XML files from each repository :
 
 ```bash
 $ qgis-plugin-manager update
-Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19...
+Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.34...
 	Ok
 $ ls .cache_qgis_plugin_manager/
-https-plugins-qgis-org-plugins-plugins-xml-qgis-3-19.xml
+https-plugins-qgis-org-plugins-plugins-xml-qgis-3-34.xml
 ```
 
 ### Cache
 
 Check if a plugin is available :
 
 ```bash
@@ -286,14 +286,16 @@
 ```
 
 ### Notify upstream if a restart is needed
 
 When a plugin is installed or removed and if the environment variable `QGIS_PLUGIN_MANAGER_RESTART_FILE` is set,
 an empty file will be created or touched. It can notify you if QGIS Server needs to be restarted for instance.
 
+This is useful for a deployment with [Ansible](https://www.ansible.com/) for instance.
+
 Note that you must manually remove this file.
 
 ## Run tests
 
 ```bash
 export PYTHONPATH=/home/etienne/dev/app/qgis-master/share/qgis/python/:/usr/lib/python3/dist-packages/
 cd test
```

### Comparing `qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/SOURCES.txt` & `qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENSE
+MANIFEST.in
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 qgis_plugin_manager/__about__.py
 qgis_plugin_manager/__init__.py
 qgis_plugin_manager/__main__.py
 qgis_plugin_manager/definitions.py
 qgis_plugin_manager/local_directory.py
 qgis_plugin_manager/remote.py
```

### Comparing `qgis-plugin-manager-1.6.1/setup.py` & `qgis-plugin-manager-1.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 python_min_version = (3, 7)
 
 if sys.version_info < python_min_version:
     sys.exit(
         "qgis-plugin-manager requires at least Python version "
         f"{python_min_version[0]}.{python_min_version[1]}.\n"
-        f"You are currently running this installation with\n\n{sys.version}"
+        f"You are currently running this installation with\n\n{sys.version}",
     )
 
 # This string might be updated on CI on runtime with a proper semantic version name with X.Y.Z
-VERSION = "1.6.1"
+VERSION = "1.6.2"
 
 if "." not in VERSION:
     # If VERSION is still not a proper semantic versioning with X.Y.Z
     # let's hardcode 0.0.0
     VERSION = "0.0.0"
 
 read_me = Path(__file__).parent.joinpath("README.md").read_text(encoding='utf8')
@@ -56,13 +56,15 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Scientific/Engineering :: GIS",
     ],
     install_requires=[],
     python_requires=f">={python_min_version[0]}.{python_min_version[1]}",
+    include_package_data=True,
 )
```

### Comparing `qgis-plugin-manager-1.6.1/test/test_full_install.py` & `qgis-plugin-manager-1.6.2/test/test_full_install.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 from qgis_plugin_manager.local_directory import LocalDirectory
 from qgis_plugin_manager.remote import Remote
 
 
 @unittest.skipIf(os.getenv('CI') != 'true', "Only run on CI")
 class FullInstallNetwork(unittest.TestCase):
 
-    def setUp(self) -> None:
+    def setUp(self):
         self.plugin_name = 'QuickOSM'
         self.repository = "https://plugins.qgis.org/plugins/plugins.xml?qgis=3.10"
         self.directory = Path('fixtures/plugins')
         self.remote = Remote(self.directory)
         self.local = LocalDirectory(self.directory)
 
         self.plugin_path = Path(self.directory / self.plugin_name)
         if self.plugin_path.exists():
             shutil.rmtree(self.plugin_path)
 
         shutil.copy(Path(self.directory / 'sources.list'), Path(self.directory / 'sources.list.back'))
 
-    def tearDown(self) -> None:
+    def tearDown(self):
         if self.plugin_path.exists():
             shutil.rmtree(self.plugin_path)
 
         shutil.copy(Path(self.directory / 'sources.list.back'), Path(self.directory / 'sources.list'))
 
     def test_install_network(self):
         """ Test install QuickOSM with a specific version, remove and try the latest. """
@@ -53,15 +53,15 @@
         self.remote.install(self.plugin_name)
         self.assertTrue(Path(self.directory / 'QuickOSM').exists())
         self.assertNotEqual(version, self.local.plugin_metadata(self.plugin_name, 'version'))
 
 
 class FullInstallLocal(unittest.TestCase):
 
-    def tearDown(self) -> None:
+    def tearDown(self):
         destination = Path('fixtures/xml_files/file_protocol/minimal_plugin')
         if destination.exists():
             shutil.rmtree(destination)
 
         cache_folder = Path('fixtures/xml_files/file_protocol/.cache_qgis_plugin_manager')
         if cache_folder.exists():
             shutil.rmtree(cache_folder)
@@ -73,15 +73,15 @@
     def test_install_local(self):
         """ Test install local file. """
         folder = Path('fixtures/xml_files/file_protocol/')
         folder.joinpath('sources.list').touch()
         folder.joinpath('.cache_qgis_plugin_manager').mkdir(parents=True, exist_ok=True)
         shutil.copy(
             folder.joinpath('plugin.xml'),
-            folder.joinpath('.cache_qgis_plugin_manager/plugins.xml')
+            folder.joinpath('.cache_qgis_plugin_manager/plugins.xml'),
         )
 
         remote = Remote(folder)
         plugins = remote._parse_xml(folder.joinpath('plugin.xml'), {})
         self.assertDictEqual({'Minimal': '1.0.0'}, plugins)
         remote.list_plugins = plugins
         local = LocalDirectory(folder)
```

### Comparing `qgis-plugin-manager-1.6.1/test/test_local.py` & `qgis-plugin-manager-1.6.2/test/test_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 
 from qgis_plugin_manager.local_directory import LocalDirectory
 
 
 class TestLocal(unittest.TestCase):
 
-    def setUp(self) -> None:
+    def setUp(self):
         self.local = LocalDirectory(Path('fixtures/plugins'))
 
     def test_list_existing_plugins(self):
         """ Test to find existing plugins. """
         self.assertCountEqual(['plugin_a', 'plugin_b'], self.local.plugin_list())
         self.assertCountEqual(['missing_init', 'missing_metadata'], self.local.invalid)
         self.assertEqual(self.local.plugin_installed_version('Plugin A'), "1.0.0")
```

### Comparing `qgis-plugin-manager-1.6.1/test/test_remote.py` & `qgis-plugin-manager-1.6.2/test/test_remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         self.assertIsNotNone(plugin)
         self.assertEqual(plugin.name, 'Data Plotly')
         self.assertEqual(plugin.tags, 'vector,python,d3,plots,graphs,datavis,dataplotly,dataviz')
         self.assertListEqual(
             plugin.search,
             [
                 'data plotly', 'dataplotly', 'vector', 'python', 'd3', 'plots', 'graphs', 'datavis',
-                'dataviz', 'data', 'plotly'
-            ]
+                'dataviz', 'data', 'plotly',
+            ],
         )
 
         # Test the search
         self.assertListEqual([], self.remote.search("foo"))
         self.assertListEqual(['Data Plotly'], self.remote.search("dataviz", strict=False))
         self.assertListEqual(['Data Plotly'], self.remote.search("dataplotly", strict=False))
 
@@ -49,58 +49,66 @@
         plugins = self.remote._parse_xml(Path('fixtures/xml_files/lizmap/lizmap.xml'), {})
         self.assertEqual(2, len(self.remote.list_plugins))
         self.assertDictEqual(
             {
                 'Lizmap': '3.7.4',
                 'Lizmap server': '1.0.0',
             },
-            plugins
+            plugins,
         )
 
         plugin = self.remote.list_plugins.get('Lizmap server')
         self.assertIsNotNone(plugin)
         self.assertEqual(plugin.name, 'Lizmap server')
 
         self.assertListEqual(
             plugin.search,
-            ['lizmap server', 'lizmapserver', 'web', 'cloud', 'lizmap', 'server']
+            ['lizmap server', 'lizmapserver', 'web', 'cloud', 'lizmap', 'server'],
         )
 
         # Test the search
         self.assertListEqual(['Lizmap', 'Lizmap server'], self.remote.search("lizmap", strict=False))
 
     def test_qgis_dev_version(self):
         """ Test check QGIS dev version number. """
         self.assertListEqual(["3", "22", "11"], Remote.check_qgis_dev_version('3.22.11'))
         self.assertListEqual(["3", "24", "0"], Remote.check_qgis_dev_version('3.23.0'))
 
+    def test_user_agent(self):
+        """ Test the User-Agent. """
+        self.remote = Remote(Path('fixtures/xml_files/lizmap'))
+        self.assertIn("Mozilla/5.0 QGIS/", self.remote.user_agent())
+
     def test_parse_url(self):
         """ Test to parse a URL for login&password. """
         self.assertTupleEqual(
             ('https://foo.bar/plugins.xml?qgis=3.10', 'login', 'pass'),
-            Remote.credentials("https://foo.bar/plugins.xml?qgis=3.10&username=login&password=pass")
+            Remote.credentials("https://foo.bar/plugins.xml?qgis=3.10&username=login&password=pass"),
         )
         self.assertTupleEqual(
             ('https://foo.bar/plugins.xml?qgis=3.10', '', ''),
-            Remote.credentials("https://foo.bar/plugins.xml?qgis=3.10")
+            Remote.credentials("https://foo.bar/plugins.xml?qgis=3.10"),
         )
 
     def test_clean_remote(self):
         """ Test to clean a URL from login&password. """
+        # "password", the keyword to look for
         self.assertEqual(
-            "https://foo.bar/plugins.xml?qgis=3.10&username=login&password=XXXXX",
-            Remote.public_remote_name("https://foo.bar/plugins.xml?qgis=3.10&username=login&password=pass")
+            "https://foo.bar/plugins.xml?qgis=3.10&username=login&password=%2A%2A%2A%2A%2A%2A",
+            Remote.public_remote_name("https://foo.bar/plugins.xml?qgis=3.10&username=login&password=pass"),
         )
+        # "pass", not the keyword to look for
         self.assertEqual(
             "https://foo.bar/plugins.xml?qgis=3.10&username=login&pass=pass",
-            Remote.public_remote_name("https://foo.bar/plugins.xml?qgis=3.10&username=login&pass=pass")
+            Remote.public_remote_name("https://foo.bar/plugins.xml?qgis=3.10&username=login&pass=pass"),
         )
+        # Nothing
         self.assertEqual(
             "https://foo.bar/plugins.xml?qgis=3.10",
-            Remote.public_remote_name("https://foo.bar/plugins.xml?qgis=3.10")
+            Remote.public_remote_name("https://foo.bar/plugins.xml?qgis=3.10"),
         )
 
     @unittest.expectedFailure
     def test_latest_pgmetadata(self):
         """ Test read multiple remotes. """
         # There is 0.1.0 and 0.2.0 in these XML files
         self.assertEqual('0.2.0', self.remote.latest("PgMetadata"))
```

### Comparing `qgis-plugin-manager-1.6.1/test/test_utils.py` & `qgis-plugin-manager-1.6.2/test/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,23 @@
         self.assertIsNone(parse_version(""))
 
     def test_similar_names(self):
         """ Test about similar names in the XML file. """
         # typo wanted
         self.assertListEqual(
             ['Lizmap'],
-            similar_names('lizma', ['a', 'Lizmap', 'QuickOSM'])
+            similar_names('lizma', ['a', 'Lizmap', 'QuickOSM']),
         )
 
         existing = ['data plotly', 'DATA PLOTLY', 'Data   PLOTLY']
 
         # lower case
         self.assertListEqual(
             existing,
-            similar_names('dataplotly', existing)
+            similar_names('dataplotly', existing),
         )
 
         # upper case
         self.assertListEqual(
             existing,
-            similar_names('DATA PLOT LY', existing)
+            similar_names('DATA PLOT LY', existing),
         )
```

