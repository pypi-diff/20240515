# Comparing `tmp/solar_registry-0.2.5.tar.gz` & `tmp/solar_registry-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.5.tar", last modified: Tue May 14 08:04:02 2024, max compression
+gzip compressed data, was "solar_registry-0.2.6.tar", last modified: Wed May 15 06:57:25 2024, max compression
```

## Comparing `solar_registry-0.2.5.tar` & `solar_registry-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-05-14 08:03:41.188820 solar_registry-0.2.5/LICENSE
--rw-r--r--   0        0        0      682 2024-05-14 08:03:41.188820 solar_registry-0.2.5/README.md
--rw-r--r--   0        0        0     1182 2024-05-14 08:04:02.041024 solar_registry-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     1880 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4959 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2051 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     2517 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     1998 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-14 08:03:41.192820 solar_registry-0.2.5/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/test_testtool.py
--rw-r--r--   0        0        0      291 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/test_validator.py
--rw-r--r--   0        0        0      731 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2778 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     2942 2024-05-14 08:03:41.192820 solar_registry-0.2.5/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 solar_registry-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 06:57:03.452157 solar_registry-0.2.6/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-15 06:57:03.452157 solar_registry-0.2.6/README.md
+-rw-r--r--   0        0        0     1240 2024-05-15 06:57:25.944105 solar_registry-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 06:57:03.452157 solar_registry-0.2.6/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-15 06:57:03.452157 solar_registry-0.2.6/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     4959 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0     2120 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     3942 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/cos_sync.py
+-rw-r--r--   0        0        0     2517 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2628 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      505 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     2068 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-15 06:57:03.456157 solar_registry-0.2.6/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0      364 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_cos_sync.py
+-rw-r--r--   0        0        0      680 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_merger.py
+-rw-r--r--   0        0        0      495 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_pr_generator.py
+-rw-r--r--   0        0        0      928 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_testtool.py
+-rw-r--r--   0        0        0      291 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/test_validator.py
+-rw-r--r--   0        0        0      731 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/error_meta_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0      736 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/error_version_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0     2778 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     2942 2024-05-15 06:57:03.456157 solar_registry-0.2.6/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.2.6/PKG-INFO
```

### Comparing `solar_registry-0.2.5/LICENSE` & `solar_registry-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/README.md` & `solar_registry-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/pyproject.toml` & `solar_registry-0.2.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "solar-registry"
-version = "0.2.5"
+version = "0.2.6"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
     "typer>=0.12.3",
     "pyyaml>=6.0.1",
     "retry>=0.9.2",
     "loguru>=0.7.2",
+    "cos-python-sdk-v5>=1.9.28",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
@@ -47,8 +48,9 @@
     "pytest>=8.2.0",
     "mypy>=1.10.0",
     "types-requests>=2.31.0.20240406",
     "types-retry>=0.9.9.4",
     "types-PyYAML>=6.0.12.20240311",
     "pytest-cov>=5.0.0",
     "ruff>=0.4.4",
+    "pytest-env>=1.1.3",
 ]
```

### Comparing `solar_registry-0.2.5/src/solar_registry/cli.py` & `solar_registry-0.2.6/src/solar_registry/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional
 
 import typer
 from loguru import logger
 from typing_extensions import Annotated
 
 from .commands.meta_merger import MetaMerger
+from .service.cos_sync import CosSyncService
 from .service.pr_generator import PullRequestGenerator
 from .service.testtool import get_testtool
 from .service.validator import ToolValidator
 
 app = typer.Typer()
 
 
@@ -59,13 +60,23 @@
 
     :param working_dir: 可选工作目录
     """
     validator = ToolValidator(working_dir)
     validator.validate()
 
 
+def sync_cos(working_dir: Optional[str] = None) -> None:
+    """
+    同步数据到COS上
+
+    :param working_dir: 可选工作目录
+    """
+    sync = CosSyncService(working_dir)
+    sync.sync_meta_data()
+
+
 def cli_entry() -> None:
     app()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `solar_registry-0.2.5/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.2.6/src/solar_registry/commands/meta_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/src/solar_registry/model/test_tool.py` & `solar_registry-0.2.6/src/solar_registry/model/test_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     name: str
     value: str
     default: str
     choices: list[ParamChoice] | None = None
 
 
 class TestTool(BaseModel):
+
+    __test__ = False
+
     """
     测试工具模型定义
     """
 
     schema_version: float = Field(alias="schemaVersion")
 
     # 必须是小写英文字母
@@ -53,14 +56,17 @@
 
 class ArchType(str, Enum):
     Amd64 = "amd64"
     Arm64 = "arm64"
 
 
 class TestToolTarget(BaseModel):
+
+    __test__ = False
+
     """
     发布包模型定义
     """
 
     os: OsType
     arch: ArchType
     download_url: str = Field(alias="downloadUrl")
@@ -73,14 +79,17 @@
     """
 
     meta_version: str = Field("1", alias="metaVersion")
     tools: list[TestTool]
 
 
 class TestToolMetadata(BaseModel):
+
+    __test__ = False
+
     """
     通过solar-registry生成的最新版本发布元数据
 
     包含元数据信息和target信息
     """
 
     meta: TestTool
```

### Comparing `solar_registry-0.2.5/src/solar_registry/service/generator.py` & `solar_registry-0.2.6/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/src/solar_registry/service/pr_generator.py` & `solar_registry-0.2.6/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/src/solar_registry/service/validator.py` & `solar_registry-0.2.6/src/solar_registry/service/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,12 +38,14 @@
                     with open(metafile) as f:
                         re = MetaDataHistory.model_validate_json(f.read())
                         if re.versions:
                             # 检查versions中是否有重复版本
                             all_versions = set(x.meta.version for x in re.versions)
 
                             if len(all_versions) != len(re.versions):
-                                raise RuntimeError(f"去重之后的版本数目 [{len(all_versions)}] != 原始版本数目 [{len(re.versions)}]")
+                                raise RuntimeError(
+                                    f"去重之后的版本数目 [{len(all_versions)}] != 原始版本数目 [{len(re.versions)}]"
+                                )
 
                             logger.info(
                                 f"✅ Validated tool [{re.versions[0].meta.name}] OK."
                             )
```

### Comparing `solar_registry-0.2.5/src/solar_registry/util/file.py` & `solar_registry-0.2.6/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/tests/test_merger.py` & `solar_registry-0.2.6/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/tests/test_testtool.py` & `solar_registry-0.2.6/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.2.6/tests/testdata/error_meta_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.2.6/tests/testdata/error_version_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.2.6/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.5/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.2.6/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'versions'": "{0: {'meta': {'version': '0.1.4'}}}"}*

```diff
@@ -54,15 +54,15 @@
                         "default": "",
                         "name": "extraFieldsConfig",
                         "value": "\u7528\u4f8b\u989d\u5916\u5c5e\u6027"
                     }
                 ],
                 "scaffoldRepo": "https://github.com/OpenTestSolar/testtool-scaffold-python-pytest/archive/refs/tags/0.1.0.tar.gz",
                 "schemaVersion": 1.0,
-                "version": "0.1.3",
+                "version": "0.1.4",
                 "versionFile": "https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/python/pytest/metadata.json"
             },
             "target": [
                 {
                     "arch": "amd64",
                     "downloadUrl": "https://github.com/xxx/python/qta/v0.4.7/win_amd64.tar.gz",
                     "os": "windows",
```

### Comparing `solar_registry-0.2.5/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.2.6/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'tools'": "{0: {'version': '0.1.4'}}"}*

```diff
@@ -53,12 +53,12 @@
                     "default": "",
                     "name": "extraFieldsConfig",
                     "value": "\u7528\u4f8b\u989d\u5916\u5c5e\u6027"
                 }
             ],
             "scaffoldRepo": "https://github.com/OpenTestSolar/testtool-scaffold-python-pytest/archive/refs/tags/0.1.0.tar.gz",
             "schemaVersion": 1.0,
-            "version": "0.1.3",
+            "version": "0.1.4",
             "versionFile": "https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/python/pytest/metadata.json"
         }
     ]
 }
```

### Comparing `solar_registry-0.2.5/PKG-INFO` & `solar_registry-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.2.5
+Version: 0.2.6
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Requires-Python: >=3.11
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic>=2.7.1
 Requires-Dist: typer>=0.12.3
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: retry>=0.9.2
 Requires-Dist: loguru>=0.7.2
+Requires-Dist: cos-python-sdk-v5>=1.9.28
 Description-Content-Type: text/markdown
 
 # solar-registry
 命令行工具`solar-registry`，提供以下功能：
 
 - 根据测试工具的`testtool.yaml`生成对应的元数据信息
 - 读取最新的元数据文件并合并
```

