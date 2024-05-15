# Comparing `tmp/dss-sdk-1.2.2.tar.gz` & `tmp/dss_sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dss-sdk-1.2.2.tar", last modified: Wed Mar  6 16:42:41 2024, max compression
+gzip compressed data, was "dss_sdk-1.3.0.tar", last modified: Wed May 15 17:30:00 2024, max compression
```

## Comparing `dss-sdk-1.2.2.tar` & `dss_sdk-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 cjriebe   (1000) cjriebe   (1000)        0 2024-03-06 16:42:41.408318 dss-sdk-1.2.2/
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    35149 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/LICENSE
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    59101 2024-03-06 16:42:41.398318 dss-sdk-1.2.2/PKG-INFO
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    17215 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/README.md
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)      751 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/backend_shim.py
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)     2468 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/pyproject.toml
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)       38 2024-03-06 16:42:41.408318 dss-sdk-1.2.2/setup.cfg
-drwxr-xr-x   0 cjriebe   (1000) cjriebe   (1000)        0 2024-03-06 16:42:41.398318 dss-sdk-1.2.2/src/
-drwxr-xr-x   0 cjriebe   (1000) cjriebe   (1000)        0 2024-03-06 16:42:41.398318 dss-sdk-1.2.2/src/dss_sdk/
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)       57 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk/__init__.py
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)      351 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk/__version__.py
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    12852 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk/cli.py
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    13765 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk/credentials.py
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    15221 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk/models.py
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    10694 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk/server.py
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)     4189 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk/utilities.py
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)     8455 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk/windows_credentials.py
-drwxr-xr-x   0 cjriebe   (1000) cjriebe   (1000)        0 2024-03-06 16:42:41.398318 dss-sdk-1.2.2/src/dss_sdk.egg-info/
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    59101 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk.egg-info/PKG-INFO
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)      461 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)        1 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)       41 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk.egg-info/entry_points.txt
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)       85 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk.egg-info/requires.txt
--rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)        8 2024-03-06 16:42:41.000000 dss-sdk-1.2.2/src/dss_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 cjriebe   (1000) cjriebe   (1000)        0 2024-05-15 17:30:00.420472 dss_sdk-1.3.0/
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    35149 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/LICENSE
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    59252 2024-05-15 17:30:00.420472 dss_sdk-1.3.0/PKG-INFO
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    17215 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/README.md
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)      751 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/backend_shim.py
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)     2609 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/pyproject.toml
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)       38 2024-05-15 17:30:00.420472 dss_sdk-1.3.0/setup.cfg
+drwxr-xr-x   0 cjriebe   (1000) cjriebe   (1000)        0 2024-05-15 17:30:00.420472 dss_sdk-1.3.0/src/
+drwxr-xr-x   0 cjriebe   (1000) cjriebe   (1000)        0 2024-05-15 17:30:00.420472 dss_sdk-1.3.0/src/dss_sdk/
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)       57 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/src/dss_sdk/__init__.py
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)      351 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/src/dss_sdk/__version__.py
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    15153 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/src/dss_sdk/cli.py
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    22344 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/src/dss_sdk/credentials.py
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    17985 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/src/dss_sdk/models.py
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    11457 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/src/dss_sdk/server.py
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)     5194 2024-05-15 17:29:59.000000 dss_sdk-1.3.0/src/dss_sdk/utilities.py
+drwxr-xr-x   0 cjriebe   (1000) cjriebe   (1000)        0 2024-05-15 17:30:00.420472 dss_sdk-1.3.0/src/dss_sdk.egg-info/
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)    59252 2024-05-15 17:30:00.000000 dss_sdk-1.3.0/src/dss_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)      426 2024-05-15 17:30:00.000000 dss_sdk-1.3.0/src/dss_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)        1 2024-05-15 17:30:00.000000 dss_sdk-1.3.0/src/dss_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)       41 2024-05-15 17:30:00.000000 dss_sdk-1.3.0/src/dss_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)      130 2024-05-15 17:30:00.000000 dss_sdk-1.3.0/src/dss_sdk.egg-info/requires.txt
+-rw-r--r--   0 cjriebe   (1000) cjriebe   (1000)        8 2024-05-15 17:30:00.000000 dss_sdk-1.3.0/src/dss_sdk.egg-info/top_level.txt
```

### Comparing `dss-sdk-1.2.2/LICENSE` & `dss_sdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dss-sdk-1.2.2/PKG-INFO` & `dss_sdk-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dss-sdk
-Version: 1.2.2
+Version: 1.3.0
 Summary: A better SDK for Delinea Secret Server
 Author: riebecj
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,18 @@
 Requires-Dist: httpx~=0.26
 Requires-Dist: pydantic~=2.4
 Requires-Dist: typer~=0.9
 Requires-Dist: click~=8.1
 Requires-Dist: rich~=13.7
 Requires-Dist: pyperclip~=1.8
 Requires-Dist: toml~=0.10
+Provides-Extra: dev
+Requires-Dist: pytest~=7.4; extra == "dev"
+Requires-Dist: pytest-cov~=4.1; extra == "dev"
+Requires-Dist: ruff~=0.3; extra == "dev"
 
 # dss-sdk
 A better SDK for Delinea Secret Server.
 
 This is an SDK and CLI for interacting with Delinea Secret Server. The CLI uses [Typer](https://typer.tiangolo.com/), 
 and the SDK uses [httpx](https://www.python-httpx.org/). Both use [Pydantic](https://docs.pydantic.dev/latest/) for 
 data serialization from the Delinea APIs.
```

### Comparing `dss-sdk-1.2.2/README.md` & `dss_sdk-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dss-sdk-1.2.2/backend_shim.py` & `dss_sdk-1.3.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `dss-sdk-1.2.2/pyproject.toml` & `dss_sdk-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,32 +37,42 @@
     "pydantic~=2.4",
     "typer~=0.9",
     "click~=8.1",
     "rich~=13.7",
     "pyperclip~=1.8",
     "toml~=0.10"
 ]
-version = "1.2.2"
+version = "1.3.0"
+
+
+[project.optional-dependencies]
+dev = [
+    "pytest~=7.4",
+    "pytest-cov~=4.1",
+    "ruff~=0.3",
+]
 
 [project.scripts]
 dss = "dss_sdk.cli:main"
 
 [tool.ruff]
 line-length = 120
 target-version = "py311"
+
+[tool.ruff.lint]
 fixable = ["ALL"]
 select = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ",
     "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE",
     "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 ignore = ["ANN101", "ANN102", "D203", "D212"]
 
-[tool.ruff.pylint]
+[tool.ruff.lint.pylint]
 max-args = 6
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 addopts = "--cov=dss_sdk --cov-report term-missing"
 testpaths = ["tests"]
 python_files = ["test_*.py"]
```

### Comparing `dss-sdk-1.2.2/src/dss_sdk/cli.py` & `dss_sdk-1.3.0/src/dss_sdk/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 """The DSS CLI."""
 import platform
-from typing import Annotated
+import time
+import typing
 
+import click
 import pyperclip
-from click import Abort, ClickException, Context, confirm, prompt
-from rich.console import Console
-from rich.table import Table
-from rich.text import Text
-from typer import Option, Typer
-
-from dss_sdk.credentials import CredFileProvider
-from dss_sdk.models import SearchFoldersParams, SearchSecretsParams
-from dss_sdk.server import RegisterClient, SecretServerClient
-from dss_sdk.utilities import (
-    HelpText,
-    OutputTypes,
-    SearchSecretsExtraFields,
-    format_dtg,
-    hide_non_windows,
-    version_callback,
-)
-from dss_sdk.windows_credentials import Windows
+import rich
+import rich.table
+import rich.text
+import typer
 
-cli = Typer()
+from . import credentials, models, utilities
+from . import server as ss
+
+cli = typer.Typer()
 
 
 def config_prompt(
         profile_config: dict,
         key: str,
         message: str,
         *,
         required: bool = False,
-        prompt_kwargs: dict = None,
+        prompt_kwargs: dict | None = None,
 ) -> str | None:
     """Method used when configuring a profile in the credentials file.
 
     Args:
         profile_config: The credentials file profile config.
         key: The key for the item in the profile config.
         message: The message used in the prompt.
@@ -44,228 +35,265 @@
     """
     if not prompt_kwargs:
         prompt_kwargs = {}
 
     current_value = profile_config.get(key)
 
     while True:
-        new_value = prompt(message, default=current_value if current_value else "", **prompt_kwargs)
+        new_value = click.prompt(message, default=current_value if current_value else "", **prompt_kwargs)
 
         if new_value:
             return new_value
         if not new_value and not current_value and required:
-            Console().print(f"A {key} is required.")
+            rich.console.Console().print(f"A {key} is required.")
         else:
             return current_value
 
 
 @cli.command()
 def register_client(
         service_account: str,
-        onboarding_key: Annotated[str, Option(prompt=True, hide_input=True)],
-        description: Annotated[str, Option(show_default=False)] = None,
-        server: Annotated[str, Option()] = None,
-        store_in_windows: Annotated[bool, Option(
-            "--store-in-windows", help=HelpText.store_in_windows, hidden=hide_non_windows(),
-        )] = False,  # noqa: FBT002
-        output_format: Annotated[OutputTypes, Option()] = OutputTypes.CLIPBOARD.value,
+        onboarding_key: typing.Annotated[str, typer.Option(prompt=True, hide_input=True)],
+        description: typing.Annotated[str | None, typer.Option(show_default=False)] = None,
+        server: typing.Annotated[str | None, typer.Option()] = None,
+        store_in_windows: typing.Annotated[bool | None, typer.Option(
+            "--store-in-windows", help=utilities.HelpText.store_in_windows,
+            hidden=utilities.hide_non_windows())] = None,
+        output_format: typing.Annotated[utilities.OutputTypes, typer.Option()] = utilities.OutputTypes.CLIPBOARD.value,
 ) -> None:
     """Registers a new client with your server."""
     if not server:
-        CredFileProvider.ensure_file()
-        creds = CredFileProvider.read_file()
+        credentials.CredFileProvider.ensure_file()
+        creds = credentials.CredFileProvider.read_file()
         server = creds.get("default", {}).get("server")
         if not server:
             msg = "No default server found and --server not provided."
-            raise ClickException(msg)
+            raise click.ClickException(msg)
 
-    client_id, client_secret = RegisterClient(
+    client_id, client_secret = ss.RegisterClient(
         server=server, service_account=service_account, onboarding_key=onboarding_key, description=description,
     )
 
     if store_in_windows:
         store_windows_credential(client_id=client_id, client_secret=client_secret)
         return
 
-    if output_format == OutputTypes.JSON:
-        Console().print({"client_id": client_id, "client_secret": client_secret})
-    elif output_format == OutputTypes.TABLE:
-        table = Table("Name", "Value")
+    if output_format == utilities.OutputTypes.JSON:
+        rich.console.Console().print({"client_id": client_id, "client_secret": client_secret})
+    elif output_format == utilities.OutputTypes.TABLE:
+        table = rich.table.Table("Name", "Value")
         table.add_row("Client ID", client_id)
         table.add_row("Client Secret", client_secret)
-        Console().print(table)
+        rich.console.Console().print(table)
     else:
-        Console().print(f"Client ID: {client_id}")
+        rich.console.Console().print(f"Client ID: {client_id}")
         pyperclip.copy(client_secret)
-        Console().print("Client Secret copied to clipboard.")
+        rich.console.Console().print("Client Secret copied to clipboard.")
 
 
 @cli.command()
 def get_secret(
-        context: Context,
+        context: click.Context,
         secret_id: int,
-        include_username: Annotated[bool, Option(
-            "--include-username", help=HelpText.include_username,
-        )] = False,  # noqa: FBT002
-        output_format: Annotated[OutputTypes, Option(help=HelpText.output_format)] = OutputTypes.CLIPBOARD.value,
+        include_username: typing.Annotated[bool | None, typer.Option(
+            "--include-username", help=utilities.HelpText.include_username)] = None,
+        output_format: typing.Annotated[utilities.OutputTypes, typer.Option(
+            help=utilities.HelpText.output_format)] = utilities.OutputTypes.CLIPBOARD.value,
 ) -> None:
     """Gets a secret."""
-    secret = context.obj.get_secret(secret_id=secret_id)
+    server: ss.SecretServerClient = context.obj
+    secret = server.get_secret(secret_id=secret_id)
 
     username = secret.get_username()
     password = secret.get_password()
 
-    if output_format == OutputTypes.JSON:
+    if output_format == utilities.OutputTypes.JSON:
         output = {"password": password}
         if include_username:
             output["username"] = username
-    elif output_format == OutputTypes.TABLE:
-        output = Table("Type", "Value")
+    elif output_format == utilities.OutputTypes.TABLE:
+        output = rich.table.Table("Type", "Value")
         output.add_row("Password", password)
         if include_username:
             output.add_row("Username", username)
     else:
         pyperclip.copy(password)
         output = f"Secret for {username} copied to clipboard."
 
-    Console().print(output)
+    rich.console.Console().print(output)
 
 
 @cli.command()
 def search_folders(
-    context: Context,
-    parent_folder_id: Annotated[int, Option(show_default=False, help=HelpText.parent_folder_id)] = None,
-    search_text: Annotated[str, Option(show_default=False, help=HelpText.search_text)] = None,
+    context: click.Context,
+    parent_folder_id: typing.Annotated[int | None, typer.Option(
+        show_default=False, help=utilities.HelpText.parent_folder_id)] = None,
+    search_text: typing.Annotated[str | None, typer.Option(
+        show_default=False, help=utilities.HelpText.search_text)] = None,
 ) -> None:
     """Search for accessible folders."""
-    params = SearchFoldersParams(
+    params = models.SearchFoldersParams(
         parent_folder_id=parent_folder_id,
         search_text=search_text,
     )
 
-    folders = context.obj.get_folders(params=params)
-    table = Table("Name", "ID", "Path", "Parent Folder ID", "Folder Type ID", "Inherit Permissions")
+    server: ss.SecretServerClient = context.obj
+    folders = server.get_folders(params=params)
+    table = rich.table.Table("Name", "ID", "Path", "Parent Folder ID", "Folder Type ID", "Inherit Permissions")
 
     for folder in folders.folders:
         table.add_row(
             folder.name, str(folder.folder_id), folder.path, str(folder.parent_folder_id),
             str(folder.folder_type_id), str(folder.inherit_permissions),
         )
 
-    Console().print(table)
+    rich.console.Console().print(table)
 
 
 @cli.command()
-def get_folder(context: Context, folder_id: int) -> None:
+def get_folder(context: click.Context, folder_id: int) -> None:
     """Get details about a Folder ID."""
-    folder_details = context.obj.get_folder_details(folder_id=folder_id)
+    server: ss.SecretServerClient = context.obj
+    folder_details = server.get_folder_details(folder_id=folder_id)
 
-    table = Table("Folder", f"{folder_details.name} ({folder_details.folder_id})")
+    table = rich.table.Table("Folder", f"{folder_details.name} ({folder_details.folder_id})")
     table.add_row("Actions", ", ".join(folder_details.actions), end_section=True)
     table.add_row("Allowed Templates", "\n".join(
         [f"{template.name} (ID: {template.template_id})" for template in folder_details.allowed_templates],
     ))
-    Console().print(table)
+    rich.console.Console().print(table)
 
 
 @cli.command()
-def get_template(context: Context, template_id: int) -> None:
+def get_template(context: click.Context, template_id: int) -> None:
     """Get details about a given Template ID."""
-    template = context.obj.get_template(template_id=template_id)
+    server: ss.SecretServerClient = context.obj
+    template = server.get_template(template_id=template_id)
 
-    table = Table("Template", f"{template.name} ({template.template_id})")
+    table = rich.table.Table("Template", f"{template.name} ({template.template_id})")
     for field in template.fields:
         table.add_row("Field Name", field.name)
         table.add_row("Field ID", str(field.secret_template_field_id))
         table.add_row("Display Name", field.display_name)
         table.add_row("Description", field.description)
         table.add_row("Slug", field.field_slug_name)
         table.add_row(
             "Required",
-            Text(str(field.is_required), style="bold red" if field.is_required else None),
+            rich.text.Text(str(field.is_required), style="bold red" if field.is_required else None),
             end_section=True,
         )
-    Console().print(table)
+    rich.console.Console().print(table)
 
 
-@cli.command(hidden=hide_non_windows())
+@cli.command(hidden=utilities.hide_non_windows())
 def store_windows_credential(
-        client_id: Annotated[str, Option(help=HelpText.client_id)],
-        client_secret: Annotated[str, Option(help=HelpText.client_secret)],
-        name: Annotated[str, Option(help=HelpText.windows)] = "dss-cli-client",
+        client_id: typing.Annotated[str, typer.Option(help=utilities.HelpText.client_id)],
+        client_secret: typing.Annotated[str, typer.Option(help=utilities.HelpText.client_secret)],
+        name: typing.Annotated[str, typer.Option(help=utilities.HelpText.windows)] = "dss-cli-client",
 ) -> None:
-    """Stores Client ID and Client Secret in Windows Credential Manager."""
-    if Windows.windows_credential_exists(name=name):
-        if not confirm(f"Credential '{name}' exists. Are you sure you want to delete it?"):
-            raise Abort
-        Windows.delete_credential(name=name)
+    """Stores Client ID and Client Secret in credentials.Windows Credential Manager."""
+    if credentials.Windows.windows_credential_exists(name=name):
+        if not click.confirm(f"Credential '{name}' exists. Are you sure you want to delete it?"):
+            raise click.Abort
+        credentials.Windows.delete_credential(name=name)
 
-    Windows.set_windows_credential(name=name, client_id=client_id, client_secret=client_secret)
-    Console().print(f"Credentials stored under: {name}")
+    credentials.Windows.set_windows_credential(name=name, client_id=client_id, client_secret=client_secret)
+    rich.console.Console().print(f"Credentials stored under: {name}")
 
 
 @cli.command()
 def search_secrets(
-        context: Context,
-        recent: Annotated[bool, Option("--recent")] = False,  # noqa: FBT002
-        search_text: Annotated[str, Option(show_default=False)] = None,
-        folder_id: Annotated[int, Option(show_default=False)] = None,
-        secret_template_ids: Annotated[list[int], Option(show_default=False)] = None,
-        extra_fields: Annotated[list[SearchSecretsExtraFields], Option(
-            "--extra-fields", "-f", show_default=False,
-        )] = None,
+        context: click.Context,
+        recent: typing.Annotated[bool, typer.Option("--recent")] = False,  # noqa: FBT002
+        search_text: typing.Annotated[str | None, typer.Option(show_default=False)] = None,
+        folder_id: typing.Annotated[int | None, typer.Option(show_default=False)] = None,
+        secret_template_ids: typing.Annotated[list[int] | None, typer.Option(show_default=False)] = None,
+        extra_fields: typing.Annotated[list[utilities.SearchSecretsExtraFields] | None, typer.Option(
+            "--extra-fields", "-f", show_default=False)] = None,
 ) -> None:
     """Search available secrets using various parameters."""
     headers = ["Name", "ID", "Template ID", "Template Name", "Folder ID", "Folder Name", "Last Accessed"]
     if extra_fields:
-        headers = SearchSecretsExtraFields.add_extra_headers(headers=headers, extra_fields=extra_fields)
-    table = Table(*headers)
+        headers = utilities.SearchSecretsExtraFields.add_extra_headers(headers=headers, extra_fields=extra_fields)
+    table = rich.table.Table(*headers)
 
-    params = SearchSecretsParams(
+    params = models.SearchSecretsParams(
         search_text=search_text,
         folder_id=folder_id,
         secret_template_ids=secret_template_ids,
         scope="Recent" if recent else None,
     )
 
-    secrets = context.obj.search_secrets(params=params)
+    server: ss.SecretServerClient = context.obj
+    secrets = server.search_secrets(params=params)
 
     for secret_info in secrets.records:
         row = [
             secret_info.name,
             str(secret_info.secret_id),
             str(secret_info.secret_template_id),
             secret_info.secret_template_name,
             str(secret_info.folder_id),
             secret_info.folder_path,
-            format_dtg(secret_info.last_accessed),
+            utilities.format_dtg(secret_info.last_accessed),
         ]
         if extra_fields:
-            row = SearchSecretsExtraFields.append_extra_data(
+            row = utilities.SearchSecretsExtraFields.append_extra_data(
                 secret_info=secret_info, row=row, extra_fields=extra_fields,
             )
         table.add_row(*row)
-    Console().print(table)
+    rich.console.Console().print(table)
+
+
+@cli.command()
+def generate_otp(
+    context: click.Context,
+    secret_id: int,
+    min_remaining: typing.Annotated[int, typer.Option(
+        help=utilities.HelpText.min_remaining_seconds, callback=utilities.constrained_integer(min=1, max=29))] = 3,
+    output_format: typing.Annotated[utilities.OutputTypes, typer.Option(
+        help=utilities.HelpText.output_format)] = utilities.OutputTypes.CLIPBOARD.value,
+) -> None:
+    """Generate an OTP if the secret supports it."""
+    server: ss.SecretServerClient = context.obj
+    otp = server.generate_otp(secret_id=secret_id)
+    if otp.remaining_seconds < min_remaining:
+        rich.console.Console().print(f"Waiting {otp.remaining_seconds} to regenerate OTP...")
+        time.sleep(otp.remaining_seconds)
+    otp = server.generate_otp(secret_id=secret_id)
+
+    if output_format == utilities.OutputTypes.JSON:
+        output = otp.model_dump_json(by_alias=True)
+    elif output_format == utilities.OutputTypes.TABLE:
+        output = rich.table.Table("Name", "Value")
+        for key, value in otp.model_dump(by_alias=True).items():
+            output.add_row(key.capitalize(), str(value))
+    else:
+        pyperclip.copy(otp.code)
+        output = f"OTP with {otp.remaining_seconds} remaining seconds copied to clipboard."
+
+    rich.console.Console().print(output)
 
 
 @cli.command()
 def config(
-        profile: Annotated[str, Option(help="The Delinea credentials profile.")] = "default",
-        server: Annotated[str, Option(help="Delinea Server", show_default=False)] = None,
-        client_id: Annotated[str, Option(help="Delinea Service Client ID", show_default=False)] = None,
-        client_secret: Annotated[str, Option(help="Delinea Service Client Secret", show_default=False)] = None,
-        windows_credential_name: Annotated[str, Option(
-            help="Delinea Service Client Windows Credential",
+        profile: typing.Annotated[str, typer.Option(help="The Delinea credentials profile.")] = "default",
+        server: typing.Annotated[str | None, typer.Option(help="Delinea Server", show_default=False)] = None,
+        client_id: typing.Annotated[str | None, typer.Option(
+            help="Delinea Service Client ID", show_default=False)] = None,
+        client_secret: typing.Annotated[str | None, typer.Option(
+            help="Delinea Service Client Secret", show_default=False)] = None,
+        windows_credential_name: typing.Annotated[str | None, typer.Option(
+            help="Delinea Service Client credentials.Windows Credential",
             show_default=False,
-            hidden=hide_non_windows(),
-        )] = None,
+            hidden=utilities.hide_non_windows())] = None,
 ) -> None:
     """Configure a DSS CLI profile."""
-    CredFileProvider.ensure_file()
-    creds = CredFileProvider.read_file()
+    credentials.CredFileProvider.ensure_file()
+    creds = credentials.CredFileProvider.read_file()
     profile_config = creds.get(profile, {})
 
     if any([server, client_id, client_secret, windows_credential_name]):
         options = {
             "server": server,
             "client_id": client_id,
             "client_secret": client_secret,
@@ -294,49 +322,49 @@
                 message="Delinea Client Secret",
                 required=bool(client_id),
                 prompt_kwargs={"show_default": False, "hide_input": True},
             )
             if client_secret:
                 profile_config["client_secret"] = client_secret
 
-        if platform.platform().startswith("Windows"):
+        if platform.platform().startswith("credentials.Windows"):
             windows_credential_name = config_prompt(
                 profile_config=profile_config,
                 key="windows_credential_name",
-                message="Delinea Windows Credential Name",
+                message="Delinea credentials.Windows Credential Name",
             )
             if windows_credential_name:
                 profile_config["windows_credential_name"] = windows_credential_name
 
     creds[profile] = profile_config
-    CredFileProvider.write_file(config=creds)
+    credentials.CredFileProvider.write_file(config=creds)
 
 
 @cli.command()
-def login(api_key: Annotated[str, Option(prompt=True, hide_input=True)]) -> None:
+def login(api_key: typing.Annotated[str, typer.Option(prompt=True, hide_input=True)]) -> None:
     """Log in to DSS using API Key."""
-    CredFileProvider.ensure_file()
-    creds = CredFileProvider.read_file()
+    credentials.CredFileProvider.ensure_file()
+    creds = credentials.CredFileProvider.read_file()
     profile_config = creds.get("default", {})
     if "server" not in profile_config:
         msg = "Server not configured for default profile. Run `dss config` to configure server."
-        raise ClickException(msg)
+        raise click.ClickException(msg)
     profile_config["api_key"] = api_key
     creds["default"] = profile_config
-    CredFileProvider.write_file(config=creds)
+    credentials.CredFileProvider.write_file(config=creds)
 
 
 @cli.callback()
 def dss(
-        context: Context,
-        profile: Annotated[str, Option(help="The Delinea credentials profile.")] = "default",
-        _: Annotated[bool, Option("--version", callback=version_callback)] = None,
+        context: click.Context,
+        profile: typing.Annotated[str, typer.Option(help="The Delinea credentials profile.")] = "default",
+        _: typing.Annotated[bool | None, typer.Option("--version", callback=utilities.version_callback)] = None,
 ) -> None:
     """Delinea Secret Server CLI."""
-    context.obj = SecretServerClient(profile=profile, mode="cli")
+    context.obj = ss.SecretServerClient(profile=profile, mode="cli")
 
 
 def main() -> None:
     """The CLI main entrypoint."""
     cli()
```

### Comparing `dss-sdk-1.2.2/src/dss_sdk/server.py` & `dss_sdk-1.3.0/src/dss_sdk/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,39 @@
 """The Delinea Secret Server SDK."""
+import abc
+import functools
 import getpass
+import os
+import typing
 import uuid
-from abc import ABC, abstractmethod
-from functools import cached_property
-from typing import TypeVar
 
+import click
 import httpx
-from click import ClickException
-from httpx import HTTPStatusError, Response
 
-from dss_sdk.credentials import ProviderChain
-from dss_sdk.models import (
-    CreateSecret,
-    FolderDetails,
-    Folders,
-    SearchFoldersParams,
-    SearchSecretsParams,
-    Secret,
-    SecretsInfo,
-    SecretTemplate,
-    Sites,
-    UpdateSecret,
-)
-
-_T = TypeVar("_T")
-ClientId = TypeVar("ClientId", bound=str)
-ClientSecret = TypeVar("ClientSecret", bound=str)
+from . import credentials, models
 
+_T = typing.TypeVar("_T")
+ClientId = typing.TypeVar("ClientId", bound=str)
+ClientSecret = typing.TypeVar("ClientSecret", bound=str)
 
-class SecretServer(ABC):
+
+class SecretServer(abc.ABC):
     """The Secret Server Abstract Class."""
 
-    def __init__(self, provider_chain: ProviderChain) -> None:
+    def __init__(self, provider_chain: credentials.ProviderChain) -> None:
         """Initialize the class.
 
         The bellow dunder properties will be overwritten by the client implementation.
         """
         self.__provider_chain__ = provider_chain
         self.__token__ = None
         self.__endpoint__ = None
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def client(self) -> httpx.Client | httpx.AsyncClient:
         """Client abstract property."""
         ...
 
     @property
     def headers(self) -> dict[str, str]:
         """The headers used by the Delinea API."""
@@ -72,37 +60,49 @@
         return self.__endpoint__
 
 
 class RegisterClient:
     """Registers a new client with Delinea."""
 
     def __new__(
-            cls, server: str, service_account: str, onboarding_key: str, description: str,
-    ) -> tuple[ClientId, ClientSecret]:
+            cls,
+            server: str,
+            service_account: str,
+            onboarding_key: str,
+            description: str = "",
+            *,
+            export: bool = False,
+    ) -> tuple[ClientId, ClientSecret] | None:
         """Registers the new client and returns the credentials.
 
         Args:
             server: The Delinea server FQDN/URL.
             service_account: The Delinea Service Account.
             onboarding_key: The onboarding key for the service account.
             description: The description of the client.
+            export: If the environment variables should be exported after registration.
         """
         server = cls.__format_server_name__(server=server)
         if not description:
             description = f"dss-sdk-{getpass.getuser()}"
 
         data = {
             "onboardingKey": onboarding_key,
             "ruleName": service_account,
             "clientId": str(uuid.uuid4()),
             "description": description,
             "name": service_account,
         }
         data = cls.__register__(server=server, data=data)
 
+        if export:
+            os.environ["DELINEA_SERVER"] = server
+            os.environ["DELINEA_CLIENT_ID"] = data["clientId"]
+            os.environ["DELINEA_CLIENT_SECRET"] = data["clientSecret"]
+            return None
         client_secret = data["clientSecret"]
         client_id = data["clientId"]
         return client_id, client_secret
 
     @classmethod
     def __format_server_name__(cls, server: str) -> str:
         """Formats the Delinea server name.
@@ -148,27 +148,27 @@
             response.raise_for_status()
             return response.json()
 
 
 class SecretServerClient(SecretServer):
     """The Synchronous Delinea Secret Server Client."""
 
-    def __init__(self, *, profile: str = None, mode: str = "sdk") -> None:
+    def __init__(self, *, profile: str = "", mode: str = "sdk") -> None:
         """Initialize the class.
 
         Args:
             profile: The credential profile to use.
             mode: The access mode (sdk or cli).
         """
-        super().__init__(provider_chain=ProviderChain(profile=profile))
+        super().__init__(provider_chain=credentials.ProviderChain(profile=profile))
         if profile:
             self.profile = profile
         self.mode = mode
 
-    @cached_property
+    @functools.cached_property
     def client(self) -> httpx.Client:
         """Creates and caches the httpx Client."""
         return httpx.Client()
 
     def __get__(self, url: str, *, params: dict[str, str] | None = None) -> _T:
         """Performs an HTTPX GET.
 
@@ -207,131 +207,143 @@
         Returns:
             The JSON response.
         """
         response = self.client.put(url=url, headers=self.headers, json=body)
         self.__handle_exception__(response=response)
         return response.json()
 
-    def __handle_exception__(self, response: Response) -> None:
+    def __handle_exception__(self, response: httpx.Response) -> None:
         """Handle any possible HTTP Exception and print a more helpful message.
 
         Args:
             response: The HTTPX response.
         """
         try:
             response.raise_for_status()
-        except HTTPStatusError as e:
+        except httpx.HTTPStatusError as e:
             err = response.json()
             err_msg = err.get("message", "No error message found in HTTP exception.")
             if "modelState" in err:
                 details = "; ".join(*err["modelState"].values())
                 err_msg = f"{err_msg} {details}"
 
             msg = f"HTTP {e.response.status_code}: {err_msg}"
             if self.mode == "cli":
-                raise ClickException(msg) from e
+                raise click.ClickException(msg) from e
             raise ConnectionError(msg) from e
 
-    def search_secrets(self, *, params: SearchSecretsParams = None) -> SecretsInfo:
+    def search_secrets(self, *, params: models.SearchSecretsParams | None = None) -> models.SecretsInfo:
         """Search Delinea Secrets.
 
         Args:
             params: The query parameters model.
 
         Returns:
             The information on available Secrets.
         """
         if not params:
-            params = SearchSecretsParams()
+            params = models.SearchSecretsParams()
 
         response = self.__get__(
             url=f"{self.endpoint}/api/v2/secrets", params=params.model_dump(by_alias=True, exclude_none=True),
         )
-        return SecretsInfo(**response)
+        return models.SecretsInfo(**response)
 
-    def get_secret(self, secret_id: int) -> Secret:
+    def get_secret(self, secret_id: int) -> models.Secret:
         """Gets a secret.
 
         Args:
             secret_id: The ID of the Secret.
 
         Returns:
             The secret.
         """
         response = self.__get__(url=f"{self.endpoint}/api/v2/secrets/{secret_id}")
-        return Secret(**response)
+        return models.Secret(**response)
 
-    def get_template(self, template_id: int) -> SecretTemplate:
+    def get_template(self, template_id: int) -> models.SecretTemplate:
         """Get a Secret Template.
 
         Args:
             template_id: The template ID.
 
         Returns:
             The SecretTemplate model.
         """
         response = self.__get__(url=f"{self.endpoint}/api/v1/secret-templates/{template_id}")
-        return SecretTemplate(**response)
+        return models.SecretTemplate(**response)
 
-    def create_secret(self, secret: CreateSecret) -> Secret:
+    def create_secret(self, secret: models.CreateSecret) -> models.Secret:
         """Create a new secret.
 
         Args:
             secret: The CreateSecret model.
 
         Returns:
             The created Secret model.
         """
         response = self.__post__(url=f"{self.endpoint}/api/v1/secrets", body=secret.model_dump(by_alias=True))
-        return Secret(**response)
+        return models.Secret(**response)
 
-    def get_folders(self, params: SearchFoldersParams = None) -> Folders:
+    def get_folders(self, params: models.SearchFoldersParams = None) -> models.Folders:
         """Get all accessible and/or filtered folders.
 
         Args:
             params: The params to filter the response by.
 
         Returns:
             The Folders model.
         """
         if not params:
-            params = SearchFoldersParams()
+            params = models.SearchFoldersParams()
         response = self.__get__(
             url=f"{self.endpoint}/api/v1/folders", params=params.model_dump(by_alias=True, exclude_none=True),
         )
-        return Folders(folders=response.get("records", []))
+        return models.Folders(folders=response.get("records", []))
 
-    def get_folder_details(self, folder_id: int) -> FolderDetails:
+    def get_folder_details(self, folder_id: int) -> models.FolderDetails:
         """Get details of a particular folder.
 
         Args:
             folder_id: The ID of the folder.
 
         Returns:
             The FolderDetails model.
         """
         response = self.__get__(url=f"{self.endpoint}/api/v1/folder-details/{folder_id}")
-        return FolderDetails(**response)
+        return models.FolderDetails(**response)
 
-    def get_sites(self) -> Sites:
+    def get_sites(self) -> models.Sites:
         """Get the available sites.
 
         Returns:
             The Sites model.
         """
         response = self.__get__(url=f"{self.endpoint}/api/v1/sites")
-        return Sites(sites=response)
+        return models.Sites(sites=response)
 
-    def update_secret(self, secret: UpdateSecret) -> Secret:
+    def update_secret(self, secret: models.UpdateSecret) -> models.Secret:
         """Updates various fields of a secret.
 
         Args:
             secret: The UpdateSecret model containing the fields to update.
 
         Returns:
             The updated Secret model.
         """
         response = self.__put__(
             url=f"{self.endpoint}/api/v1/secrets/{secret.secret_id}",
             body=secret.model_dump(by_alias=True, exclude_none=True),
         )
-        return Secret(**response)
+        return models.Secret(**response)
+
+    def generate_otp(self, secret_id: int) -> models.OneTimePasscode:
+        """Generates an One Time Passcode if the secret supports it.
+
+        Args:
+            secret_id (int): The secret ID.
+
+        Returns:
+            The One Time Passcode model.
+        """
+        response = self.__get__(url=f"{self.endpoint}/api/v1/one-time-password-code/{secret_id}")
+        return models.OneTimePasscode(**response[0])
```

### Comparing `dss-sdk-1.2.2/src/dss_sdk/utilities.py` & `dss_sdk-1.3.0/src/dss_sdk/utilities.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Utilities for DSS SDK."""
+import collections.abc
 import datetime
+import enum
 import platform
-from enum import Enum, StrEnum, auto
-from typing import TypeVar
+import typing
 
-from click.exceptions import Exit
+import click
 
-from dss_sdk import __version__
-from dss_sdk.models import SecretInfo
+from . import __version__, models
 
-_T = TypeVar("_T")
+_T = typing.TypeVar("_T")
 
 
-class OutputTypes(Enum):
+class OutputTypes(enum.Enum):
     """Console output types."""
     TABLE = "table"
     JSON = "json"
     CLIPBOARD = "clipboard"
 
 
-class SearchSecretsExtraFields(StrEnum):
+class SearchSecretsExtraFields(enum.StrEnum):
     """Extra fields to print for secret info."""
-    site_id = auto()
-    checked_out = auto()
-    is_restricted = auto()
-    create_date = auto()
-    days_until_expiration = auto()
-    auto_change_enabled = auto()
+    site_id = enum.auto()
+    checked_out = enum.auto()
+    is_restricted = enum.auto()
+    create_date = enum.auto()
+    days_until_expiration = enum.auto()
+    auto_change_enabled = enum.auto()
 
     @classmethod
     def add_extra_headers(cls, headers: list[str], extra_fields: list[str]) -> list[str]:
         """Adds additional headers if the extra field is applied."""
         for field in extra_fields:
             match field:
                 case cls.site_id:
@@ -44,15 +44,15 @@
                 case cls.days_until_expiration:
                     headers.append("Days Until Expiration")
                 case cls.auto_change_enabled:
                     headers.append("Auto Change Enabled")
         return headers
 
     @classmethod
-    def append_extra_data(cls, secret_info: SecretInfo, row: list[_T], extra_fields: list[str]) -> list[_T]:
+    def append_extra_data(cls, secret_info: models.SecretInfo, row: list[_T], extra_fields: list[str]) -> list[_T]:
         """Adds requisite data if the extra field is applied."""
         for field in extra_fields:
             match field:
                 case cls.site_id:
                     row.append(str(secret_info.site_id))
                 case cls.checked_out:
                     row.append(str(secret_info.checked_out))
@@ -63,25 +63,26 @@
                 case cls.days_until_expiration:
                     row.append(str(secret_info.days_until_expiration))
                 case cls.auto_change_enabled:
                     row.append(str(secret_info.auto_change_enabled))
         return row
 
 
-class HelpText(StrEnum):
+class HelpText(enum.StrEnum):
     """Help Text for CLI."""
     client_id = "The client ID registered with your Delinea server."
     client_secret = "The client secret for the specified client ID registered with your Delinea server."  # noqa: S105
     include_username = "Include the username in the output (Does not copy username to clipboard)."
     output_format = "Output as a table, JSON, or copy to clipboard."
     server = "The FQDN of your Delinea Secret Server."
     windows = "The name of a Windows Credential containing the Client ID and Client Secret"
     parent_folder_id = "The parent folder ID to search for child folders."
     search_text = "Text to search for."
     store_in_windows = "Store the registered client ID and secret as Windows credentials."
+    min_remaining_seconds = "The required minimum seconds remaining before outputting OTP. (Must be between 1 and 30)"
 
 
 def hide_non_windows() -> bool:
     """Used as a Typer callback to check if a platform is Windows.
 
     Args:
         value: The value of the option/argument from Typer.
@@ -96,22 +97,43 @@
     """Prints the version when the version flag is set.
 
     Args:
         value: `True`, if the `--version` flag is set.
     """
     if value:
         print(f"DSS CLI v{__version__.version}")  # noqa: T201
-        raise Exit
+        raise click.exceptions.Exit
 
 
 def format_dtg(date_string: datetime.datetime | _T) -> str | _T:
     """Formats datetime date in `isoformat()`.
 
     Args:
         date_string: The optional datetime string.
 
     Returns:
         The formatted string if the `date_string` is a datetime object, otherwise it just returns the value.
     """
     if not date_string:
         return date_string
     return date_string.isoformat()
+
+
+def constrained_integer(*, minimum: int | None = None, maximum: int | None = None) -> collections.abc.Callable:
+    """Ensures a constrained integer value between a provided minimum and/or maximum.
+
+    Args:
+        minimum (int | None, optional): The minimum value. Defaults to None.
+        maximum (int | None, optional): The maximum value. Defaults to None.
+
+    Returns:
+        The callback method used by Typer to ensure an integer value within the constraints.
+    """
+    def _callback(value: int) -> None:
+        if min and value < min:
+            msg = f"{value} is less then the required minimum: {minimum}"
+            raise click.BadParameter(msg)
+        if max and value > max:
+            msg = f"{value} is greater then the required maximum: {maximum}"
+            raise click.BadParameter(msg)
+        return value
+    return _callback
```

### Comparing `dss-sdk-1.2.2/src/dss_sdk.egg-info/PKG-INFO` & `dss_sdk-1.3.0/src/dss_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dss-sdk
-Version: 1.2.2
+Version: 1.3.0
 Summary: A better SDK for Delinea Secret Server
 Author: riebecj
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,18 @@
 Requires-Dist: httpx~=0.26
 Requires-Dist: pydantic~=2.4
 Requires-Dist: typer~=0.9
 Requires-Dist: click~=8.1
 Requires-Dist: rich~=13.7
 Requires-Dist: pyperclip~=1.8
 Requires-Dist: toml~=0.10
+Provides-Extra: dev
+Requires-Dist: pytest~=7.4; extra == "dev"
+Requires-Dist: pytest-cov~=4.1; extra == "dev"
+Requires-Dist: ruff~=0.3; extra == "dev"
 
 # dss-sdk
 A better SDK for Delinea Secret Server.
 
 This is an SDK and CLI for interacting with Delinea Secret Server. The CLI uses [Typer](https://typer.tiangolo.com/), 
 and the SDK uses [httpx](https://www.python-httpx.org/). Both use [Pydantic](https://docs.pydantic.dev/latest/) for 
 data serialization from the Delinea APIs.
```

