# Comparing `tmp/remla24_team8_lib_ml-0.1.1.tar.gz` & `tmp/remla24_team8_lib_ml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla24_team8_lib_ml-0.1.1.tar", max compression
+gzip compressed data, was "remla24_team8_lib_ml-0.1.2.tar", max compression
```

## Comparing `remla24_team8_lib_ml-0.1.1.tar` & `remla24_team8_lib_ml-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      863 2024-05-11 15:54:04.015277 remla24_team8_lib_ml-0.1.1/README.md
--rw-r--r--   0        0        0      407 2024-05-11 15:54:04.015277 remla24_team8_lib_ml-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-11 15:54:04.015277 remla24_team8_lib_ml-0.1.1/src/lib_ml/__init__.py
--rw-r--r--   0        0        0       30 2024-05-11 15:54:04.015277 remla24_team8_lib_ml-0.1.1/src/lib_ml/foo.py
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 remla24_team8_lib_ml-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1544 2024-05-15 16:06:45.899107 remla24_team8_lib_ml-0.1.2/README.md
+-rw-r--r--   0        0        0      490 2024-05-15 16:06:45.899107 remla24_team8_lib_ml-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 16:06:45.899107 remla24_team8_lib_ml-0.1.2/src/lib_ml/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-15 16:06:45.899107 remla24_team8_lib_ml-0.1.2/src/lib_ml/foo.py
+-rw-r--r--   0        0        0     4307 2024-05-15 16:06:45.899107 remla24_team8_lib_ml-0.1.2/src/lib_ml/process_data.py
+-rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 remla24_team8_lib_ml-0.1.2/PKG-INFO
```

### Comparing `remla24_team8_lib_ml-0.1.1/README.md` & `remla24_team8_lib_ml-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,43 @@
 # lib-ml
 
 Contains the pre-processing logic for data that is used for training or queries.
 
 • Factor out the pre-processing logic from the training pipeline.
 
-• Fetch relevant dependencies through a package manager, e.g., by creating a separate requirements.txt.
+• Fetch relevant dependencies through a package manager, e.g., by creating a separate requirements.txt. (DONE)
 
-• The library is versioned automatically, e.g., by picking-up on the corresponding Git version tag.
+• The library is versioned automatically, e.g., by picking-up on the corresponding Git version tag. (DONE)
 
-• A workflow is used to automatically release the library in a package registry that matches the language. (As stated before, this includes either supported package registries on GitHub or repository tags in languages that support it.)
+• A workflow is used to automatically release the library in a package registry that matches the language. (As stated before, this includes either supported package registries on GitHub or repository tags in languages that support it.) (DONE)
+
+## Usage
+
+Install with
+
+```
+pip install remla24-team8-lib-ml
+
+```
+
+Use as
+
+```
+from lib_ml import DataProcessor 
+
+data_processor = DataProcessor()
+
+```
 
 ## Publish a release
 
-To publish a new release, simply create a new release in GitHub with the appropriate tag name. Be sure that this tag name matches the version in the `pyproject.toml`. GitHub Actions will then automatically release and publish this.
+To publish a new release, simply create a new release in GitHub with the appropriate tag name. Be sure that this tag name matches the version in the `pyproject.toml`. GitHub Actions will then automatically release and publish this. If the release failed, then remove the tag while in the Git repo using `git push origin --delete <tag name>`, after which you can then re-release the (now draft) release on GitHub.
+
+When using Poetry, you can also depend on the latest commit using the following dependency:
+
+```
+remla24-team8-lib-ml = { git = "https://github.com/remla24-team8/lib-ml.git", branch = "main" }
+```
+
+### PyPi organization
+
+For now it is owned by tmtenbrink on PyPI, but hopefully we get an organization so we can put it there.
```

### Comparing `remla24_team8_lib_ml-0.1.1/PKG-INFO` & `remla24_team8_lib_ml-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,58 @@
 Metadata-Version: 2.1
 Name: remla24-team8-lib-ml
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Tip ten Brink
 Author-email: T.M.tenBrink@student.tudelft.nl
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: joblib (>=1.4.2,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: tensorflow (>=2.16.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # lib-ml
 
 Contains the pre-processing logic for data that is used for training or queries.
 
 • Factor out the pre-processing logic from the training pipeline.
 
-• Fetch relevant dependencies through a package manager, e.g., by creating a separate requirements.txt.
+• Fetch relevant dependencies through a package manager, e.g., by creating a separate requirements.txt. (DONE)
 
-• The library is versioned automatically, e.g., by picking-up on the corresponding Git version tag.
+• The library is versioned automatically, e.g., by picking-up on the corresponding Git version tag. (DONE)
 
-• A workflow is used to automatically release the library in a package registry that matches the language. (As stated before, this includes either supported package registries on GitHub or repository tags in languages that support it.)
+• A workflow is used to automatically release the library in a package registry that matches the language. (As stated before, this includes either supported package registries on GitHub or repository tags in languages that support it.) (DONE)
+
+## Usage
+
+Install with
+
+```
+pip install remla24-team8-lib-ml
+
+```
+
+Use as
+
+```
+from lib_ml import DataProcessor 
+
+data_processor = DataProcessor()
+
+```
 
 ## Publish a release
 
-To publish a new release, simply create a new release in GitHub with the appropriate tag name. Be sure that this tag name matches the version in the `pyproject.toml`. GitHub Actions will then automatically release and publish this.
+To publish a new release, simply create a new release in GitHub with the appropriate tag name. Be sure that this tag name matches the version in the `pyproject.toml`. GitHub Actions will then automatically release and publish this. If the release failed, then remove the tag while in the Git repo using `git push origin --delete <tag name>`, after which you can then re-release the (now draft) release on GitHub.
+
+When using Poetry, you can also depend on the latest commit using the following dependency:
+
+```
+remla24-team8-lib-ml = { git = "https://github.com/remla24-team8/lib-ml.git", branch = "main" }
+```
+
+### PyPi organization
+
+For now it is owned by tmtenbrink on PyPI, but hopefully we get an organization so we can put it there.
```

