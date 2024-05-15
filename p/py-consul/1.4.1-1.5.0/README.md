# Comparing `tmp/py-consul-1.4.1.tar.gz` & `tmp/py_consul-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-consul-1.4.1.tar", last modified: Wed Mar 27 14:08:01 2024, max compression
+gzip compressed data, was "py_consul-1.5.0.tar", last modified: Wed May 15 13:31:14 2024, max compression
```

## Comparing `py-consul-1.4.1.tar` & `py_consul-1.5.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:08:01.738953 py-consul-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-27 14:07:52.000000 py-consul-1.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-27 14:07:52.000000 py-consul-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 14:07:52.000000 py-consul-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-03-27 14:08:01.738953 py-consul-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-27 14:07:52.000000 py-consul-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:08:01.730953 py-consul-1.4.1/consul/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/aio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:08:01.734953 py-consul-1.4.1/consul/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/kv.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/api/txn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-27 14:07:52.000000 py-consul-1.4.1/consul/std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:08:01.734953 py-consul-1.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:07:52.000000 py-consul-1.4.1/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-03-27 14:07:52.000000 py-consul-1.4.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:08:01.738953 py-consul-1.4.1/py_consul.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-03-27 14:08:01.000000 py-consul-1.4.1/py_consul.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-27 14:08:01.000000 py-consul-1.4.1/py_consul.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:08:01.000000 py-consul-1.4.1/py_consul.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 14:08:01.000000 py-consul-1.4.1/py_consul.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-27 14:08:01.000000 py-consul-1.4.1/py_consul.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-27 14:07:52.000000 py-consul-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-27 14:07:52.000000 py-consul-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-27 14:08:01.738953 py-consul-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-27 14:07:52.000000 py-consul-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:08:01.734953 py-consul-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-03-27 14:07:54.000000 py-consul-1.4.1/tests/test_aio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-03-27 14:07:54.000000 py-consul-1.4.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-27 14:07:54.000000 py-consul-1.4.1/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-27 14:07:54.000000 py-consul-1.4.1/tests/test_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-27 14:07:54.000000 py-consul-1.4.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-27 14:07:52.000000 py-consul-1.4.1/tests-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.813481 py_consul-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-15 13:31:03.000000 py_consul-1.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 13:31:03.000000 py_consul-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 13:31:03.000000 py_consul-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-15 13:31:14.813481 py_consul-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-15 13:31:03.000000 py_consul-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.809481 py_consul-1.5.0/consul/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/aio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.809481 py_consul-1.5.0/consul/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.809481 py_consul-1.5.0/consul/api/acl/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/acl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/acl/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/acl/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/kv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/txn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.809481 py_consul-1.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:03.000000 py_consul-1.5.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-05-15 13:31:03.000000 py_consul-1.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.813481 py_consul-1.5.0/py_consul.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-15 13:31:03.000000 py_consul-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 13:31:03.000000 py_consul-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 13:31:14.813481 py_consul-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-15 13:31:03.000000 py_consul-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.813481 py_consul-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-15 13:31:03.000000 py_consul-1.5.0/tests-requirements.txt
```

### Comparing `py-consul-1.4.1/CHANGELOG.md` & `py_consul-1.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change log
 
+## 1.5.0
+
+- **[Breaking]** ACL endpoint change, consul.acl is now consul.acl.token
+- **feature:** add consul.acl.policy.list and acl.policy.read
+
 ## 1.4.1
 
 - **ci:** fix package publishing and update GH actions versions
 
 ## 1.4.0 (unreleased)
 
 - **[Breaking]** due to the re-implementation of the ACL endpoint and the drop of the support of OSX and consul 1.1.0.
```

### Comparing `py-consul-1.4.1/LICENSE` & `py_consul-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/PKG-INFO` & `py_consul-1.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-consul
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python client for Consul (http://www.consul.io/)
 Home-page: https://github.com/criteo-forks/py-consul
 Author: Criteo
 Author-email: github@criteo.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,22 +19,24 @@
 License-File: LICENSE
 Requires-Dist: requests>=2.0
 Provides-Extra: asyncio
 Requires-Dist: aiohttp; extra == "asyncio"
 
 # py-consul [![PyPi version](https://img.shields.io/pypi/v/py-consul.svg)](https://pypi.python.org/pypi/py-consul/) [![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/) ![Status](https://img.shields.io/badge/status-maintained-green.svg)
 
-Fork intent
+Status
 -----------
+This project is maintained and actively developed by Criteo.
+We aim at converging towards a full compatibility with the official Consul API.
 
-The origin project https://github.com/cablehead/python-consul is not maintained
-since 2018.  As we're not able to get in touch with the maintainer (cablehead)
-to merge and release our PRs, we've forked the project in order to continue the
-maintenance of the project.  We also renamed the project to be able to upload
-on pypi; see https://pypi.org/project/py-consul/
+We're currently supporting consul 1.13 up to 1.17. Due to quite a few changes 
+since our development started (see section "A bit of history"), some endpoints are 
+still partially handled.
+
+Therefore, we are open to contributions and suggestions.
 
 Example
 -------
 
 ```python
     import consul
 
@@ -52,32 +54,50 @@
 
 Installation
 ------------
 ```bash
     pip install py-consul
 ```
 
-**Note:** When using py-consul library in environment with proxy server, setting of ``http_proxy``, ``https_proxy`` and ``no_proxy`` environment variables can be required for proper functionality.
+**Note:** When using py-consul library in environment with proxy server, 
+setting of ``http_proxy``, ``https_proxy`` and ``no_proxy`` environment variables 
+can be required for proper functionality.
+
+A bit of history
+-----------
+
+The origin project [python-consul](https://github.com/cablehead/python-consul) is not maintained
+since 2018.  As we were not able to get in touch with the maintainer (cablehead)
+to merge and release our PRs, we've forked the project in order to continue the
+maintenance of the project. We also renamed the project to be able to upload
+on pypi; see [PyPI](https://pypi.org/project/py-consul/)
+
+Following some major changes, we decided to detach this fork from the original project
+and move from [criteo fork space](https://github.com/criteo-forks/) 
+to [criteo space](https://github.com/criteo/).
 
 Contributing
 ------------
 
-py-consul is currently maintained by Criteo folks.
-
 Please reach out if you're interested in being a maintainer as well. Otherwise,
-open a PR or Issue we'll try and respond as quickly as we're able.
+open a PR or Issue we'll try and respond as quickly as possible.
 
 When you create a PR please ensure:
 
-- To add tests for your new features, if reasonable
-- To add docstrings for new api features you may add
+- To add tests for your new features, if applicable
+- To add docstrings for new API features you may add
 
 
 # Change log
 
+## 1.5.0
+
+- **[Breaking]** ACL endpoint change, consul.acl is now consul.acl.token
+- **feature:** add consul.acl.policy.list and acl.policy.read
+
 ## 1.4.1
 
 - **ci:** fix package publishing and update GH actions versions
 
 ## 1.4.0 (unreleased)
 
 - **[Breaking]** due to the re-implementation of the ACL endpoint and the drop of the support of OSX and consul 1.1.0.
```

### Comparing `py-consul-1.4.1/consul/aio.py` & `py_consul-1.5.0/consul/aio.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/acl.py` & `py_consul-1.5.0/consul/api/acl/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 
 from consul.callback import CB
 
 
-class ACL:
+class Token:
     def __init__(self, agent):
         self.agent = agent
 
     def list(self, token=None):
         """
         Lists all the active ACL tokens. This is a privileged endpoint, and
         requires a management token. *token* will override this client's
```

### Comparing `py-consul-1.4.1/consul/api/agent.py` & `py_consul-1.5.0/consul/api/agent.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/catalog.py` & `py_consul-1.5.0/consul/api/catalog.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/connect.py` & `py_consul-1.5.0/consul/api/connect.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/coordinates.py` & `py_consul-1.5.0/consul/api/coordinates.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/event.py` & `py_consul-1.5.0/consul/api/event.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/health.py` & `py_consul-1.5.0/consul/api/health.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/kv.py` & `py_consul-1.5.0/consul/api/kv.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/query.py` & `py_consul-1.5.0/consul/api/query.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/session.py` & `py_consul-1.5.0/consul/api/session.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/status.py` & `py_consul-1.5.0/consul/api/status.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/api/txn.py` & `py_consul-1.5.0/consul/api/txn.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/base.py` & `py_consul-1.5.0/consul/base.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/callback.py` & `py_consul-1.5.0/consul/callback.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/check.py` & `py_consul-1.5.0/consul/check.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/consul/std.py` & `py_consul-1.5.0/consul/std.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/docs/conf.py` & `py_consul-1.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/py_consul.egg-info/PKG-INFO` & `py_consul-1.5.0/py_consul.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-consul
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python client for Consul (http://www.consul.io/)
 Home-page: https://github.com/criteo-forks/py-consul
 Author: Criteo
 Author-email: github@criteo.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,22 +19,24 @@
 License-File: LICENSE
 Requires-Dist: requests>=2.0
 Provides-Extra: asyncio
 Requires-Dist: aiohttp; extra == "asyncio"
 
 # py-consul [![PyPi version](https://img.shields.io/pypi/v/py-consul.svg)](https://pypi.python.org/pypi/py-consul/) [![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/) ![Status](https://img.shields.io/badge/status-maintained-green.svg)
 
-Fork intent
+Status
 -----------
+This project is maintained and actively developed by Criteo.
+We aim at converging towards a full compatibility with the official Consul API.
 
-The origin project https://github.com/cablehead/python-consul is not maintained
-since 2018.  As we're not able to get in touch with the maintainer (cablehead)
-to merge and release our PRs, we've forked the project in order to continue the
-maintenance of the project.  We also renamed the project to be able to upload
-on pypi; see https://pypi.org/project/py-consul/
+We're currently supporting consul 1.13 up to 1.17. Due to quite a few changes 
+since our development started (see section "A bit of history"), some endpoints are 
+still partially handled.
+
+Therefore, we are open to contributions and suggestions.
 
 Example
 -------
 
 ```python
     import consul
 
@@ -52,32 +54,50 @@
 
 Installation
 ------------
 ```bash
     pip install py-consul
 ```
 
-**Note:** When using py-consul library in environment with proxy server, setting of ``http_proxy``, ``https_proxy`` and ``no_proxy`` environment variables can be required for proper functionality.
+**Note:** When using py-consul library in environment with proxy server, 
+setting of ``http_proxy``, ``https_proxy`` and ``no_proxy`` environment variables 
+can be required for proper functionality.
+
+A bit of history
+-----------
+
+The origin project [python-consul](https://github.com/cablehead/python-consul) is not maintained
+since 2018.  As we were not able to get in touch with the maintainer (cablehead)
+to merge and release our PRs, we've forked the project in order to continue the
+maintenance of the project. We also renamed the project to be able to upload
+on pypi; see [PyPI](https://pypi.org/project/py-consul/)
+
+Following some major changes, we decided to detach this fork from the original project
+and move from [criteo fork space](https://github.com/criteo-forks/) 
+to [criteo space](https://github.com/criteo/).
 
 Contributing
 ------------
 
-py-consul is currently maintained by Criteo folks.
-
 Please reach out if you're interested in being a maintainer as well. Otherwise,
-open a PR or Issue we'll try and respond as quickly as we're able.
+open a PR or Issue we'll try and respond as quickly as possible.
 
 When you create a PR please ensure:
 
-- To add tests for your new features, if reasonable
-- To add docstrings for new api features you may add
+- To add tests for your new features, if applicable
+- To add docstrings for new API features you may add
 
 
 # Change log
 
+## 1.5.0
+
+- **[Breaking]** ACL endpoint change, consul.acl is now consul.acl.token
+- **feature:** add consul.acl.policy.list and acl.policy.read
+
 ## 1.4.1
 
 - **ci:** fix package publishing and update GH actions versions
 
 ## 1.4.0 (unreleased)
 
 - **[Breaking]** due to the re-implementation of the ACL endpoint and the drop of the support of OSX and consul 1.1.0.
```

### Comparing `py-consul-1.4.1/py_consul.egg-info/SOURCES.txt` & `py_consul-1.5.0/py_consul.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 consul/aio.py
 consul/base.py
 consul/callback.py
 consul/check.py
 consul/exceptions.py
 consul/std.py
 consul/api/__init__.py
-consul/api/acl.py
 consul/api/agent.py
 consul/api/catalog.py
 consul/api/connect.py
 consul/api/coordinates.py
 consul/api/event.py
 consul/api/health.py
 consul/api/kv.py
 consul/api/operator.py
 consul/api/query.py
 consul/api/session.py
 consul/api/status.py
 consul/api/txn.py
+consul/api/acl/__init__.py
+consul/api/acl/policy.py
+consul/api/acl/token.py
 docs/__init__.py
 docs/conf.py
 py_consul.egg-info/PKG-INFO
 py_consul.egg-info/SOURCES.txt
 py_consul.egg-info/dependency_links.txt
 py_consul.egg-info/requires.txt
 py_consul.egg-info/top_level.txt
```

### Comparing `py-consul-1.4.1/pyproject.toml` & `py_consul-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/setup.py` & `py_consul-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/tests/test_aio.py` & `py_consul-1.5.0/tests/test_aio.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     c = consul.aio.Consul(port=consul_port)
     yield c, consul_version
     await c.close()
 
 
 @pytest.fixture()
 async def consul_acl_obj(acl_consul):
-    consul_port, token, consul_version = acl_consul
-    c = consul.aio.Consul(port=consul_port, token=token)
-    yield c, consul_version
-    await c.close()
+    consul, token, consul_version = acl_consul
+    consul.token = token
+    yield consul, consul_version
+    await consul.close()
 
 
 class TestAsyncioConsul:
     async def test_kv(self, consul_obj):
         c, _consul_version = consul_obj
         _index, data = await c.kv.get("foo")
         assert data is None
```

### Comparing `py-consul-1.4.1/tests/test_base.py` & `py_consul-1.5.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/tests/test_callback.py` & `py_consul-1.5.0/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `py-consul-1.4.1/tests/test_utils.py` & `py_consul-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

