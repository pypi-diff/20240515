# Comparing `tmp/tableplus_db_urls-0.1.1.tar.gz` & `tmp/tableplus_db_urls-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableplus_db_urls-0.1.1.tar", last modified: Tue Apr 23 20:48:26 2024, max compression
+gzip compressed data, was "tableplus_db_urls-0.1.2.tar", last modified: Wed May 15 13:27:35 2024, max compression
```

## Comparing `tableplus_db_urls-0.1.1.tar` & `tableplus_db_urls-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 20:48:26.045420 tableplus_db_urls-0.1.1/
--rw-r--r--   0 tsantor    (501) staff       (20)      200 2024-04-09 19:33:00.000000 tableplus_db_urls-0.1.1/AUTHORS.md
--rw-r--r--   0 tsantor    (501) staff       (20)      327 2024-04-23 20:41:57.000000 tableplus_db_urls-0.1.1/HISTORY.md
--rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-12 15:32:17.000000 tableplus_db_urls-0.1.1/LICENSE
--rw-r--r--   0 tsantor    (501) staff       (20)      159 2024-04-12 15:50:09.000000 tableplus_db_urls-0.1.1/MANIFEST.in
--rw-r--r--   0 tsantor    (501) staff       (20)     2648 2024-04-23 20:48:26.045153 tableplus_db_urls-0.1.1/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     1263 2024-04-23 20:46:44.000000 tableplus_db_urls-0.1.1/README.md
--rw-r--r--   0 tsantor    (501) staff       (20)     4700 2024-04-23 20:31:04.000000 tableplus_db_urls-0.1.1/pyproject.toml
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 20:48:26.042462 tableplus_db_urls-0.1.1/requirements/
--rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-12 15:37:55.000000 tableplus_db_urls-0.1.1/requirements/requirements.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-23 19:49:37.000000 tableplus_db_urls-0.1.1/requirements/requirements_dev.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-23 19:49:29.000000 tableplus_db_urls-0.1.1/requirements/requirements_test.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-23 20:48:26.045479 tableplus_db_urls-0.1.1/setup.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-09 19:33:00.000000 tableplus_db_urls-0.1.1/setup.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 20:48:26.040159 tableplus_db_urls-0.1.1/src/
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 20:48:26.043298 tableplus_db_urls-0.1.1/src/tableplus/
--rw-r--r--   0 tsantor    (501) staff       (20)       42 2024-04-23 20:41:44.000000 tableplus_db_urls-0.1.1/src/tableplus/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1608 2024-04-23 20:28:41.000000 tableplus_db_urls-0.1.1/src/tableplus/cli.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1964 2024-04-23 20:36:20.000000 tableplus_db_urls-0.1.1/src/tableplus/core.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 20:48:26.044855 tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/
--rw-r--r--   0 tsantor    (501) staff       (20)     2648 2024-04-23 20:48:26.000000 tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)      534 2024-04-23 20:48:26.000000 tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/SOURCES.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-23 20:48:26.000000 tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/dependency_links.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       48 2024-04-23 20:48:26.000000 tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/entry_points.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-04-23 20:48:26.000000 tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/requires.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       10 2024-04-23 20:48:26.000000 tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/top_level.txt
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 20:48:26.044539 tableplus_db_urls-0.1.1/tests/
--rw-r--r--   0 tsantor    (501) staff       (20)     1341 2024-04-23 20:38:30.000000 tableplus_db_urls-0.1.1/tests/test_core.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.876666 tableplus_db_urls-0.1.2/
+-rw-r--r--   0 tsantor    (501) staff       (20)      200 2024-04-09 19:33:00.000000 tableplus_db_urls-0.1.2/AUTHORS.md
+-rw-r--r--   0 tsantor    (501) staff       (20)      399 2024-05-15 13:26:57.000000 tableplus_db_urls-0.1.2/HISTORY.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-12 15:32:17.000000 tableplus_db_urls-0.1.2/LICENSE
+-rw-r--r--   0 tsantor    (501) staff       (20)      159 2024-04-12 15:50:09.000000 tableplus_db_urls-0.1.2/MANIFEST.in
+-rw-r--r--   0 tsantor    (501) staff       (20)     2720 2024-05-15 13:27:35.876435 tableplus_db_urls-0.1.2/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     1263 2024-04-23 20:51:37.000000 tableplus_db_urls-0.1.2/README.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     4700 2024-04-23 20:31:04.000000 tableplus_db_urls-0.1.2/pyproject.toml
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.874327 tableplus_db_urls-0.1.2/requirements/
+-rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.2/requirements/requirements.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.2/requirements/requirements_dev.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.2/requirements/requirements_test.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-05-15 13:27:35.876721 tableplus_db_urls-0.1.2/setup.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-09 19:33:00.000000 tableplus_db_urls-0.1.2/setup.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.871853 tableplus_db_urls-0.1.2/src/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.874901 tableplus_db_urls-0.1.2/src/tableplus/
+-rw-r--r--   0 tsantor    (501) staff       (20)       42 2024-05-15 13:26:44.000000 tableplus_db_urls-0.1.2/src/tableplus/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1705 2024-05-14 22:10:33.000000 tableplus_db_urls-0.1.2/src/tableplus/cli.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1969 2024-05-15 13:25:38.000000 tableplus_db_urls-0.1.2/src/tableplus/core.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.876191 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/
+-rw-r--r--   0 tsantor    (501) staff       (20)     2720 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)      534 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/SOURCES.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/dependency_links.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       48 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/entry_points.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/requires.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       10 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.875873 tableplus_db_urls-0.1.2/tests/
+-rw-r--r--   0 tsantor    (501) staff       (20)     1367 2024-05-15 13:23:41.000000 tableplus_db_urls-0.1.2/tests/test_core.py
```

### Comparing `tableplus_db_urls-0.1.1/LICENSE` & `tableplus_db_urls-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tableplus_db_urls-0.1.1/PKG-INFO` & `tableplus_db_urls-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableplus-db-urls
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate TablePlus DB URLs from CookieCutter Django to make setting up connections easier.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/tableplus-db-urls.git
 Project-URL: Issues, https://github.com/tsantor/tableplus-db-urls/issues
 Project-URL: Changelog, https://github.com/tsantor/tableplus-db-urls/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -72,14 +72,18 @@
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/tableplus-db-urls/issues) on Github.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.2 (2024-05-15)
+
+- Added `name` argument to name the connection.
+
 ## 0.1.1 (2024-04-23)
 
 - Moved from `argparse` to `click`
 - Moved from `python-environ` to `python-dotenv`
 - Fixed bug with production URL
 
 ## 0.1.0 (2024-04-09)
```

### Comparing `tableplus_db_urls-0.1.1/README.md` & `tableplus_db_urls-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tableplus_db_urls-0.1.1/pyproject.toml` & `tableplus_db_urls-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tableplus_db_urls-0.1.1/src/tableplus/cli.py` & `tableplus_db_urls-0.1.2/src/tableplus/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 
 def silent_echo(*args, **kwargs):
     pass
 
 
 @click.command()
 @click.option("-p", "--path", required=True, help="Path to the project")
+@click.option("-n", "--name", required=True, help="TablePlus Connection Name")
 @click.option("--ssh-user", required=True, help="SSH User")
 @click.option("--ssh-host", required=True, help="SSH Host")
 @click.option("-v", "--verbose", is_flag=True, help="Verbose output")
-def generate(path, ssh_user, ssh_host, verbose) -> None:
+def generate(path, name, ssh_user, ssh_host, verbose) -> None:
     """Main entry point for the CLI."""
 
     if not verbose:
         click.echo = silent_echo
 
     project_path = Path(path).expanduser()
     local_env_path = str(project_path / ".envs/.local/.postgres")
     prod_env_path = str(project_path / ".envs/.production/.postgres")
 
-    local_db_url = get_local_db_conn_str(local_env_path)
-    prod_db_url = get_prod_db_conn_str(prod_env_path, ssh_user, ssh_host)
+    local_db_url = get_local_db_conn_str(name, local_env_path)
+    prod_db_url = get_prod_db_conn_str(prod_env_path, name, ssh_user, ssh_host)
 
     click.secho("=> TablePlus: Right click > New > Connection from URL...", fg="green")
     click.secho("\nLOCAL:", dim=True)
     click.secho(f"{local_db_url}")
     click.secho("\nPROD:", dim=True)
     click.secho(f"{prod_db_url}")
```

### Comparing `tableplus_db_urls-0.1.1/src/tableplus/core.py` & `tableplus_db_urls-0.1.2/src/tableplus/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,46 +23,45 @@
 
     return (
         f"{scheme}://{ssh}{username}:{password}@{host}:{port}{path}?"
         f"{query_string}".rstrip("?")
     )
 
 
-def get_local_db_conn_str(env_path=None) -> str:
+def get_local_db_conn_str(env_path, name: str) -> str:
     """Get the local DB connection string."""
     env = dotenv_values(Path(env_path))
     params = {
-        "statusColor": "F8F8F8",
+        "statusColor": "DAEBC2",
         "env": "local",
-        "name": "USTA",
+        "name": name,
         "lazyload": "true",
     }
 
     db_user = env["POSTGRES_USER"]
     db_pass = env["POSTGRES_PASSWORD"]
     db_name = env["POSTGRES_DB"]
 
     return build_db_url(db_user, db_pass, db_name, params=params)
 
 
-def get_prod_db_conn_str(env_path, ssh_user: str, ssh_host: str) -> str:
+def get_prod_db_conn_str(env_path, name: str, ssh_user: str, ssh_host: str) -> str:
     """Get the production DB connection string."""
     env = dotenv_values(Path(env_path))
     params = {
         "statusColor": "FFD7D4",
         "env": "production",
-        "name": "USTA [TEST]",
+        "name": name,
         "tLSMode": "0",
         "usePrivateKey": "true",
         # "safeModeLevel": "0",
         # "advancedSafeModeLevel": "0",
         # "driverVersion": "0",
         "lazyload": "true",
     }
-
     db_user = env["POSTGRES_USER"]
     db_pass = env["POSTGRES_PASSWORD"]
     db_name = env["POSTGRES_DB"]
 
     return build_db_url(
         db_user,
         db_pass,
```

### Comparing `tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/PKG-INFO` & `tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableplus-db-urls
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate TablePlus DB URLs from CookieCutter Django to make setting up connections easier.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/tableplus-db-urls.git
 Project-URL: Issues, https://github.com/tsantor/tableplus-db-urls/issues
 Project-URL: Changelog, https://github.com/tsantor/tableplus-db-urls/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -72,14 +72,18 @@
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/tableplus-db-urls/issues) on Github.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.2 (2024-05-15)
+
+- Added `name` argument to name the connection.
+
 ## 0.1.1 (2024-04-23)
 
 - Moved from `argparse` to `click`
 - Moved from `python-environ` to `python-dotenv`
 - Fixed bug with production URL
 
 ## 0.1.0 (2024-04-09)
```

### Comparing `tableplus_db_urls-0.1.1/src/tableplus_db_urls.egg-info/SOURCES.txt` & `tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tableplus_db_urls-0.1.1/tests/test_core.py` & `tableplus_db_urls-0.1.2/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 
     assert (
         url == "postgresql://testuser@127.0.0.1/user:pass@127.0.0.1:5432/path?foo=bar"
     )
 
 
 def test_get_local_db_conn_str(temp_env):
-    conn_str = get_local_db_conn_str(temp_env.name)
+    conn_str = get_local_db_conn_str(temp_env.name, name="Test")
     assert conn_str.startswith("postgresql://user:pass@127.0.0.1:5432/path")
 
 
 def test_get_prod_db_conn_str(temp_env):
     conn_str = get_prod_db_conn_str(
-        temp_env.name, ssh_user="testuser", ssh_host="127.0.0.1"
+        temp_env.name, name="Test", ssh_user="testuser", ssh_host="127.0.0.1"
     )
     assert conn_str.startswith(
         "postgresql+ssh://testuser@127.0.0.1/user:pass@127.0.0.1:5432/path"
     )
```

