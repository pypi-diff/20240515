# Comparing `tmp/poetry_plugin_lambda_build-0.5.3.tar.gz` & `tmp/poetry_plugin_lambda_build-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_lambda_build-0.5.3.tar", max compression
+gzip compressed data, was "poetry_plugin_lambda_build-0.5.5.tar", max compression
```

## Comparing `poetry_plugin_lambda_build-0.5.3.tar` & `poetry_plugin_lambda_build-0.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-05-14 08:44:58.698134 poetry_plugin_lambda_build-0.5.3/LICENSE
--rw-r--r--   0        0        0     5519 2024-05-14 08:44:58.698134 poetry_plugin_lambda_build-0.5.3/README.md
--rw-r--r--   0        0        0        0 2024-05-14 08:44:58.698134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/__init__.py
--rw-r--r--   0        0        0      901 2024-05-14 08:44:58.698134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/commands.py
--rw-r--r--   0        0        0     2862 2024-05-14 08:44:58.698134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/docker.py
--rw-r--r--   0        0        0     3977 2024-05-14 08:44:58.702134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/parameters.py
--rw-r--r--   0        0        0     2041 2024-05-14 08:44:58.702134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/plugin.py
--rw-r--r--   0        0        0    11409 2024-05-14 08:44:58.702134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/recipes.py
--rw-r--r--   0        0        0     6752 2024-05-14 08:44:58.702134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/requirements.py
--rw-r--r--   0        0        0     2120 2024-05-14 08:44:58.702134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/utils.py
--rw-r--r--   0        0        0     9831 2024-05-14 08:44:58.702134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/walker.py
--rw-r--r--   0        0        0      767 2024-05-14 08:44:58.702134 poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/zip.py
--rw-r--r--   0        0        0     1042 2024-05-14 08:44:58.702134 poetry_plugin_lambda_build-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     6229 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-15 10:35:22.003968 poetry_plugin_lambda_build-0.5.5/LICENSE
+-rw-r--r--   0        0        0     5414 2024-05-15 10:35:22.003968 poetry_plugin_lambda_build-0.5.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 10:35:22.003968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/__init__.py
+-rw-r--r--   0        0        0      901 2024-05-15 10:35:22.003968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/commands.py
+-rw-r--r--   0        0        0     2862 2024-05-15 10:35:22.003968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/docker.py
+-rw-r--r--   0        0        0     3838 2024-05-15 10:35:22.003968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/parameters.py
+-rw-r--r--   0        0        0     2041 2024-05-15 10:35:22.003968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/plugin.py
+-rw-r--r--   0        0        0    11417 2024-05-15 10:35:22.007968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/recipes.py
+-rw-r--r--   0        0        0     6752 2024-05-15 10:35:22.007968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/requirements.py
+-rw-r--r--   0        0        0     2120 2024-05-15 10:35:22.007968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/utils.py
+-rw-r--r--   0        0        0     9831 2024-05-15 10:35:22.007968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/walker.py
+-rw-r--r--   0        0        0      767 2024-05-15 10:35:22.007968 poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/zip.py
+-rw-r--r--   0        0        0     1042 2024-05-15 10:35:22.007968 poetry_plugin_lambda_build-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.5.5/PKG-INFO
```

### Comparing `poetry_plugin_lambda_build-0.5.3/LICENSE` & `poetry_plugin_lambda_build-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.3/README.md` & `poetry_plugin_lambda_build-0.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 [tool.poetry-plugin-lambda-build]
 artifact_path = "package.zip"
 ```
 
 ### AWS Lambda - all in one - layer package
 ```.toml
 [tool.poetry-plugin-lambda-build]
-install_dir = "python"
-artifact_path = "layer.zip"
+package_install_dir = "python"
+package_artifact_path = "layer.zip"
 ```
 ### AWS Lambda - separated - separate layer package and function package
 
 ```.toml
 [tool.poetry-plugin-lambda-build]
 layer_artifact_path = "layer.zip"
 layer_install_dir = "python"
@@ -79,31 +79,29 @@
 
 ```
 Description:
   Execute to build lambda lambda artifacts
 
 Usage:
   build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<docker_platform> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<zip_compresslevel> [<zip_compression>]]]]]]]]]]]]]]]]]]]]
-
 Arguments:
   docker_image               The image to run
   docker_entrypoint          The entrypoint for the container (comma separated string)
   docker_environment         Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2
   docker_dns                 Set custom DNS servers (comma separated string)
   docker_network             The name of the network this container will be connected to at creation time
   docker_network_disabled    Disable networking ex. docker_network_disabled=0
   docker_network_mode        Network_mode
   docker_platform            Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image.
+  package_artifact_path      Output package path
   package_install_dir        Installation directory inside zip artifact for single zip package
-  layer_install_dir          Installation directory inside zip artifact for layer zip package
+  function_artifact_path     Output function package path
   function_install_dir       Installation directory inside zip artifact for function zip package
-  install_dir                Installation directory inside zip artifact for zip package (not function layer separation)
-  package_artifact_path      Output package path
   layer_artifact_path        Output layer package path
-  function_artifact_path     Output function package path
+  layer_install_dir          Installation directory inside zip artifact for layer zip package
   only                       The only dependency groups to include
   without                    The dependency groups to ignore
   with                       The optional dependency groups to include
   zip_compresslevel          None (default for the given compression type) or an integer specifying the level to pass to the compressor. When using ZIP_STORED or ZIP_LZMA this keyword has no effect. When using ZIP_DEFLATED integers 0 through 9 are accepted. When using ZIP_BZIP2 integers 1 through 9 are accepted.
   zip_compression            ZIP_STORED (no compression), ZIP_DEFLATED (requires zlib), ZIP_BZIP2 (requires bz2) or ZIP_LZMA (requires lzma)
 
 Options:
```

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/commands.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/commands.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/docker.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/docker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/parameters.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,21 +24,20 @@
     "docker_entrypoint": ("The entrypoint for the container (comma separated string)", True, False, None, str),
     "docker_environment": ("Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2", True, False, None, str),
     "docker_dns": ("Set custom DNS servers (comma separated string)", True, False, None, str),
     "docker_network": ("The name of the network this container will be connected to at creation time", True, False, None, str),
     "docker_network_disabled": ("Disable networking ex. docker_network_disabled=0", True, False, None, str),
     "docker_network_mode": ("Network_mode", True, False, None),
     "docker_platform": ("Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image.", True, False, None, str),
+    "package_artifact_path": ("Output package path", True, False, None, str),
     "package_install_dir": ("Installation directory inside zip artifact for single zip package", True, False, None, str),
-    "layer_install_dir": ("Installation directory inside zip artifact for layer zip package", True, False, None, str),
+    "function_artifact_path": ("Output function package path", True, False, None, str),
     "function_install_dir": ("Installation directory inside zip artifact for function zip package", True, False, None, str),
-    "install_dir": ("Installation directory inside zip artifact for zip package (not function layer separation)", True, False, None, str),
-    "package_artifact_path": ("Output package path", True, False, None, str),
     "layer_artifact_path": ("Output layer package path", True, False, None, str),
-    "function_artifact_path": ("Output function package path", True, False, None, str),
+    "layer_install_dir": ("Installation directory inside zip artifact for layer zip package", True, False, None, str),
     "only": ("The only dependency groups to include", True, False, None, comma_separated_collection),
     "without": ("The dependency groups to ignore", True, False, None, comma_separated_collection),
     "with": ("The optional dependency groups to include", True, False, None, comma_separated_collection),
     "zip_compresslevel": ("None (default for the given compression type) or an integer "
                           "specifying the level to pass to the compressor. "
                           "When using ZIP_STORED or ZIP_LZMA this keyword has no effect. "
                           "When using ZIP_DEFLATED integers 0 through 9 are accepted. "
```

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/plugin.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/recipes.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/recipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         self.cmd.debug(
             f"Executing: {print_safe_cmd}")
         run_python_cmd("-m", cmd, logger=self.cmd)
 
     def build_package(self):
         self.cmd.info("Building package...")
         with TemporaryDirectory() as package_dir:
-            install_dir = self.parameters.get("install_dir", "")
+            install_dir = self.parameters.get("package_install_dir", "")
             package_dir = os.path.join(package_dir, install_dir)
             os.makedirs(package_dir, exist_ok=True)
             target = os.path.join(
                 CURRENT_WORK_DIR, self.parameters.get(
                     "package_artifact_path", "")
             )
```

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/requirements.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/utils.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/walker.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/walker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.3/poetry_plugin_lambda_build/zip.py` & `poetry_plugin_lambda_build-0.5.5/poetry_plugin_lambda_build/zip.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.3/pyproject.toml` & `poetry_plugin_lambda_build-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-lambda-build"
-version = "0.5.3"
+version = "0.5.5"
 description = "The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more..."
 authors = ["Michal Murawski <mmurawski777@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docker = "^7.0.0"
```

### Comparing `poetry_plugin_lambda_build-0.5.3/PKG-INFO` & `poetry_plugin_lambda_build-0.5.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-lambda-build
-Version: 0.5.3
+Version: 0.5.5
 Summary: The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more...
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -61,16 +61,16 @@
 [tool.poetry-plugin-lambda-build]
 artifact_path = "package.zip"
 ```
 
 ### AWS Lambda - all in one - layer package
 ```.toml
 [tool.poetry-plugin-lambda-build]
-install_dir = "python"
-artifact_path = "layer.zip"
+package_install_dir = "python"
+package_artifact_path = "layer.zip"
 ```
 ### AWS Lambda - separated - separate layer package and function package
 
 ```.toml
 [tool.poetry-plugin-lambda-build]
 layer_artifact_path = "layer.zip"
 layer_install_dir = "python"
@@ -95,31 +95,29 @@
 
 ```
 Description:
   Execute to build lambda lambda artifacts
 
 Usage:
   build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<docker_platform> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<zip_compresslevel> [<zip_compression>]]]]]]]]]]]]]]]]]]]]
-
 Arguments:
   docker_image               The image to run
   docker_entrypoint          The entrypoint for the container (comma separated string)
   docker_environment         Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2
   docker_dns                 Set custom DNS servers (comma separated string)
   docker_network             The name of the network this container will be connected to at creation time
   docker_network_disabled    Disable networking ex. docker_network_disabled=0
   docker_network_mode        Network_mode
   docker_platform            Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image.
+  package_artifact_path      Output package path
   package_install_dir        Installation directory inside zip artifact for single zip package
-  layer_install_dir          Installation directory inside zip artifact for layer zip package
+  function_artifact_path     Output function package path
   function_install_dir       Installation directory inside zip artifact for function zip package
-  install_dir                Installation directory inside zip artifact for zip package (not function layer separation)
-  package_artifact_path      Output package path
   layer_artifact_path        Output layer package path
-  function_artifact_path     Output function package path
+  layer_install_dir          Installation directory inside zip artifact for layer zip package
   only                       The only dependency groups to include
   without                    The dependency groups to ignore
   with                       The optional dependency groups to include
   zip_compresslevel          None (default for the given compression type) or an integer specifying the level to pass to the compressor. When using ZIP_STORED or ZIP_LZMA this keyword has no effect. When using ZIP_DEFLATED integers 0 through 9 are accepted. When using ZIP_BZIP2 integers 1 through 9 are accepted.
   zip_compression            ZIP_STORED (no compression), ZIP_DEFLATED (requires zlib), ZIP_BZIP2 (requires bz2) or ZIP_LZMA (requires lzma)
 
 Options:
```

