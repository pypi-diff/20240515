# Comparing `tmp/mypy_boto3_grafana-1.34.106.tar.gz` & `tmp/mypy-boto3-grafana-1.34.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_grafana-1.34.106.tar", last modified: Wed May 15 19:32:40 2024, max compression
+gzip compressed data, was "mypy-boto3-grafana-1.34.58.tar", last modified: Thu Mar  7 20:22:52 2024, max compression
```

## Comparing `mypy_boto3_grafana-1.34.106.tar` & `mypy-boto3-grafana-1.34.58.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:40.021519 mypy_boto3_grafana-1.34.106/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-15 19:32:40.021519 mypy_boto3_grafana-1.34.106/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:40.021519 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23191 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-15 19:32:06.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-15 19:32:06.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-15 19:32:06.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-15 19:32:06.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25419 2024-05-15 19:32:06.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25419 2024-05-15 19:32:06.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:40.021519 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-15 19:32:39.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-15 19:32:39.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:32:39.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:32:39.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 19:32:39.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:32:39.000000 mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:32:40.021519 mypy_boto3_grafana-1.34.106/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-15 19:32:05.000000 mypy_boto3_grafana-1.34.106/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:52.486005 mypy-boto3-grafana-1.34.58/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-03-07 20:22:52.486005 mypy-boto3-grafana-1.34.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:52.482005 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-03-07 20:22:16.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-03-07 20:22:16.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:52.486005 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-03-07 20:22:52.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-07 20:22:52.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 20:22:52.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 20:22:52.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-07 20:22:52.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-07 20:22:52.000000 mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 20:22:52.486005 mypy-boto3-grafana-1.34.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-07 20:22:15.000000 mypy-boto3-grafana-1.34.58/setup.py
```

### Comparing `mypy_boto3_grafana-1.34.106/LICENSE` & `mypy-boto3-grafana-1.34.58/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_grafana-1.34.106/PKG-INFO` & `mypy-boto3-grafana-1.34.58/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.34.106
-Summary: Type annotations for boto3.ManagedGrafana 1.34.106 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.58
+Summary: Type annotations for boto3.ManagedGrafana 1.34.58 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.34.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,31 +282,23 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_grafana import ManagedGrafanaClient
 from mypy_boto3_grafana.paginator import (
     ListPermissionsPaginator,
     ListVersionsPaginator,
-    ListWorkspaceServiceAccountTokensPaginator,
-    ListWorkspaceServiceAccountsPaginator,
     ListWorkspacesPaginator,
 )
 
 client: ManagedGrafanaClient = Session().client("grafana")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
 list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
-list_workspace_service_account_tokens_paginator: ListWorkspaceServiceAccountTokensPaginator = (
-    client.get_paginator("list_workspace_service_account_tokens")
-)
-list_workspace_service_accounts_paginator: ListWorkspaceServiceAccountsPaginator = (
-    client.get_paginator("list_workspace_service_accounts")
-)
 list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `mypy_boto3_grafana-1.34.106/README.md` & `mypy-boto3-grafana-1.34.58/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.34.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -249,31 +249,23 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_grafana import ManagedGrafanaClient
 from mypy_boto3_grafana.paginator import (
     ListPermissionsPaginator,
     ListVersionsPaginator,
-    ListWorkspaceServiceAccountTokensPaginator,
-    ListWorkspaceServiceAccountsPaginator,
     ListWorkspacesPaginator,
 )
 
 client: ManagedGrafanaClient = Session().client("grafana")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
 list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
-list_workspace_service_account_tokens_paginator: ListWorkspaceServiceAccountTokensPaginator = (
-    client.get_paginator("list_workspace_service_account_tokens")
-)
-list_workspace_service_accounts_paginator: ListWorkspaceServiceAccountsPaginator = (
-    client.get_paginator("list_workspace_service_accounts")
-)
 list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/__main__.py` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedGrafana 1.34.106\n"
-        "Version:         1.34.106\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.ManagedGrafana 1.34.58\n"
+        "Version:         1.34.58\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.106")
+    print("1.34.58")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/client.py` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,51 +21,38 @@
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
-    RoleType,
     UserTypeType,
 )
-from .paginator import (
-    ListPermissionsPaginator,
-    ListVersionsPaginator,
-    ListWorkspaceServiceAccountsPaginator,
-    ListWorkspaceServiceAccountTokensPaginator,
-    ListWorkspacesPaginator,
-)
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 from .type_defs import (
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
-    CreateWorkspaceServiceAccountResponseTypeDef,
-    CreateWorkspaceServiceAccountTokenResponseTypeDef,
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
-    DeleteWorkspaceServiceAccountResponseTypeDef,
-    DeleteWorkspaceServiceAccountTokenResponseTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVersionsResponseTypeDef,
-    ListWorkspaceServiceAccountsResponseTypeDef,
-    ListWorkspaceServiceAccountTokensResponseTypeDef,
     ListWorkspacesResponseTypeDef,
-    NetworkAccessConfigurationUnionTypeDef,
-    SamlConfigurationUnionTypeDef,
-    UpdateInstructionUnionTypeDef,
+    NetworkAccessConfigurationTypeDef,
+    SamlConfigurationTypeDef,
+    UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    VpcConfigurationUnionTypeDef,
+    VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -139,19 +126,19 @@
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
         configuration: str = ...,
         grafanaVersion: str = ...,
-        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
+        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
         stackSetName: str = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...,
     ) -> CreateWorkspaceResponseTypeDef:
@@ -168,36 +155,14 @@
         """
         Creates a Grafana API key for the workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace_api_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#create_workspace_api_key)
         """
 
-    def create_workspace_service_account(
-        self, *, grafanaRole: RoleType, name: str, workspaceId: str
-    ) -> CreateWorkspaceServiceAccountResponseTypeDef:
-        """
-        Creates a service account for the workspace.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace_service_account)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#create_workspace_service_account)
-        """
-
-    def create_workspace_service_account_token(
-        self, *, name: str, secondsToLive: int, serviceAccountId: str, workspaceId: str
-    ) -> CreateWorkspaceServiceAccountTokenResponseTypeDef:
-        """
-        Creates a token that can be used to authenticate and authorize Grafana HTTP API
-        operations for the given [workspace service
-        account](https://docs.aws.amazon.com/grafana/latest/userguide/service-accounts.html).
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace_service_account_token)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#create_workspace_service_account_token)
-        """
-
     def delete_workspace(self, *, workspaceId: str) -> DeleteWorkspaceResponseTypeDef:
         """
         Deletes an Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#delete_workspace)
         """
@@ -208,34 +173,14 @@
         """
         Deletes a Grafana API key for the workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace_api_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#delete_workspace_api_key)
         """
 
-    def delete_workspace_service_account(
-        self, *, serviceAccountId: str, workspaceId: str
-    ) -> DeleteWorkspaceServiceAccountResponseTypeDef:
-        """
-        Deletes a workspace service account from the workspace.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace_service_account)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#delete_workspace_service_account)
-        """
-
-    def delete_workspace_service_account_token(
-        self, *, serviceAccountId: str, tokenId: str, workspaceId: str
-    ) -> DeleteWorkspaceServiceAccountTokenResponseTypeDef:
-        """
-        Deletes a token for the workspace service account.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace_service_account_token)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#delete_workspace_service_account_token)
-        """
-
     def describe_workspace(self, *, workspaceId: str) -> DescribeWorkspaceResponseTypeDef:
         """
         Displays information about one Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.describe_workspace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#describe_workspace)
         """
@@ -321,39 +266,14 @@
         """
         Lists available versions of Grafana.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_versions)
         """
 
-    def list_workspace_service_account_tokens(
-        self,
-        *,
-        serviceAccountId: str,
-        workspaceId: str,
-        maxResults: int = ...,
-        nextToken: str = ...,
-    ) -> ListWorkspaceServiceAccountTokensResponseTypeDef:
-        """
-        Returns a list of tokens for a workspace service account.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_workspace_service_account_tokens)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_workspace_service_account_tokens)
-        """
-
-    def list_workspace_service_accounts(
-        self, *, workspaceId: str, maxResults: int = ..., nextToken: str = ...
-    ) -> ListWorkspaceServiceAccountsResponseTypeDef:
-        """
-        Returns a list of service accounts for a workspace.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_workspace_service_accounts)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_workspace_service_accounts)
-        """
-
     def list_workspaces(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Returns a list of Amazon Managed Grafana workspaces in the account, with some
         information about each
         workspace.
@@ -378,35 +298,35 @@
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#untag_resource)
         """
 
     def update_permissions(
-        self, *, updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef], workspaceId: str
+        self, *, updateInstructionBatch: Sequence[UpdateInstructionTypeDef], workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_permissions)
         """
 
     def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
-        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
+        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
         permissionType: PermissionTypeType = ...,
         removeNetworkAccessConfiguration: bool = ...,
         removeVpcConfiguration: bool = ...,
         stackSetName: str = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...,
     ) -> UpdateWorkspaceResponseTypeDef:
@@ -418,15 +338,15 @@
         """
 
     def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: SamlConfigurationUnionTypeDef = ...,
+        samlConfiguration: SamlConfigurationTypeDef = ...,
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using
         SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
@@ -457,30 +377,12 @@
     def get_paginator(self, operation_name: Literal["list_versions"]) -> ListVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
         """
 
     @overload
-    def get_paginator(
-        self, operation_name: Literal["list_workspace_service_account_tokens"]
-    ) -> ListWorkspaceServiceAccountTokensPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
-        """
-
-    @overload
-    def get_paginator(
-        self, operation_name: Literal["list_workspace_service_accounts"]
-    ) -> ListWorkspaceServiceAccountsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
-        """
-
-    @overload
     def get_paginator(self, operation_name: Literal["list_workspaces"]) -> ListWorkspacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
         """
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/client.pyi` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/client.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -21,51 +21,38 @@
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
-    RoleType,
     UserTypeType,
 )
-from .paginator import (
-    ListPermissionsPaginator,
-    ListVersionsPaginator,
-    ListWorkspaceServiceAccountsPaginator,
-    ListWorkspaceServiceAccountTokensPaginator,
-    ListWorkspacesPaginator,
-)
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 from .type_defs import (
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
-    CreateWorkspaceServiceAccountResponseTypeDef,
-    CreateWorkspaceServiceAccountTokenResponseTypeDef,
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
-    DeleteWorkspaceServiceAccountResponseTypeDef,
-    DeleteWorkspaceServiceAccountTokenResponseTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVersionsResponseTypeDef,
-    ListWorkspaceServiceAccountsResponseTypeDef,
-    ListWorkspaceServiceAccountTokensResponseTypeDef,
     ListWorkspacesResponseTypeDef,
-    NetworkAccessConfigurationUnionTypeDef,
-    SamlConfigurationUnionTypeDef,
-    UpdateInstructionUnionTypeDef,
+    NetworkAccessConfigurationTypeDef,
+    SamlConfigurationTypeDef,
+    UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    VpcConfigurationUnionTypeDef,
+    VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -136,19 +123,19 @@
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
         configuration: str = ...,
         grafanaVersion: str = ...,
-        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
+        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
         stackSetName: str = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...,
     ) -> CreateWorkspaceResponseTypeDef:
@@ -165,36 +152,14 @@
         """
         Creates a Grafana API key for the workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace_api_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#create_workspace_api_key)
         """
 
-    def create_workspace_service_account(
-        self, *, grafanaRole: RoleType, name: str, workspaceId: str
-    ) -> CreateWorkspaceServiceAccountResponseTypeDef:
-        """
-        Creates a service account for the workspace.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace_service_account)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#create_workspace_service_account)
-        """
-
-    def create_workspace_service_account_token(
-        self, *, name: str, secondsToLive: int, serviceAccountId: str, workspaceId: str
-    ) -> CreateWorkspaceServiceAccountTokenResponseTypeDef:
-        """
-        Creates a token that can be used to authenticate and authorize Grafana HTTP API
-        operations for the given [workspace service
-        account](https://docs.aws.amazon.com/grafana/latest/userguide/service-accounts.html).
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace_service_account_token)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#create_workspace_service_account_token)
-        """
-
     def delete_workspace(self, *, workspaceId: str) -> DeleteWorkspaceResponseTypeDef:
         """
         Deletes an Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#delete_workspace)
         """
@@ -205,34 +170,14 @@
         """
         Deletes a Grafana API key for the workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace_api_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#delete_workspace_api_key)
         """
 
-    def delete_workspace_service_account(
-        self, *, serviceAccountId: str, workspaceId: str
-    ) -> DeleteWorkspaceServiceAccountResponseTypeDef:
-        """
-        Deletes a workspace service account from the workspace.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace_service_account)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#delete_workspace_service_account)
-        """
-
-    def delete_workspace_service_account_token(
-        self, *, serviceAccountId: str, tokenId: str, workspaceId: str
-    ) -> DeleteWorkspaceServiceAccountTokenResponseTypeDef:
-        """
-        Deletes a token for the workspace service account.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace_service_account_token)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#delete_workspace_service_account_token)
-        """
-
     def describe_workspace(self, *, workspaceId: str) -> DescribeWorkspaceResponseTypeDef:
         """
         Displays information about one Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.describe_workspace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#describe_workspace)
         """
@@ -318,39 +263,14 @@
         """
         Lists available versions of Grafana.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_versions)
         """
 
-    def list_workspace_service_account_tokens(
-        self,
-        *,
-        serviceAccountId: str,
-        workspaceId: str,
-        maxResults: int = ...,
-        nextToken: str = ...,
-    ) -> ListWorkspaceServiceAccountTokensResponseTypeDef:
-        """
-        Returns a list of tokens for a workspace service account.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_workspace_service_account_tokens)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_workspace_service_account_tokens)
-        """
-
-    def list_workspace_service_accounts(
-        self, *, workspaceId: str, maxResults: int = ..., nextToken: str = ...
-    ) -> ListWorkspaceServiceAccountsResponseTypeDef:
-        """
-        Returns a list of service accounts for a workspace.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_workspace_service_accounts)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_workspace_service_accounts)
-        """
-
     def list_workspaces(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Returns a list of Amazon Managed Grafana workspaces in the account, with some
         information about each
         workspace.
@@ -375,35 +295,35 @@
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#untag_resource)
         """
 
     def update_permissions(
-        self, *, updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef], workspaceId: str
+        self, *, updateInstructionBatch: Sequence[UpdateInstructionTypeDef], workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_permissions)
         """
 
     def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
-        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
+        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
         permissionType: PermissionTypeType = ...,
         removeNetworkAccessConfiguration: bool = ...,
         removeVpcConfiguration: bool = ...,
         stackSetName: str = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...,
     ) -> UpdateWorkspaceResponseTypeDef:
@@ -415,15 +335,15 @@
         """
 
     def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: SamlConfigurationUnionTypeDef = ...,
+        samlConfiguration: SamlConfigurationTypeDef = ...,
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using
         SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
@@ -454,30 +374,12 @@
     def get_paginator(self, operation_name: Literal["list_versions"]) -> ListVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
         """
 
     @overload
-    def get_paginator(
-        self, operation_name: Literal["list_workspace_service_account_tokens"]
-    ) -> ListWorkspaceServiceAccountTokensPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
-        """
-
-    @overload
-    def get_paginator(
-        self, operation_name: Literal["list_workspace_service_accounts"]
-    ) -> ListWorkspaceServiceAccountsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
-        """
-
-    @overload
     def get_paginator(self, operation_name: Literal["list_workspaces"]) -> ListWorkspacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
         """
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/literals.py` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 __all__ = (
     "AccountAccessTypeType",
     "AuthenticationProviderTypesType",
     "DataSourceTypeType",
     "LicenseTypeType",
     "ListPermissionsPaginatorName",
     "ListVersionsPaginatorName",
-    "ListWorkspaceServiceAccountTokensPaginatorName",
-    "ListWorkspaceServiceAccountsPaginatorName",
     "ListWorkspacesPaginatorName",
     "NotificationDestinationTypeType",
     "PermissionTypeType",
     "RoleType",
     "SamlConfigurationStatusType",
     "UpdateActionType",
     "UserTypeType",
@@ -55,16 +53,14 @@
     "TIMESTREAM",
     "TWINMAKER",
     "XRAY",
 ]
 LicenseTypeType = Literal["ENTERPRISE", "ENTERPRISE_FREE_TRIAL"]
 ListPermissionsPaginatorName = Literal["list_permissions"]
 ListVersionsPaginatorName = Literal["list_versions"]
-ListWorkspaceServiceAccountTokensPaginatorName = Literal["list_workspace_service_account_tokens"]
-ListWorkspaceServiceAccountsPaginatorName = Literal["list_workspace_service_accounts"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 NotificationDestinationTypeType = Literal["SNS"]
 PermissionTypeType = Literal["CUSTOMER_MANAGED", "SERVICE_MANAGED"]
 RoleType = Literal["ADMIN", "EDITOR", "VIEWER"]
 SamlConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 UpdateActionType = Literal["ADD", "REVOKE"]
 UserTypeType = Literal["SSO_GROUP", "SSO_USER"]
@@ -151,15 +147,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -172,26 +167,24 @@
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
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -252,14 +245,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -388,15 +382,14 @@
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
@@ -440,15 +433,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -477,21 +469,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal[
-    "list_permissions",
-    "list_versions",
-    "list_workspace_service_account_tokens",
-    "list_workspace_service_accounts",
-    "list_workspaces",
-]
+PaginatorName = Literal["list_permissions", "list_versions", "list_workspaces"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-west-1",
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/literals.pyi` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/literals.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 __all__ = (
     "AccountAccessTypeType",
     "AuthenticationProviderTypesType",
     "DataSourceTypeType",
     "LicenseTypeType",
     "ListPermissionsPaginatorName",
     "ListVersionsPaginatorName",
-    "ListWorkspaceServiceAccountTokensPaginatorName",
-    "ListWorkspaceServiceAccountsPaginatorName",
     "ListWorkspacesPaginatorName",
     "NotificationDestinationTypeType",
     "PermissionTypeType",
     "RoleType",
     "SamlConfigurationStatusType",
     "UpdateActionType",
     "UserTypeType",
@@ -55,16 +53,14 @@
     "TIMESTREAM",
     "TWINMAKER",
     "XRAY",
 ]
 LicenseTypeType = Literal["ENTERPRISE", "ENTERPRISE_FREE_TRIAL"]
 ListPermissionsPaginatorName = Literal["list_permissions"]
 ListVersionsPaginatorName = Literal["list_versions"]
-ListWorkspaceServiceAccountTokensPaginatorName = Literal["list_workspace_service_account_tokens"]
-ListWorkspaceServiceAccountsPaginatorName = Literal["list_workspace_service_accounts"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 NotificationDestinationTypeType = Literal["SNS"]
 PermissionTypeType = Literal["CUSTOMER_MANAGED", "SERVICE_MANAGED"]
 RoleType = Literal["ADMIN", "EDITOR", "VIEWER"]
 SamlConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 UpdateActionType = Literal["ADD", "REVOKE"]
 UserTypeType = Literal["SSO_GROUP", "SSO_USER"]
@@ -151,15 +147,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -172,26 +167,24 @@
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
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -252,14 +245,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -388,15 +382,14 @@
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
@@ -440,15 +433,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -477,21 +469,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal[
-    "list_permissions",
-    "list_versions",
-    "list_workspace_service_account_tokens",
-    "list_workspace_service_accounts",
-    "list_workspaces",
-]
+PaginatorName = Literal["list_permissions", "list_versions", "list_workspaces"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-west-1",
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/paginator.pyi` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/paginator.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -8,51 +8,39 @@
     ```python
     from boto3.session import Session
 
     from mypy_boto3_grafana.client import ManagedGrafanaClient
     from mypy_boto3_grafana.paginator import (
         ListPermissionsPaginator,
         ListVersionsPaginator,
-        ListWorkspaceServiceAccountTokensPaginator,
-        ListWorkspaceServiceAccountsPaginator,
         ListWorkspacesPaginator,
     )
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
 
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
     list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
-    list_workspace_service_account_tokens_paginator: ListWorkspaceServiceAccountTokensPaginator = client.get_paginator("list_workspace_service_account_tokens")
-    list_workspace_service_accounts_paginator: ListWorkspaceServiceAccountsPaginator = client.get_paginator("list_workspace_service_accounts")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import UserTypeType
 from .type_defs import (
     ListPermissionsResponseTypeDef,
     ListVersionsResponseTypeDef,
-    ListWorkspaceServiceAccountsResponseTypeDef,
-    ListWorkspaceServiceAccountTokensResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
-__all__ = (
-    "ListPermissionsPaginator",
-    "ListVersionsPaginator",
-    "ListWorkspaceServiceAccountTokensPaginator",
-    "ListWorkspaceServiceAccountsPaginator",
-    "ListWorkspacesPaginator",
-)
+__all__ = ("ListPermissionsPaginator", "ListVersionsPaginator", "ListWorkspacesPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -88,46 +76,14 @@
         self, *, workspaceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
         """
 
-class ListWorkspaceServiceAccountTokensPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaceServiceAccountTokens)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspaceserviceaccounttokenspaginator)
-    """
-
-    def paginate(
-        self,
-        *,
-        serviceAccountId: str,
-        workspaceId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListWorkspaceServiceAccountTokensResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaceServiceAccountTokens.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspaceserviceaccounttokenspaginator)
-        """
-
-class ListWorkspaceServiceAccountsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaceServiceAccounts)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspaceserviceaccountspaginator)
-    """
-
-    def paginate(
-        self, *, workspaceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListWorkspaceServiceAccountsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaceServiceAccounts.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspaceserviceaccountspaginator)
-        """
-
 class ListWorkspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspacespaginator)
     """
 
     def paginate(
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/type_defs.py` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AssertionAttributesTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
@@ -47,85 +47,59 @@
     "AssociateLicenseRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
     "NetworkAccessConfigurationTypeDef",
     "VpcConfigurationTypeDef",
-    "CreateWorkspaceServiceAccountRequestRequestTypeDef",
-    "CreateWorkspaceServiceAccountTokenRequestRequestTypeDef",
-    "ServiceAccountTokenSummaryWithKeyTypeDef",
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
-    "DeleteWorkspaceServiceAccountRequestRequestTypeDef",
-    "DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef",
     "DescribeWorkspaceAuthenticationRequestRequestTypeDef",
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
     "IdpMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVersionsRequestRequestTypeDef",
-    "ListWorkspaceServiceAccountTokensRequestRequestTypeDef",
-    "ServiceAccountTokenSummaryTypeDef",
-    "ListWorkspaceServiceAccountsRequestRequestTypeDef",
-    "ServiceAccountSummaryTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
-    "NetworkAccessConfigurationOutputTypeDef",
     "UserTypeDef",
-    "RoleValuesOutputTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "CreateWorkspaceApiKeyResponseTypeDef",
-    "CreateWorkspaceServiceAccountResponseTypeDef",
     "DeleteWorkspaceApiKeyResponseTypeDef",
-    "DeleteWorkspaceServiceAccountResponseTypeDef",
-    "DeleteWorkspaceServiceAccountTokenResponseTypeDef",
     "DescribeWorkspaceConfigurationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListVersionsResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
-    "CreateWorkspaceServiceAccountTokenResponseTypeDef",
+    "WorkspaceDescriptionTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListVersionsRequestListVersionsPaginateTypeDef",
-    "ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef",
-    "ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
-    "ListWorkspaceServiceAccountTokensResponseTypeDef",
-    "ListWorkspaceServiceAccountsResponseTypeDef",
-    "NetworkAccessConfigurationUnionTypeDef",
     "PermissionEntryTypeDef",
-    "UpdateInstructionOutputTypeDef",
     "UpdateInstructionTypeDef",
-    "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
-    "VpcConfigurationUnionTypeDef",
-    "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "UpdateErrorTypeDef",
-    "UpdateInstructionUnionTypeDef",
-    "SamlAuthenticationTypeDef",
-    "SamlConfigurationUnionTypeDef",
-    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
-    "UpdatePermissionsResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "UpdateErrorTypeDef",
     "UpdatePermissionsRequestRequestTypeDef",
+    "SamlAuthenticationTypeDef",
+    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    "UpdatePermissionsResponseTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
@@ -177,48 +151,23 @@
         "secondsToLive": int,
         "workspaceId": str,
     },
 )
 NetworkAccessConfigurationTypeDef = TypedDict(
     "NetworkAccessConfigurationTypeDef",
     {
-        "prefixListIds": Sequence[str],
-        "vpceIds": Sequence[str],
+        "prefixListIds": List[str],
+        "vpceIds": List[str],
     },
 )
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
-        "securityGroupIds": Sequence[str],
-        "subnetIds": Sequence[str],
-    },
-)
-CreateWorkspaceServiceAccountRequestRequestTypeDef = TypedDict(
-    "CreateWorkspaceServiceAccountRequestRequestTypeDef",
-    {
-        "grafanaRole": RoleType,
-        "name": str,
-        "workspaceId": str,
-    },
-)
-CreateWorkspaceServiceAccountTokenRequestRequestTypeDef = TypedDict(
-    "CreateWorkspaceServiceAccountTokenRequestRequestTypeDef",
-    {
-        "name": str,
-        "secondsToLive": int,
-        "serviceAccountId": str,
-        "workspaceId": str,
-    },
-)
-ServiceAccountTokenSummaryWithKeyTypeDef = TypedDict(
-    "ServiceAccountTokenSummaryWithKeyTypeDef",
-    {
-        "id": str,
-        "key": str,
-        "name": str,
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
     },
 )
 DeleteWorkspaceApiKeyRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
         "workspaceId": str,
@@ -226,29 +175,14 @@
 )
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
-DeleteWorkspaceServiceAccountRequestRequestTypeDef = TypedDict(
-    "DeleteWorkspaceServiceAccountRequestRequestTypeDef",
-    {
-        "serviceAccountId": str,
-        "workspaceId": str,
-    },
-)
-DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef = TypedDict(
-    "DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef",
-    {
-        "serviceAccountId": str,
-        "tokenId": str,
-        "workspaceId": str,
-    },
-)
 DescribeWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceAuthenticationRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 DescribeWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
@@ -306,83 +240,33 @@
     "ListVersionsRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "workspaceId": NotRequired[str],
     },
 )
-ListWorkspaceServiceAccountTokensRequestRequestTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountTokensRequestRequestTypeDef",
-    {
-        "serviceAccountId": str,
-        "workspaceId": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
-ServiceAccountTokenSummaryTypeDef = TypedDict(
-    "ServiceAccountTokenSummaryTypeDef",
-    {
-        "createdAt": datetime,
-        "expiresAt": datetime,
-        "id": str,
-        "name": str,
-        "lastUsedAt": NotRequired[datetime],
-    },
-)
-ListWorkspaceServiceAccountsRequestRequestTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountsRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
-ServiceAccountSummaryTypeDef = TypedDict(
-    "ServiceAccountSummaryTypeDef",
-    {
-        "grafanaRole": RoleType,
-        "id": str,
-        "isDisabled": str,
-        "name": str,
-    },
-)
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
-NetworkAccessConfigurationOutputTypeDef = TypedDict(
-    "NetworkAccessConfigurationOutputTypeDef",
-    {
-        "prefixListIds": List[str],
-        "vpceIds": List[str],
-    },
-)
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "id": str,
         "type": UserTypeType,
     },
 )
-RoleValuesOutputTypeDef = TypedDict(
-    "RoleValuesOutputTypeDef",
-    {
-        "admin": NotRequired[List[str]],
-        "editor": NotRequired[List[str]],
-    },
-)
 RoleValuesTypeDef = TypedDict(
     "RoleValuesTypeDef",
     {
-        "admin": NotRequired[Sequence[str]],
-        "editor": NotRequired[Sequence[str]],
+        "admin": NotRequired[List[str]],
+        "editor": NotRequired[List[str]],
     },
 )
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -399,65 +283,31 @@
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
         "grafanaVersion": NotRequired[str],
     },
 )
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-    },
-)
 CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
     "CreateWorkspaceApiKeyResponseTypeDef",
     {
         "key": str,
         "keyName": str,
         "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateWorkspaceServiceAccountResponseTypeDef = TypedDict(
-    "CreateWorkspaceServiceAccountResponseTypeDef",
-    {
-        "grafanaRole": RoleType,
-        "id": str,
-        "name": str,
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DeleteWorkspaceApiKeyResponseTypeDef = TypedDict(
     "DeleteWorkspaceApiKeyResponseTypeDef",
     {
         "keyName": str,
         "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DeleteWorkspaceServiceAccountResponseTypeDef = TypedDict(
-    "DeleteWorkspaceServiceAccountResponseTypeDef",
-    {
-        "serviceAccountId": str,
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DeleteWorkspaceServiceAccountTokenResponseTypeDef = TypedDict(
-    "DeleteWorkspaceServiceAccountTokenResponseTypeDef",
-    {
-        "serviceAccountId": str,
-        "tokenId": str,
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
     "DescribeWorkspaceConfigurationResponseTypeDef",
     {
         "configuration": str,
         "grafanaVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -533,21 +383,42 @@
         "workspaceDescription": NotRequired[str],
         "workspaceName": NotRequired[str],
         "workspaceNotificationDestinations": NotRequired[Sequence[Literal["SNS"]]],
         "workspaceOrganizationalUnits": NotRequired[Sequence[str]],
         "workspaceRoleArn": NotRequired[str],
     },
 )
-CreateWorkspaceServiceAccountTokenResponseTypeDef = TypedDict(
-    "CreateWorkspaceServiceAccountTokenResponseTypeDef",
+WorkspaceDescriptionTypeDef = TypedDict(
+    "WorkspaceDescriptionTypeDef",
     {
-        "serviceAccountId": str,
-        "serviceAccountToken": ServiceAccountTokenSummaryWithKeyTypeDef,
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "authentication": AuthenticationSummaryTypeDef,
+        "created": datetime,
+        "dataSources": List[DataSourceTypeType],
+        "endpoint": str,
+        "grafanaVersion": str,
+        "id": str,
+        "modified": datetime,
+        "status": WorkspaceStatusType,
+        "accountAccessType": NotRequired[AccountAccessTypeType],
+        "description": NotRequired[str],
+        "freeTrialConsumed": NotRequired[bool],
+        "freeTrialExpiration": NotRequired[datetime],
+        "grafanaToken": NotRequired[str],
+        "licenseExpiration": NotRequired[datetime],
+        "licenseType": NotRequired[LicenseTypeType],
+        "name": NotRequired[str],
+        "networkAccessControl": NotRequired[NetworkAccessConfigurationTypeDef],
+        "notificationDestinations": NotRequired[List[Literal["SNS"]]],
+        "organizationRoleName": NotRequired[str],
+        "organizationalUnits": NotRequired[List[str]],
+        "permissionType": NotRequired[PermissionTypeType],
+        "stackSetName": NotRequired[str],
+        "tags": NotRequired[Dict[str, str]],
+        "vpcConfiguration": NotRequired[VpcConfigurationTypeDef],
+        "workspaceRoleArn": NotRequired[str],
     },
 )
 ListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "workspaceId": str,
         "groupId": NotRequired[str],
@@ -559,174 +430,53 @@
 ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
     "ListVersionsRequestListVersionsPaginateTypeDef",
     {
         "workspaceId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef = (
-    TypedDict(
-        "ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef",
-        {
-            "serviceAccountId": str,
-            "workspaceId": str,
-            "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-        },
-    )
-)
-ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef",
-    {
-        "workspaceId": str,
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-    },
-)
 ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListWorkspaceServiceAccountTokensResponseTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountTokensResponseTypeDef",
-    {
-        "nextToken": str,
-        "serviceAccountId": str,
-        "serviceAccountTokens": List[ServiceAccountTokenSummaryTypeDef],
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListWorkspaceServiceAccountsResponseTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountsResponseTypeDef",
-    {
-        "nextToken": str,
-        "serviceAccounts": List[ServiceAccountSummaryTypeDef],
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-NetworkAccessConfigurationUnionTypeDef = Union[
-    NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
-]
 PermissionEntryTypeDef = TypedDict(
     "PermissionEntryTypeDef",
     {
         "role": RoleType,
         "user": UserTypeDef,
     },
 )
-UpdateInstructionOutputTypeDef = TypedDict(
-    "UpdateInstructionOutputTypeDef",
-    {
-        "action": UpdateActionType,
-        "role": RoleType,
-        "users": List[UserTypeDef],
-    },
-)
 UpdateInstructionTypeDef = TypedDict(
     "UpdateInstructionTypeDef",
     {
         "action": UpdateActionType,
         "role": RoleType,
         "users": Sequence[UserTypeDef],
     },
 )
-SamlConfigurationOutputTypeDef = TypedDict(
-    "SamlConfigurationOutputTypeDef",
-    {
-        "idpMetadata": IdpMetadataTypeDef,
-        "allowedOrganizations": NotRequired[List[str]],
-        "assertionAttributes": NotRequired[AssertionAttributesTypeDef],
-        "loginValidityDuration": NotRequired[int],
-        "roleValues": NotRequired[RoleValuesOutputTypeDef],
-    },
-)
 SamlConfigurationTypeDef = TypedDict(
     "SamlConfigurationTypeDef",
     {
         "idpMetadata": IdpMetadataTypeDef,
-        "allowedOrganizations": NotRequired[Sequence[str]],
+        "allowedOrganizations": NotRequired[List[str]],
         "assertionAttributes": NotRequired[AssertionAttributesTypeDef],
         "loginValidityDuration": NotRequired[int],
         "roleValues": NotRequired[RoleValuesTypeDef],
     },
 )
-VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
-WorkspaceDescriptionTypeDef = TypedDict(
-    "WorkspaceDescriptionTypeDef",
-    {
-        "authentication": AuthenticationSummaryTypeDef,
-        "created": datetime,
-        "dataSources": List[DataSourceTypeType],
-        "endpoint": str,
-        "grafanaVersion": str,
-        "id": str,
-        "modified": datetime,
-        "status": WorkspaceStatusType,
-        "accountAccessType": NotRequired[AccountAccessTypeType],
-        "description": NotRequired[str],
-        "freeTrialConsumed": NotRequired[bool],
-        "freeTrialExpiration": NotRequired[datetime],
-        "grafanaToken": NotRequired[str],
-        "licenseExpiration": NotRequired[datetime],
-        "licenseType": NotRequired[LicenseTypeType],
-        "name": NotRequired[str],
-        "networkAccessControl": NotRequired[NetworkAccessConfigurationOutputTypeDef],
-        "notificationDestinations": NotRequired[List[Literal["SNS"]]],
-        "organizationRoleName": NotRequired[str],
-        "organizationalUnits": NotRequired[List[str]],
-        "permissionType": NotRequired[PermissionTypeType],
-        "stackSetName": NotRequired[str],
-        "tags": NotRequired[Dict[str, str]],
-        "vpcConfiguration": NotRequired[VpcConfigurationOutputTypeDef],
-        "workspaceRoleArn": NotRequired[str],
-    },
-)
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "permissions": List[PermissionEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateErrorTypeDef = TypedDict(
-    "UpdateErrorTypeDef",
-    {
-        "causedBy": UpdateInstructionOutputTypeDef,
-        "code": int,
-        "message": str,
-    },
-)
-UpdateInstructionUnionTypeDef = Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
-SamlAuthenticationTypeDef = TypedDict(
-    "SamlAuthenticationTypeDef",
-    {
-        "status": SamlConfigurationStatusType,
-        "configuration": NotRequired[SamlConfigurationOutputTypeDef],
-    },
-)
-SamlConfigurationUnionTypeDef = Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef]
-UpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
-    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
-    {
-        "authenticationProviders": Sequence[AuthenticationProviderTypesType],
-        "workspaceId": str,
-        "samlConfiguration": NotRequired[SamlConfigurationTypeDef],
-    },
-)
 AssociateLicenseResponseTypeDef = TypedDict(
     "AssociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -761,26 +511,57 @@
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdatePermissionsResponseTypeDef = TypedDict(
-    "UpdatePermissionsResponseTypeDef",
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
     {
-        "errors": List[UpdateErrorTypeDef],
+        "nextToken": str,
+        "permissions": List[PermissionEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateErrorTypeDef = TypedDict(
+    "UpdateErrorTypeDef",
+    {
+        "causedBy": UpdateInstructionTypeDef,
+        "code": int,
+        "message": str,
+    },
+)
 UpdatePermissionsRequestRequestTypeDef = TypedDict(
     "UpdatePermissionsRequestRequestTypeDef",
     {
-        "updateInstructionBatch": Sequence[UpdateInstructionUnionTypeDef],
+        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "workspaceId": str,
+    },
+)
+SamlAuthenticationTypeDef = TypedDict(
+    "SamlAuthenticationTypeDef",
+    {
+        "status": SamlConfigurationStatusType,
+        "configuration": NotRequired[SamlConfigurationTypeDef],
+    },
+)
+UpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
+    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    {
+        "authenticationProviders": Sequence[AuthenticationProviderTypesType],
         "workspaceId": str,
+        "samlConfiguration": NotRequired[SamlConfigurationTypeDef],
+    },
+)
+UpdatePermissionsResponseTypeDef = TypedDict(
+    "UpdatePermissionsResponseTypeDef",
+    {
+        "errors": List[UpdateErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 AuthenticationDescriptionTypeDef = TypedDict(
     "AuthenticationDescriptionTypeDef",
     {
         "providers": List[AuthenticationProviderTypesType],
         "awsSso": NotRequired[AwsSsoAuthenticationTypeDef],
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana/type_defs.pyi` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AssertionAttributesTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
@@ -47,85 +47,59 @@
     "AssociateLicenseRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
     "NetworkAccessConfigurationTypeDef",
     "VpcConfigurationTypeDef",
-    "CreateWorkspaceServiceAccountRequestRequestTypeDef",
-    "CreateWorkspaceServiceAccountTokenRequestRequestTypeDef",
-    "ServiceAccountTokenSummaryWithKeyTypeDef",
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
-    "DeleteWorkspaceServiceAccountRequestRequestTypeDef",
-    "DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef",
     "DescribeWorkspaceAuthenticationRequestRequestTypeDef",
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
     "IdpMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVersionsRequestRequestTypeDef",
-    "ListWorkspaceServiceAccountTokensRequestRequestTypeDef",
-    "ServiceAccountTokenSummaryTypeDef",
-    "ListWorkspaceServiceAccountsRequestRequestTypeDef",
-    "ServiceAccountSummaryTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
-    "NetworkAccessConfigurationOutputTypeDef",
     "UserTypeDef",
-    "RoleValuesOutputTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "CreateWorkspaceApiKeyResponseTypeDef",
-    "CreateWorkspaceServiceAccountResponseTypeDef",
     "DeleteWorkspaceApiKeyResponseTypeDef",
-    "DeleteWorkspaceServiceAccountResponseTypeDef",
-    "DeleteWorkspaceServiceAccountTokenResponseTypeDef",
     "DescribeWorkspaceConfigurationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListVersionsResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
-    "CreateWorkspaceServiceAccountTokenResponseTypeDef",
+    "WorkspaceDescriptionTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListVersionsRequestListVersionsPaginateTypeDef",
-    "ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef",
-    "ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
-    "ListWorkspaceServiceAccountTokensResponseTypeDef",
-    "ListWorkspaceServiceAccountsResponseTypeDef",
-    "NetworkAccessConfigurationUnionTypeDef",
     "PermissionEntryTypeDef",
-    "UpdateInstructionOutputTypeDef",
     "UpdateInstructionTypeDef",
-    "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
-    "VpcConfigurationUnionTypeDef",
-    "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "UpdateErrorTypeDef",
-    "UpdateInstructionUnionTypeDef",
-    "SamlAuthenticationTypeDef",
-    "SamlConfigurationUnionTypeDef",
-    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
-    "UpdatePermissionsResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "UpdateErrorTypeDef",
     "UpdatePermissionsRequestRequestTypeDef",
+    "SamlAuthenticationTypeDef",
+    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    "UpdatePermissionsResponseTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
@@ -177,48 +151,23 @@
         "secondsToLive": int,
         "workspaceId": str,
     },
 )
 NetworkAccessConfigurationTypeDef = TypedDict(
     "NetworkAccessConfigurationTypeDef",
     {
-        "prefixListIds": Sequence[str],
-        "vpceIds": Sequence[str],
+        "prefixListIds": List[str],
+        "vpceIds": List[str],
     },
 )
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
-        "securityGroupIds": Sequence[str],
-        "subnetIds": Sequence[str],
-    },
-)
-CreateWorkspaceServiceAccountRequestRequestTypeDef = TypedDict(
-    "CreateWorkspaceServiceAccountRequestRequestTypeDef",
-    {
-        "grafanaRole": RoleType,
-        "name": str,
-        "workspaceId": str,
-    },
-)
-CreateWorkspaceServiceAccountTokenRequestRequestTypeDef = TypedDict(
-    "CreateWorkspaceServiceAccountTokenRequestRequestTypeDef",
-    {
-        "name": str,
-        "secondsToLive": int,
-        "serviceAccountId": str,
-        "workspaceId": str,
-    },
-)
-ServiceAccountTokenSummaryWithKeyTypeDef = TypedDict(
-    "ServiceAccountTokenSummaryWithKeyTypeDef",
-    {
-        "id": str,
-        "key": str,
-        "name": str,
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
     },
 )
 DeleteWorkspaceApiKeyRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
         "workspaceId": str,
@@ -226,29 +175,14 @@
 )
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
-DeleteWorkspaceServiceAccountRequestRequestTypeDef = TypedDict(
-    "DeleteWorkspaceServiceAccountRequestRequestTypeDef",
-    {
-        "serviceAccountId": str,
-        "workspaceId": str,
-    },
-)
-DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef = TypedDict(
-    "DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef",
-    {
-        "serviceAccountId": str,
-        "tokenId": str,
-        "workspaceId": str,
-    },
-)
 DescribeWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceAuthenticationRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 DescribeWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
@@ -306,83 +240,33 @@
     "ListVersionsRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "workspaceId": NotRequired[str],
     },
 )
-ListWorkspaceServiceAccountTokensRequestRequestTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountTokensRequestRequestTypeDef",
-    {
-        "serviceAccountId": str,
-        "workspaceId": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
-ServiceAccountTokenSummaryTypeDef = TypedDict(
-    "ServiceAccountTokenSummaryTypeDef",
-    {
-        "createdAt": datetime,
-        "expiresAt": datetime,
-        "id": str,
-        "name": str,
-        "lastUsedAt": NotRequired[datetime],
-    },
-)
-ListWorkspaceServiceAccountsRequestRequestTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountsRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
-ServiceAccountSummaryTypeDef = TypedDict(
-    "ServiceAccountSummaryTypeDef",
-    {
-        "grafanaRole": RoleType,
-        "id": str,
-        "isDisabled": str,
-        "name": str,
-    },
-)
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
-NetworkAccessConfigurationOutputTypeDef = TypedDict(
-    "NetworkAccessConfigurationOutputTypeDef",
-    {
-        "prefixListIds": List[str],
-        "vpceIds": List[str],
-    },
-)
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "id": str,
         "type": UserTypeType,
     },
 )
-RoleValuesOutputTypeDef = TypedDict(
-    "RoleValuesOutputTypeDef",
-    {
-        "admin": NotRequired[List[str]],
-        "editor": NotRequired[List[str]],
-    },
-)
 RoleValuesTypeDef = TypedDict(
     "RoleValuesTypeDef",
     {
-        "admin": NotRequired[Sequence[str]],
-        "editor": NotRequired[Sequence[str]],
+        "admin": NotRequired[List[str]],
+        "editor": NotRequired[List[str]],
     },
 )
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -399,65 +283,31 @@
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
         "grafanaVersion": NotRequired[str],
     },
 )
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-    },
-)
 CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
     "CreateWorkspaceApiKeyResponseTypeDef",
     {
         "key": str,
         "keyName": str,
         "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateWorkspaceServiceAccountResponseTypeDef = TypedDict(
-    "CreateWorkspaceServiceAccountResponseTypeDef",
-    {
-        "grafanaRole": RoleType,
-        "id": str,
-        "name": str,
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DeleteWorkspaceApiKeyResponseTypeDef = TypedDict(
     "DeleteWorkspaceApiKeyResponseTypeDef",
     {
         "keyName": str,
         "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DeleteWorkspaceServiceAccountResponseTypeDef = TypedDict(
-    "DeleteWorkspaceServiceAccountResponseTypeDef",
-    {
-        "serviceAccountId": str,
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DeleteWorkspaceServiceAccountTokenResponseTypeDef = TypedDict(
-    "DeleteWorkspaceServiceAccountTokenResponseTypeDef",
-    {
-        "serviceAccountId": str,
-        "tokenId": str,
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
     "DescribeWorkspaceConfigurationResponseTypeDef",
     {
         "configuration": str,
         "grafanaVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -533,21 +383,42 @@
         "workspaceDescription": NotRequired[str],
         "workspaceName": NotRequired[str],
         "workspaceNotificationDestinations": NotRequired[Sequence[Literal["SNS"]]],
         "workspaceOrganizationalUnits": NotRequired[Sequence[str]],
         "workspaceRoleArn": NotRequired[str],
     },
 )
-CreateWorkspaceServiceAccountTokenResponseTypeDef = TypedDict(
-    "CreateWorkspaceServiceAccountTokenResponseTypeDef",
+WorkspaceDescriptionTypeDef = TypedDict(
+    "WorkspaceDescriptionTypeDef",
     {
-        "serviceAccountId": str,
-        "serviceAccountToken": ServiceAccountTokenSummaryWithKeyTypeDef,
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "authentication": AuthenticationSummaryTypeDef,
+        "created": datetime,
+        "dataSources": List[DataSourceTypeType],
+        "endpoint": str,
+        "grafanaVersion": str,
+        "id": str,
+        "modified": datetime,
+        "status": WorkspaceStatusType,
+        "accountAccessType": NotRequired[AccountAccessTypeType],
+        "description": NotRequired[str],
+        "freeTrialConsumed": NotRequired[bool],
+        "freeTrialExpiration": NotRequired[datetime],
+        "grafanaToken": NotRequired[str],
+        "licenseExpiration": NotRequired[datetime],
+        "licenseType": NotRequired[LicenseTypeType],
+        "name": NotRequired[str],
+        "networkAccessControl": NotRequired[NetworkAccessConfigurationTypeDef],
+        "notificationDestinations": NotRequired[List[Literal["SNS"]]],
+        "organizationRoleName": NotRequired[str],
+        "organizationalUnits": NotRequired[List[str]],
+        "permissionType": NotRequired[PermissionTypeType],
+        "stackSetName": NotRequired[str],
+        "tags": NotRequired[Dict[str, str]],
+        "vpcConfiguration": NotRequired[VpcConfigurationTypeDef],
+        "workspaceRoleArn": NotRequired[str],
     },
 )
 ListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "workspaceId": str,
         "groupId": NotRequired[str],
@@ -559,174 +430,53 @@
 ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
     "ListVersionsRequestListVersionsPaginateTypeDef",
     {
         "workspaceId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef = (
-    TypedDict(
-        "ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef",
-        {
-            "serviceAccountId": str,
-            "workspaceId": str,
-            "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-        },
-    )
-)
-ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef",
-    {
-        "workspaceId": str,
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-    },
-)
 ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListWorkspaceServiceAccountTokensResponseTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountTokensResponseTypeDef",
-    {
-        "nextToken": str,
-        "serviceAccountId": str,
-        "serviceAccountTokens": List[ServiceAccountTokenSummaryTypeDef],
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListWorkspaceServiceAccountsResponseTypeDef = TypedDict(
-    "ListWorkspaceServiceAccountsResponseTypeDef",
-    {
-        "nextToken": str,
-        "serviceAccounts": List[ServiceAccountSummaryTypeDef],
-        "workspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-NetworkAccessConfigurationUnionTypeDef = Union[
-    NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
-]
 PermissionEntryTypeDef = TypedDict(
     "PermissionEntryTypeDef",
     {
         "role": RoleType,
         "user": UserTypeDef,
     },
 )
-UpdateInstructionOutputTypeDef = TypedDict(
-    "UpdateInstructionOutputTypeDef",
-    {
-        "action": UpdateActionType,
-        "role": RoleType,
-        "users": List[UserTypeDef],
-    },
-)
 UpdateInstructionTypeDef = TypedDict(
     "UpdateInstructionTypeDef",
     {
         "action": UpdateActionType,
         "role": RoleType,
         "users": Sequence[UserTypeDef],
     },
 )
-SamlConfigurationOutputTypeDef = TypedDict(
-    "SamlConfigurationOutputTypeDef",
-    {
-        "idpMetadata": IdpMetadataTypeDef,
-        "allowedOrganizations": NotRequired[List[str]],
-        "assertionAttributes": NotRequired[AssertionAttributesTypeDef],
-        "loginValidityDuration": NotRequired[int],
-        "roleValues": NotRequired[RoleValuesOutputTypeDef],
-    },
-)
 SamlConfigurationTypeDef = TypedDict(
     "SamlConfigurationTypeDef",
     {
         "idpMetadata": IdpMetadataTypeDef,
-        "allowedOrganizations": NotRequired[Sequence[str]],
+        "allowedOrganizations": NotRequired[List[str]],
         "assertionAttributes": NotRequired[AssertionAttributesTypeDef],
         "loginValidityDuration": NotRequired[int],
         "roleValues": NotRequired[RoleValuesTypeDef],
     },
 )
-VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
-WorkspaceDescriptionTypeDef = TypedDict(
-    "WorkspaceDescriptionTypeDef",
-    {
-        "authentication": AuthenticationSummaryTypeDef,
-        "created": datetime,
-        "dataSources": List[DataSourceTypeType],
-        "endpoint": str,
-        "grafanaVersion": str,
-        "id": str,
-        "modified": datetime,
-        "status": WorkspaceStatusType,
-        "accountAccessType": NotRequired[AccountAccessTypeType],
-        "description": NotRequired[str],
-        "freeTrialConsumed": NotRequired[bool],
-        "freeTrialExpiration": NotRequired[datetime],
-        "grafanaToken": NotRequired[str],
-        "licenseExpiration": NotRequired[datetime],
-        "licenseType": NotRequired[LicenseTypeType],
-        "name": NotRequired[str],
-        "networkAccessControl": NotRequired[NetworkAccessConfigurationOutputTypeDef],
-        "notificationDestinations": NotRequired[List[Literal["SNS"]]],
-        "organizationRoleName": NotRequired[str],
-        "organizationalUnits": NotRequired[List[str]],
-        "permissionType": NotRequired[PermissionTypeType],
-        "stackSetName": NotRequired[str],
-        "tags": NotRequired[Dict[str, str]],
-        "vpcConfiguration": NotRequired[VpcConfigurationOutputTypeDef],
-        "workspaceRoleArn": NotRequired[str],
-    },
-)
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "permissions": List[PermissionEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateErrorTypeDef = TypedDict(
-    "UpdateErrorTypeDef",
-    {
-        "causedBy": UpdateInstructionOutputTypeDef,
-        "code": int,
-        "message": str,
-    },
-)
-UpdateInstructionUnionTypeDef = Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
-SamlAuthenticationTypeDef = TypedDict(
-    "SamlAuthenticationTypeDef",
-    {
-        "status": SamlConfigurationStatusType,
-        "configuration": NotRequired[SamlConfigurationOutputTypeDef],
-    },
-)
-SamlConfigurationUnionTypeDef = Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef]
-UpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
-    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
-    {
-        "authenticationProviders": Sequence[AuthenticationProviderTypesType],
-        "workspaceId": str,
-        "samlConfiguration": NotRequired[SamlConfigurationTypeDef],
-    },
-)
 AssociateLicenseResponseTypeDef = TypedDict(
     "AssociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -761,26 +511,57 @@
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdatePermissionsResponseTypeDef = TypedDict(
-    "UpdatePermissionsResponseTypeDef",
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
     {
-        "errors": List[UpdateErrorTypeDef],
+        "nextToken": str,
+        "permissions": List[PermissionEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateErrorTypeDef = TypedDict(
+    "UpdateErrorTypeDef",
+    {
+        "causedBy": UpdateInstructionTypeDef,
+        "code": int,
+        "message": str,
+    },
+)
 UpdatePermissionsRequestRequestTypeDef = TypedDict(
     "UpdatePermissionsRequestRequestTypeDef",
     {
-        "updateInstructionBatch": Sequence[UpdateInstructionUnionTypeDef],
+        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "workspaceId": str,
+    },
+)
+SamlAuthenticationTypeDef = TypedDict(
+    "SamlAuthenticationTypeDef",
+    {
+        "status": SamlConfigurationStatusType,
+        "configuration": NotRequired[SamlConfigurationTypeDef],
+    },
+)
+UpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
+    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    {
+        "authenticationProviders": Sequence[AuthenticationProviderTypesType],
         "workspaceId": str,
+        "samlConfiguration": NotRequired[SamlConfigurationTypeDef],
+    },
+)
+UpdatePermissionsResponseTypeDef = TypedDict(
+    "UpdatePermissionsResponseTypeDef",
+    {
+        "errors": List[UpdateErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 AuthenticationDescriptionTypeDef = TypedDict(
     "AuthenticationDescriptionTypeDef",
     {
         "providers": List[AuthenticationProviderTypesType],
         "awsSso": NotRequired[AwsSsoAuthenticationTypeDef],
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/PKG-INFO` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.34.106
-Summary: Type annotations for boto3.ManagedGrafana 1.34.106 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.58
+Summary: Type annotations for boto3.ManagedGrafana 1.34.58 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.34.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,31 +282,23 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_grafana import ManagedGrafanaClient
 from mypy_boto3_grafana.paginator import (
     ListPermissionsPaginator,
     ListVersionsPaginator,
-    ListWorkspaceServiceAccountTokensPaginator,
-    ListWorkspaceServiceAccountsPaginator,
     ListWorkspacesPaginator,
 )
 
 client: ManagedGrafanaClient = Session().client("grafana")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
 list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
-list_workspace_service_account_tokens_paginator: ListWorkspaceServiceAccountTokensPaginator = (
-    client.get_paginator("list_workspace_service_account_tokens")
-)
-list_workspace_service_accounts_paginator: ListWorkspaceServiceAccountsPaginator = (
-    client.get_paginator("list_workspace_service_accounts")
-)
 list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `mypy_boto3_grafana-1.34.106/mypy_boto3_grafana.egg-info/SOURCES.txt` & `mypy-boto3-grafana-1.34.58/mypy_boto3_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_grafana-1.34.106/setup.py` & `mypy-boto3-grafana-1.34.58/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-grafana",
-    version="1.34.106",
+    version="1.34.58",
     packages=["mypy_boto3_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ManagedGrafana 1.34.106 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.ManagedGrafana 1.34.58 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

