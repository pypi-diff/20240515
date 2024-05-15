# Comparing `tmp/solar_registry-0.2.6.tar.gz` & `tmp/solar_registry-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.6.tar", last modified: Wed May 15 06:57:25 2024, max compression
+gzip compressed data, was "solar_registry-0.2.7.tar", last modified: Wed May 15 07:08:54 2024, max compression
```

## Comparing `solar_registry-0.2.6.tar` & `solar_registry-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-05-15 06:57:03.452157 solar_registry-0.2.6/LICENSE
--rw-r--r--   0        0        0      682 2024-05-15 06:57:03.452157 solar_registry-0.2.6/README.md
--rw-r--r--   0        0        0     1240 2024-05-15 06:57:25.944105 solar_registry-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 06:57:03.452157 solar_registry-0.2.6/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-15 06:57:03.452157 solar_registry-0.2.6/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4959 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2120 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     3942 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/cos_sync.py
--rw-r--r--   0        0        0     2517 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     2068 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0      364 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_cos_sync.py
--rw-r--r--   0        0        0      680 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_testtool.py
--rw-r--r--   0        0        0      291 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_validator.py
--rw-r--r--   0        0        0      731 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2778 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     2942 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 07:08:31.581664 solar_registry-0.2.7/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-15 07:08:31.581664 solar_registry-0.2.7/README.md
+-rw-r--r--   0        0        0     1240 2024-05-15 07:08:54.149713 solar_registry-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     2158 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     4959 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0     2120 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     3942 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/cos_sync.py
+-rw-r--r--   0        0        0     2517 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2628 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      505 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     2068 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0      364 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_cos_sync.py
+-rw-r--r--   0        0        0      680 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_merger.py
+-rw-r--r--   0        0        0      495 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_pr_generator.py
+-rw-r--r--   0        0        0      928 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_testtool.py
+-rw-r--r--   0        0        0      291 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_validator.py
+-rw-r--r--   0        0        0      731 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/testdata/error_meta_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0      736 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/testdata/error_version_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0     2778 2024-05-15 07:08:31.585665 solar_registry-0.2.7/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-15 07:08:31.585665 solar_registry-0.2.7/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     2942 2024-05-15 07:08:31.585665 solar_registry-0.2.7/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.2.7/PKG-INFO
```

### Comparing `solar_registry-0.2.6/LICENSE` & `solar_registry-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/README.md` & `solar_registry-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/pyproject.toml` & `solar_registry-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.2.6"
+version = "0.2.7"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.2.6/src/solar_registry/cli.py` & `solar_registry-0.2.7/src/solar_registry/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     testtool = get_testtool(tool_name, working_dir)
     merger = MetaMerger(testtool)
     merger.merge_index_and_history(Path(output))
 
 
 @app.command()
 def pull_request(
-    tool_name: Annotated[str, typer.Argument(help="工具名称")],
-    working_dir: Annotated[Optional[str], typer.Argument(help="可选工作目录")] = None,
+        tool_name: Annotated[str, typer.Argument(help="工具名称")],
+        working_dir: Annotated[Optional[str], typer.Argument(help="可选工作目录")] = None,
 ) -> None:
     """
     合并元数据之后，向项目提PR进行合并操作
     """
     testtool = get_testtool(tool_name, working_dir)
     pr_gen = PullRequestGenerator(testtool)
     pr_gen.merge_and_create_pull_request()
@@ -60,14 +60,15 @@
 
     :param working_dir: 可选工作目录
     """
     validator = ToolValidator(working_dir)
     validator.validate()
 
 
+@app.command()
 def sync_cos(working_dir: Optional[str] = None) -> None:
     """
     同步数据到COS上
 
     :param working_dir: 可选工作目录
     """
     sync = CosSyncService(working_dir)
```

### Comparing `solar_registry-0.2.6/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.2.7/src/solar_registry/commands/meta_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/src/solar_registry/model/test_tool.py` & `solar_registry-0.2.7/src/solar_registry/model/test_tool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/src/solar_registry/service/cos_sync.py` & `solar_registry-0.2.7/src/solar_registry/service/cos_sync.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/src/solar_registry/service/generator.py` & `solar_registry-0.2.7/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/src/solar_registry/service/pr_generator.py` & `solar_registry-0.2.7/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/src/solar_registry/service/validator.py` & `solar_registry-0.2.7/src/solar_registry/service/validator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/src/solar_registry/util/file.py` & `solar_registry-0.2.7/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/tests/test_merger.py` & `solar_registry-0.2.7/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/tests/test_testtool.py` & `solar_registry-0.2.7/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.2.7/tests/testdata/error_meta_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.2.7/tests/testdata/error_version_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.2.7/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.2.7/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.2.7/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.6/PKG-INFO` & `solar_registry-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.2.6
+Version: 0.2.7
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

