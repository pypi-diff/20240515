# Comparing `tmp/atsphinx_mini18n-0.3.1.tar.gz` & `tmp/atsphinx_mini18n-0.4.0.tar.gz`

## Comparing `atsphinx_mini18n-0.3.1.tar` & `atsphinx_mini18n-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.age.toml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.editorconfig
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.python-version
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/CHANGES.rst
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/requirements-dev.lock
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/requirements.lock
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.github/release-body.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.github/workflows/deploy-doc.yml
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.github/workflows/main.yml
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.github/workflows/release.yml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/.gitignore
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/.ruff.toml
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/Makefile
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/conf.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/make.bat
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/changelogs/index.po
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/configuration.po
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/index.po
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/setup.po
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_static/.gitignore
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_templates/.gitignore
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/0.1.0.rst
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/0.2.0.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/0.2.1.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/0.3.0.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/index.rst
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/usage/configuration.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/usage/index.rst
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/usage/setup.rst
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/__init__.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/templates/mini18n/index.html
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/templates/mini18n/snippets/select-lang.html
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/.ruff.toml
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/test_it.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/test-root/conf.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/test-root/index.rst
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tools/archive_changelog.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.gitignore
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/LICENSE
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/README.rst
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.age.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.editorconfig
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.python-version
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/CHANGES.rst
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/requirements.lock
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.github/release-body.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.github/workflows/deploy-doc.yml
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/.gitignore
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/.ruff.toml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/Makefile
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/conf.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/make.bat
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/changelogs/index.po
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/usage/configuration.po
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/usage/index.po
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/usage/setup.po
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/_static/.gitignore
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/_templates/.gitignore
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/changelogs/0.1.0.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/changelogs/0.2.0.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/changelogs/0.2.1.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/changelogs/0.3.0.rst
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/changelogs/0.3.1.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/changelogs/index.rst
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/usage/configuration.rst
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/usage/index.rst
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/doc/usage/setup.rst
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/src/atsphinx/mini18n/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/src/atsphinx/mini18n/templates/mini18n/index.html
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/src/atsphinx/mini18n/templates/mini18n/snippets/select-lang.html
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tests/.ruff.toml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tests/test_it.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tests/test_javascript.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tests/test-e2e/conf.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tests/test-e2e/index.rst
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tests/test-root/conf.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tests/test-root/index.rst
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/tools/run_age.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/.gitignore
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/README.rst
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.4.0/PKG-INFO
```

### Comparing `atsphinx_mini18n-0.3.1/.age.toml` & `atsphinx_mini18n-0.4.0/.age.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-current_version = "0.3.1"
+current_version = "0.4.0"
 
 [[files]]
 path = "pyproject.toml"
 search = "version = \"{{current_version}}\""
 replace = "version = \"{{new_version}}\""
 
 [[files]]
```

### Comparing `atsphinx_mini18n-0.3.1/.editorconfig` & `atsphinx_mini18n-0.4.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/requirements-dev.lock` & `atsphinx_mini18n-0.4.0/requirements-dev.lock`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     # via sphinx-revealjs
     # via sphinx-tabs
 esbonio==0.16.4
 exceptiongroup==1.2.0
     # via cattrs
     # via pytest
 furo==2024.1.29
+greenlet==3.0.3
+    # via playwright
 idna==3.6
     # via requests
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==7.1.0
     # via sphinx
 iniconfig==2.0.0
@@ -56,28 +58,40 @@
     # via jinja2
 packaging==24.0
     # via pytest
     # via sphinx
     # via sphinx-revealjs
 platformdirs==4.2.0
     # via esbonio
+playwright==1.43.0
+    # via pytest-playwright
 pluggy==1.4.0
     # via pytest
+pyee==11.1.0
+    # via playwright
 pygls==1.3.0
     # via esbonio
 pygments==2.17.2
     # via furo
     # via sphinx
     # via sphinx-tabs
 pyspellchecker==0.8.1
     # via esbonio
 pytest==7.4.4
+    # via pytest-base-url
+    # via pytest-playwright
+pytest-base-url==2.1.0
+    # via pytest-playwright
+pytest-playwright==0.5.0
+python-slugify==8.0.4
+    # via pytest-playwright
 pytz==2024.1
     # via babel
 requests==2.31.0
+    # via pytest-base-url
     # via sphinx
 setuptools==69.2.0
     # via sphinx-intl
 six==1.16.0
     # via livereload
 snowballstemmer==2.2.0
     # via sphinx
@@ -106,17 +120,20 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
+text-unidecode==1.3
+    # via python-slugify
 tomli==2.0.1
     # via pytest
 tornado==6.4
     # via livereload
 typing-extensions==4.10.0
     # via cattrs
+    # via pyee
 urllib3==2.2.1
     # via requests
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `atsphinx_mini18n-0.3.1/requirements.lock` & `atsphinx_mini18n-0.4.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/.github/workflows/deploy-doc.yml` & `atsphinx_mini18n-0.4.0/.github/workflows/deploy-doc.yml`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/.github/workflows/main.yml` & `atsphinx_mini18n-0.4.0/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
           pip install uv
           uv venv
           uv pip install -r requirements-dev.lock
           uv pip install 'sphinx==${{ matrix.sphinx-version }}'
       - name: Run tests
         run: |
           source .venv/bin/activate
+          playwright install firefox
           pytest
   doc-test:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
```

### Comparing `atsphinx_mini18n-0.3.1/.github/workflows/release.yml` & `atsphinx_mini18n-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/Makefile` & `atsphinx_mini18n-0.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/conf.py` & `atsphinx_mini18n-0.4.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/make.bat` & `atsphinx_mini18n-0.4.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/index.po` & `atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/changelogs/index.po` & `atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/changelogs/index.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/configuration.po` & `atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/usage/configuration.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/index.po` & `atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/usage/index.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/setup.po` & `atsphinx_mini18n-0.4.0/doc/_locales/ja/LC_MESSAGES/usage/setup.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/usage/configuration.rst` & `atsphinx_mini18n-0.4.0/doc/usage/configuration.rst`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/doc/usage/setup.rst` & `atsphinx_mini18n-0.4.0/doc/usage/setup.rst`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/__init__.py` & `atsphinx_mini18n-0.4.0/src/atsphinx/mini18n/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from subprocess import PIPE, run
 
 from jinja2 import Template
 from sphinx.application import Sphinx
 from sphinx.builders.dummy import DummyBuilder
 from sphinx.config import Config
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 package_root = Path(__file__).parent.resolve()
 
 
 @dataclass
 class BuildArgs:
     """Parameter class to build other language."""
```

### Comparing `atsphinx_mini18n-0.3.1/tests/test_it.py` & `atsphinx_mini18n-0.4.0/tests/test_it.py`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/.gitignore` & `atsphinx_mini18n-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/LICENSE` & `atsphinx_mini18n-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/README.rst` & `atsphinx_mini18n-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.1/pyproject.toml` & `atsphinx_mini18n-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atsphinx-mini18n"
-version = "0.3.1"
+version = "0.4.0"
 description = "Sphinx builder for i18n site on single deployment"
 authors = [{name = "Kazuya Takei", email = "myself@attakei.net"}]
 license = "Apache-2.0"
 requires-python = ">= 3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Sphinx",
@@ -45,21 +45,27 @@
     "esbonio~=0.16.4",
     "sphinx-tabs~=3.4.5",
     "sphinx-autobuild~=2021.3.14",
     "furo~=2024.1.29",
     "beautifulsoup4~=4.12.3",
     "sphinx-intl~=2.1.0",
     "sphinx-revealjs~=3.0.2",
+    "pytest-playwright~=0.5.0",
 ]
 
 [tool.rye.scripts]
-setup = {chain = ["setup:sync", "setup:pre-commit"]}
+setup = {chain = ["setup:sync", "setup:pre-commit", "setup:playwright"]}
 "setup:sync" = "rye sync --no-lock --all-features"
 "setup:pre-commit" = "pre-commit install"
+"setup:playwright" = "rye run playwright install firefox"
 doc = "make -C doc"
+age = "python tools/run_age.py"
+
+[tool.pytest.ini_options]
+addopts = "--browser firefox"
 
 [tool.ruff.lint]
 select = ["C90", "D", "E", "F", "I", "W"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
```

### Comparing `atsphinx_mini18n-0.3.1/PKG-INFO` & `atsphinx_mini18n-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atsphinx-mini18n
-Version: 0.3.1
+Version: 0.4.0
 Summary: Sphinx builder for i18n site on single deployment
 Project-URL: Repository, https://github.com/atsphinx/mini18n
 Project-URL: Issues, https://github.com/atsphinx/mini18n/issues
 Project-URL: Document, https://atsphinx.github.io/mini18n/
 Author-email: Kazuya Takei <myself@attakei.net>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

