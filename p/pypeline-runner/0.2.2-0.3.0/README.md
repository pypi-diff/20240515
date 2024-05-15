# Comparing `tmp/pypeline_runner-0.2.2.tar.gz` & `tmp/pypeline_runner-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeline_runner-0.2.2.tar", max compression
+gzip compressed data, was "pypeline_runner-0.3.0.tar", max compression
```

## Comparing `pypeline_runner-0.2.2.tar` & `pypeline_runner-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1066 2024-04-15 08:48:34.906640 pypeline_runner-0.2.2/LICENSE
--rw-r--r--   0        0        0     5929 2024-04-15 08:48:34.906640 pypeline_runner-0.2.2/README.md
--rw-r--r--   0        0        0     3925 2024-04-15 08:48:35.690652 pypeline_runner-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-15 08:48:35.690652 pypeline_runner-0.2.2/src/pypeline/__init__.py
--rw-r--r--   0        0        0      350 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/__run.py
--rw-r--r--   0        0        0        0 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/domain/__init__.py
--rw-r--r--   0        0        0     1355 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/domain/artifacts.py
--rw-r--r--   0        0        0     1663 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/domain/config.py
--rw-r--r--   0        0        0     1101 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/domain/execution_context.py
--rw-r--r--   0        0        0      980 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/domain/pipeline.py
--rw-r--r--   0        0        0      894 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/domain/project_slurper.py
--rw-r--r--   0        0        0        0 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/__init__.py
--rw-r--r--   0        0        0     2235 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/create.py
--rw-r--r--   0        0        0     5772 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1
--rw-r--r--   0        0        0    15971 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/bootstrap/bootstrap.py
--rw-r--r--   0        0        0       13 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/project/.gitignore
--rw-r--r--   0        0        0       34 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/project/poetry.toml
--rw-r--r--   0        0        0       36 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/project/pypeline.ps1
--rw-r--r--   0        0        0      219 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/project/pypeline.yaml
--rw-r--r--   0        0        0      225 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/project/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/project/scoopfile.json
--rw-r--r--   0        0        0      651 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/kickstart/templates/project/steps/my_step.py
--rw-r--r--   0        0        0     3260 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/main.py
--rw-r--r--   0        0        0        0 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/py.typed
--rw-r--r--   0        0        0     4359 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/pypeline.py
--rw-r--r--   0        0        0        0 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/steps/__init__.py
--rw-r--r--   0        0        0     1954 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/steps/create_venv.py
--rw-r--r--   0        0        0     3356 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/steps/scoop_install.py
--rw-r--r--   0        0        0     1930 2024-04-15 08:48:34.910641 pypeline_runner-0.2.2/src/pypeline/steps/west_install.py
--rw-r--r--   0        0        0     7168 1970-01-01 00:00:00.000000 pypeline_runner-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5929 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/README.md
+-rw-r--r--   0        0        0     3903 2024-05-15 18:20:34.066054 pypeline_runner-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-15 18:20:34.070054 pypeline_runner-0.3.0/src/pypeline/__init__.py
+-rw-r--r--   0        0        0      350 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/__run.py
+-rw-r--r--   0        0        0        0 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/domain/__init__.py
+-rw-r--r--   0        0        0     1355 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/domain/artifacts.py
+-rw-r--r--   0        0        0     1650 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/domain/config.py
+-rw-r--r--   0        0        0     1101 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/domain/execution_context.py
+-rw-r--r--   0        0        0     1997 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/domain/pipeline.py
+-rw-r--r--   0        0        0      894 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/domain/project_slurper.py
+-rw-r--r--   0        0        0        0 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/kickstart/__init__.py
+-rw-r--r--   0        0        0     2235 2024-05-15 18:20:32.630051 pypeline_runner-0.3.0/src/pypeline/kickstart/create.py
+-rw-r--r--   0        0        0     5772 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1
+-rw-r--r--   0        0        0    15971 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0       13 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/project/.gitignore
+-rw-r--r--   0        0        0       34 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/project/poetry.toml
+-rw-r--r--   0        0        0       36 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/project/pypeline.ps1
+-rw-r--r--   0        0        0      219 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/project/pypeline.yaml
+-rw-r--r--   0        0        0      225 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/project/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/project/scoopfile.json
+-rw-r--r--   0        0        0      651 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/kickstart/templates/project/steps/my_step.py
+-rw-r--r--   0        0        0     3260 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/main.py
+-rw-r--r--   0        0        0        0 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/py.typed
+-rw-r--r--   0        0        0     8335 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/pypeline.py
+-rw-r--r--   0        0        0        0 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/steps/__init__.py
+-rw-r--r--   0        0        0     1954 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/steps/create_venv.py
+-rw-r--r--   0        0        0     3356 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/steps/scoop_install.py
+-rw-r--r--   0        0        0     1930 2024-05-15 18:20:32.634051 pypeline_runner-0.3.0/src/pypeline/steps/west_install.py
+-rw-r--r--   0        0        0     7156 1970-01-01 00:00:00.000000 pypeline_runner-0.3.0/PKG-INFO
```

### Comparing `pypeline_runner-0.2.2/LICENSE` & `pypeline_runner-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/README.md` & `pypeline_runner-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/pyproject.toml` & `pypeline_runner-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypeline-runner"
-version = "0.2.2"
+version = "0.3.0"
 description = "Configure and execute pipelines with Python (similar to GitHub workflows or Jenkins pipelines)."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/pypeline"
 documentation = "https://pypeline-runner.readthedocs.io"
 classifiers = [
@@ -23,33 +23,33 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/cuinixam/pypeline/issues"
 "Changelog" = "https://github.com/cuinixam/pypeline/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-py-app-dev = "^2.1.1"
-typer = {extras = ["all"], version = "^0.12.0"}
-pyyaml = "^6.0.1"
+py-app-dev = "^2.2"
+typer = {extras = ["all"], version = "^0.12"}
+pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0"
-pre-commit = "^3.1.1"
-ruff = "^0.3.0"
+pre-commit = "^3.1"
+ruff = "^0.3"
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
-sphinxcontrib-mermaid = "^0.8.1"
-mlx-traceability = "^10.0.0"
-sphinx-copybutton = "^0.5.2"
-sphinx-new-tab-link = "^0.2.2"
-sphinx-book-theme = "^1.1.2"
-sphinx-design = "^0.5.0"
+sphinxcontrib-mermaid = "^0.8"
+mlx-traceability = "^10.0"
+sphinx-copybutton = "^0.5"
+sphinx-new-tab-link = "^0.2"
+sphinx-book-theme = "^1.1"
+sphinx-design = "^0.5"
 
 [tool.semantic_release]
 version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variables = [
     "src/pypeline/__init__.py:__version__",
     "docs/conf.py:release",
 ]
```

### Comparing `pypeline_runner-0.2.2/src/pypeline/domain/artifacts.py` & `pypeline_runner-0.3.0/src/pypeline/domain/artifacts.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/domain/config.py` & `pypeline_runner-0.3.0/src/pypeline/domain/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import yaml
 from mashumaro import DataClassDictMixin
 from py_app_dev.core.exceptions import UserNotificationException
-from py_app_dev.core.pipeline import PipelineConfig
 from yaml.parser import ParserError
 from yaml.scanner import ScannerError
 
+from .pipeline import PipelineConfig
+
 
 @dataclass
 class ProjectConfig(DataClassDictMixin):
     pipeline: PipelineConfig
     # This field is intended to keep track of where configuration was loaded from and
     # it is automatically added when configuration is loaded from file
     file: Optional[Path] = None
```

### Comparing `pypeline_runner-0.2.2/src/pypeline/domain/execution_context.py` & `pypeline_runner-0.3.0/src/pypeline/domain/execution_context.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/domain/project_slurper.py` & `pypeline_runner-0.3.0/src/pypeline/domain/project_slurper.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/kickstart/create.py` & `pypeline_runner-0.3.0/src/pypeline/kickstart/create.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1` & `pypeline_runner-0.3.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/kickstart/templates/bootstrap/bootstrap.py` & `pypeline_runner-0.3.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/kickstart/templates/project/steps/my_step.py` & `pypeline_runner-0.3.0/src/pypeline/kickstart/templates/project/steps/my_step.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/main.py` & `pypeline_runner-0.3.0/src/pypeline/main.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/steps/create_venv.py` & `pypeline_runner-0.3.0/src/pypeline/steps/create_venv.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/steps/scoop_install.py` & `pypeline_runner-0.3.0/src/pypeline/steps/scoop_install.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/src/pypeline/steps/west_install.py` & `pypeline_runner-0.3.0/src/pypeline/steps/west_install.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.2.2/PKG-INFO` & `pypeline_runner-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeline-runner
-Version: 0.2.2
+Version: 0.3.0
 Summary: Configure and execute pipelines with Python (similar to GitHub workflows or Jenkins pipelines).
 Home-page: https://github.com/cuinixam/pypeline
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,17 +13,17 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: py-app-dev (>=2.1.1,<3.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: typer[all] (>=0.12.0,<0.13.0)
+Requires-Dist: py-app-dev (>=2.2,<3.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: typer[all] (>=0.12,<0.13)
 Project-URL: Bug Tracker, https://github.com/cuinixam/pypeline/issues
 Project-URL: Changelog, https://github.com/cuinixam/pypeline/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://pypeline-runner.readthedocs.io
 Project-URL: Repository, https://github.com/cuinixam/pypeline
 Description-Content-Type: text/markdown
 
 # Pypeline
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pypeline-runner Version: 0.2.2 Summary: Configure
+Metadata-Version: 2.1 Name: pypeline-runner Version: 0.3.0 Summary: Configure
 and execute pipelines with Python (similar to GitHub workflows or Jenkins
 pipelines). Home-page: https://github.com/cuinixam/pypeline License: MIT
 Author: cuinixam Author-email: me@cuinixam.com Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
-Software Development :: Libraries Requires-Dist: py-app-dev (>=2.1.1,<3.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: typer[all]
-(>=0.12.0,<0.13.0) Project-URL: Bug Tracker, https://github.com/cuinixam/
-pypeline/issues Project-URL: Changelog, https://github.com/cuinixam/pypeline/
-blob/main/CHANGELOG.md Project-URL: Documentation, https://pypeline-
-runner.readthedocs.io Project-URL: Repository, https://github.com/cuinixam/
-pypeline Description-Content-Type: text/markdown # Pypeline
+Software Development :: Libraries Requires-Dist: py-app-dev (>=2.2,<3.0)
+Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: typer[all] (>=0.12,<0.13)
+Project-URL: Bug Tracker, https://github.com/cuinixam/pypeline/issues Project-
+URL: Changelog, https://github.com/cuinixam/pypeline/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://pypeline-runner.readthedocs.io Project-URL:
+Repository, https://github.com/cuinixam/pypeline Description-Content-Type:
+text/markdown # Pypeline
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_r_u_f_f_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 Pypeline is a Python application designed to streamline and automate the
 software development lifecycle, particularly the pipeline execution processes
 across various environments such as GitHub and Jenkins. The primary motivation
 for developing Pypeline stemmed from the need to unify and simplify the
```

