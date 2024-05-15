# Comparing `tmp/sphinx_click-5.2.2.tar.gz` & `tmp/sphinx_click-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_click-5.2.2.tar", last modified: Tue May 14 12:09:01 2024, max compression
+gzip compressed data, was "sphinx_click-6.0.0.tar", last modified: Wed May 15 14:49:10 2024, max compression
```

## Comparing `sphinx_click-5.2.2.tar` & `sphinx_click-6.0.0.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/examples/commandcollections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/examples/commands.rst
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/examples/groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/examples/commandcollections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/commandcollections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/commandcollections/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/examples/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/commands/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.302283 sphinx_click-5.2.2/examples/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/groups/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.294283 sphinx_click-5.2.2/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.302283 sphinx_click-5.2.2/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/add-auto_envvar_prefix-support-a08e68aba792ee26.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/add-mock-modules-support-d4663c3265eeba5e.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/add-show_default-from-context-support-ab4aeffcc513502d.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/drop-python-3-7-support-3d3cab951fc6ae82.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/python-3.11-support-64013e70ae9926f4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/python-3.12-support-f2ed1dc438bd42ee.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/show-typer-arg-help-text-fae802f6878fa100.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.302283 sphinx_click-5.2.2/sphinx_click/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/sphinx_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18813 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/sphinx_click/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/sphinx_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.294283 sphinx_click-5.2.2/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/tests/roots/basics/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/basics/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/basics/greet.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/basics/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/tests/roots/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/commands/greet.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/commands/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/tests/roots/nested-full/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/nested-full/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/nested-full/greet.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/nested-full/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.946174 sphinx_click-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.934174 sphinx_click-6.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.938174 sphinx_click-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-15 14:49:10.946174 sphinx_click-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.938174 sphinx_click-6.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.938174 sphinx_click-6.0.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/examples/commandcollections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/examples/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/examples/groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.938174 sphinx_click-6.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.938174 sphinx_click-6.0.0/examples/commandcollections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/examples/commandcollections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/examples/commandcollections/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.938174 sphinx_click-6.0.0/examples/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/examples/commands/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.938174 sphinx_click-6.0.0/examples/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/examples/groups/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/examples/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.934174 sphinx_click-6.0.0/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.942174 sphinx_click-6.0.0/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/add-auto_envvar_prefix-support-a08e68aba792ee26.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/add-mock-modules-support-d4663c3265eeba5e.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/add-show_default-from-context-support-ab4aeffcc513502d.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/better-string-defaults-3664ae102b044972.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/drop-click-7-cbdaccc6a64029d0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/drop-python-3-7-support-3d3cab951fc6ae82.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/python-3.11-support-64013e70ae9926f4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/python-3.12-support-f2ed1dc438bd42ee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/releasenotes/notes/show-typer-arg-help-text-fae802f6878fa100.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-15 14:49:10.946174 sphinx_click-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.942174 sphinx_click-6.0.0/sphinx_click/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/sphinx_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18888 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/sphinx_click/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.946174 sphinx_click-6.0.0/sphinx_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/sphinx_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/sphinx_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/sphinx_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/sphinx_click.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/sphinx_click.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/sphinx_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 14:49:10.000000 sphinx_click-6.0.0/sphinx_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.942174 sphinx_click-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.934174 sphinx_click-6.0.0/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.942174 sphinx_click-6.0.0/tests/roots/basics/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/basics/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/basics/greet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/basics/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.946174 sphinx_click-6.0.0/tests/roots/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/commands/greet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/commands/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:49:10.946174 sphinx_click-6.0.0/tests/roots/nested-full/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/nested-full/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/nested-full/greet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/roots/nested-full/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27265 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-15 14:49:06.000000 sphinx_click-6.0.0/tox.ini
```

### Comparing `sphinx_click-5.2.2/.editorconfig` & `sphinx_click-6.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/.github/workflows/ci.yaml` & `sphinx_click-6.0.0/.github/workflows/ci.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -31,18 +31,17 @@
         with:
           fetch-depth: 0
       - name: Set up Python ${{ matrix.python }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
-        run: python -m pip install tox
+        run: python -m pip install tox tox-gh-actions
       - name: Run unit tests (via tox)
-        # Run tox using the version of Python in `PATH`
-        run: tox -e py
+        run: tox
   docs:
     name: Build docs
     runs-on: ubuntu-latest
     steps:
       - name: Checkout source code
         uses: actions/checkout@v3
         # We need history for release notes
```

### Comparing `sphinx_click-5.2.2/.pre-commit-config.yaml` & `sphinx_click-6.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/AUTHORS` & `sphinx_click-6.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/ChangeLog` & `sphinx_click-6.0.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 CHANGES
 =======
 
-5.2.2
+6.0.0
 -----
 
+* FIX Format string defaults correctly
+* Remove errant prints
+* Drop support for click 7.x, Sphinx < 5.x
+* readthedocs: Use dirhtml builder
+
+5.2.1
+-----
+
+* docs: Add discrete mocking section
+* actions: Integrate tox-gh-actions
+* Distinguish between click and asyncclick
+* tests: Set maxDiff
+* Skip test with click 7.x
 * FIX If the \`help\` of an argument is \`None\`, don't fail
 * Add defusedxml to tox deps
 * Add defusedxml as test requirement
 * typing: Remove unused ignore
 * Add readthedocs config file
 
 5.2.0
```

### Comparing `sphinx_click-5.2.2/LICENSE` & `sphinx_click-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/PKG-INFO` & `sphinx_click-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-click
-Version: 5.2.2
+Version: 6.0.0
 Summary: Sphinx extension that automatically documents click applications
 Home-page: https://github.com/click-contrib/sphinx-click
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/click-contrib/sphinx-click/issues
 Project-URL: Documentation, https://sphinx-click.readthedocs.io/en/latest
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
-Requires-Dist: sphinx>=2.0
-Requires-Dist: click>=7.0
+Requires-Dist: sphinx>=4.0
+Requires-Dist: click>=8.0
 Requires-Dist: docutils
 
 ============
 sphinx-click
 ============
 
 .. image:: https://github.com/click-contrib/sphinx-click/actions/workflows/ci.yaml/badge.svg
```

### Comparing `sphinx_click-5.2.2/README.rst` & `sphinx_click-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/docs/conf.py` & `sphinx_click-6.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/docs/contributing.rst` & `sphinx_click-6.0.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/docs/examples/commandcollections.rst` & `sphinx_click-6.0.0/docs/examples/commandcollections.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/docs/index.rst` & `sphinx_click-6.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/docs/installation.rst` & `sphinx_click-6.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/docs/usage.rst` & `sphinx_click-6.0.0/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,14 @@
    ``:show-nested:``
      This option is deprecated; use ``nested`` instead.
 
    The generated documentation includes anchors for the generated commands,
    their options and their environment variables using the `Sphinx standard
    domain`_.
 
-*sphinx-click* allows for modules to be mocked out using the same method used by
-`sphinx.ext.autodoc`_. Modules to mock while the documentation is being built
-can be specified using the ``sphinx_click_mock_imports`` config value, if specified.
-Otherwise the value of ``autodoc_mock_imports`` is used, following the behavior
-of ``sphinx.ext.autosummary``. The value of this config option should be a list
-of module names; see `sphinx.ext.autodoc`_ for more information.
-
 .. _cross-referencing:
 
 Cross-referencing
 -----------------
 
 As discussed above, the documentation generated by *sphinx-click* includes
 anchors for the generated commands, their options and their environment
@@ -93,17 +86,30 @@
 
 Programs
   Sphinx currently does not allow you to cross-reference programs. See `Sphinx
   issue #880`__ for more information.
 
   __ https://github.com/sphinx-doc/sphinx/issues/880
 
+.. _mocking:
 
-Docstring processing
---------------------
+Mocking
+-------
+
+*sphinx-click* allows for modules to be mocked out using the same method used by
+`sphinx.ext.autodoc`_. Modules to mock while the documentation is being built
+can be specified using the ``sphinx_click_mock_imports`` config value, if specified.
+Otherwise the value of ``autodoc_mock_imports`` is used, following the behavior
+of ``sphinx.ext.autosummary``. The value of this config option should be a list
+of module names; see `sphinx.ext.autodoc`_ for more information.
+
+.. _events:
+
+Events
+------
 
 *sphinx-click* provides the following additional events:
 
 .. py:function:: sphinx-click-process-description(app, ctx, lines)
 .. py:function:: sphinx-click-process-usage(app, ctx, lines)
 .. py:function:: sphinx-click-process-options(app, ctx, lines)
 .. py:function:: sphinx-click-process-arguments(app, ctx, lines)
@@ -125,15 +131,14 @@
         """Append some text to the "example" command description."""
         if ctx.command.name == "example":
             lines.extend(["Hello, World!", ""])
 
     def setup(app):
         app.connect("sphinx-click-process-description", process_description)
 
-
 Example
 -------
 
 Take the below ``click`` application, which is defined in the ``hello_world``
 module:
 
 .. code-block:: python
@@ -229,15 +234,14 @@
    .. click:: cli:cli
       :prog: cli
       :nested: full
 
 This will render the subcommands of each group in different sections, one for each
 group in ``sources``. An example is provided in :doc:`examples/commandcollections`.
 
-
 Modifying ``sys.path``
 ----------------------
 
 If the application or script you wish to document is not installed (i.e. you
 have not installed it with *pip* or run ``python setup.py``), then you may need
 to modify ``sys.path``. For example, given the following application::
```

### Comparing `sphinx_click-5.2.2/examples/commandcollections/cli.py` & `sphinx_click-6.0.0/examples/commandcollections/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/examples/commands/cli.py` & `sphinx_click-6.0.0/examples/commands/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml` & `sphinx_click-6.0.0/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/setup.cfg` & `sphinx_click-6.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/sphinx_click/ext.py` & `sphinx_click-6.0.0/sphinx_click/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import typing as ty
 import warnings
 
 try:
     import asyncclick as click
 except ImportError:
     import click
+import click.core
 from docutils import nodes
 from docutils.parsers import rst
 from docutils.parsers.rst import directives
 from docutils import statemachine
 from sphinx import application
 from sphinx.util import logging
 from sphinx.util import nodes as sphinx_nodes
@@ -59,15 +60,15 @@
     """Alternative, non-prefixed version of 'get_usage'."""
     formatter = ctx.make_formatter()
     pieces = ctx.command.collect_usage_pieces(ctx)
     formatter.write_usage(ctx.command_path, ' '.join(pieces), prefix='')
     return formatter.getvalue().rstrip('\n')  # type: ignore
 
 
-def _get_help_record(ctx: click.Context, opt: click.Option) -> ty.Tuple[str, str]:
+def _get_help_record(ctx: click.Context, opt: click.core.Option) -> ty.Tuple[str, str]:
     """Re-implementation of click.Opt.get_help_record.
 
     The variant of 'get_help_record' found in Click makes uses of slashes to
     separate multiple opts, and formats option arguments using upper case. This
     is not compatible with Sphinx's 'option' directive, which expects
     comma-separated opts and option arguments surrounded by angle brackets [1].
 
@@ -104,22 +105,22 @@
     else:
         show_default = ctx.show_default
 
     if isinstance(show_default, str):
         # Starting from Click 7.0 show_default can be a string. This is
         # mostly useful when the default is not a constant and
         # documentation thus needs a manually written string.
-        extras.append(':default: ``%s``' % show_default)
-    elif opt.default is not None and show_default:
+        extras.append(':default: ``%r``' % ANSI_ESC_SEQ_RE.sub('', show_default))
+    elif show_default and opt.default is not None:
         extras.append(
             ':default: ``%s``'
             % (
-                ', '.join(str(d) for d in opt.default)
+                ', '.join(repr(d) for d in opt.default)
                 if isinstance(opt.default, (list, tuple))
-                else opt.default,
+                else repr(opt.default),
             )
         )
 
     if isinstance(opt.type, click.Choice):
         extras.append(':options: %s' % ' | '.join(str(x) for x in opt.type.choices))
 
     if extras:
@@ -167,17 +168,17 @@
     yield ''
     for line in _get_usage(ctx).splitlines():
         yield _indent(line)
     yield ''
 
 
 def _format_option(
-    ctx: click.Context, opt: click.Option
+    ctx: click.Context, opt: click.core.Option
 ) -> ty.Generator[str, None, None]:
-    """Format the output for a `click.Option`."""
+    """Format the output for a `click.core.Option`."""
     opt_help = _get_help_record(ctx, opt)
 
     yield '.. option:: {}'.format(opt_help[0])
     if opt_help[1]:
         yield ''
         bar_enabled = False
         for line in statemachine.string2lines(
@@ -195,15 +196,15 @@
 @_process_lines("sphinx-click-process-options")
 def _format_options(ctx: click.Context) -> ty.Generator[str, None, None]:
     """Format all `click.Option` for a `click.Command`."""
     # the hidden attribute is part of click 7.x only hence use of getattr
     params = [
         param
         for param in ctx.command.params
-        if isinstance(param, click.Option) and not getattr(param, 'hidden', False)
+        if isinstance(param, click.core.Option) and not getattr(param, 'hidden', False)
     ]
 
     for param in params:
         for line in _format_option(ctx, param):
             yield line
         yield ''
 
@@ -234,15 +235,15 @@
     for param in params:
         for line in _format_argument(param):
             yield line
         yield ''
 
 
 def _format_envvar(
-    param: ty.Union[click.Option, click.Argument]
+    param: ty.Union[click.core.Option, click.Argument]
 ) -> ty.Generator[str, None, None]:
     """Format the envvars of a `click.Option` or `click.Argument`."""
     yield '.. envvar:: {}'.format(param.envvar)
     yield '   :noindex:'
     yield ''
     if isinstance(param, click.Argument):
         param_ref = param.human_readable_name
```

### Comparing `sphinx_click-5.2.2/sphinx_click.egg-info/PKG-INFO` & `sphinx_click-6.0.0/sphinx_click.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-click
-Version: 5.2.2
+Version: 6.0.0
 Summary: Sphinx extension that automatically documents click applications
 Home-page: https://github.com/click-contrib/sphinx-click
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/click-contrib/sphinx-click/issues
 Project-URL: Documentation, https://sphinx-click.readthedocs.io/en/latest
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
-Requires-Dist: sphinx>=2.0
-Requires-Dist: click>=7.0
+Requires-Dist: sphinx>=4.0
+Requires-Dist: click>=8.0
 Requires-Dist: docutils
 
 ============
 sphinx-click
 ============
 
 .. image:: https://github.com/click-contrib/sphinx-click/actions/workflows/ci.yaml/badge.svg
```

### Comparing `sphinx_click-5.2.2/sphinx_click.egg-info/SOURCES.txt` & `sphinx_click-6.0.0/sphinx_click.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 examples/commandcollections/cli.py
 examples/commands/cli.py
 examples/groups/cli.py
 releasenotes/notes/add-auto_envvar_prefix-support-a08e68aba792ee26.yaml
 releasenotes/notes/add-event-support-e55edb86d86d1082.yaml
 releasenotes/notes/add-mock-modules-support-d4663c3265eeba5e.yaml
 releasenotes/notes/add-show_default-from-context-support-ab4aeffcc513502d.yaml
+releasenotes/notes/better-string-defaults-3664ae102b044972.yaml
+releasenotes/notes/drop-click-7-cbdaccc6a64029d0.yaml
 releasenotes/notes/drop-python-3-7-support-3d3cab951fc6ae82.yaml
 releasenotes/notes/python-3.11-support-64013e70ae9926f4.yaml
 releasenotes/notes/python-3.12-support-f2ed1dc438bd42ee.yaml
 releasenotes/notes/show-typer-arg-help-text-fae802f6878fa100.yaml
 sphinx_click/__init__.py
 sphinx_click/ext.py
 sphinx_click.egg-info/PKG-INFO
```

### Comparing `sphinx_click-5.2.2/tests/conftest.py` & `sphinx_click-6.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/tests/test_extension.py` & `sphinx_click-6.0.0/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.2/tests/test_formatter.py` & `sphinx_click-6.0.0/tests/test_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,16 @@
             multiple=True,
             show_default=True,
         )
         @click.option(
             '--only-show-default',
             show_default="Some default computed at runtime!",
         )
+        @click.option('--string-default', default="abc", show_default=True)
+        @click.option('--empty-string-default', default="", show_default=True)
         def foobar(bar):
             """A sample command."""
             pass
 
         ctx = click.Context(foobar, info_name='foobar')
         output = list(ext._format_command(ctx, nested='short'))
 
@@ -269,23 +271,31 @@
 
         .. option:: --num-param <num_param>
 
             :default: ``42``
 
         .. option:: --param <param>
 
-            :default: ``Something computed at runtime``
+            :default: ``'Something computed at runtime'``
 
         .. option:: --group <group>
 
             :default: ``('foo', 'bar')``
 
         .. option:: --only-show-default <only_show_default>
 
-            :default: ``Some default computed at runtime!``
+            :default: ``'Some default computed at runtime!'``
+
+        .. option:: --string-default <string_default>
+
+            :default: ``'abc'``
+
+        .. option:: --empty-string-default <empty_string_default>
+
+            :default: ``''``
         """
             ).lstrip(),
             '\n'.join(output),
         )
 
     def test_show_default(self):
         """Validate formatting of show_default via context_settings."""
@@ -434,15 +444,15 @@
 
             A sample option with choices
 
             :options: Option1 | Option2
 
         .. option:: --param <param>
 
-            :default: ``Something computed at runtime``
+            :default: ``'Something computed at runtime'``
 
         A sample epilog.
         """
             ).lstrip(),
             '\n'.join(output),
         )
 
@@ -586,14 +596,16 @@
             '\n'.join(output),
         )
 
 
 class GroupTestCase(unittest.TestCase):
     """Validate basic ``click.Group`` instances."""
 
+    maxDiff = None
+
     def test_no_parameters(self):
         """Validate a `click.Group` with no parameters.
 
         This exercises the code paths for a group with *no* arguments, *no*
         options and *no* environment variables.
         """
 
@@ -678,14 +690,16 @@
             '\n'.join(output),
         )
 
 
 class NestedCommandsTestCase(unittest.TestCase):
     """Validate ``click.Command`` instances inside ``click.Group`` instances."""
 
+    maxDiff = None
+
     @staticmethod
     def _get_ctx():
         @click.group()
         def cli():
             """A sample command group."""
             pass
 
@@ -772,14 +786,16 @@
             '\n'.join(output),
         )
 
 
 class CommandFilterTestCase(unittest.TestCase):
     """Validate filtering of commands."""
 
+    maxDiff = None
+
     @staticmethod
     def _get_ctx():
         @click.group()
         def cli():
             """A sample command group."""
 
         @cli.command()
@@ -844,14 +860,16 @@
             '\n'.join(output),
         )
 
 
 class CustomMultiCommandTestCase(unittest.TestCase):
     """Validate ``click.MultiCommand`` instances."""
 
+    maxDiff = None
+
     def test_basics(self):
         """Validate a custom ``click.MultiCommand`` with no parameters.
 
         This exercises the code paths to extract commands correctly from these
         commands.
         """
 
@@ -960,14 +978,16 @@
             '\n'.join(output),
         )
 
 
 class CommandCollectionTestCase(unittest.TestCase):
     """Validate ``click.CommandCollection`` instances."""
 
+    maxDiff = None
+
     def test_basics(self):
         "Validate a ``click.CommandCollection`` with grouped outputs."
 
         @click.group()
         def grp1():
             """A first group."""
             pass
@@ -1031,14 +1051,16 @@
             '\n'.join(output),
         )
 
 
 class AutoEnvvarPrefixTestCase(unittest.TestCase):
     """Validate ``click auto_envvar_prefix``-setup instances."""
 
+    maxDiff = None
+
     def test_basics(self):
         """Validate a click application with ``auto_envvar_prefix`` option enabled."""
 
         @click.command(
             context_settings={"auto_envvar_prefix": "PREFIX"},
         )
         @click.option('--param', help='Help for param')
```

### Comparing `sphinx_click-5.2.2/tox.ini` & `sphinx_click-6.0.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 [tox]
 minversion = 2.0
-envlist = py{38,39}-click{7,8,8-async},py{310,311,312}-click{8,8-async},style,docs
+envlist = py{38,39,310,311,312}-click{8,8-async},style,docs
 
 [testenv]
 setenv =
     PYTHONDEVMODE = 1
     PYTHONWARNINGS = all
     PYTEST_ADDOPTS = {env:PYTEST_ADDOPTS:} --color yes
 deps =
     pytest
     pytest-cov
     coverage
     defusedxml
-    click7: click>=7.0,<8.0
     click8: click>=8.0,<9.0
     click8-async: asyncclick>=8.0,<9.0
     defusedxml
 commands =
     python -m pytest --cov {toxinidir}/sphinx_click {posargs}
 pip_pre =
     pre: true
 
 [testenv:coverage]
 commands =
     {[testenv]commands}
     coverage {posargs:html}
 
 [testenv:style]
+skip_install = true
 deps =
     pre-commit
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:docs]
 commands =
     sphinx-build -Wn -b html -d docs/_build/doctrees docs docs/_build/html
 
+[gh-actions]
+python =
+    3.8: py38
+    3.9: py39
+    3.10: py310
+    3.11: py311
+    3.12: py312
+
 [coverage:run]
 branch = True
```

