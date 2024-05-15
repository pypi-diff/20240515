# Comparing `tmp/streamlitgo-0.1.0.tar.gz` & `tmp/streamlitgo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitgo-0.1.0.tar", max compression
+gzip compressed data, was "streamlitgo-0.1.1.tar", max compression
```

## Comparing `streamlitgo-0.1.0.tar` & `streamlitgo-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     2546 2024-03-22 02:34:25.311392 streamlitgo-0.1.0/README.md
--rw-r--r--   0        0        0      733 2024-03-22 02:34:31.143325 streamlitgo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 02:34:25.311392 streamlitgo-0.1.0/streamlitgo/__init__.py
--rw-r--r--   0        0        0       61 2024-03-22 02:34:25.315392 streamlitgo-0.1.0/streamlitgo/__main__.py
--rw-r--r--   0        0        0      813 2024-03-22 02:34:25.315392 streamlitgo-0.1.0/streamlitgo/cli.py
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 streamlitgo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2597 2024-05-15 09:08:52.775556 streamlitgo-0.1.1/README.md
+-rw-r--r--   0        0        0      733 2024-05-15 09:08:57.771587 streamlitgo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 09:08:52.775556 streamlitgo-0.1.1/streamlitgo/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-15 09:08:52.775556 streamlitgo-0.1.1/streamlitgo/__main__.py
+-rw-r--r--   0        0        0      930 2024-05-15 09:08:52.775556 streamlitgo-0.1.1/streamlitgo/cli.py
+-rw-r--r--   0        0        0     1842 2024-05-15 09:08:52.775556 streamlitgo-0.1.1/streamlitgo/config/stgo.py
+-rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 streamlitgo-0.1.1/PKG-INFO
```

### Comparing `streamlitgo-0.1.0/README.md` & `streamlitgo-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Streamlit GO
 
 Package for loading a script before streamlit server start
 
+This package will load `stgo.py` in current working directory before the streamlit server starts. You can use this to patch the streamlit server or to load some data before the server starts!
+
+For example:
+
+- add some code before each page run
+- add a custom endpoint to the streamlit server
+- get current authenticated user info by custom header
+
 ## Installation
 
 ```bash
 pip install streamlitgo
 ```
 
 ## Usage
 
-This package will load `stgo.py` in current working directory before the streamlit server starts. You can use this to patch the streamlit server or to load some data before the server starts!
-
-For example:
-
-- add some command before each script run
-- add a custom endpoint to the streamlit server
-- get current authenticated user info by custom header
-
-Just use `streamlitgo` instead of `streamlit` in your command line.
+Just create your own `stgo.py` in your working directory and use `streamlitgo` instead of `streamlit` in your command line.
 
 ```bash
 streamlitgo run your_script.py
 ```
 
 ### Example
```

### Comparing `streamlitgo-0.1.0/pyproject.toml` & `streamlitgo-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlitgo"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["paleneutron <paleneutron@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 streamlit = "^1.32.2"
```

### Comparing `streamlitgo-0.1.0/streamlitgo/cli.py` & `streamlitgo-0.1.1/streamlitgo/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import importlib.util
 import os
 import sys
+from pathlib import Path
+
 from streamlit.logger import get_logger
+
 logger = get_logger(__name__)
 
 
 def main():
     fixed_setup_script_path = os.path.abspath("./stgo.py")
     module_name = "streamlitgo.override"
     if os.path.exists(fixed_setup_script_path):
         logger.info(f"loading setup script at {fixed_setup_script_path}")
-        spec = importlib.util.spec_from_file_location(module_name, fixed_setup_script_path)
-        override_mod = importlib.util.module_from_spec(spec)
-        sys.modules[module_name] = override_mod
-        spec.loader.exec_module(override_mod)
     else:
-        logger.info(f"No fixed setup script found at {fixed_setup_script_path}, skipping")
-
+        logger.info(f"No fixed setup script found at {fixed_setup_script_path}, use default settings")
+        fixed_setup_script_path = Path(__file__).parent / "config" / "stgo.py"
+        
+    spec = importlib.util.spec_from_file_location(module_name, fixed_setup_script_path)
+    override_mod = importlib.util.module_from_spec(spec)
+    sys.modules[module_name] = override_mod
+    spec.loader.exec_module(override_mod)
+    
     from streamlit.web.cli import main as stmain  # isort:skip
+
     stmain()
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `streamlitgo-0.1.0/PKG-INFO` & `streamlitgo-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlitgo
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: paleneutron
 Author-email: paleneutron@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,31 +12,31 @@
 Requires-Dist: streamlit (>=1.32.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Streamlit GO
 
 Package for loading a script before streamlit server start
 
+This package will load `stgo.py` in current working directory before the streamlit server starts. You can use this to patch the streamlit server or to load some data before the server starts!
+
+For example:
+
+- add some code before each page run
+- add a custom endpoint to the streamlit server
+- get current authenticated user info by custom header
+
 ## Installation
 
 ```bash
 pip install streamlitgo
 ```
 
 ## Usage
 
-This package will load `stgo.py` in current working directory before the streamlit server starts. You can use this to patch the streamlit server or to load some data before the server starts!
-
-For example:
-
-- add some command before each script run
-- add a custom endpoint to the streamlit server
-- get current authenticated user info by custom header
-
-Just use `streamlitgo` instead of `streamlit` in your command line.
+Just create your own `stgo.py` in your working directory and use `streamlitgo` instead of `streamlit` in your command line.
 
 ```bash
 streamlitgo run your_script.py
 ```
 
 ### Example
```

