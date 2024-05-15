# Comparing `tmp/galileo_protect-0.6.1.tar.gz` & `tmp/galileo_protect-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_protect-0.6.1.tar", max compression
+gzip compressed data, was "galileo_protect-0.7.0.tar", max compression
```

## Comparing `galileo_protect-0.6.1.tar` & `galileo_protect-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    10946 2024-05-06 22:55:32.556611 galileo_protect-0.6.1/LICENSE
--rw-r--r--   0        0        0      118 2024-05-06 22:55:32.556611 galileo_protect-0.6.1/README.md
--rw-r--r--   0        0        0     2583 2024-05-06 22:55:33.532610 galileo_protect-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      508 2024-05-06 22:55:33.532610 galileo_protect-0.6.1/src/galileo_protect/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/constants/__init__.py
--rw-r--r--   0        0        0       80 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/constants/invoke.py
--rw-r--r--   0        0        0      324 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/constants/routes.py
--rw-r--r--   0        0        0        0 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/helpers/__init__.py
--rw-r--r--   0        0        0      530 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/helpers/config.py
--rw-r--r--   0        0        0     2088 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/invoke.py
--rw-r--r--   0        0        0      638 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/project.py
--rw-r--r--   0        0        0      665 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/schemas/__init__.py
--rw-r--r--   0        0        0      212 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/schemas/invoke.py
--rw-r--r--   0        0        0      308 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/schemas/rule.py
--rw-r--r--   0        0        0      124 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/schemas/stage.py
--rw-r--r--   0        0        0     3529 2024-05-06 22:55:32.560611 galileo_protect-0.6.1/src/galileo_protect/stage.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-05-14 19:28:21.159421 galileo_protect-0.7.0/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-14 19:28:21.159421 galileo_protect-0.7.0/README.md
+-rw-r--r--   0        0        0     2743 2024-05-14 19:28:22.179442 galileo_protect-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      695 2024-05-14 19:28:22.179442 galileo_protect-0.7.0/src/galileo_protect/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/constants/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/constants/invoke.py
+-rw-r--r--   0        0        0      324 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/helpers/__init__.py
+-rw-r--r--   0        0        0      530 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/helpers/config.py
+-rw-r--r--   0        0        0     2095 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/invoke.py
+-rw-r--r--   0        0        0     3190 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/langchain.py
+-rw-r--r--   0        0        0      638 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/project.py
+-rw-r--r--   0        0        0      672 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/schemas/__init__.py
+-rw-r--r--   0        0        0      308 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/schemas/rule.py
+-rw-r--r--   0        0        0      124 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/schemas/stage.py
+-rw-r--r--   0        0        0     3529 2024-05-14 19:28:21.163421 galileo_protect-0.7.0/src/galileo_protect/stage.py
+-rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 galileo_protect-0.7.0/PKG-INFO
```

### Comparing `galileo_protect-0.6.1/LICENSE` & `galileo_protect-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.1/pyproject.toml` & `galileo_protect-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 [tool.poetry]
 name = "galileo-protect"
-version = "0.6.1"
+version = "0.7.0"
 description = "🛡️ Secure your Generative AI applications with Galileo Protect!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_protect", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
-galileo-core = "^0.13.0"
+galileo-core = "^0.15.0"
+langchain-core = { version = "^0.1.52", optional = true }
+
+
+[tool.poetry.extras]
+langchain = ["langchain-core"]
+all = ["langchain-core"]
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.3.4"
 pytest-cov = "^5.0.0"
 pytest-xdist = "^3.5.0"
@@ -76,19 +82,21 @@
 recursive = true
 wrap-summaries = 120
 wrap-descriptions = 120
 
 # Linters.
 [tool.ruff]
 line-length = 120
-ignore = ["D10", "D415"]
 fix = true
+
+[tool.ruff.lint]
+ignore = ["D10", "D415"]
 ignore-init-module-imports = true
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.mypy]
 mypy_path = ["src"]
 disallow_untyped_defs = true
 plugins = ["pydantic.mypy"]
```

### Comparing `galileo_protect-0.6.1/src/galileo_protect/helpers/config.py` & `galileo_protect-0.7.0/src/galileo_protect/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.1/src/galileo_protect/invoke.py` & `galileo_protect-0.7.0/src/galileo_protect/invoke.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Dict, Optional, Sequence
 
+from galileo_core.schemas.protect.response import Response
 from pydantic import UUID4
 from requests import post
 
 from galileo_protect.constants.invoke import TIMEOUT
 from galileo_protect.constants.routes import Routes
 from galileo_protect.helpers.config import ProtectConfig
 from galileo_protect.schemas import Payload, Request, Ruleset
-from galileo_protect.schemas.invoke import Response
 
 
 def invoke(
     payload: Payload,
     prioritized_rulesets: Optional[Sequence[Ruleset]] = None,
     project_id: Optional[UUID4] = None,
     stage_name: Optional[str] = None,
```

### Comparing `galileo_protect-0.6.1/src/galileo_protect/project.py` & `galileo_protect-0.7.0/src/galileo_protect/project.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.6.1/src/galileo_protect/schemas/__init__.py` & `galileo_protect-0.7.0/src/galileo_protect/schemas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 )
 from galileo_core.schemas.protect.metric import (
     MetricComputation,
     MetricComputationStatus,
 )
 from galileo_core.schemas.protect.payload import Payload
 from galileo_core.schemas.protect.request import Request
+from galileo_core.schemas.protect.response import Response
 from galileo_core.schemas.protect.rule import Rule, RuleOperator
 from galileo_core.schemas.protect.ruleset import Ruleset
 from galileo_core.schemas.protect.stage import Stage
 
-from galileo_protect.schemas.invoke import Response
 from galileo_protect.schemas.rule import RuleMetrics
```

### Comparing `galileo_protect-0.6.1/src/galileo_protect/stage.py` & `galileo_protect-0.7.0/src/galileo_protect/stage.py`

 * *Files identical despite different names*

