# Comparing `tmp/tableplus_db_urls-0.1.2.tar.gz` & `tmp/tableplus_db_urls-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableplus_db_urls-0.1.2.tar", last modified: Wed May 15 13:27:35 2024, max compression
+gzip compressed data, was "tableplus_db_urls-0.1.3.tar", last modified: Wed May 15 14:18:09 2024, max compression
```

## Comparing `tableplus_db_urls-0.1.2.tar` & `tableplus_db_urls-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.876666 tableplus_db_urls-0.1.2/
--rw-r--r--   0 tsantor    (501) staff       (20)      200 2024-04-09 19:33:00.000000 tableplus_db_urls-0.1.2/AUTHORS.md
--rw-r--r--   0 tsantor    (501) staff       (20)      399 2024-05-15 13:26:57.000000 tableplus_db_urls-0.1.2/HISTORY.md
--rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-12 15:32:17.000000 tableplus_db_urls-0.1.2/LICENSE
--rw-r--r--   0 tsantor    (501) staff       (20)      159 2024-04-12 15:50:09.000000 tableplus_db_urls-0.1.2/MANIFEST.in
--rw-r--r--   0 tsantor    (501) staff       (20)     2720 2024-05-15 13:27:35.876435 tableplus_db_urls-0.1.2/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     1263 2024-04-23 20:51:37.000000 tableplus_db_urls-0.1.2/README.md
--rw-r--r--   0 tsantor    (501) staff       (20)     4700 2024-04-23 20:31:04.000000 tableplus_db_urls-0.1.2/pyproject.toml
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.874327 tableplus_db_urls-0.1.2/requirements/
--rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.2/requirements/requirements.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.2/requirements/requirements_dev.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.2/requirements/requirements_test.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-05-15 13:27:35.876721 tableplus_db_urls-0.1.2/setup.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-09 19:33:00.000000 tableplus_db_urls-0.1.2/setup.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.871853 tableplus_db_urls-0.1.2/src/
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.874901 tableplus_db_urls-0.1.2/src/tableplus/
--rw-r--r--   0 tsantor    (501) staff       (20)       42 2024-05-15 13:26:44.000000 tableplus_db_urls-0.1.2/src/tableplus/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1705 2024-05-14 22:10:33.000000 tableplus_db_urls-0.1.2/src/tableplus/cli.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1969 2024-05-15 13:25:38.000000 tableplus_db_urls-0.1.2/src/tableplus/core.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.876191 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/
--rw-r--r--   0 tsantor    (501) staff       (20)     2720 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)      534 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/SOURCES.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/dependency_links.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       48 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/entry_points.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/requires.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       10 2024-05-15 13:27:35.000000 tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/top_level.txt
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 13:27:35.875873 tableplus_db_urls-0.1.2/tests/
--rw-r--r--   0 tsantor    (501) staff       (20)     1367 2024-05-15 13:23:41.000000 tableplus_db_urls-0.1.2/tests/test_core.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 14:18:09.613164 tableplus_db_urls-0.1.3/
+-rw-r--r--   0 tsantor    (501) staff       (20)      200 2024-04-09 19:33:00.000000 tableplus_db_urls-0.1.3/AUTHORS.md
+-rw-r--r--   0 tsantor    (501) staff       (20)      477 2024-05-15 14:17:16.000000 tableplus_db_urls-0.1.3/HISTORY.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-12 15:32:17.000000 tableplus_db_urls-0.1.3/LICENSE
+-rw-r--r--   0 tsantor    (501) staff       (20)      159 2024-04-12 15:50:09.000000 tableplus_db_urls-0.1.3/MANIFEST.in
+-rw-r--r--   0 tsantor    (501) staff       (20)     2815 2024-05-15 14:18:09.612910 tableplus_db_urls-0.1.3/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     1280 2024-05-15 14:13:27.000000 tableplus_db_urls-0.1.3/README.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     4700 2024-04-23 20:31:04.000000 tableplus_db_urls-0.1.3/pyproject.toml
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 14:18:09.610184 tableplus_db_urls-0.1.3/requirements/
+-rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.3/requirements/requirements.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.3/requirements/requirements_dev.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-23 20:50:00.000000 tableplus_db_urls-0.1.3/requirements/requirements_test.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-05-15 14:18:09.613514 tableplus_db_urls-0.1.3/setup.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-09 19:33:00.000000 tableplus_db_urls-0.1.3/setup.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 14:18:09.607869 tableplus_db_urls-0.1.3/src/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 14:18:09.610737 tableplus_db_urls-0.1.3/src/tableplus/
+-rw-r--r--   0 tsantor    (501) staff       (20)       42 2024-05-15 14:17:22.000000 tableplus_db_urls-0.1.3/src/tableplus/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1705 2024-05-15 14:16:41.000000 tableplus_db_urls-0.1.3/src/tableplus/cli.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1969 2024-05-15 13:25:38.000000 tableplus_db_urls-0.1.3/src/tableplus/core.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 14:18:09.612652 tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/
+-rw-r--r--   0 tsantor    (501) staff       (20)     2815 2024-05-15 14:18:09.000000 tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)      534 2024-05-15 14:18:09.000000 tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/SOURCES.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-05-15 14:18:09.000000 tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/dependency_links.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       48 2024-05-15 14:18:09.000000 tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/entry_points.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-05-15 14:18:09.000000 tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/requires.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       10 2024-05-15 14:18:09.000000 tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-15 14:18:09.612213 tableplus_db_urls-0.1.3/tests/
+-rw-r--r--   0 tsantor    (501) staff       (20)     1367 2024-05-15 13:23:41.000000 tableplus_db_urls-0.1.3/tests/test_core.py
```

### Comparing `tableplus_db_urls-0.1.2/LICENSE` & `tableplus_db_urls-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tableplus_db_urls-0.1.2/PKG-INFO` & `tableplus_db_urls-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableplus-db-urls
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate TablePlus DB URLs from CookieCutter Django to make setting up connections easier.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/tableplus-db-urls.git
 Project-URL: Issues, https://github.com/tsantor/tableplus-db-urls/issues
 Project-URL: Changelog, https://github.com/tsantor/tableplus-db-urls/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -41,15 +41,15 @@
 $ python3 -m pip install tableplus-db-urls
 ```
 
 ## Usage
 
 ```bash
 # --path should be your django project root
-$ tableplus generate --path="." --ssh-user="user" --ssh-host="xxx.xxx.x.x"
+$ tableplus generate --path="." --name="DB Name" --ssh-user="user" --ssh-host="xxx.xxx.x.x"
 ```
 
 > **NOTE:** TablePlus DB URLs assumes you use an SSH Key to login and not password.
 
 Then in TablePlus, on the main screen, right-click and choose `New` > `Connection from URL...` and use the URLs provided by the output.
 
 ## Development
@@ -66,20 +66,24 @@
 make pytest
 make coverage
 make open_coverage
 ```
 
 ## Issues
 
-If you experience any issues, please create an [issue](https://github.com/tsantor/tableplus-db-urls/issues) on Github.
+If you experience any issues, please create an [issue](https://github.com/tsantor/tableplus-db-urls/issues) on GitHub.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.3 (2024-05-15)
+
+- Bug fix with CLI implementation after `name` added.
+
 ## 0.1.2 (2024-05-15)
 
 - Added `name` argument to name the connection.
 
 ## 0.1.1 (2024-04-23)
 
 - Moved from `argparse` to `click`
```

### Comparing `tableplus_db_urls-0.1.2/README.md` & `tableplus_db_urls-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 $ python3 -m pip install tableplus-db-urls
 ```
 
 ## Usage
 
 ```bash
 # --path should be your django project root
-$ tableplus generate --path="." --ssh-user="user" --ssh-host="xxx.xxx.x.x"
+$ tableplus generate --path="." --name="DB Name" --ssh-user="user" --ssh-host="xxx.xxx.x.x"
 ```
 
 > **NOTE:** TablePlus DB URLs assumes you use an SSH Key to login and not password.
 
 Then in TablePlus, on the main screen, right-click and choose `New` > `Connection from URL...` and use the URLs provided by the output.
 
 ## Development
@@ -41,8 +41,8 @@
 make pytest
 make coverage
 make open_coverage
 ```
 
 ## Issues
 
-If you experience any issues, please create an [issue](https://github.com/tsantor/tableplus-db-urls/issues) on Github.
+If you experience any issues, please create an [issue](https://github.com/tsantor/tableplus-db-urls/issues) on GitHub.
```

### Comparing `tableplus_db_urls-0.1.2/pyproject.toml` & `tableplus_db_urls-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tableplus_db_urls-0.1.2/src/tableplus/cli.py` & `tableplus_db_urls-0.1.3/src/tableplus/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         click.echo = silent_echo
 
     project_path = Path(path).expanduser()
     local_env_path = str(project_path / ".envs/.local/.postgres")
     prod_env_path = str(project_path / ".envs/.production/.postgres")
 
     local_db_url = get_local_db_conn_str(name, local_env_path)
-    prod_db_url = get_prod_db_conn_str(prod_env_path, name, ssh_user, ssh_host)
+    prod_db_url = get_prod_db_conn_str(name, prod_env_path, ssh_user, ssh_host)
 
     click.secho("=> TablePlus: Right click > New > Connection from URL...", fg="green")
     click.secho("\nLOCAL:", dim=True)
     click.secho(f"{local_db_url}")
     click.secho("\nPROD:", dim=True)
     click.secho(f"{prod_db_url}")
```

### Comparing `tableplus_db_urls-0.1.2/src/tableplus/core.py` & `tableplus_db_urls-0.1.3/src/tableplus/core.py`

 * *Files identical despite different names*

### Comparing `tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/PKG-INFO` & `tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableplus-db-urls
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate TablePlus DB URLs from CookieCutter Django to make setting up connections easier.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/tableplus-db-urls.git
 Project-URL: Issues, https://github.com/tsantor/tableplus-db-urls/issues
 Project-URL: Changelog, https://github.com/tsantor/tableplus-db-urls/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -41,15 +41,15 @@
 $ python3 -m pip install tableplus-db-urls
 ```
 
 ## Usage
 
 ```bash
 # --path should be your django project root
-$ tableplus generate --path="." --ssh-user="user" --ssh-host="xxx.xxx.x.x"
+$ tableplus generate --path="." --name="DB Name" --ssh-user="user" --ssh-host="xxx.xxx.x.x"
 ```
 
 > **NOTE:** TablePlus DB URLs assumes you use an SSH Key to login and not password.
 
 Then in TablePlus, on the main screen, right-click and choose `New` > `Connection from URL...` and use the URLs provided by the output.
 
 ## Development
@@ -66,20 +66,24 @@
 make pytest
 make coverage
 make open_coverage
 ```
 
 ## Issues
 
-If you experience any issues, please create an [issue](https://github.com/tsantor/tableplus-db-urls/issues) on Github.
+If you experience any issues, please create an [issue](https://github.com/tsantor/tableplus-db-urls/issues) on GitHub.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.3 (2024-05-15)
+
+- Bug fix with CLI implementation after `name` added.
+
 ## 0.1.2 (2024-05-15)
 
 - Added `name` argument to name the connection.
 
 ## 0.1.1 (2024-04-23)
 
 - Moved from `argparse` to `click`
```

### Comparing `tableplus_db_urls-0.1.2/src/tableplus_db_urls.egg-info/SOURCES.txt` & `tableplus_db_urls-0.1.3/src/tableplus_db_urls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tableplus_db_urls-0.1.2/tests/test_core.py` & `tableplus_db_urls-0.1.3/tests/test_core.py`

 * *Files identical despite different names*

