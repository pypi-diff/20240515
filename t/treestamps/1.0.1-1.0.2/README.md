# Comparing `tmp/treestamps-1.0.1.tar.gz` & `tmp/treestamps-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treestamps-1.0.1.tar", max compression
+gzip compressed data, was "treestamps-1.0.2.tar", max compression
```

## Comparing `treestamps-1.0.1.tar` & `treestamps-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2024-02-19 00:54:30.275977 treestamps-1.0.1/LICENSE
--rw-r--r--   0        0        0     1583 2024-02-19 00:54:30.275977 treestamps-1.0.1/NEWS.md
--rw-r--r--   0        0        0     1598 2024-02-19 00:54:30.275977 treestamps-1.0.1/README.md
--rw-r--r--   0        0        0     4058 2024-02-19 00:54:30.280311 treestamps-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      501 2024-02-19 00:54:30.280311 treestamps-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0       25 2024-02-19 00:54:30.280311 treestamps-1.0.1/tests/integration/__init__.py
--rw-r--r--   0        0        0      661 2024-02-19 00:54:30.280311 treestamps-1.0.1/tests/integration/base_test.py
--rw-r--r--   0        0        0     1970 2024-02-19 00:54:30.280311 treestamps-1.0.1/tests/integration/test_cycle.py
--rw-r--r--   0        0        0       13 2024-02-19 00:54:30.280311 treestamps-1.0.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     1920 2024-02-19 00:54:30.280311 treestamps-1.0.1/tests/unit/test_classmethods.py
--rw-r--r--   0        0        0      693 2024-02-19 00:54:30.280311 treestamps-1.0.1/tests/unit/test_staticmethods.py
--rw-r--r--   0        0        0      172 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/__init__.py
--rw-r--r--   0        0        0     1533 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/config.py
--rw-r--r--   0        0        0     1961 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/grove.py
--rw-r--r--   0        0        0      300 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/tree/__init__.py
--rw-r--r--   0        0        0     3646 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/tree/common.py
--rw-r--r--   0        0        0     1283 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/tree/dump.py
--rw-r--r--   0        0        0      855 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/tree/get.py
--rw-r--r--   0        0        0     5133 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/tree/load.py
--rw-r--r--   0        0        0     2605 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/tree/set.py
--rw-r--r--   0        0        0     1298 2024-02-19 00:54:30.280311 treestamps-1.0.1/treestamps/tree/write.py
--rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 treestamps-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-15 17:04:00.823537 treestamps-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1648 2024-05-15 17:04:00.823537 treestamps-1.0.2/NEWS.md
+-rw-r--r--   0        0        0     1598 2024-05-15 17:04:00.823537 treestamps-1.0.2/README.md
+-rw-r--r--   0        0        0     4058 2024-05-15 17:04:00.823537 treestamps-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      501 2024-05-15 17:04:00.823537 treestamps-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-15 17:04:00.823537 treestamps-1.0.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0      661 2024-05-15 17:04:00.823537 treestamps-1.0.2/tests/integration/base_test.py
+-rw-r--r--   0        0        0     1970 2024-05-15 17:04:00.823537 treestamps-1.0.2/tests/integration/test_cycle.py
+-rw-r--r--   0        0        0       13 2024-05-15 17:04:00.823537 treestamps-1.0.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1920 2024-05-15 17:04:00.823537 treestamps-1.0.2/tests/unit/test_classmethods.py
+-rw-r--r--   0        0        0      693 2024-05-15 17:04:00.823537 treestamps-1.0.2/tests/unit/test_staticmethods.py
+-rw-r--r--   0        0        0      172 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/config.py
+-rw-r--r--   0        0        0     1961 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/grove.py
+-rw-r--r--   0        0        0      300 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/tree/__init__.py
+-rw-r--r--   0        0        0     3712 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/tree/common.py
+-rw-r--r--   0        0        0     1283 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/tree/dump.py
+-rw-r--r--   0        0        0      855 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/tree/get.py
+-rw-r--r--   0        0        0     5133 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/tree/load.py
+-rw-r--r--   0        0        0     2605 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/tree/set.py
+-rw-r--r--   0        0        0     1298 2024-05-15 17:04:00.823537 treestamps-1.0.2/treestamps/tree/write.py
+-rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 treestamps-1.0.2/PKG-INFO
```

### Comparing `treestamps-1.0.1/LICENSE` & `treestamps-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/NEWS.md` & `treestamps-1.0.2/NEWS.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # 📰 Treestamps News
 
+## v1.0.2
+
+- Indent lists with an offset the way Prettier does.
+
 ## v1.0.1
 
 - Quote yaml keys in wal to handle illegal characters.
 - Fixed incorrect, but still inadequate README docs.
 
 ## v1.0.0
```

### Comparing `treestamps-1.0.1/README.md` & `treestamps-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/pyproject.toml` & `treestamps-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "treestamps"
-version = "1.0.1"
+version = "1.0.2"
 description = "Create timestamp records for recursive operations on directory trees."
 authors = ["AJ Slater <aj@slater.net>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/ajslater/treestamps"
 documentation = "https://github.com/ajslater/treestamps"
 keywords = ["timestamps", "library", "recursive", "directory"]
```

### Comparing `treestamps-1.0.1/tests/integration/base_test.py` & `treestamps-1.0.2/tests/integration/base_test.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/tests/integration/test_cycle.py` & `treestamps-1.0.2/tests/integration/test_cycle.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/tests/unit/test_classmethods.py` & `treestamps-1.0.2/tests/unit/test_classmethods.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/tests/unit/test_staticmethods.py` & `treestamps-1.0.2/tests/unit/test_staticmethods.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/treestamps/config.py` & `treestamps-1.0.2/treestamps/config.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/treestamps/grove.py` & `treestamps-1.0.2/treestamps/grove.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/treestamps/tree/common.py` & `treestamps-1.0.2/treestamps/tree/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,16 @@
         # init variables
         # Do not normalize root_dir because symlinks behave weird.
         root_dir = self.get_dir(self._config.path).absolute()
         # root_dir = normpath(root_dir)
         self.root_dir = root_dir
         self._YAML = YAML()
         self._YAML.allow_duplicate_keys = True
+        # Conform to Prettier
+        self._YAML.indent(offset=2)
         self._filename = self._get_filename(self._config.program_name)
         self._wal_filename = self._get_wal_filename(self._config.program_name)
         self._dump_path = self.root_dir / self._filename
         self._wal_path = self.root_dir / self._wal_filename
         self._wal: TextIO | None = None
         self._consumed_paths: set[Path] = set()
         self._timestamps: dict[Path, float] = {}
```

### Comparing `treestamps-1.0.1/treestamps/tree/dump.py` & `treestamps-1.0.2/treestamps/tree/dump.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/treestamps/tree/get.py` & `treestamps-1.0.2/treestamps/tree/get.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/treestamps/tree/load.py` & `treestamps-1.0.2/treestamps/tree/load.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/treestamps/tree/set.py` & `treestamps-1.0.2/treestamps/tree/set.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/treestamps/tree/write.py` & `treestamps-1.0.2/treestamps/tree/write.py`

 * *Files identical despite different names*

### Comparing `treestamps-1.0.1/PKG-INFO` & `treestamps-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treestamps
-Version: 1.0.1
+Version: 1.0.2
 Summary: Create timestamp records for recursive operations on directory trees.
 Home-page: https://github.com/ajslater/treestamps
 License: GPL-3.0-only
 Keywords: timestamps,library,recursive,directory
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.10,<4.0
```

