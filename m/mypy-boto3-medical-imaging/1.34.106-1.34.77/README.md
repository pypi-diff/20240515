# Comparing `tmp/mypy_boto3_medical_imaging-1.34.106.tar.gz` & `tmp/mypy-boto3-medical-imaging-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_medical_imaging-1.34.106.tar", last modified: Wed May 15 19:32:40 2024, max compression
+gzip compressed data, was "mypy-boto3-medical-imaging-1.34.77.tar", last modified: Wed Apr  3 19:32:40 2024, max compression
```

## Comparing `mypy_boto3_medical_imaging-1.34.106.tar` & `mypy-boto3-medical-imaging-1.34.77.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:40.357520 mypy_boto3_medical_imaging-1.34.106/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-05-15 19:32:40.357520 mypy_boto3_medical_imaging-1.34.106/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:40.357520 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:40.357520 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-05-15 19:32:40.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-15 19:32:40.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:32:40.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:32:40.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 19:32:40.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 19:32:40.000000 mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:32:40.357520 mypy_boto3_medical_imaging-1.34.106/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-15 19:32:07.000000 mypy_boto3_medical_imaging-1.34.106/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.560159 mypy-boto3-medical-imaging-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-04-03 19:32:40.556159 mypy-boto3-medical-imaging-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.556159 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19327 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19327 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.556159 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 19:32:40.000000 mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:40.560159 mypy-boto3-medical-imaging-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-03 19:32:24.000000 mypy-boto3-medical-imaging-1.34.77/setup.py
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/LICENSE` & `mypy-boto3-medical-imaging-1.34.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_medical_imaging-1.34.106/PKG-INFO` & `mypy-boto3-medical-imaging-1.34.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medical-imaging
-Version: 1.34.106
-Summary: Type annotations for boto3.HealthImaging 1.34.106 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.77
+Summary: Type annotations for boto3.HealthImaging 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.34.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/README.md` & `mypy-boto3-medical-imaging-1.34.77/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.34.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/__init__.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/__init__.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/__main__.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.HealthImaging 1.34.106\n"
-        "Version:         1.34.106\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.HealthImaging 1.34.77\n"
+        "Version:         1.34.77\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.106")
+    print("1.34.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/client.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
         *,
         dataAccessRoleArn: str,
         clientToken: str,
         datastoreId: str,
         inputS3Uri: str,
         outputS3Uri: str,
         jobName: str = ...,
-        inputOwnerAccountId: str = ...,
     ) -> StartDICOMImportJobResponseTypeDef:
         """
         Start importing bulk data into an `ACTIVE` data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.start_dicom_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#start_dicom_import_job)
         """
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/client.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,14 @@
         *,
         dataAccessRoleArn: str,
         clientToken: str,
         datastoreId: str,
         inputS3Uri: str,
         outputS3Uri: str,
         jobName: str = ...,
-        inputOwnerAccountId: str = ...,
     ) -> StartDICOMImportJobResponseTypeDef:
         """
         Start importing bulk data into an `ACTIVE` data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client.start_dicom_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/client/#start_dicom_import_job)
         """
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/literals.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,14 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
@@ -364,15 +363,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/literals.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,14 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
@@ -364,15 +363,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/paginator.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/paginator.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/type_defs.py` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,14 @@
     {
         "dataAccessRoleArn": str,
         "clientToken": str,
         "datastoreId": str,
         "inputS3Uri": str,
         "outputS3Uri": str,
         "jobName": NotRequired[str],
-        "inputOwnerAccountId": NotRequired[str],
     },
 )
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging/type_defs.pyi` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,14 @@
     {
         "dataAccessRoleArn": str,
         "clientToken": str,
         "datastoreId": str,
         "inputS3Uri": str,
         "outputS3Uri": str,
         "jobName": NotRequired[str],
-        "inputOwnerAccountId": NotRequired[str],
     },
 )
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/PKG-INFO` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medical-imaging
-Version: 1.34.106
-Summary: Type annotations for boto3.HealthImaging 1.34.106 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.77
+Summary: Type annotations for boto3.HealthImaging 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.34.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_medical_imaging-1.34.106/mypy_boto3_medical_imaging.egg-info/SOURCES.txt` & `mypy-boto3-medical-imaging-1.34.77/mypy_boto3_medical_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_medical_imaging-1.34.106/setup.py` & `mypy-boto3-medical-imaging-1.34.77/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medical-imaging",
-    version="1.34.106",
+    version="1.34.77",
     packages=["mypy_boto3_medical_imaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.HealthImaging 1.34.106 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.HealthImaging 1.34.77 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

