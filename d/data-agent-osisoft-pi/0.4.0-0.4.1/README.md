# Comparing `tmp/data_agent_osisoft_pi-0.4.0.tar.gz` & `tmp/data_agent_osisoft_pi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_agent_osisoft_pi-0.4.0.tar", last modified: Mon May 13 16:09:56 2024, max compression
+gzip compressed data, was "data_agent_osisoft_pi-0.4.1.tar", last modified: Wed May 15 17:32:42 2024, max compression
```

## Comparing `data_agent_osisoft_pi-0.4.0.tar` & `data_agent_osisoft_pi-0.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.888380 data_agent_osisoft_pi-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.876380 data_agent_osisoft_pi-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.880380 data_agent_osisoft_pi-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-13 16:09:56.888380 data_agent_osisoft_pi-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.884380 data_agent_osisoft_pi-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.884380 data_agent_osisoft_pi-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-13 16:09:56.888380 data_agent_osisoft_pi-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.876380 data_agent_osisoft_pi-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.884380 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.884380 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-13 16:09:56.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-13 16:09:56.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:09:56.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 16:09:56.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:09:56.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 16:09:56.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 16:09:56.000000 data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:09:56.884380 data_agent_osisoft_pi-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-13 16:09:31.000000 data_agent_osisoft_pi-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.506669 data_agent_osisoft_pi-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.498669 data_agent_osisoft_pi-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.498669 data_agent_osisoft_pi-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-15 17:32:42.506669 data_agent_osisoft_pi-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.502669 data_agent_osisoft_pi-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.502669 data_agent_osisoft_pi-0.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-15 17:32:42.506669 data_agent_osisoft_pi-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.498669 data_agent_osisoft_pi-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.502669 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19244 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.506669 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-15 17:32:42.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-15 17:32:42.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:32:42.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 17:32:42.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:32:42.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-15 17:32:42.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 17:32:42.000000 data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:32:42.506669 data_agent_osisoft_pi-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-15 17:32:11.000000 data_agent_osisoft_pi-0.4.1/tox.ini
```

### Comparing `data_agent_osisoft_pi-0.4.0/.coveragerc` & `data_agent_osisoft_pi-0.4.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/.github/workflows/ci.yml` & `data_agent_osisoft_pi-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/.gitignore` & `data_agent_osisoft_pi-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/.pre-commit-config.yaml` & `data_agent_osisoft_pi-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/CONTRIBUTING.md` & `data_agent_osisoft_pi-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/LICENSE.txt` & `data_agent_osisoft_pi-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/PKG-INFO` & `data_agent_osisoft_pi-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-agent-osisoft-pi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Osisoft PI historian plugin for `data-agent` package
 Home-page: https://github.com/imubit/data-agent-osisoft-pi/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPL v3
 Project-URL: Documentation, https://github.com/imubit/data-agent-osisoft-pi/
 Project-URL: Source, https://github.com/imubit/data-agent-osisoft-pi/
```

### Comparing `data_agent_osisoft_pi-0.4.0/README.md` & `data_agent_osisoft_pi-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/docs/Makefile` & `data_agent_osisoft_pi-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/docs/conf.py` & `data_agent_osisoft_pi-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/docs/index.md` & `data_agent_osisoft_pi-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/setup.cfg` & `data_agent_osisoft_pi-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/setup.py` & `data_agent_osisoft_pi-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi/__init__.py` & `data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi/connector.py` & `data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,14 +531,15 @@
 
             if not tag_series:
                 return None
 
             if result_format == "dataframe":
                 df = pd.concat(tag_series, axis=1, sort=True)
                 df.index.name = "timestamp"
+                df.index = pd.to_datetime(df.index)
                 return df
             elif result_format == "series":
                 return tag_series if len(tag_series) > 1 else tag_series[0]
             else:
                 raise NotImplementedError(f"{result_format} not yet implemented")
 
             # TODO: Bulk Support - https://csharp.hotexamples.com/examples/-/PIPointList/RecordedValues/php-pipointlist-recordedvalues-method-examples.html # noqa: E501
```

### Comparing `data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/PKG-INFO` & `data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-agent-osisoft-pi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Osisoft PI historian plugin for `data-agent` package
 Home-page: https://github.com/imubit/data-agent-osisoft-pi/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPL v3
 Project-URL: Documentation, https://github.com/imubit/data-agent-osisoft-pi/
 Project-URL: Source, https://github.com/imubit/data-agent-osisoft-pi/
```

### Comparing `data_agent_osisoft_pi-0.4.0/src/data_agent_osisoft_pi.egg-info/SOURCES.txt` & `data_agent_osisoft_pi-0.4.1/src/data_agent_osisoft_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/tests/test_connector.py` & `data_agent_osisoft_pi-0.4.1/tests/test_connector.py`

 * *Files identical despite different names*

### Comparing `data_agent_osisoft_pi-0.4.0/tox.ini` & `data_agent_osisoft_pi-0.4.1/tox.ini`

 * *Files identical despite different names*

