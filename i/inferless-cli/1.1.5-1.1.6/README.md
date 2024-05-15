# Comparing `tmp/inferless_cli-1.1.5.tar.gz` & `tmp/inferless_cli-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferless_cli-1.1.5.tar", max compression
+gzip compressed data, was "inferless_cli-1.1.6.tar", max compression
```

## Comparing `inferless_cli-1.1.5.tar` & `inferless_cli-1.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.5/README.md
--rw-r--r--   0        0        0       37 2024-04-30 05:02:10.511402 inferless_cli-1.1.5/inferless_cli/__init__.py
--rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.5/inferless_cli/__main__.py
--rw-r--r--   0        0        0     7282 2024-04-29 12:49:54.155402 inferless_cli-1.1.5/inferless_cli/main.py
--rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.5/inferless_cli/prompts/__init__.py
--rw-r--r--   0        0        0    23068 2024-04-29 12:49:54.155748 inferless_cli-1.1.5/inferless_cli/prompts/deploy.py
--rw-r--r--   0        0        0     1802 2024-04-29 12:49:54.156043 inferless_cli-1.1.5/inferless_cli/prompts/export.py
--rw-r--r--   0        0        0    11391 2024-04-29 12:49:54.156678 inferless_cli-1.1.5/inferless_cli/prompts/init.py
--rw-r--r--   0        0        0     3779 2024-04-29 12:49:54.157030 inferless_cli-1.1.5/inferless_cli/prompts/log.py
--rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.5/inferless_cli/prompts/login.py
--rw-r--r--   0        0        0    15846 2024-04-29 12:49:54.157620 inferless_cli-1.1.5/inferless_cli/prompts/model.py
--rw-r--r--   0        0        0    18882 2024-04-29 12:49:54.157892 inferless_cli-1.1.5/inferless_cli/prompts/run.py
--rw-r--r--   0        0        0     5984 2024-04-29 12:49:54.158229 inferless_cli-1.1.5/inferless_cli/prompts/runtime.py
--rw-r--r--   0        0        0     2026 2024-04-29 12:49:54.158392 inferless_cli-1.1.5/inferless_cli/prompts/secret.py
--rw-r--r--   0        0        0     4231 2024-04-29 12:49:54.158770 inferless_cli-1.1.5/inferless_cli/prompts/token.py
--rw-r--r--   0        0        0    22378 2024-04-29 18:01:24.312203 inferless_cli-1.1.5/inferless_cli/prompts/volume.py
--rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.5/inferless_cli/prompts/workspace.py
--rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.5/inferless_cli/utils/__init__.py
--rw-r--r--   0        0        0     2870 2024-04-29 12:49:54.159619 inferless_cli-1.1.5/inferless_cli/utils/api.py
--rw-r--r--   0        0        0    14752 2024-04-29 12:49:54.160026 inferless_cli-1.1.5/inferless_cli/utils/constants.py
--rw-r--r--   0        0        0     1068 2024-04-29 12:49:54.160238 inferless_cli-1.1.5/inferless_cli/utils/convertors.py
--rw-r--r--   0        0        0     7179 2024-04-29 12:49:54.160563 inferless_cli-1.1.5/inferless_cli/utils/credentials.py
--rw-r--r--   0        0        0    28870 2024-04-30 05:01:57.867634 inferless_cli-1.1.5/inferless_cli/utils/helpers.py
--rw-r--r--   0        0        0    26839 2024-04-29 12:49:54.161332 inferless_cli-1.1.5/inferless_cli/utils/services.py
--rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.5/inferless_cli/utils/validators.py
--rw-r--r--   0        0        0      671 2024-04-30 05:02:13.981000 inferless_cli-1.1.5/pyproject.toml
--rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.6/README.md
+-rw-r--r--   0        0        0       37 2024-05-15 17:36:04.247694 inferless_cli-1.1.6/inferless_cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.6/inferless_cli/__main__.py
+-rw-r--r--   0        0        0     7282 2024-04-29 12:49:54.155402 inferless_cli-1.1.6/inferless_cli/main.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.6/inferless_cli/prompts/__init__.py
+-rw-r--r--   0        0        0    23068 2024-04-29 12:49:54.155748 inferless_cli-1.1.6/inferless_cli/prompts/deploy.py
+-rw-r--r--   0        0        0     1802 2024-04-29 12:49:54.156043 inferless_cli-1.1.6/inferless_cli/prompts/export.py
+-rw-r--r--   0        0        0    11391 2024-04-29 12:49:54.156678 inferless_cli-1.1.6/inferless_cli/prompts/init.py
+-rw-r--r--   0        0        0     3779 2024-04-30 07:21:43.512104 inferless_cli-1.1.6/inferless_cli/prompts/log.py
+-rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.6/inferless_cli/prompts/login.py
+-rw-r--r--   0        0        0    15846 2024-04-29 12:49:54.157620 inferless_cli-1.1.6/inferless_cli/prompts/model.py
+-rw-r--r--   0        0        0    18882 2024-04-29 12:49:54.157892 inferless_cli-1.1.6/inferless_cli/prompts/run.py
+-rw-r--r--   0        0        0     5984 2024-04-29 12:49:54.158229 inferless_cli-1.1.6/inferless_cli/prompts/runtime.py
+-rw-r--r--   0        0        0     2026 2024-04-29 12:49:54.158392 inferless_cli-1.1.6/inferless_cli/prompts/secret.py
+-rw-r--r--   0        0        0     4231 2024-04-29 12:49:54.158770 inferless_cli-1.1.6/inferless_cli/prompts/token.py
+-rw-r--r--   0        0        0    22378 2024-04-29 18:01:24.312203 inferless_cli-1.1.6/inferless_cli/prompts/volume.py
+-rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.6/inferless_cli/prompts/workspace.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.6/inferless_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2870 2024-04-29 12:49:54.159619 inferless_cli-1.1.6/inferless_cli/utils/api.py
+-rw-r--r--   0        0        0    14752 2024-04-29 12:49:54.160026 inferless_cli-1.1.6/inferless_cli/utils/constants.py
+-rw-r--r--   0        0        0     1277 2024-05-15 17:23:04.668037 inferless_cli-1.1.6/inferless_cli/utils/convertors.py
+-rw-r--r--   0        0        0     7179 2024-04-29 12:49:54.160563 inferless_cli-1.1.6/inferless_cli/utils/credentials.py
+-rw-r--r--   0        0        0    29299 2024-05-15 17:35:52.807108 inferless_cli-1.1.6/inferless_cli/utils/helpers.py
+-rw-r--r--   0        0        0    26839 2024-04-29 12:49:54.161332 inferless_cli-1.1.6/inferless_cli/utils/services.py
+-rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.6/inferless_cli/utils/validators.py
+-rw-r--r--   0        0        0      671 2024-05-15 17:34:36.026866 inferless_cli-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.6/PKG-INFO
```

### Comparing `inferless_cli-1.1.5/README.md` & `inferless_cli-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/main.py` & `inferless_cli-1.1.6/inferless_cli/main.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/deploy.py` & `inferless_cli-1.1.6/inferless_cli/prompts/deploy.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/export.py` & `inferless_cli-1.1.6/inferless_cli/prompts/export.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/init.py` & `inferless_cli-1.1.6/inferless_cli/prompts/init.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/log.py` & `inferless_cli-1.1.6/inferless_cli/prompts/log.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/login.py` & `inferless_cli-1.1.6/inferless_cli/prompts/login.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/model.py` & `inferless_cli-1.1.6/inferless_cli/prompts/model.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/run.py` & `inferless_cli-1.1.6/inferless_cli/prompts/run.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/runtime.py` & `inferless_cli-1.1.6/inferless_cli/prompts/runtime.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/secret.py` & `inferless_cli-1.1.6/inferless_cli/prompts/secret.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/token.py` & `inferless_cli-1.1.6/inferless_cli/prompts/token.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/volume.py` & `inferless_cli-1.1.6/inferless_cli/prompts/volume.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/prompts/workspace.py` & `inferless_cli-1.1.6/inferless_cli/prompts/workspace.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/utils/api.py` & `inferless_cli-1.1.6/inferless_cli/utils/api.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/utils/constants.py` & `inferless_cli-1.1.6/inferless_cli/utils/constants.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/utils/convertors.py` & `inferless_cli-1.1.6/inferless_cli/utils/convertors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import typer
 from inferless_cli.utils.helpers import read_yaml, create_yaml
+import rich
 
 
 class Convertors:
     @staticmethod
     def get_cuda_version(cuda_version: str) -> str:
         cuda_version = float(cuda_version)
         if cuda_version >= 11.0 and cuda_version < 12.0:
@@ -13,20 +15,23 @@
     @staticmethod
     def convert_cog_to_runtime_yaml(
         source_file: str, destination_file: str, return_as_json: bool = False
     ):
         cog_yaml = read_yaml(source_file)
 
         filtered_data = {"build": {}}
-        for key, value in cog_yaml.get("build", {}).items():
-            if key in ["cuda", "python_packages", "system_packages"]:
-                if key == "cuda":
-                    filtered_data["build"]["cuda_version"] = (
-                        Convertors.get_cuda_version(value)
-                    )
-                else:
-                    filtered_data["build"][key] = value
-
+        if cog_yaml is not None:
+            for key, value in cog_yaml.get("build", {}).items():
+                if key in ["cuda", "python_packages", "system_packages"]:
+                    if key == "cuda":
+                        filtered_data["build"]["cuda_version"] = (
+                            Convertors.get_cuda_version(value)
+                        )
+                    else:
+                        filtered_data["build"][key] = value
+        else:
+            rich.print("[bold red]Error:[/bold red] cog.yaml not found.")
+            raise typer.Exit(1)
         if return_as_json:
             return filtered_data
 
         create_yaml(filtered_data, destination_file)
```

### Comparing `inferless_cli-1.1.5/inferless_cli/utils/credentials.py` & `inferless_cli-1.1.6/inferless_cli/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/utils/helpers.py` & `inferless_cli-1.1.6/inferless_cli/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,23 +472,34 @@
             log_exception(e)
             rich.print("Failed to read YAML file: {}".format(e))
 
     return None
 
 
 def read_yaml(file_name):
-    if os.path.isfile(file_name):
-        with open(file_name, "r") as yaml_file:
-            try:
+    try:
+        if os.path.isfile(file_name):
+            with open(file_name, "r", encoding="utf-8") as yaml_file:
                 inferless_config = yaml.load(yaml_file)
                 return inferless_config
-            except Exception as e:
-                log_exception(e)
-                rich.print("Failed to read YAML file: {}".format(e))
-    return None
+        else:
+            rich.print(f"File not found: {file_name}")
+            return None
+    except UnicodeDecodeError:
+        try:
+            with open(file_name, "r", encoding="cp1252") as yaml_file:
+                inferless_config = yaml.load(yaml_file)
+                return inferless_config
+        except Exception as e:
+            rich.print(f"Failed to read YAML file with cp1252 encoding: {e}")
+            raise
+    except Exception as e:
+        log_exception(e)
+        rich.print("Failed to read YAML file: {}".format(e))
+        return None
 
 
 def read_json(file_name):
     try:
         with open(file_name, "r") as json_file:
             file_data = json.load(json_file)
             return file_data
```

### Comparing `inferless_cli-1.1.5/inferless_cli/utils/services.py` & `inferless_cli-1.1.6/inferless_cli/utils/services.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/inferless_cli/utils/validators.py` & `inferless_cli-1.1.6/inferless_cli/utils/validators.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.5/pyproject.toml` & `inferless_cli-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inferless-cli"
-version = "1.1.5"
+version = "1.1.6"
 description = "Inferless - Deploy Machine Learning Models in Minutes."
 authors = ["Naveen <naveen@inferless.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 inferless = "inferless_cli.main:app"
```

### Comparing `inferless_cli-1.1.5/PKG-INFO` & `inferless_cli-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferless-cli
-Version: 1.1.5
+Version: 1.1.6
 Summary: Inferless - Deploy Machine Learning Models in Minutes.
 Author: Naveen
 Author-email: naveen@inferless.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

