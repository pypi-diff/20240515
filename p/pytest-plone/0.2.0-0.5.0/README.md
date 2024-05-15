# Comparing `tmp/pytest-plone-0.2.0.tar.gz` & `tmp/pytest_plone-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-plone-0.2.0.tar", last modified: Thu Jan  5 19:43:10 2023, max compression
+gzip compressed data, was "pytest_plone-0.5.0.tar", last modified: Wed May 15 17:08:19 2024, max compression
```

## Comparing `pytest-plone-0.2.0.tar` & `pytest_plone-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,40 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-01-05 19:43:10.048532 pytest-plone-0.2.0/
--rw-r--r--   0 ericof     (501) staff       (20)      972 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)      396 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/LICENSE.GPL
--rw-r--r--   0 ericof     (501) staff       (20)      157 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     2772 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)     9702 2023-01-05 19:43:10.048363 pytest-plone-0.2.0/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     8313 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/README.md
--rw-r--r--   0 ericof     (501) staff       (20)      828 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-01-05 19:43:10.048568 pytest-plone-0.2.0/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     1734 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-01-05 19:43:10.041371 pytest-plone-0.2.0/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-01-05 19:43:10.042641 pytest-plone-0.2.0/src/pytest_plone/
--rw-r--r--   0 ericof     (501) staff       (20)       46 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/src/pytest_plone/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-01-05 19:43:10.047900 pytest-plone-0.2.0/src/pytest_plone/fixtures/
--rw-r--r--   0 ericof     (501) staff       (20)      591 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/src/pytest_plone/fixtures/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      840 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/src/pytest_plone/fixtures/addons.py
--rw-r--r--   0 ericof     (501) staff       (20)      268 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/src/pytest_plone/fixtures/base.py
--rw-r--r--   0 ericof     (501) staff       (20)      629 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/src/pytest_plone/fixtures/content.py
--rw-r--r--   0 ericof     (501) staff       (20)      450 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/src/pytest_plone/fixtures/vocabularies.py
--rw-r--r--   0 ericof     (501) staff       (20)      422 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/src/pytest_plone/helpers.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-01-05 19:43:10.044682 pytest-plone-0.2.0/src/pytest_plone.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     9702 2023-01-05 19:43:10.000000 pytest-plone-0.2.0/src/pytest_plone.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)      657 2023-01-05 19:43:10.000000 pytest-plone-0.2.0/src/pytest_plone.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-01-05 19:43:10.000000 pytest-plone-0.2.0/src/pytest_plone.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)       41 2023-01-05 19:43:10.000000 pytest-plone-0.2.0/src/pytest_plone.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-01-05 19:43:10.000000 pytest-plone-0.2.0/src/pytest_plone.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)       86 2023-01-05 19:43:10.000000 pytest-plone-0.2.0/src/pytest_plone.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-01-05 19:43:10.000000 pytest-plone-0.2.0/src/pytest_plone.egg-info/top_level.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-01-05 19:43:10.048124 pytest-plone-0.2.0/tests/
--rw-r--r--   0 ericof     (501) staff       (20)     1080 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/tests/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)      720 2023-01-05 19:43:09.000000 pytest-plone-0.2.0/tests/test_fixtures.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 17:08:19.709559 pytest_plone-0.5.0/
+-rw-r--r--   0 ericof     (501) staff       (20)     1381 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)     1102 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/LICENSE.GPL
+-rw-r--r--   0 ericof     (501) staff       (20)      290 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)    11414 2024-05-15 17:08:19.709273 pytest_plone-0.5.0/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     8568 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       61 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/constraints.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      322 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/dependabot.yml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 17:08:19.706499 pytest_plone-0.5.0/news/
+-rw-r--r--   0 ericof     (501) staff       (20)      308 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/news/.changelog_template.jinja
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/news/.gitkeep
+-rw-r--r--   0 ericof     (501) staff       (20)     4599 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)       32 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2024-05-15 17:08:19.709602 pytest_plone-0.5.0/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2277 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 17:08:19.704734 pytest_plone-0.5.0/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 17:08:19.706742 pytest_plone-0.5.0/src/pytest_plone/
+-rw-r--r--   0 ericof     (501) staff       (20)       46 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 17:08:19.708264 pytest_plone-0.5.0/src/pytest_plone/fixtures/
+-rw-r--r--   0 ericof     (501) staff       (20)      638 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone/fixtures/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      929 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone/fixtures/addons.py
+-rw-r--r--   0 ericof     (501) staff       (20)      269 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone/fixtures/base.py
+-rw-r--r--   0 ericof     (501) staff       (20)      630 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone/fixtures/content.py
+-rw-r--r--   0 ericof     (501) staff       (20)      576 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone/fixtures/env.py
+-rw-r--r--   0 ericof     (501) staff       (20)      451 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone/fixtures/vocabularies.py
+-rw-r--r--   0 ericof     (501) staff       (20)      418 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone/helpers.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 17:08:19.708796 pytest_plone-0.5.0/src/pytest_plone.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)    11414 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)      808 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       41 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      229 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/src/pytest_plone.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 17:08:19.708505 pytest_plone-0.5.0/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)      736 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 17:08:19.708615 pytest_plone-0.5.0/tests/env/
+-rw-r--r--   0 ericof     (501) staff       (20)      787 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/tests/env/test_env_generate_mo.py
+-rw-r--r--   0 ericof     (501) staff       (20)      842 2024-05-15 17:08:19.000000 pytest_plone-0.5.0/tests/test_fixtures.py
```

### Comparing `pytest-plone-0.2.0/.editorconfig` & `pytest_plone-0.5.0/.editorconfig`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-# EditorConfig Configurtaion file, for more details see:
-# https://EditorConfig.org
+# Generated from:
+# https://github.com/plone/meta/tree/main/config/default
+# See the inline comments on how to expand/tweak this configuration file
+#
+# EditorConfig Configuration file, for more details see:
+# http://EditorConfig.org
 # EditorConfig is a convention description, that could be interpreted
 # by multiple editors to enforce common coding conventions for specific
 # file types
 
 # top-most EditorConfig file:
 # Will ignore other EditorConfig files in Home directory or upper tree level.
 root = true
 
 
-[*]  # For All Files
+[*]
+# Default settings for all files.
 # Unix-style newlines with a newline ending every file
 end_of_line = lf
 insert_final_newline = true
 trim_trailing_whitespace = true
 # Set default charset
 charset = utf-8
 # Indent style default
@@ -21,16 +26,31 @@
 # Max Line Length - a hard line wrap, should be disabled
 max_line_length = off
 
 [*.{py,cfg,ini}]
 # 4 space indentation
 indent_size = 4
 
-[*.{html,dtml,pt,zpt,xml,zcml,js,json,less,css,yml,yaml}]
+[*.{yml,zpt,pt,dtml,zcml,html,xml}]
 # 2 space indentation
 indent_size = 2
 
+[*.{json,jsonl,js,jsx,ts,tsx,css,less,scss}]
+# Frontend development
+# 2 space indentation
+indent_size = 2
+max_line_length = 80
+
 [{Makefile,.gitmodules}]
 # Tab indentation (no size specified, but view as 4 spaces)
 indent_style = tab
 indent_size = unset
 tab_width = unset
+
+
+##
+# Add extra configuration options in .meta.toml:
+#  [editorconfig]
+#  extra_lines = """
+#  _your own configuration lines_
+#  """
+##
```

### Comparing `pytest-plone-0.2.0/LICENSE.GPL` & `pytest_plone-0.5.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `pytest-plone-0.2.0/PKG-INFO` & `pytest_plone-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,31 @@
-Metadata-Version: 2.1
-Name: pytest-plone
-Version: 0.2.0
-Summary: Pytest plugin to test Plone addons
-Home-page: http://pypi.python.org/pypi/pytest-plone
-Author: Plone
-Author-email: test@plone.org
-License: GPL
-Keywords: Plone Pytest Testing
-Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 6.0
-Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.GPL
-
-
 <h1 align="center">pytest-plone</h1>
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - License](https://img.shields.io/pypi/l/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pytest-plone)](https://pypi.org/project/pytest-plone/)
 
 
 [![PyPI - Plone Versions](https://img.shields.io/pypi/frameworkversions/plone/pytest-plone)](https://pypi.org/project/pytest-plone/)
 
-[![Code analysis checks](https://github.com/collective/pytest-plone/actions/workflows/code-analysis.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/code-analysis.yml)
-[![Tests](https://github.com/collective/pytest-plone/actions/workflows/tests.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/tests.yml)
+[![Tests](https://github.com/collective/pytest-plone/actions/workflows/meta.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/meta.yml)
 ![Code Style](https://img.shields.io/badge/Code%20Style-Black-000000)
 
 [![GitHub contributors](https://img.shields.io/github/contributors/collective/pytest-plone)](https://github.com/collective/pytest-plone)
 [![GitHub Repo stars](https://img.shields.io/github/stars/collective/pytest-plone?style=social)](https://github.com/collective/pytest-plone)
 </div>
 
 **pytest-plone** is a [pytest](https://docs.pytest.org) plugin providing fixtures and helpers to test [Plone](https://plone.org) add-ons.
 
 
-This package is built on top of [gocept.pytestlayer](https://github.com/gocept/gocept.pytestlayer).
+This package is built on top of [zope.pytestlayer](https://github.com/zopefoundation/zope.pytestlayer).
 
 
 ## Reasoning
 
 Despite the fact Plone, and Zope, have their codebases tested with `unittest`, over the years
 `pytest` became the most popular choice for testing in Python.
 
@@ -96,14 +67,33 @@
 | integration_session | Session |
 | integration_class | Class |
 | integration | Function |
 
 
 ## Fixtures
 
+### generate_mo
+
+|  |  |
+| --- | --- |
+| Description | Set environment variable to force Zope to compile translation files |
+| Required Fixture |  |
+| Scope | **Session** |
+
+Add a new fixture to your `conftest.py` to force `generate_mo` to be called for all tests.
+
+```python
+
+@pytest.fixture(scope="session", autouse=True)
+def session_initialization(generate_mo):
+    """Fixture used to force translation files to be compiled."""
+    yield
+
+```
+
 ### app
 
 |  |  |
 | --- | --- |
 | Description | Zope root |
 | Required Fixture | **integration** |
 | Scope | **Function** |
@@ -332,50 +322,21 @@
 ## Plugin Development
 
 You need a working `python` environment (system, virtualenv, pyenv, etc) version 3.8 or superior.
 
 Then install the dependencies and a development instance using:
 
 ```bash
-make build
+make install
 ```
 
 To run tests for this package:
 
 ```bash
 make test
 ```
 
 By default we use the latest Plone version in the 6.x series.
 
 ## License
 
 The project is licensed under the GPLv2.
-
-
-# Changelog
-
-## 0.2.0 (2023-01-05)
-
-
-- Add `app` fixture.
-  [ericof]
-
-- Add `setup_tool` and `profile_last_version` fixtures.
-  [ericof]
-
-- Add `get_fti` and `get_behaviors` fixtures.
-  [ericof]
-
-- Add `get_vocabulary` fixture.
-  [ericof]
-
-
-## 0.1.0 (2023-01-04)
-
-- Fixtures `portal`, `http_request`, `installer`, `browser_layers`, `controlpanel_actions`
-  [ericof]
-
-- Initial release
-  [ericof]
-
-
```

### Comparing `pytest-plone-0.2.0/README.md` & `pytest_plone-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,78 @@
+Metadata-Version: 2.1
+Name: pytest-plone
+Version: 0.5.0
+Summary: Pytest plugin to test Plone addons
+Home-page: http://pypi.python.org/pypi/pytest-plone
+Author: Plone
+Author-email: test@plone.org
+License: GPL
+Project-URL: PyPI, https://pypi.python.org/pypi/pytest-plone
+Project-URL: Source, https://github.com/collective/pytest-plone
+Project-URL: Tracker, https://github.com/collective/pytest-plone/issues
+Keywords: Plone Pytest Testing
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Plone
+Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.GPL
+Requires-Dist: zope.pytestlayer
+Requires-Dist: plone.api
+Requires-Dist: plone.app.testing
+Requires-Dist: plone.base
+Requires-Dist: plone.browserlayer
+Requires-Dist: plone.dexterity
+Requires-Dist: Products.CMFPlone
+Requires-Dist: pytest<8.0.0
+Requires-Dist: setuptools
+Requires-Dist: zope.component
+Requires-Dist: zope.schema
+Provides-Extra: test
+Requires-Dist: zest.releaser[recommended]; extra == "test"
+Requires-Dist: zestreleaser.towncrier; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
+
 <h1 align="center">pytest-plone</h1>
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - License](https://img.shields.io/pypi/l/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pytest-plone)](https://pypi.org/project/pytest-plone/)
 
 
 [![PyPI - Plone Versions](https://img.shields.io/pypi/frameworkversions/plone/pytest-plone)](https://pypi.org/project/pytest-plone/)
 
-[![Code analysis checks](https://github.com/collective/pytest-plone/actions/workflows/code-analysis.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/code-analysis.yml)
-[![Tests](https://github.com/collective/pytest-plone/actions/workflows/tests.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/tests.yml)
+[![Tests](https://github.com/collective/pytest-plone/actions/workflows/meta.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/meta.yml)
 ![Code Style](https://img.shields.io/badge/Code%20Style-Black-000000)
 
 [![GitHub contributors](https://img.shields.io/github/contributors/collective/pytest-plone)](https://github.com/collective/pytest-plone)
 [![GitHub Repo stars](https://img.shields.io/github/stars/collective/pytest-plone?style=social)](https://github.com/collective/pytest-plone)
 </div>
 
 **pytest-plone** is a [pytest](https://docs.pytest.org) plugin providing fixtures and helpers to test [Plone](https://plone.org) add-ons.
 
 
-This package is built on top of [gocept.pytestlayer](https://github.com/gocept/gocept.pytestlayer).
+This package is built on top of [zope.pytestlayer](https://github.com/zopefoundation/zope.pytestlayer).
 
 
 ## Reasoning
 
 Despite the fact Plone, and Zope, have their codebases tested with `unittest`, over the years
 `pytest` became the most popular choice for testing in Python.
 
@@ -68,14 +114,33 @@
 | integration_session | Session |
 | integration_class | Class |
 | integration | Function |
 
 
 ## Fixtures
 
+### generate_mo
+
+|  |  |
+| --- | --- |
+| Description | Set environment variable to force Zope to compile translation files |
+| Required Fixture |  |
+| Scope | **Session** |
+
+Add a new fixture to your `conftest.py` to force `generate_mo` to be called for all tests.
+
+```python
+
+@pytest.fixture(scope="session", autouse=True)
+def session_initialization(generate_mo):
+    """Fixture used to force translation files to be compiled."""
+    yield
+
+```
+
 ### app
 
 |  |  |
 | --- | --- |
 | Description | Zope root |
 | Required Fixture | **integration** |
 | Scope | **Function** |
@@ -304,21 +369,74 @@
 ## Plugin Development
 
 You need a working `python` environment (system, virtualenv, pyenv, etc) version 3.8 or superior.
 
 Then install the dependencies and a development instance using:
 
 ```bash
-make build
+make install
 ```
 
 To run tests for this package:
 
 ```bash
 make test
 ```
 
 By default we use the latest Plone version in the 6.x series.
 
 ## License
 
 The project is licensed under the GPLv2.
+
+
+# Changelog
+
+<!--
+   You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+-->
+
+<!-- towncrier release notes start -->
+
+## 0.5.0 (2024-05-15)
+
+
+### New features:
+
+- Add fixture `generate_mo` to compile translation files during tests [@ericof] #5
+- Move from `gocept.pytestlayer` to `zope.pytestlayer` [@ericof] #11
+
+
+### Internal:
+
+- Implement plone/meta [@ericof] #6
+- Clean up dependencies for pytest-plone [@thet], [@gforcada], [@ericof] #9
+- Pin pytest version to be lower than 8.0 [@ericof] #12
+- Update plone/meta [@ericof] #13
+
+## 0.2.0 (2023-01-05)
+
+- Add `app` fixture.
+  [ericof]
+
+- Add `setup_tool` and `profile_last_version` fixtures.
+  [ericof]
+
+- Add `get_fti` and `get_behaviors` fixtures.
+  [ericof]
+
+- Add `get_vocabulary` fixture.
+  [ericof]
+
+
+## 0.1.0 (2023-01-04)
+
+- Fixtures `portal`, `http_request`, `installer`, `browser_layers`, `controlpanel_actions`
+  [ericof]
+
+- Initial release
+  [ericof]
+
+
```

### Comparing `pytest-plone-0.2.0/setup.py` & `pytest_plone-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Installer for the pytest-plone package."""
+
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
 long_description = f"""
 {Path("README.md").read_text()}\n
@@ -10,15 +11,15 @@
 """
 
 
 description = "Pytest plugin to test Plone addons"
 
 setup(
     name="pytest-plone",
-    version="0.2.0",
+    version="0.5.0",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
@@ -26,32 +27,49 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python",
         "Topic :: Software Development :: Testing",
     ],
     keywords="Plone Pytest Testing",
     author="Plone",
     author_email="test@plone.org",
     url="http://pypi.python.org/pypi/pytest-plone",
+    project_urls={
+        "PyPI": "https://pypi.python.org/pypi/pytest-plone",
+        "Source": "https://github.com/collective/pytest-plone",
+        "Tracker": "https://github.com/collective/pytest-plone/issues",
+    },
     license="GPL",
     packages=find_packages("src", exclude=["ez_setup"]),
     package_dir={"": "src"},
     python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        "Plone",
-        "setuptools",
-        "gocept.pytestlayer",
+        "zope.pytestlayer",
+        "plone.api",
         "plone.app.testing",
-        "plone.app.robotframework",
-        "pytest",
+        "plone.base",
+        "plone.browserlayer",
+        "plone.dexterity",
+        "Products.CMFPlone",
+        "pytest<8.0.0",
+        "setuptools",
+        "zope.component",
+        "zope.schema",
     ],
-    extras_require={},
+    extras_require={
+        "test": [
+            "zest.releaser[recommended]",
+            "zestreleaser.towncrier",
+            "pytest-cov",
+        ],
+    },
     entry_points={"pytest11": ["plone = pytest_plone.fixtures"]},
 )
```

### Comparing `pytest-plone-0.2.0/src/pytest_plone/fixtures/__init__.py` & `pytest_plone-0.5.0/src/pytest_plone/fixtures/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """All Fixtures."""
+
 from .addons import browser_layers
 from .addons import controlpanel_actions
 from .addons import installer
 from .addons import profile_last_version
 from .addons import setup_tool
 from .base import app
 from .base import http_request
 from .base import portal
 from .content import get_behaviors
 from .content import get_fti
+from .env import generate_mo
 from .vocabularies import get_vocabulary
 
 
 __all__ = [
     app,
     browser_layers,
     controlpanel_actions,
     get_behaviors,
+    generate_mo,
     get_fti,
     get_vocabulary,
     http_request,
     installer,
     profile_last_version,
     portal,
     setup_tool,
```

### Comparing `pytest-plone-0.2.0/src/pytest_plone/fixtures/addons.py` & `pytest_plone-0.5.0/src/pytest_plone/fixtures/addons.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Fixtures used in add-on install / uninstall tests."""
+
 from plone import api
 from plone.base.utils import get_installer
 from plone.browserlayer import utils
+from Products.CMFPlone.Portal import PloneSite
 
 import pytest
 
 
 @pytest.fixture
-def installer(portal):
+def installer(portal: PloneSite):
     return get_installer(portal)
 
 
 @pytest.fixture
-def browser_layers(portal):
+def browser_layers(portal: PloneSite):
     return utils.registered_layers()
 
 
 @pytest.fixture
-def controlpanel_actions(portal):
+def controlpanel_actions(portal: PloneSite) -> list:
     controlpanel = portal.portal_controlpanel
     return [a.getAction(portal)["id"] for a in controlpanel.listActions()]
 
 
 @pytest.fixture
 def setup_tool(integration):
     return api.portal.get_tool("portal_setup")
```

### Comparing `pytest-plone-0.2.0/src/pytest_plone/fixtures/content.py` & `pytest_plone-0.5.0/src/pytest_plone/fixtures/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Fixtures used in content tests."""
+
 from plone.dexterity.fti import DexterityFTI
 from plone.dexterity.interfaces import IDexterityFTI
 from zope.component import queryUtility
 
 import pytest
```

### Comparing `pytest-plone-0.2.0/src/pytest_plone.egg-info/PKG-INFO` & `pytest_plone-0.5.0/src/pytest_plone.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 Metadata-Version: 2.1
 Name: pytest-plone
-Version: 0.2.0
+Version: 0.5.0
 Summary: Pytest plugin to test Plone addons
 Home-page: http://pypi.python.org/pypi/pytest-plone
 Author: Plone
 Author-email: test@plone.org
 License: GPL
+Project-URL: PyPI, https://pypi.python.org/pypi/pytest-plone
+Project-URL: Source, https://github.com/collective/pytest-plone
+Project-URL: Tracker, https://github.com/collective/pytest-plone/issues
 Keywords: Plone Pytest Testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.GPL
+Requires-Dist: zope.pytestlayer
+Requires-Dist: plone.api
+Requires-Dist: plone.app.testing
+Requires-Dist: plone.base
+Requires-Dist: plone.browserlayer
+Requires-Dist: plone.dexterity
+Requires-Dist: Products.CMFPlone
+Requires-Dist: pytest<8.0.0
+Requires-Dist: setuptools
+Requires-Dist: zope.component
+Requires-Dist: zope.schema
+Provides-Extra: test
+Requires-Dist: zest.releaser[recommended]; extra == "test"
+Requires-Dist: zestreleaser.towncrier; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 
 <h1 align="center">pytest-plone</h1>
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-plone)](https://pypi.org/project/pytest-plone/)
@@ -35,26 +54,25 @@
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - License](https://img.shields.io/pypi/l/pytest-plone)](https://pypi.org/project/pytest-plone/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pytest-plone)](https://pypi.org/project/pytest-plone/)
 
 
 [![PyPI - Plone Versions](https://img.shields.io/pypi/frameworkversions/plone/pytest-plone)](https://pypi.org/project/pytest-plone/)
 
-[![Code analysis checks](https://github.com/collective/pytest-plone/actions/workflows/code-analysis.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/code-analysis.yml)
-[![Tests](https://github.com/collective/pytest-plone/actions/workflows/tests.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/tests.yml)
+[![Tests](https://github.com/collective/pytest-plone/actions/workflows/meta.yml/badge.svg)](https://github.com/collective/pytest-plone/actions/workflows/meta.yml)
 ![Code Style](https://img.shields.io/badge/Code%20Style-Black-000000)
 
 [![GitHub contributors](https://img.shields.io/github/contributors/collective/pytest-plone)](https://github.com/collective/pytest-plone)
 [![GitHub Repo stars](https://img.shields.io/github/stars/collective/pytest-plone?style=social)](https://github.com/collective/pytest-plone)
 </div>
 
 **pytest-plone** is a [pytest](https://docs.pytest.org) plugin providing fixtures and helpers to test [Plone](https://plone.org) add-ons.
 
 
-This package is built on top of [gocept.pytestlayer](https://github.com/gocept/gocept.pytestlayer).
+This package is built on top of [zope.pytestlayer](https://github.com/zopefoundation/zope.pytestlayer).
 
 
 ## Reasoning
 
 Despite the fact Plone, and Zope, have their codebases tested with `unittest`, over the years
 `pytest` became the most popular choice for testing in Python.
 
@@ -96,14 +114,33 @@
 | integration_session | Session |
 | integration_class | Class |
 | integration | Function |
 
 
 ## Fixtures
 
+### generate_mo
+
+|  |  |
+| --- | --- |
+| Description | Set environment variable to force Zope to compile translation files |
+| Required Fixture |  |
+| Scope | **Session** |
+
+Add a new fixture to your `conftest.py` to force `generate_mo` to be called for all tests.
+
+```python
+
+@pytest.fixture(scope="session", autouse=True)
+def session_initialization(generate_mo):
+    """Fixture used to force translation files to be compiled."""
+    yield
+
+```
+
 ### app
 
 |  |  |
 | --- | --- |
 | Description | Zope root |
 | Required Fixture | **integration** |
 | Scope | **Function** |
@@ -332,15 +369,15 @@
 ## Plugin Development
 
 You need a working `python` environment (system, virtualenv, pyenv, etc) version 3.8 or superior.
 
 Then install the dependencies and a development instance using:
 
 ```bash
-make build
+make install
 ```
 
 To run tests for this package:
 
 ```bash
 make test
 ```
@@ -350,16 +387,40 @@
 ## License
 
 The project is licensed under the GPLv2.
 
 
 # Changelog
 
-## 0.2.0 (2023-01-05)
+<!--
+   You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+-->
+
+<!-- towncrier release notes start -->
+
+## 0.5.0 (2024-05-15)
+
+
+### New features:
 
+- Add fixture `generate_mo` to compile translation files during tests [@ericof] #5
+- Move from `gocept.pytestlayer` to `zope.pytestlayer` [@ericof] #11
+
+
+### Internal:
+
+- Implement plone/meta [@ericof] #6
+- Clean up dependencies for pytest-plone [@thet], [@gforcada], [@ericof] #9
+- Pin pytest version to be lower than 8.0 [@ericof] #12
+- Update plone/meta [@ericof] #13
+
+## 0.2.0 (2023-01-05)
 
 - Add `app` fixture.
   [ericof]
 
 - Add `setup_tool` and `profile_last_version` fixtures.
   [ericof]
```

### Comparing `pytest-plone-0.2.0/src/pytest_plone.egg-info/SOURCES.txt` & `pytest_plone-0.5.0/src/pytest_plone.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 .editorconfig
 CHANGES.md
 LICENSE.GPL
 MANIFEST.in
-Makefile
 README.md
+constraints.txt
+dependabot.yml
 pyproject.toml
+requirements.txt
 setup.py
+news/.changelog_template.jinja
+news/.gitkeep
 src/pytest_plone/__init__.py
 src/pytest_plone/helpers.py
 src/pytest_plone.egg-info/PKG-INFO
 src/pytest_plone.egg-info/SOURCES.txt
 src/pytest_plone.egg-info/dependency_links.txt
 src/pytest_plone.egg-info/entry_points.txt
 src/pytest_plone.egg-info/not-zip-safe
 src/pytest_plone.egg-info/requires.txt
 src/pytest_plone.egg-info/top_level.txt
 src/pytest_plone/fixtures/__init__.py
 src/pytest_plone/fixtures/addons.py
 src/pytest_plone/fixtures/base.py
 src/pytest_plone/fixtures/content.py
+src/pytest_plone/fixtures/env.py
 src/pytest_plone/fixtures/vocabularies.py
 tests/conftest.py
-tests/test_fixtures.py
+tests/test_fixtures.py
+tests/env/test_env_generate_mo.py
```

### Comparing `pytest-plone-0.2.0/tests/test_fixtures.py` & `pytest_plone-0.5.0/tests/test_fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 def test_all_fixtures(testdir):
     """Test pytest-plone fixtures exist."""
-
     fixtures = [
         "app",
         "browser_layers",
         "controlpanel_actions",
+        "generate_mo",
         "get_behaviors",
         "get_fti",
         "get_vocabulary",
         "http_request",
         "installer",
-        "profile_last_version",
         "portal",
+        "profile_last_version",
         "setup_tool",
     ]
     pyfile = ""
     for fixture in fixtures:
         pyfile = f"""
         {pyfile}
 
-        def test_{fixture}({fixture}):
-            assert {fixture} is not None
+        def test_{fixture}_exists({fixture}):
+            # Just pass the test, because if a fixture is not available,
+            # it will raise an error
+            assert True
 
         """
 
     testdir.makepyfile(pyfile)
 
     # run all tests with pytest
     result = testdir.runpytest()
```

