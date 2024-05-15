# Comparing `tmp/oterm-0.2.8.tar.gz` & `tmp/oterm-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oterm-0.2.8.tar", max compression
+gzip compressed data, was "oterm-0.2.9.tar", max compression
```

## Comparing `oterm-0.2.8.tar` & `oterm-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1064 2024-05-03 12:41:59.688509 oterm-0.2.8/LICENSE
--rw-r--r--   0        0        0     3798 2024-05-03 12:41:59.688509 oterm-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/__init__.py
--rw-r--r--   0        0        0     7948 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/chat_edit.py
--rw-r--r--   0        0        0     1593 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/chat_export.py
--rw-r--r--   0        0        0      734 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/chat_rename.py
--rw-r--r--   0        0        0     2313 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/image_browser.py
--rw-r--r--   0        0        0     3428 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/oterm.py
--rw-r--r--   0        0        0     3323 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/oterm.tcss
--rw-r--r--   0        0        0     1058 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/prompt_history.py
--rw-r--r--   0        0        0     1947 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/splash.py
--rw-r--r--   0        0        0       46 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/__init__.py
--rw-r--r--   0        0        0    10087 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/chat.py
--rw-r--r--   0        0        0     1823 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/image.py
--rw-r--r--   0        0        0      627 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/monkey.py
--rw-r--r--   0        0        0     5569 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/prompt.py
--rw-r--r--   0        0        0      879 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/text_area.py
--rw-r--r--   0        0        0        0 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/cli/__init__.py
--rw-r--r--   0        0        0      724 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/cli/oterm.py
--rw-r--r--   0        0        0     3131 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/config.py
--rw-r--r--   0        0        0     2295 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/ollama.py
--rw-r--r--   0        0        0        0 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/__init__.py
--rw-r--r--   0        0        0      967 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/chat.py
--rw-r--r--   0        0        0      608 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/setup.py
--rw-r--r--   0        0        0     5988 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/store.py
--rw-r--r--   0        0        0      469 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/upgrades/__init__.py
--rw-r--r--   0        0        0      574 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/upgrades/v0_1_11.py
--rw-r--r--   0        0        0      514 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/upgrades/v0_1_6.py
--rw-r--r--   0        0        0      522 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/upgrades/v0_2_0.py
--rw-r--r--   0        0        0      533 2024-05-03 12:41:59.692510 oterm-0.2.8/oterm/store/upgrades/v0_2_4.py
--rw-r--r--   0        0        0      535 2024-05-03 12:41:59.692510 oterm-0.2.8/oterm/store/upgrades/v0_2_8.py
--rw-r--r--   0        0        0     1408 2024-05-03 12:41:59.692510 oterm-0.2.8/oterm/utils.py
--rw-r--r--   0        0        0     2040 2024-05-03 12:41:59.692510 oterm-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 oterm-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-15 16:35:57.932519 oterm-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3798 2024-05-15 16:35:57.936519 oterm-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/__init__.py
+-rw-r--r--   0        0        0     7948 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/chat_edit.py
+-rw-r--r--   0        0        0     1593 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/chat_export.py
+-rw-r--r--   0        0        0      734 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/chat_rename.py
+-rw-r--r--   0        0        0     2313 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/image_browser.py
+-rw-r--r--   0        0        0     3428 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/oterm.py
+-rw-r--r--   0        0        0     3323 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/oterm.tcss
+-rw-r--r--   0        0        0     1058 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/prompt_history.py
+-rw-r--r--   0        0        0     1947 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/splash.py
+-rw-r--r--   0        0        0       46 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/widgets/__init__.py
+-rw-r--r--   0        0        0    10087 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/widgets/chat.py
+-rw-r--r--   0        0        0     1823 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/widgets/image.py
+-rw-r--r--   0        0        0      627 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/widgets/monkey.py
+-rw-r--r--   0        0        0     5569 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/widgets/prompt.py
+-rw-r--r--   0        0        0      879 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/app/widgets/text_area.py
+-rw-r--r--   0        0        0        0 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/cli/__init__.py
+-rw-r--r--   0        0        0      724 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/cli/oterm.py
+-rw-r--r--   0        0        0     3131 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/config.py
+-rw-r--r--   0        0        0     2295 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/ollama.py
+-rw-r--r--   0        0        0        0 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/__init__.py
+-rw-r--r--   0        0        0      967 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/chat.py
+-rw-r--r--   0        0        0      608 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/setup.py
+-rw-r--r--   0        0        0     5988 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/store.py
+-rw-r--r--   0        0        0      469 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/upgrades/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/upgrades/v0_1_11.py
+-rw-r--r--   0        0        0      514 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/upgrades/v0_1_6.py
+-rw-r--r--   0        0        0      522 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/upgrades/v0_2_0.py
+-rw-r--r--   0        0        0      533 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/upgrades/v0_2_4.py
+-rw-r--r--   0        0        0      535 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/store/upgrades/v0_2_8.py
+-rw-r--r--   0        0        0     1408 2024-05-15 16:35:57.936519 oterm-0.2.9/oterm/utils.py
+-rw-r--r--   0        0        0     2041 2024-05-15 16:35:57.936519 oterm-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 oterm-0.2.9/PKG-INFO
```

### Comparing `oterm-0.2.8/LICENSE` & `oterm-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/README.md` & `oterm-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/chat_edit.py` & `oterm-0.2.9/oterm/app/chat_edit.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/chat_export.py` & `oterm-0.2.9/oterm/app/chat_export.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/chat_rename.py` & `oterm-0.2.9/oterm/app/chat_rename.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/image_browser.py` & `oterm-0.2.9/oterm/app/image_browser.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/oterm.py` & `oterm-0.2.9/oterm/app/oterm.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/oterm.tcss` & `oterm-0.2.9/oterm/app/oterm.tcss`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/prompt_history.py` & `oterm-0.2.9/oterm/app/prompt_history.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/splash.py` & `oterm-0.2.9/oterm/app/splash.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/widgets/chat.py` & `oterm-0.2.9/oterm/app/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/widgets/image.py` & `oterm-0.2.9/oterm/app/widgets/image.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/widgets/monkey.py` & `oterm-0.2.9/oterm/app/widgets/monkey.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/widgets/prompt.py` & `oterm-0.2.9/oterm/app/widgets/prompt.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/app/widgets/text_area.py` & `oterm-0.2.9/oterm/app/widgets/text_area.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/cli/oterm.py` & `oterm-0.2.9/oterm/cli/oterm.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/config.py` & `oterm-0.2.9/oterm/config.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/ollama.py` & `oterm-0.2.9/oterm/ollama.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/store/chat.py` & `oterm-0.2.9/oterm/store/chat.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/store/setup.py` & `oterm-0.2.9/oterm/store/setup.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/store/store.py` & `oterm-0.2.9/oterm/store/store.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/store/upgrades/v0_1_11.py` & `oterm-0.2.9/oterm/store/upgrades/v0_1_11.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/store/upgrades/v0_1_6.py` & `oterm-0.2.9/oterm/store/upgrades/v0_1_6.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/store/upgrades/v0_2_0.py` & `oterm-0.2.9/oterm/store/upgrades/v0_2_0.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/store/upgrades/v0_2_4.py` & `oterm-0.2.9/oterm/store/upgrades/v0_2_4.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/store/upgrades/v0_2_8.py` & `oterm-0.2.9/oterm/store/upgrades/v0_2_8.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/oterm/utils.py` & `oterm-0.2.9/oterm/utils.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.8/pyproject.toml` & `oterm-0.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oterm"
-version = "0.2.8"
+version = "0.2.9"
 description = "A text-based terminal client for Ollama."
 authors = ["Yiorgis Gozadinos <ggozadinos@gmail.com>"]
 homepage = "https://github.com/ggozad/oterm"
 repository = "https://github.com/ggozad/oterm"
 license = "MIT"
 readme = "README.md"
 classifiers = [
@@ -25,31 +25,31 @@
 oterm = "oterm.cli.oterm:cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/ggozad/oterm/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-textual = "^0.53.1"
-typer = "^0.9.0"
+textual = "^0.59.0"
+typer = "^0.12.0"
 python-dotenv = "^1.0.1"
 aiosql = "^10.1"
 aiosqlite = "^0.20.0"
 pyperclip = "^1.8.2"
 packaging = "^24.0"
-rich-pixels = "^2.2.0"
-pillow = "^10.2.0"
-ollama = "^0.1.7"
+rich-pixels = "^3.0.1"
+pillow = "^10.3.0"
+ollama = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pdbpp = "^0.10.3"
-pytest = "^7.4.4"
-pytest-asyncio = "^0.23.3"
-textual-dev = "^1.4.0"
-ruff = "^0.3.3"
+pytest = "^8.2.0"
+pytest-asyncio = "^0.23.6"
+textual-dev = "^1.5.1"
+ruff = "^0.4.4"
 
 [tool.ruff]
 line-length = 88
 # Enable Flake's "E" and "F" codes by default and "I" for sorting imports.
 lint.select = ["E", "F", "I"]
 lint.ignore = ["E501", "E741"] # E741 should not be ignored
 # Exclude a variety of commonly ignored directories.
```

### Comparing `oterm-0.2.8/PKG-INFO` & `oterm-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oterm
-Version: 0.2.8
+Version: 0.2.9
 Summary: A text-based terminal client for Ollama.
 Home-page: https://github.com/ggozad/oterm
 License: MIT
 Author: Yiorgis Gozadinos
 Author-email: ggozadinos@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -18,22 +18,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Dist: aiosql (>=10.1,<11.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
-Requires-Dist: ollama (>=0.1.7,<0.2.0)
+Requires-Dist: ollama (>=0.2.0,<0.3.0)
 Requires-Dist: packaging (>=24.0,<25.0)
-Requires-Dist: pillow (>=10.2.0,<11.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: rich-pixels (>=2.2.0,<3.0.0)
-Requires-Dist: textual (>=0.53.1,<0.54.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: rich-pixels (>=3.0.1,<4.0.0)
+Requires-Dist: textual (>=0.59.0,<0.60.0)
+Requires-Dist: typer (>=0.12.0,<0.13.0)
 Project-URL: Bug Tracker, https://github.com/ggozad/oterm/issues
 Project-URL: Repository, https://github.com/ggozad/oterm
 Description-Content-Type: text/markdown
 
 # oterm
 
 the text-based terminal client for [Ollama](https://github.com/jmorganca/ollama).
```

