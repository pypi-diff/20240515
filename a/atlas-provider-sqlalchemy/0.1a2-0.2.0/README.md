# Comparing `tmp/atlas_provider_sqlalchemy-0.1a2.tar.gz` & `tmp/atlas_provider_sqlalchemy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas_provider_sqlalchemy-0.1a2.tar", max compression
+gzip compressed data, was "atlas_provider_sqlalchemy-0.2.0.tar", max compression
```

## Comparing `atlas_provider_sqlalchemy-0.1a2.tar` & `atlas_provider_sqlalchemy-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     3417 2023-10-25 17:43:20.718520 atlas_provider_sqlalchemy-0.1a2/README.md
--rw-r--r--   0        0        0        0 2023-10-25 17:21:50.982376 atlas_provider_sqlalchemy-0.1a2/cli/__init__.py
--rw-r--r--   0        0        0     3389 2023-10-25 16:59:26.289056 atlas_provider_sqlalchemy-0.1a2/cli/main.py
--rw-r--r--   0        0        0      541 2023-10-25 17:43:27.135158 atlas_provider_sqlalchemy-0.1a2/pyproject.toml
--rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 atlas_provider_sqlalchemy-0.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 06:53:16.155091 atlas_provider_sqlalchemy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3960 2024-05-15 06:53:16.155091 atlas_provider_sqlalchemy-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 06:53:16.155091 atlas_provider_sqlalchemy-0.2.0/atlas_provider_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2937 2024-05-15 06:53:16.155091 atlas_provider_sqlalchemy-0.2.0/atlas_provider_sqlalchemy/ddl.py
+-rw-r--r--   0        0        0     1255 2024-05-15 06:53:16.159091 atlas_provider_sqlalchemy-0.2.0/atlas_provider_sqlalchemy/main.py
+-rw-r--r--   0        0        0      723 2024-05-15 06:53:24.427144 atlas_provider_sqlalchemy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 atlas_provider_sqlalchemy-0.2.0/PKG-INFO
```

### Comparing `atlas_provider_sqlalchemy-0.1a2/README.md` & `atlas_provider_sqlalchemy-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,138 @@
-# DRAFT
-
 # atlas-provider-sqlalchemy
-Atlas provider for sqlalchemy
 
 Load [SQLAlchemy](https://www.sqlalchemy.org/) models into an [Atlas](https://atlasgo.io) project.
 
 ### Use-cases
 1. **Declarative migrations** - use a Terraform-like `atlas schema apply --env sqlalchemy` to apply your SQLAlchemy schema to the database.
 2. **Automatic migration planning** - use `atlas migrate diff --env sqlalchemy` to automatically plan a migration from the current database version to the SQLAlchemy schema.
 
 ### Installation
 
 Install Atlas from macOS or Linux by running:
 ```bash
 curl -sSf https://atlasgo.sh | sh
 ```
+
 See [atlasgo.io](https://atlasgo.io/getting-started#installation) for more installation options.
 
 Install the provider by running:
 ```bash
+# The Provider works by importing your SQLAlchemy models and extracting the schema from them.
+# Therefore, you will need to run the provider from within your project's Python environment.
 pip install atlas-provider-sqlalchemy
 ```
 
-
 #### Standalone 
 
 If all of your SQLAlchemy models exist in a single package, 
 you can use the provider directly to load your SQLAlchemy schema into Atlas.
 
 In your project directory, create a new file named `atlas.hcl` with the following contents:
 
 ```hcl
 data "external_schema" "sqlalchemy" {
   program = [
     "atlas-provider-sqlalchemy",
-    "--dialect", "mysql", // postgresql | mysql | oracle | sqlite | mssql
+    "--path", "./path/to/models",
+    "--dialect", "mysql" // mariadb | postgresql | sqlite | mssql
   ]
 }
 
 env "sqlalchemy" {
   src = data.external_schema.sqlalchemy.url
   dev = "docker://mysql/8/dev"
+  migration {
+    dir = "file://migrations"
+  }
+  format {
+    migrate {
+      diff = "{{ sql . \"  \" }}"
+    }
+  }
 }
 ```
 
 #### As Python Script 
-...   
+
 If you want to use the provider as a python script, you can use the provider as follows:
 
 Create a new file named `load_models.py` with the following contents:
 
 ```python
 # import all models
-from models import User, Task;
-from ariga_provider_sqlalchemy import print_ddl
+from models import User, Task
+from atlas_provider_sqlalchemy.ddl import print_ddl
 print_ddl("mysql", [User, Task])
 ```
 
 Next, in your project directory, create a new file named `atlas.hcl` with the following contents:
 
 ```hcl
 data "external_schema" "sqlalchemy" {
     program = [
         "python",
         "load_models.py"
     ]
 }
 
 env "sqlalchemy" {
-    src = data.external_schema.sqlalchemy.url
-    dev = "docker://mysql/8/dev"
+  src = data.external_schema.sqlalchemy.url
+  dev = "docker://mysql/8/dev"
+  migration {
+    dir = "file://migrations"
+  }
+  format {
+    migrate {
+      diff = "{{ sql . \"  \" }}"
+    }
+  }
 }
 ```
 
 ### Usage
 
 Once you have the provider installed, you can use it to apply your SQLAlchemy schema to the database:
 
 #### Apply
 
-You can use the `atlas schema apply` command to plan and apply a migration of your database to your current SQLAlchemy schema. This works by inspecting the target database and comparing it to the SQLAlchemy schema and creating a migration plan. Atlas will prompt you to confirm the migration plan before applying it to the database.
+You can use the `atlas schema apply` command to plan and apply a migration of your database to your current SQLAlchemy schema.
+This works by inspecting the target database and comparing it to the SQLAlchemy schema and creating a migration plan.
+Atlas will prompt you to confirm the migration plan before applying it to the database.
 
 ```bash
 atlas schema apply --env sqlalchemy -u "mysql://root:password@localhost:3306/mydb"
 ```
 Where the `-u` flag accepts the [URL](https://atlasgo.io/concepts/url) to the
 target database.
 
 #### Diff
 
 Atlas supports a [version migration](https://atlasgo.io/concepts/declarative-vs-versioned#versioned-migrations) 
 workflow, where each change to the database is versioned and recorded in a migration file. You can use the
 `atlas migrate diff` command to automatically generate a migration file that will migrate the database
-from its latest revision to the current Sequelize schema.
+from its latest revision to the current SQLAlchemy schema.
 
 ```bash
 atlas migrate diff --env sqlalchemy 
 ````
 
 ### Supported Databases
 
 The provider supports the following databases:
 * MySQL
 * MariaDB
 * PostgreSQL
 * SQLite
 * Microsoft SQL Server
-* Oracle
+
+### Credit
+
+The code in this repository is based on [noamtamir/atlas-provider-sqlalchemy](https://github.com/noamtamir/atlas-provider-sqlalchemy).
 
 ### Issues
 
 Please report any issues or feature requests in the [ariga/atlas](https://github.com/ariga/atlas/issues) repository.
 
 ### License
 
-This project is licensed under the [Apache License 2.0](LICENSE).
+This project is licensed under the [Apache License 2.0](LICENSE).
```

### Comparing `atlas_provider_sqlalchemy-0.1a2/pyproject.toml` & `atlas_provider_sqlalchemy-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 [tool.poetry]
 name = "atlas-provider-sqlalchemy"
-version = "0.1a2"
-description = ""
-authors = ["noamtamir <noam.tamir@gmail.com>"]
+version = "0.2.0"
+description = "Load sqlalchemy models into an Atlas project."
+authors = ["Your Name <you@example.com>"]
 readme = "README.md"
-packages = [{include = "cli"}]
+packages = [{include = "atlas_provider_sqlalchemy"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-sqlalchemy = "^2.0.21"
-typer = {extras = ["all"], version = "^0.9.0"}
-
+typer = ">0.9.0,<=1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
+tox = "^4.15.0"
+ruff = "^0.1.8"
 autopep8 = "^2.0.4"
 mypy = "^1.5.1"
 
+[tool.poetry.group.inttests]
+optional = true
+
+[tool.poetry.group.inttests.dependencies]
+sqlalchemy = "^2.0.21"
+
 [tool.poetry.scripts]
-atlas-provider-sqlalchemy = "cli.main:app"
+atlas-provider-sqlalchemy = "atlas_provider_sqlalchemy.main:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `atlas_provider_sqlalchemy-0.1a2/PKG-INFO` & `atlas_provider_sqlalchemy-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,155 @@
 Metadata-Version: 2.1
 Name: atlas-provider-sqlalchemy
-Version: 0.1a2
-Summary: 
-Author: noamtamir
-Author-email: noam.tamir@gmail.com
+Version: 0.2.0
+Summary: Load sqlalchemy models into an Atlas project.
+Author: Your Name
+Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: typer (>0.9.0,<=1.0.0)
 Description-Content-Type: text/markdown
 
-# DRAFT
-
 # atlas-provider-sqlalchemy
-Atlas provider for sqlalchemy
 
 Load [SQLAlchemy](https://www.sqlalchemy.org/) models into an [Atlas](https://atlasgo.io) project.
 
 ### Use-cases
 1. **Declarative migrations** - use a Terraform-like `atlas schema apply --env sqlalchemy` to apply your SQLAlchemy schema to the database.
 2. **Automatic migration planning** - use `atlas migrate diff --env sqlalchemy` to automatically plan a migration from the current database version to the SQLAlchemy schema.
 
 ### Installation
 
 Install Atlas from macOS or Linux by running:
 ```bash
 curl -sSf https://atlasgo.sh | sh
 ```
+
 See [atlasgo.io](https://atlasgo.io/getting-started#installation) for more installation options.
 
 Install the provider by running:
 ```bash
+# The Provider works by importing your SQLAlchemy models and extracting the schema from them.
+# Therefore, you will need to run the provider from within your project's Python environment.
 pip install atlas-provider-sqlalchemy
 ```
 
-
 #### Standalone 
 
 If all of your SQLAlchemy models exist in a single package, 
 you can use the provider directly to load your SQLAlchemy schema into Atlas.
 
 In your project directory, create a new file named `atlas.hcl` with the following contents:
 
 ```hcl
 data "external_schema" "sqlalchemy" {
   program = [
     "atlas-provider-sqlalchemy",
-    "--dialect", "mysql", // postgresql | mysql | oracle | sqlite | mssql
+    "--path", "./path/to/models",
+    "--dialect", "mysql" // mariadb | postgresql | sqlite | mssql
   ]
 }
 
 env "sqlalchemy" {
   src = data.external_schema.sqlalchemy.url
   dev = "docker://mysql/8/dev"
+  migration {
+    dir = "file://migrations"
+  }
+  format {
+    migrate {
+      diff = "{{ sql . \"  \" }}"
+    }
+  }
 }
 ```
 
 #### As Python Script 
-...   
+
 If you want to use the provider as a python script, you can use the provider as follows:
 
 Create a new file named `load_models.py` with the following contents:
 
 ```python
 # import all models
-from models import User, Task;
-from ariga_provider_sqlalchemy import print_ddl
+from models import User, Task
+from atlas_provider_sqlalchemy.ddl import print_ddl
 print_ddl("mysql", [User, Task])
 ```
 
 Next, in your project directory, create a new file named `atlas.hcl` with the following contents:
 
 ```hcl
 data "external_schema" "sqlalchemy" {
     program = [
         "python",
         "load_models.py"
     ]
 }
 
 env "sqlalchemy" {
-    src = data.external_schema.sqlalchemy.url
-    dev = "docker://mysql/8/dev"
+  src = data.external_schema.sqlalchemy.url
+  dev = "docker://mysql/8/dev"
+  migration {
+    dir = "file://migrations"
+  }
+  format {
+    migrate {
+      diff = "{{ sql . \"  \" }}"
+    }
+  }
 }
 ```
 
 ### Usage
 
 Once you have the provider installed, you can use it to apply your SQLAlchemy schema to the database:
 
 #### Apply
 
-You can use the `atlas schema apply` command to plan and apply a migration of your database to your current SQLAlchemy schema. This works by inspecting the target database and comparing it to the SQLAlchemy schema and creating a migration plan. Atlas will prompt you to confirm the migration plan before applying it to the database.
+You can use the `atlas schema apply` command to plan and apply a migration of your database to your current SQLAlchemy schema.
+This works by inspecting the target database and comparing it to the SQLAlchemy schema and creating a migration plan.
+Atlas will prompt you to confirm the migration plan before applying it to the database.
 
 ```bash
 atlas schema apply --env sqlalchemy -u "mysql://root:password@localhost:3306/mydb"
 ```
 Where the `-u` flag accepts the [URL](https://atlasgo.io/concepts/url) to the
 target database.
 
 #### Diff
 
 Atlas supports a [version migration](https://atlasgo.io/concepts/declarative-vs-versioned#versioned-migrations) 
 workflow, where each change to the database is versioned and recorded in a migration file. You can use the
 `atlas migrate diff` command to automatically generate a migration file that will migrate the database
-from its latest revision to the current Sequelize schema.
+from its latest revision to the current SQLAlchemy schema.
 
 ```bash
 atlas migrate diff --env sqlalchemy 
 ````
 
 ### Supported Databases
 
 The provider supports the following databases:
 * MySQL
 * MariaDB
 * PostgreSQL
 * SQLite
 * Microsoft SQL Server
-* Oracle
+
+### Credit
+
+The code in this repository is based on [noamtamir/atlas-provider-sqlalchemy](https://github.com/noamtamir/atlas-provider-sqlalchemy).
 
 ### Issues
 
 Please report any issues or feature requests in the [ariga/atlas](https://github.com/ariga/atlas/issues) repository.
 
 ### License
 
 This project is licensed under the [Apache License 2.0](LICENSE).
+
```

