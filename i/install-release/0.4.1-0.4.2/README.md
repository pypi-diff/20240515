# Comparing `tmp/install_release-0.4.1.tar.gz` & `tmp/install_release-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install_release-0.4.1.tar", max compression
+gzip compressed data, was "install_release-0.4.2.tar", max compression
```

## Comparing `install_release-0.4.1.tar` & `install_release-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      295 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/Makefile
--rw-r--r--   0        0        0        0 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/__init__.py
--rw-r--r--   0        0        0     5949 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/cli.py
--rw-r--r--   0        0        0     9718 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/cli_interact.py
--rw-r--r--   0        0        0     1295 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/constants.py
--rw-r--r--   0        0        0     7465 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/core.py
--rw-r--r--   0        0        0     2221 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/data.py
--rw-r--r--   0        0        0     2285 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/state.py
--rw-r--r--   0        0        0     8504 2024-02-27 16:31:52.846449 install_release-0.4.1/InstallRelease/utils.py
--rw-r--r--   0        0        0    35149 2024-02-27 16:31:52.846449 install_release-0.4.1/LICENSE
--rw-r--r--   0        0        0    10119 2024-02-27 16:31:52.846449 install_release-0.4.1/README.md
--rw-r--r--   0        0        0      951 2024-02-27 16:31:52.846449 install_release-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    11036 1970-01-01 00:00:00.000000 install_release-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      295 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/Makefile
+-rw-r--r--   0        0        0        0 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/__init__.py
+-rw-r--r--   0        0        0     5949 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/cli.py
+-rw-r--r--   0        0        0     9718 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/cli_interact.py
+-rw-r--r--   0        0        0     1295 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/constants.py
+-rw-r--r--   0        0        0     7465 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/core.py
+-rw-r--r--   0        0        0     2221 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/data.py
+-rw-r--r--   0        0        0     2285 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/state.py
+-rw-r--r--   0        0        0     8504 2024-05-15 06:27:47.272467 install_release-0.4.2/InstallRelease/utils.py
+-rw-r--r--   0        0        0    35149 2024-05-15 06:27:47.272467 install_release-0.4.2/LICENSE
+-rw-r--r--   0        0        0    10186 2024-05-15 06:27:47.272467 install_release-0.4.2/README.md
+-rw-r--r--   0        0        0      951 2024-05-15 06:27:47.272467 install_release-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    11103 1970-01-01 00:00:00.000000 install_release-0.4.2/PKG-INFO
```

### Comparing `install_release-0.4.1/InstallRelease/cli.py` & `install_release-0.4.2/InstallRelease/cli.py`

 * *Files identical despite different names*

### Comparing `install_release-0.4.1/InstallRelease/cli_interact.py` & `install_release-0.4.2/InstallRelease/cli_interact.py`

 * *Files identical despite different names*

### Comparing `install_release-0.4.1/InstallRelease/constants.py` & `install_release-0.4.2/InstallRelease/constants.py`

 * *Files identical despite different names*

### Comparing `install_release-0.4.1/InstallRelease/core.py` & `install_release-0.4.2/InstallRelease/core.py`

 * *Files identical despite different names*

### Comparing `install_release-0.4.1/InstallRelease/data.py` & `install_release-0.4.2/InstallRelease/data.py`

 * *Files identical despite different names*

### Comparing `install_release-0.4.1/InstallRelease/state.py` & `install_release-0.4.2/InstallRelease/state.py`

 * *Files identical despite different names*

### Comparing `install_release-0.4.1/InstallRelease/utils.py` & `install_release-0.4.2/InstallRelease/utils.py`

 * *Files identical despite different names*

### Comparing `install_release-0.4.1/LICENSE` & `install_release-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `install_release-0.4.1/README.md` & `install_release-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Python Version](https://img.shields.io/badge/Python-3.8_to_3.11-xx.svg)](https://shields.io/) [![Downloads](https://static.pepy.tech/personalized-badge/install-release?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/install-release)
 
 
 `install-release` is a CLI tool to install any tool for your device directly from their GitHub releases and keep them updated. Consider it as a small package manager to install tools from GitHub releases.
 
 This can be any tool you want to install, which is pre-compiled for your device and present on GitHub releases.
 
-> INFO: It's mainly for installing tools that are not directly available officially by package managers like `apt, yum, pacman` etc.
+> INFO: It's mainly for installing tools that are not directly available officially by package managers like `apt, yum, pacman, brew` etc.
 
 
 <!-- Table of content -->
 ## Table of Contents
 - [Install Release 🚀](#install-release-)
   - [Table of Contents](#table-of-contents)
   - [Getting started](#getting-started)
@@ -41,15 +41,15 @@
 # Example Installation a tool named `gron` directly from its GitHub releases
 
 # install-release get [GITHUB-URL]
 
 ❯ install-release get https://github.com/tomnomnom/gron 
 ```
 
-![demo](./.github/images/demo.png)
+![demo](https://raw.githubusercontent.com/Rishang/install-release/main/.github/images/demo.png)
 
 
 Checking for gron is installed using `installed-release`:
 
 ```
 ❯ which gron
 /home/noobi/bin/gron
```

### Comparing `install_release-0.4.1/pyproject.toml` & `install_release-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [virtualenvs]
 in-project = true
 
 [tool.poetry]
 name = "install-release"
-version = "0.4.1"
+version = "0.4.2"
 readme = "README.md"
 description = "A cli tool to install tools based on your device info directly from github releases and keep them updated."
 authors = ["Rishang <rishangbhavsarcs@gmail.com>"]
 packages = [
   { include = "InstallRelease" }
 ]
 homepage = "https://github.com/Rishang/install-releases"
```

### Comparing `install_release-0.4.1/PKG-INFO` & `install_release-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-release
-Version: 0.4.1
+Version: 0.4.2
 Summary: A cli tool to install tools based on your device info directly from github releases and keep them updated.
 Home-page: https://github.com/Rishang/install-releases
 Author: Rishang
 Author-email: rishangbhavsarcs@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,15 @@
 [![Python Version](https://img.shields.io/badge/Python-3.8_to_3.11-xx.svg)](https://shields.io/) [![Downloads](https://static.pepy.tech/personalized-badge/install-release?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/install-release)
 
 
 `install-release` is a CLI tool to install any tool for your device directly from their GitHub releases and keep them updated. Consider it as a small package manager to install tools from GitHub releases.
 
 This can be any tool you want to install, which is pre-compiled for your device and present on GitHub releases.
 
-> INFO: It's mainly for installing tools that are not directly available officially by package managers like `apt, yum, pacman` etc.
+> INFO: It's mainly for installing tools that are not directly available officially by package managers like `apt, yum, pacman, brew` etc.
 
 
 <!-- Table of content -->
 ## Table of Contents
 - [Install Release 🚀](#install-release-)
   - [Table of Contents](#table-of-contents)
   - [Getting started](#getting-started)
@@ -63,15 +63,15 @@
 # Example Installation a tool named `gron` directly from its GitHub releases
 
 # install-release get [GITHUB-URL]
 
 ❯ install-release get https://github.com/tomnomnom/gron 
 ```
 
-![demo](./.github/images/demo.png)
+![demo](https://raw.githubusercontent.com/Rishang/install-release/main/.github/images/demo.png)
 
 
 Checking for gron is installed using `installed-release`:
 
 ```
 ❯ which gron
 /home/noobi/bin/gron
```

