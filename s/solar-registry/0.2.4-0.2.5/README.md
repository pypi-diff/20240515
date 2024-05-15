# Comparing `tmp/solar_registry-0.2.4.tar.gz` & `tmp/solar_registry-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.4.tar", last modified: Tue May 14 07:31:00 2024, max compression
+gzip compressed data, was "solar_registry-0.2.5.tar", last modified: Tue May 14 08:04:02 2024, max compression
```

## Comparing `solar_registry-0.2.4.tar` & `solar_registry-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-05-14 07:30:40.762310 solar_registry-0.2.4/LICENSE
--rw-r--r--   0        0        0      682 2024-05-14 07:30:40.762310 solar_registry-0.2.4/README.md
--rw-r--r--   0        0        0     1182 2024-05-14 07:31:00.970325 solar_registry-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     1880 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4950 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2051 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     2517 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     1998 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/test_testtool.py
--rw-r--r--   0        0        0      291 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/test_validator.py
--rw-r--r--   0        0        0      731 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2778 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     2942 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 solar_registry-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 08:03:41.188820 solar_registry-0.2.5/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-14 08:03:41.188820 solar_registry-0.2.5/README.md
+-rw-r--r--   0        0        0     1182 2024-05-14 08:04:02.041024 solar_registry-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     1880 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     4959 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0     2051 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     2517 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2628 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      505 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     1998 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/test_merger.py
+-rw-r--r--   0        0        0      495 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/test_pr_generator.py
+-rw-r--r--   0        0        0      928 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/test_testtool.py
+-rw-r--r--   0        0        0      291 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/test_validator.py
+-rw-r--r--   0        0        0      731 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/error_meta_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0      736 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/error_version_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0     2778 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     2942 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 solar_registry-0.2.5/PKG-INFO
```

### Comparing `solar_registry-0.2.4/LICENSE` & `solar_registry-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/README.md` & `solar_registry-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/pyproject.toml` & `solar_registry-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.2.4"
+version = "0.2.5"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.2.4/src/solar_registry/cli.py` & `solar_registry-0.2.5/src/solar_registry/cli.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.2.5/src/solar_registry/commands/meta_merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             stable_result = StableIndexMetaData.model_validate_json(f.read())
 
             if not stable_result.tools:
                 stable_result.tools = []
 
             for index, tool in enumerate(stable_result.tools):
                 if tool.name == self.testtool.name:
-                    stable_result.tools[index] = tool
+                    stable_result.tools[index] = self.testtool
                     break
             else:
                 stable_result.tools.append(self.testtool)
 
             logger.info(f"Merge stable index: {stable_result}")
             return stable_result
```

### Comparing `solar_registry-0.2.4/src/solar_registry/model/test_tool.py` & `solar_registry-0.2.5/src/solar_registry/model/test_tool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/src/solar_registry/service/generator.py` & `solar_registry-0.2.5/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/src/solar_registry/service/pr_generator.py` & `solar_registry-0.2.5/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/src/solar_registry/service/validator.py` & `solar_registry-0.2.5/src/solar_registry/service/validator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/src/solar_registry/util/file.py` & `solar_registry-0.2.5/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/tests/test_merger.py` & `solar_registry-0.2.5/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/tests/test_testtool.py` & `solar_registry-0.2.5/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.2.5/tests/testdata/error_meta_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.2.5/tests/testdata/error_version_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.2.5/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.2.5/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.2.5/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.4/PKG-INFO` & `solar_registry-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.2.4
+Version: 0.2.5
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

