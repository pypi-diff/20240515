# Comparing `tmp/process_time_azure_devops-0.0.7.tar.gz` & `tmp/process_time_azure_devops-0.0.8.tar.gz`

## Comparing `process_time_azure_devops-0.0.7.tar` & `process_time_azure_devops-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/azure-pipelines.yml
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.github/workflows/pr.yml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/process-time-azure-devops.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/__init__.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/arts/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/arts/process_time_logo.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/models/ArgumentParseResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/parsers/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/tests/generate_test_run.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/tests/test_get_last_attempt_to_deliver.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/LICENSE
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/README.md
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/azure-pipelines.yml
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.github/workflows/pr.yml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.idea/process-time-azure-devops.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/src/process_time_azure_devops/__init__.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/src/process_time_azure_devops/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/src/process_time_azure_devops/arts/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/src/process_time_azure_devops/arts/process_time_logo.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/src/process_time_azure_devops/models/ArgumentParseResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/src/process_time_azure_devops/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/src/process_time_azure_devops/parsers/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/tests/generate_test_run.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/tests/test_get_last_attempt_to_deliver.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/README.md
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.8/PKG-INFO
```

### Comparing `process_time_azure_devops-0.0.7/.github/workflows/pr.yml` & `process_time_azure_devops-0.0.8/.github/workflows/pr.yml`

 * *Files 10% similar despite different names*

```diff
@@ -76,12 +76,17 @@
           pip install .[test]
       - name: Build
         run: |
           pip install build
           python -m build .
       - name: Install
         run: |
-          pip install dist/process_time_azure_devops-0.0.5-py3-none-any.whl
+          # Path to the pyproject.toml file
+          file_path="pyproject.toml"
+          # Use grep to find the line with 'version' and then use awk to print the version value
+          version=$(grep 'version =' $file_path | awk -F'"' '{print $2}')
+          # Install the package
+          pip install dist/process_time_azure_devops-$version-py3-none-any.whl
       - name: Test Help -h
         run: |
           pip list
           python -m process_time_azure_devops -h
```

### Comparing `process_time_azure_devops-0.0.7/.github/workflows/publish.yml` & `process_time_azure_devops-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.7/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py` & `process_time_azure_devops-0.0.8/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.7/tests/test_get_last_attempt_to_deliver.py` & `process_time_azure_devops-0.0.8/tests/test_get_last_attempt_to_deliver.py`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.7/.gitignore` & `process_time_azure_devops-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.7/LICENSE` & `process_time_azure_devops-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.7/pyproject.toml` & `process_time_azure_devops-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/process_time_azure_devops"]
 
 [project]
 name = "process_time_azure_devops"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name="Andrei Kniazev" },
 ]
 description = "Will collect process time for projects that are hosted in Azure DevOps"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
```

### Comparing `process_time_azure_devops-0.0.7/PKG-INFO` & `process_time_azure_devops-0.0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: process_time_azure_devops
-Version: 0.0.7
+Version: 0.0.8
 Summary: Will collect process time for projects that are hosted in Azure DevOps
 Project-URL: GitHub, https://github.com/worldpwn/process-time-azure-devops
 Project-URL: Issues, https://github.com/worldpwn/process-time-azure-devops/issues
 Author: Andrei Kniazev
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
@@ -18,31 +18,28 @@
 Requires-Dist: pytest==8.2.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Publish](https://github.com/worldpwn/process-time-azure-devops/actions/workflows/publish.yml/badge.svg)](https://github.com/worldpwn/process-time-azure-devops/actions/workflows/publish.yml)
 <a href="https://pypi.org/project/process-time-azure-devops/"><img alt="PyPI" src="https://img.shields.io/pypi/v/process-time-azure-devops"></a>
 <img width="1597" alt="image" src="https://github.com/worldpwn/process-time-azure-devops/assets/6351780/d8adb7ce-e284-48e2-a56b-65ead73b17a6">
 
-# Local Dev
-Build project with a watch-like mode.
 
-```bash
-python -m pip install -e .
-```
-# Test
-Install Dependencies for Tests
-```bash
-py -m pip install -e .[test]
-```
-Run Tests
-```bash
-py -m pytest tests --verbose
-```
-# Run
-```bash
-py src/example.py
-```
+# Tutorial
+## Azure Devops repository Access
+To access repository in Azure DevOps with pipline access token you need either run pipeline.yml file from the repository itself or reference needed repository in reosource.
+```yml
+resources:
+  repositories:
+    - repository: process-time
+      type: git
+      name: process-time
+      ref: main
 
-# Build
-```bash
-py src/main
+steps:
+- checkout: process-time
+- checkout: self
+- script: |
+    # do something
+  displayName: 'Can access both repositories'
+  env:
+    System.AccessToken: $(System.AccessToken)
 ```
```

#### html2text {}

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 2.3 Name: process_time_azure_devops Version: 0.0.7 Summary:
+Metadata-Version: 2.3 Name: process_time_azure_devops Version: 0.0.8 Summary:
 Will collect process time for projects that are hosted in Azure DevOps Project-
 URL: GitHub, https://github.com/worldpwn/process-time-azure-devops Project-URL:
 Issues, https://github.com/worldpwn/process-time-azure-devops/issues Author:
 Andrei Kniazev License-Expression: GPL-3.0-or-later License-File: LICENSE
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.8 Provides-Extra: build Requires-Dist:
 azure-devops==7.1.0b4; extra == 'build' Requires-Dist: hatchling==1.24.2; extra
 == 'build' Provides-Extra: test Requires-Dist: azure-devops==7.1.0b4; extra ==
 'test' Requires-Dist: pytest==8.2.0; extra == 'test' Description-Content-Type:
 text/markdown [![Publish](https://github.com/worldpwn/process-time-azure-
 devops/actions/workflows/publish.yml/badge.svg)](https://github.com/worldpwn/
-process-time-azure-devops/actions/workflows/publish.yml) _[_P_y_P_I_][image]# Local
-Dev Build project with a watch-like mode. ```bash python -m pip install -e .
-``` # Test Install Dependencies for Tests ```bash py -m pip install -e .[test]
-``` Run Tests ```bash py -m pytest tests --verbose ``` # Run ```bash py src/
-example.py ``` # Build ```bash py src/main ```
+process-time-azure-devops/actions/workflows/publish.yml) _[_P_y_P_I_][image]#
+Tutorial ## Azure Devops repository Access To access repository in Azure DevOps
+with pipline access token you need either run pipeline.yml file from the
+repository itself or reference needed repository in reosource. ```yml
+resources: repositories: - repository: process-time type: git name: process-
+time ref: main steps: - checkout: process-time - checkout: self - script: | #
+do something displayName: 'Can access both repositories' env:
+System.AccessToken: $(System.AccessToken) ```
```

