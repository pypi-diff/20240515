# Comparing `tmp/ghastoolkit-0.9.1.tar.gz` & `tmp/ghastoolkit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.9.1.tar", last modified: Fri Oct 20 11:17:55 2023, max compression
+gzip compressed data, was "ghastoolkit-0.9.2.tar", last modified: Fri Oct 27 11:19:35 2023, max compression
```

## Comparing `ghastoolkit-0.9.1.tar` & `ghastoolkit-0.9.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.840005 ghastoolkit-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-20 11:17:55.840005 ghastoolkit-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-20 11:17:55.840005 ghastoolkit-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.832005 ghastoolkit-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.836005 ghastoolkit-0.9.1/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.836005 ghastoolkit-0.9.1/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.836005 ghastoolkit-0.9.1/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/dataextensions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.836005 ghastoolkit-0.9.1/src/ghastoolkit/codeql/packs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/packs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/packs/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/packs/packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/codeql/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.836005 ghastoolkit-0.9.1/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/advisories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (127)    10843 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9630 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.836005 ghastoolkit-0.9.1/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.840005 ghastoolkit-0.9.1/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.840005 ghastoolkit-0.9.1/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/supplychain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.840005 ghastoolkit-0.9.1/src/ghastoolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/src/ghastoolkit/utils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.836005 ghastoolkit-0.9.1/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-20 11:17:55.000000 ghastoolkit-0.9.1/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2023-10-20 11:17:55.000000 ghastoolkit-0.9.1/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 11:17:55.000000 ghastoolkit-0.9.1/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-20 11:17:55.000000 ghastoolkit-0.9.1/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-20 11:17:55.000000 ghastoolkit-0.9.1/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 11:17:55.840005 ghastoolkit-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_codeql_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-10-20 11:17:22.000000 ghastoolkit-0.9.1/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.876816 ghastoolkit-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-27 11:19:35.876816 ghastoolkit-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 11:19:35.876816 ghastoolkit-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.860816 ghastoolkit-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.864816 ghastoolkit-0.9.2/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.864816 ghastoolkit-0.9.2/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8993 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.864816 ghastoolkit-0.9.2/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.868816 ghastoolkit-0.9.2/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.868816 ghastoolkit-0.9.2/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10843 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9630 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.868816 ghastoolkit-0.9.2/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.872816 ghastoolkit-0.9.2/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.872816 ghastoolkit-0.9.2/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/supplychain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.872816 ghastoolkit-0.9.2/src/ghastoolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/src/ghastoolkit/utils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.864816 ghastoolkit-0.9.2/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-27 11:19:35.000000 ghastoolkit-0.9.2/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2023-10-27 11:19:35.000000 ghastoolkit-0.9.2/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 11:19:35.000000 ghastoolkit-0.9.2/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-27 11:19:35.000000 ghastoolkit-0.9.2/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-27 11:19:35.000000 ghastoolkit-0.9.2/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 11:19:35.876816 ghastoolkit-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_codeql_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-10-27 11:19:00.000000 ghastoolkit-0.9.2/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.9.1/LICENSE` & `ghastoolkit-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/PKG-INFO` & `ghastoolkit-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.9.1
+Version: 0.9.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi==2023.7.22
-Requires-Dist: charset-normalizer==3.3.0
+Requires-Dist: charset-normalizer==3.3.1
 Requires-Dist: idna==3.4
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: ratelimit==2.2.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: semantic-version==2.10.0
 Requires-Dist: urllib3==2.0.7
```

### Comparing `ghastoolkit-0.9.1/README.md` & `ghastoolkit-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/pyproject.toml` & `ghastoolkit-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.9.1"
+version = "0.9.2"
 authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "certifi==2023.7.22",
-    "charset-normalizer==3.3.0",
+    "charset-normalizer==3.3.1",
     "idna==3.4",
     "PyYAML==6.0.1",
     "ratelimit==2.2.1",
     "requests==2.31.0",
     "semantic-version==2.10.0",
     "urllib3==2.0.7",
 ]
```

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/__init__.py` & `ghastoolkit-0.9.2/src/ghastoolkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """GitHub Advanced Security Toolkit."""
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/__main__.py` & `ghastoolkit-0.9.2/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/__main__.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/packs/__main__.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/packs/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/packs/pack.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/packs/pack.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/packs/packs.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/packs/packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.9.2/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/advisories.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/enterprise.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/enterprise.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,19 +71,20 @@
         self,
         enterprise: Optional[str] = None,
     ) -> None:
         """Initialise Enterprise."""
         self.enterprise = enterprise or GitHub.enterprise
         self.rest = RestRequest(GitHub.repository)
 
-    def getOrganizations(self) -> List[Organization]:
+    def getOrganizations(self, include_github: bool = False) -> List[Organization]:
         """Get all the Organizations in an enterprise.
 
         You will need to be authenticated as an enterprise owner to use this API.
         """
+        github_orgs = ["github", "actions"]
         organizations = []
         url = Octokit.route("/organizations", GitHub.repository)
         # pagination uses a different API versus the rest of the API
         # https://docs.github.com/en/enterprise-cloud@latest/rest/orgs/orgs#list-organizations
         last_org_id = 1
 
         while True:
@@ -98,14 +99,16 @@
             result = response.json()
 
             if not isinstance(result, list):
                 logger.error("Error getting organizations")
                 return []
 
             for org in result:
+                if not include_github and org.get("login") in github_orgs:
+                    continue
                 organizations.append(Organization(org.get("login"), org.get("id")))
 
             if len(result) < 100:
                 break
             # set last org ID
             last_org_id = organizations[-1].id
```

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/repository.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/repository.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.9.2/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.9.2/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/supplychain/__main__.py` & `ghastoolkit-0.9.2/src/ghastoolkit/supplychain/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.9.2/src/ghastoolkit/supplychain/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.9.2/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.9.2/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.9.2/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit/utils/cli.py` & `ghastoolkit-0.9.2/src/ghastoolkit/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.9.2/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.9.1
+Version: 0.9.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi==2023.7.22
-Requires-Dist: charset-normalizer==3.3.0
+Requires-Dist: charset-normalizer==3.3.1
 Requires-Dist: idna==3.4
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: ratelimit==2.2.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: semantic-version==2.10.0
 Requires-Dist: urllib3==2.0.7
```

### Comparing `ghastoolkit-0.9.1/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.9.2/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_advisories.py` & `ghastoolkit-0.9.2/tests/test_advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_codeql_dataext.py` & `ghastoolkit-0.9.2/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_codeql_packs.py` & `ghastoolkit-0.9.2/tests/test_codeql_packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_codeqldb.py` & `ghastoolkit-0.9.2/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_codescanning.py` & `ghastoolkit-0.9.2/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_default.py` & `ghastoolkit-0.9.2/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_dependencies.py` & `ghastoolkit-0.9.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_depgraph.py` & `ghastoolkit-0.9.2/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_github.py` & `ghastoolkit-0.9.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_licenses.py` & `ghastoolkit-0.9.2/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_octokit.py` & `ghastoolkit-0.9.2/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.9.1/tests/test_secretscanning.py` & `ghastoolkit-0.9.2/tests/test_secretscanning.py`

 * *Files identical despite different names*

