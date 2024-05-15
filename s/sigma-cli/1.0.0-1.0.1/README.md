# Comparing `tmp/sigma_cli-1.0.0.tar.gz` & `tmp/sigma_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigma_cli-1.0.0.tar", max compression
+gzip compressed data, was "sigma_cli-1.0.1.tar", max compression
```

## Comparing `sigma_cli-1.0.0.tar` & `sigma_cli-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3775 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/README.md
--rw-r--r--   0        0        0     1040 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1747 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/analyze/attack.py
--rw-r--r--   0        0        0     3201 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/cli/analyze.py
--rw-r--r--   0        0        0     8953 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/cli/check.py
--rw-r--r--   0        0        0    11019 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/cli/convert.py
--rw-r--r--   0        0        0     6594 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/cli/list.py
--rw-r--r--   0        0        0     2046 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/cli/main.py
--rw-r--r--   0        0        0     7046 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/cli/plugin.py
--rw-r--r--   0        0        0     2986 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/cli/pysigma.py
--rw-r--r--   0        0        0      767 2024-01-29 23:29:23.835758 sigma_cli-1.0.0/sigma/cli/rules.py
--rw-r--r--   0        0        0     4884 1970-01-01 00:00:00.000000 sigma_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3775 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/README.md
+-rw-r--r--   0        0        0     1040 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1747 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/analyze/attack.py
+-rw-r--r--   0        0        0     3201 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/cli/analyze.py
+-rw-r--r--   0        0        0     8953 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/cli/check.py
+-rw-r--r--   0        0        0    11019 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/cli/convert.py
+-rw-r--r--   0        0        0     6594 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/cli/list.py
+-rw-r--r--   0        0        0     2046 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/cli/main.py
+-rw-r--r--   0        0        0     7046 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/cli/plugin.py
+-rw-r--r--   0        0        0     2986 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/cli/pysigma.py
+-rw-r--r--   0        0        0      813 2024-02-18 01:00:55.308200 sigma_cli-1.0.1/sigma/cli/rules.py
+-rw-r--r--   0        0        0     4884 1970-01-01 00:00:00.000000 sigma_cli-1.0.1/PKG-INFO
```

### Comparing `sigma_cli-1.0.0/README.md` & `sigma_cli-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/pyproject.toml` & `sigma_cli-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sigma-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = "Sigma Command Line Interface (conversion, check etc.) based on pySigma"
 authors = ["Thomas Patzke <thomas@patzke.org>"]
 license = "LGPL-2.1-or-later"
 readme = "README.md"
 repository = "https://github.com/SigmaHQ/sigma-cli"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `sigma_cli-1.0.0/sigma/analyze/attack.py` & `sigma_cli-1.0.1/sigma/analyze/attack.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/sigma/cli/analyze.py` & `sigma_cli-1.0.1/sigma/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/sigma/cli/check.py` & `sigma_cli-1.0.1/sigma/cli/check.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/sigma/cli/convert.py` & `sigma_cli-1.0.1/sigma/cli/convert.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/sigma/cli/list.py` & `sigma_cli-1.0.1/sigma/cli/list.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/sigma/cli/main.py` & `sigma_cli-1.0.1/sigma/cli/main.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/sigma/cli/plugin.py` & `sigma_cli-1.0.1/sigma/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/sigma/cli/pysigma.py` & `sigma_cli-1.0.1/sigma/cli/pysigma.py`

 * *Files identical despite different names*

### Comparing `sigma_cli-1.0.0/sigma/cli/rules.py` & `sigma_cli-1.0.1/sigma/cli/rules.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,8 +15,9 @@
         with click.progressbar(
             list(rule_paths), label="Parsing Sigma rules", file=stderr
         ) as progress_rule_paths:
             rule_collection = SigmaCollection.load_ruleset(
                 progress_rule_paths,
                 collect_errors=True,
             )
+    rule_collection.resolve_rule_references()
     return rule_collection
```

### Comparing `sigma_cli-1.0.0/PKG-INFO` & `sigma_cli-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigma-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sigma Command Line Interface (conversion, check etc.) based on pySigma
 Home-page: https://github.com/SigmaHQ/sigma-cli
 License: LGPL-2.1-or-later
 Author: Thomas Patzke
 Author-email: thomas@patzke.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

