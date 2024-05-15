# Comparing `tmp/oida-0.2.0.tar.gz` & `tmp/oida-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oida-0.2.0.tar", max compression
+gzip compressed data, was "oida-0.2.1.tar", max compression
```

## Comparing `oida-0.2.0.tar` & `oida-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     3663 2023-05-04 12:53:25.672179 oida-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 12:53:25.672179 oida-0.2.0/oida/__init__.py
--rw-r--r--   0        0        0       65 2023-05-04 12:53:25.672179 oida-0.2.0/oida/__main__.py
--rw-r--r--   0        0        0      616 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/__init__.py
--rw-r--r--   0        0        0     1628 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/base.py
--rw-r--r--   0        0        0     7001 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/components.py
--rw-r--r--   0        0        0     4325 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/config.py
--rw-r--r--   0        0        0     1334 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/imports.py
--rw-r--r--   0        0        0      190 2023-05-04 12:53:25.672179 oida-0.2.0/oida/commands/__init__.py
--rw-r--r--   0        0        0     9720 2023-05-04 12:53:25.672179 oida-0.2.0/oida/commands/componentize.py
--rw-r--r--   0        0        0     1007 2023-05-04 12:53:25.672179 oida-0.2.0/oida/commands/config.py
--rw-r--r--   0        0        0     1177 2023-05-04 12:53:25.672179 oida-0.2.0/oida/commands/linter.py
--rw-r--r--   0        0        0     1419 2023-05-04 12:53:25.672179 oida-0.2.0/oida/config.py
--rw-r--r--   0        0        0     5568 2023-05-04 12:53:25.672179 oida-0.2.0/oida/config_generator.py
--rw-r--r--   0        0        0     1875 2023-05-04 12:53:25.672179 oida-0.2.0/oida/console.py
--rw-r--r--   0        0        0     3755 2023-05-04 12:53:25.672179 oida-0.2.0/oida/discovery.py
--rw-r--r--   0        0        0     1245 2023-05-04 12:53:25.672179 oida-0.2.0/oida/flake8.py
--rw-r--r--   0        0        0      548 2023-05-04 12:53:25.672179 oida-0.2.0/oida/module.py
--rw-r--r--   0        0        0      985 2023-05-04 12:53:25.672179 oida-0.2.0/oida/utils.py
--rw-r--r--   0        0        0     1869 2023-05-04 12:53:25.676179 oida-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 oida-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-15 07:55:03.209633 oida-0.2.1/LICENCE
+-rw-r--r--   0        0        0     3663 2024-05-15 07:55:03.209633 oida-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 07:55:03.209633 oida-0.2.1/oida/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-15 07:55:03.209633 oida-0.2.1/oida/__main__.py
+-rw-r--r--   0        0        0      616 2024-05-15 07:55:03.209633 oida-0.2.1/oida/checkers/__init__.py
+-rw-r--r--   0        0        0     1628 2024-05-15 07:55:03.209633 oida-0.2.1/oida/checkers/base.py
+-rw-r--r--   0        0        0     7001 2024-05-15 07:55:03.209633 oida-0.2.1/oida/checkers/components.py
+-rw-r--r--   0        0        0     4325 2024-05-15 07:55:03.209633 oida-0.2.1/oida/checkers/config.py
+-rw-r--r--   0        0        0     1334 2024-05-15 07:55:03.209633 oida-0.2.1/oida/checkers/imports.py
+-rw-r--r--   0        0        0      190 2024-05-15 07:55:03.209633 oida-0.2.1/oida/commands/__init__.py
+-rw-r--r--   0        0        0     9720 2024-05-15 07:55:03.209633 oida-0.2.1/oida/commands/componentize.py
+-rw-r--r--   0        0        0     1007 2024-05-15 07:55:03.209633 oida-0.2.1/oida/commands/config.py
+-rw-r--r--   0        0        0     1177 2024-05-15 07:55:03.209633 oida-0.2.1/oida/commands/linter.py
+-rw-r--r--   0        0        0      420 2024-05-15 07:55:03.209633 oida-0.2.1/oida/component.py
+-rw-r--r--   0        0        0     1419 2024-05-15 07:55:03.209633 oida-0.2.1/oida/config.py
+-rw-r--r--   0        0        0     5808 2024-05-15 07:55:03.209633 oida-0.2.1/oida/config_generator.py
+-rw-r--r--   0        0        0     2255 2024-05-15 07:55:03.209633 oida-0.2.1/oida/console.py
+-rw-r--r--   0        0        0     6085 2024-05-15 07:55:03.209633 oida-0.2.1/oida/discovery.py
+-rw-r--r--   0        0        0     1245 2024-05-15 07:55:03.209633 oida-0.2.1/oida/flake8.py
+-rw-r--r--   0        0        0      548 2024-05-15 07:55:03.209633 oida-0.2.1/oida/module.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:55:03.209633 oida-0.2.1/oida/statistics/__init__.py
+-rw-r--r--   0        0        0     6145 2024-05-15 07:55:03.209633 oida-0.2.1/oida/statistics/statistics_generator.py
+-rw-r--r--   0        0        0      985 2024-05-15 07:55:03.209633 oida-0.2.1/oida/utils.py
+-rw-r--r--   0        0        0     1869 2024-05-15 07:55:03.209633 oida-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4752 1970-01-01 00:00:00.000000 oida-0.2.1/PKG-INFO
```

### Comparing `oida-0.2.0/README.md` & `oida-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/checkers/__init__.py` & `oida-0.2.1/oida/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/checkers/base.py` & `oida-0.2.1/oida/checkers/base.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/checkers/components.py` & `oida-0.2.1/oida/checkers/components.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/checkers/config.py` & `oida-0.2.1/oida/checkers/config.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/checkers/imports.py` & `oida-0.2.1/oida/checkers/imports.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/commands/componentize.py` & `oida-0.2.1/oida/commands/componentize.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/commands/config.py` & `oida-0.2.1/oida/commands/config.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/commands/linter.py` & `oida-0.2.1/oida/commands/linter.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/config.py` & `oida-0.2.1/oida/config.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/config_generator.py` & `oida-0.2.1/oida/config_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,20 +124,26 @@
     """
 
     if not violations:
         return cst.RemovalSentinel
 
     if node.value and m.matches(node.value, m.Set()):
         value = ensure_type(node.value, cst.Set)
-        current_rules: set[str] = {
+        current_rules = {
             ensure_type(element.value, cst.SimpleString).evaluated_value
             for element in value.elements
         }
 
-        updated_rules = update_allowed_imports(current_rules, violations)
+        # Make sure all items in the set where string literals
+        if not all(isinstance(rule, str) for rule in current_rules):
+            raise ValueError("Found bytes literal in ALLOWED_IMPORTS setting")
+
+        updated_rules = update_allowed_imports(
+            cast(set[str], current_rules), violations
+        )
 
         new_elements = [
             element
             for element in value.elements
             if ensure_type(element.value, cst.SimpleString).evaluated_value
             in updated_rules
         ]
```

### Comparing `oida-0.2.0/oida/console.py` & `oida-0.2.1/oida/console.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
-import os
 import sys
 from pathlib import Path
 
+from oida.statistics.statistics_generator import generate_statistics
+
 from .checkers import get_checkers
 from .commands import componentize_app, generate_config, run_linter
 
 
 def main() -> None:
 
     parser = argparse.ArgumentParser(description="Django project linter.")
@@ -34,28 +35,37 @@
         "config",
         help="Generate component config files that whitelist all isolation violations",
     )
     config_parser.add_argument(
         "project_root", type=Path, help="Path to project root directory"
     )
 
+    config_parser = subparsers.add_parser(
+        "statistics",
+        help="Generate statistics about the modularization state",
+    )
+    config_parser.add_argument(
+        "project_root", type=Path, help="Path to project root directory"
+    )
+
     componentize_parser = subparsers.add_parser(
         "componentize",
         help=componentize_app.__doc__,
     )
     componentize_parser.add_argument("old_path", type=Path, help="Current path to app")
     componentize_parser.add_argument("new_path", type=Path, help="Path to move app to")
 
     args = parser.parse_args()
 
-    # Needed to parse Python 3.10 documents
-    os.environ.setdefault("LIBCST_PARSER_TYPE", "native")
-
     if args.command == "lint":
-        if not run_linter(*args.paths, checks=args.checks):
+        has_violations = run_linter(*args.paths, checks=args.checks)
+        if has_violations:
             sys.exit(1)
     elif args.command == "config":
         generate_config(args.project_root)
+    elif args.command == "statistics":
+        statistics = generate_statistics(args.project_root)
+        print(f"{statistics.json()}")
     elif args.command == "componentize":
         componentize_app(args.old_path, args.new_path)
     else:
         sys.exit(f"Unknown command: {args.command}")
```

### Comparing `oida-0.2.0/oida/flake8.py` & `oida-0.2.1/oida/flake8.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/module.py` & `oida-0.2.1/oida/module.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/oida/utils.py` & `oida-0.2.1/oida/utils.py`

 * *Files identical despite different names*

### Comparing `oida-0.2.0/pyproject.toml` & `oida-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oida"
-version = "0.2.0"
+version = "0.2.1"
 description = "Oida is Oda's linter that enforces code style and modularization in our Django projects."
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/oida"
 repository = "https://github.com/kolonialno/oida"
 classifiers = [
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-libcst = "^0.4.3"
+libcst = "^1.0.0"
 tomli = {version = ">=1.0.0", python = "<3.11"}
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 isort = "^5.10.1"
 mypy = "^0.971"
 flake8 = "^5.0.4"
```

### Comparing `oida-0.2.0/PKG-INFO` & `oida-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oida
-Version: 0.2.0
+Version: 0.2.1
 Summary: Oida is Oda's linter that enforces code style and modularization in our Django projects.
 Home-page: https://github.com/kolonialno/oida
 License: MIT
 Author: Oda
 Author-email: tech@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,19 +13,18 @@
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Dist: libcst (>=0.4.3,<0.5.0)
+Requires-Dist: libcst (>=1.0.0,<2.0.0)
 Requires-Dist: tomli (>=1.0.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/kolonialno/oida
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   💅<br>
   Oida
```

