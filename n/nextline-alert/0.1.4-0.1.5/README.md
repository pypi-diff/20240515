# Comparing `tmp/nextline_alert-0.1.4.tar.gz` & `tmp/nextline_alert-0.1.5.tar.gz`

## Comparing `nextline_alert-0.1.4.tar` & `nextline_alert-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/setup.cfg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/release.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/workflows/release.yml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/__about__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/default.toml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/emitter.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/py.typed
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/schema/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/schema/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/tests/test_emitter.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/tests/test_version.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/README.md
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/setup.cfg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/release.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/__about__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/default.toml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/emitter.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/py.typed
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/schema/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/src/nextline_alert/schema/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/tests/test_emitter.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/tests/test_version.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/README.md
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 nextline_alert-0.1.5/PKG-INFO
```

### Comparing `nextline_alert-0.1.4/.github/workflows/pypi.yml` & `nextline_alert-0.1.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.4/.github/workflows/release.yml` & `nextline_alert-0.1.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.4/.github/workflows/type-check.yml` & `nextline_alert-0.1.5/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.4/.github/workflows/unit-test.yml` & `nextline_alert-0.1.5/.github/workflows/unit-test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 env:
   PYTHONUNBUFFERED: "1"
   FORCE_COLOR: "1"
 
 jobs:
   run:
     name: Python ${{ matrix.python-version }} on Linux
-    runs-on: ${{ matrix.os }}
+    runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
         python-version: ["3.10", "3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
@@ -39,12 +38,13 @@
           pip install --upgrade pip
           pip install -e '.[tests]'
           pip list
 
       - name: Run tests
         run: pytest -vv --cov --cov-report=xml
 
-      # - name: Upload coverage to Codecov
-      #   uses: codecov/codecov-action@v4
-      #   with:
-      #     fail_ci_if_error: true
-      #     verbose: true
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v4
+        with:
+          fail_ci_if_error: true
+          token: ${{ secrets.CODECOV_TOKEN }}
+          verbose: true
```

### Comparing `nextline_alert-0.1.4/src/nextline_alert/emitter.py` & `nextline_alert-0.1.5/src/nextline_alert/emitter.py`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.4/src/nextline_alert/plugin.py` & `nextline_alert-0.1.5/src/nextline_alert/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.4/tests/test_emitter.py` & `nextline_alert-0.1.5/tests/test_emitter.py`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.4/.gitignore` & `nextline_alert-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.4/LICENSE.txt` & `nextline_alert-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.4/README.md` & `nextline_alert-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,53 @@
+Metadata-Version: 2.3
+Name: nextline-alert
+Version: 0.1.5
+Summary: A plugin of nextline-graphql. Emit alerts to Campana
+Project-URL: Documentation, https://github.com/simonsobs/nextline-alert#readme
+Project-URL: Issues, https://github.com/simonsobs/nextline-alert/issues
+Project-URL: Source, https://github.com/simonsobs/nextline-alert
+Author-email: Simons Observatory <so_software@simonsobservatory.org>
+License-Expression: MIT
+License-File: LICENSE.txt
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Requires-Dist: httpx>=0.26
+Requires-Dist: nextline-graphql>=0.7.8
+Provides-Extra: tests
+Requires-Dist: pytest-asyncio>=0.23; extra == 'tests'
+Requires-Dist: pytest-cov>=4.1; extra == 'tests'
+Requires-Dist: pytest-timeout>=2.2; extra == 'tests'
+Requires-Dist: pytest>=7.4; extra == 'tests'
+Requires-Dist: respx>=0.20; extra == 'tests'
+Description-Content-Type: text/markdown
+
 # Nextline Alert
 
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline-alert.svg)](https://pypi.org/project/nextline-alert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline-alert.svg)](https://pypi.org/project/nextline-alert)
+
 [![Test Status](https://github.com/simonsobs/nextline-alert/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline-alert/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-alert/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline-alert/actions/workflows/type-check.yml)
+[![codecov](https://codecov.io/gh/simonsobs/nextline-alert/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline-alert)
 
 A plugin for [nextline-graphql](https://github.com/simonsobs/nextline-graphql).
 Emit alerts to [Campana](https://github.com/simonsobs/campana)
 
----
-
-**Table of Contents**
-
-- [Nextline Alert](#nextline-alert)
-  - [Installation](#installation)
-  - [Configuration](#configuration)
-  - [License](#license)
-  - [Contact](#contact)
 
 ## Installation
 
 ```console
 pip install nextline-alert
 ```
 
 ## Configuration
 
 | Environment variable          | Default value             | Description          |
 | ----------------------------- | ------------------------- | -------------------- |
 | `NEXTLINE_ALERT__CAMPANA_URL` | `http://httpbin.org/post` | The CAMPANA endpoint |
 | `NEXTLINE_ALERT__PLATFORM`    | `localhost`               | The platform name    |
-
-## License
-
-`nextline-alert` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
-
-## Contact
-
-- [Tai Sakuma](https://github.com/TaiSakuma) <span itemscope itemtype="https://schema.org/Person"><a itemprop="sameAs" content="https://orcid.org/0000-0003-3225-9861" href="https://orcid.org/0000-0003-3225-9861" target="orcid.widget" rel="me noopener noreferrer" style="vertical-align:text-top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a></span>
```

### Comparing `nextline_alert-0.1.4/pyproject.toml` & `nextline_alert-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-dependencies = ["nextline-graphql>=0.7.6", "httpx>=0.26"]
+dependencies = ["nextline-graphql>=0.7.8", "httpx>=0.26"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 tests = [
   "pytest-asyncio>=0.23",
   "pytest-cov>=4.1",
   "pytest-timeout>=2.2",
```

