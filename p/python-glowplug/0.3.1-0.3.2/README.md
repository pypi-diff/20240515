# Comparing `tmp/python_glowplug-0.3.1.tar.gz` & `tmp/python_glowplug-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glowplug-0.3.1.tar", max compression
+gzip compressed data, was "python_glowplug-0.3.2.tar", max compression
```

## Comparing `python_glowplug-0.3.1.tar` & `python_glowplug-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,11 @@
--rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.3.1/LICENSE
--rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.3.1/README.md
--rw-r--r--   0        0        0      515 2024-05-10 21:47:25.862700 python_glowplug-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      378 2024-05-10 21:38:36.780174 python_glowplug-0.3.1/src/glowplug/__init__.py
--rw-r--r--   0        0        0     1628 2024-05-10 21:46:38.763517 python_glowplug-0.3.1/src/glowplug/config/__init__.py
--rw-r--r--   0        0        0     3583 2024-05-10 21:46:44.469058 python_glowplug-0.3.1/src/glowplug/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-05-10 21:34:44.661098 python_glowplug-0.3.1/src/glowplug/driver/__init__.py
--rw-r--r--   0        0        0      178 2024-05-10 21:36:15.846033 python_glowplug-0.3.1/src/glowplug/driver/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6373 2024-05-10 21:36:15.848539 python_glowplug-0.3.1/src/glowplug/driver/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     4576 2024-05-10 21:36:17.022664 python_glowplug-0.3.1/src/glowplug/driver/__pycache__/mssql.cpython-311.pyc
--rw-r--r--   0        0        0     4805 2024-05-10 21:36:17.021555 python_glowplug-0.3.1/src/glowplug/driver/__pycache__/pg.cpython-311.pyc
--rw-r--r--   0        0        0     2437 2024-05-10 21:36:17.022045 python_glowplug-0.3.1/src/glowplug/driver/__pycache__/sqlite.cpython-311.pyc
--rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.3.1/src/glowplug/driver/base.py
--rw-r--r--   0        0        0     2635 2024-05-10 21:18:25.176417 python_glowplug-0.3.1/src/glowplug/driver/mssql.py
--rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.3.1/src/glowplug/driver/pg.py
--rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.3.1/src/glowplug/driver/sqlite.py
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 python_glowplug-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.3.2/LICENSE
+-rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.3.2/README.md
+-rw-r--r--   0        0        0      515 2024-05-15 00:26:42.282568 python_glowplug-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      378 2024-05-10 21:38:36.780174 python_glowplug-0.3.2/src/glowplug/__init__.py
+-rw-r--r--   0        0        0     1628 2024-05-10 21:46:38.763517 python_glowplug-0.3.2/src/glowplug/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 21:34:44.661098 python_glowplug-0.3.2/src/glowplug/driver/__init__.py
+-rw-r--r--   0        0        0     2896 2024-05-15 00:26:23.709109 python_glowplug-0.3.2/src/glowplug/driver/base.py
+-rw-r--r--   0        0        0     2635 2024-05-10 21:18:25.176417 python_glowplug-0.3.2/src/glowplug/driver/mssql.py
+-rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.3.2/src/glowplug/driver/pg.py
+-rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.3.2/src/glowplug/driver/sqlite.py
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 python_glowplug-0.3.2/PKG-INFO
```

### Comparing `python_glowplug-0.3.1/LICENSE` & `python_glowplug-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.3.1/README.md` & `python_glowplug-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.3.1/pyproject.toml` & `python_glowplug-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-glowplug"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Joe Nudell <jnudell@hks.harvard.edu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/jnu/python-glowplug"
 packages = [
     { include = "glowplug", from = "src" }
```

### Comparing `python_glowplug-0.3.1/src/glowplug/config/__init__.py` & `python_glowplug-0.3.2/src/glowplug/config/__init__.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.3.1/src/glowplug/driver/base.py` & `python_glowplug-0.3.2/src/glowplug/driver/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 class AlembicCommandProxy:
     """Proxy for running alembic commands with a given config."""
 
     def __init__(self, config: alembic.config.Config) -> None:
         self.config = config
 
     def __getattribute__(self, name: str) -> Any:
-        cmd = getattr(alembic.command, name)
+        cmd = getattr(alembic.command, name, None)
         if callable(cmd):
-            return lambda *args, **kwargs: cmd(self.config, *args, **kwargs)
+            cfg = super().__getattribute__("config")
+            return lambda *args, **kwargs: cmd(cfg, *args, **kwargs)
         return super().__getattribute__(name)
 
 
 class DbDriver(ABC):
     def __init__(
         self, debug: bool = False, alembic_config: str = "alembic.ini"
     ) -> None:
```

### Comparing `python_glowplug-0.3.1/src/glowplug/driver/mssql.py` & `python_glowplug-0.3.2/src/glowplug/driver/mssql.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.3.1/src/glowplug/driver/pg.py` & `python_glowplug-0.3.2/src/glowplug/driver/pg.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.3.1/src/glowplug/driver/sqlite.py` & `python_glowplug-0.3.2/src/glowplug/driver/sqlite.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.3.1/PKG-INFO` & `python_glowplug-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-glowplug
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Home-page: https://github.com/jnu/python-glowplug
 License: MIT
 Author: Joe Nudell
 Author-email: jnudell@hks.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

