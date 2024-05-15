# Comparing `tmp/rayvision_houdini-1.5.0.tar.gz` & `tmp/rayvision_houdini-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rayvision_houdini-1.5.0.tar", last modified: Mon Dec 25 11:40:56 2023, max compression
+gzip compressed data, was "dist/rayvision_houdini-1.5.1.tar", last modified: Wed May 15 08:29:30 2024, max compression
```

## Comparing `rayvision_houdini-1.5.0.tar` & `rayvision_houdini-1.5.1.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      252 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      187 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1121 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-09-06 06:16:59.000000 rayvision_houdini-1.5.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      472 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      664 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       44 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/dev_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5357 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/docs/rayvision_houdini/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/docs/rayvision_houdini/core/
--rw-rw-rw-   0 root         (0) root         (0)      141 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/rayvision_houdini/core/cg.rst
--rw-rw-rw-   0 root         (0) root         (0)      296 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/rayvision_houdini/core/constants.rst
--rw-rw-rw-   0 root         (0) root         (0)     5108 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/rayvision_houdini/first_look.rst
--rw-rw-rw-   0 root         (0) root         (0)      854 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/rayvision_houdini/installation_guide.rst
--rw-rw-rw-   0 root         (0) root         (0)      128 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/docs/rayvision_houdini/modules.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/help/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/help/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/help/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/help/doc/docs/
--rw-rw-rw-   0 root         (0) root         (0)     8755 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/help/doc/docs/Configuration Documentation--Maya.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/help/doc/docs_zh/
--rw-rw-rw-   0 root         (0) root         (0)     8250 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/help/doc/docs_zh/配置文件文档之Maya.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/help/examples/
--rw-rw-rw-   0 root         (0) root         (0)     3338 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/help/examples/houdini_demo.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/help/examples/only_analyze.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/help/scenes/
--rw-rw-rw-   0 root         (0) root         (0)   277555 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/help/scenes/sphere.hip
--rw-rw-rw-   0 root         (0) root         (0)      452 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/init_pycharm_setup.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/rayvision_houdini/
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-09-06 06:16:59.000000 rayvision_houdini-1.5.0/rayvision_houdini/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15635 2023-12-25 06:33:16.000000 rayvision_houdini-1.5.0/rayvision_houdini/analyze_houdini.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/rayvision_houdini/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/
--rw-rw-rw-   0 root         (0) root         (0)      498 2022-09-06 06:09:27.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py27/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py27/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   612864 2023-05-19 09:43:05.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py27/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  4217104 2023-05-10 11:23:49.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py27/hanalyse.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py37/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py37/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   561664 2023-05-19 09:43:05.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py37/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  5355088 2023-05-10 11:23:49.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py37/hanalyse.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py39/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py39/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   564224 2023-05-19 09:43:05.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py39/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  5511584 2023-05-10 11:23:50.000000 rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py39/hanalyse.so
--rw-rw-rw-   0 root         (0) root         (0)      787 2022-09-06 04:23:37.000000 rayvision_houdini-1.5.0/rayvision_houdini/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/rayvision_houdini/tests/
--rw-rw-rw-   0 root         (0) root         (0)       39 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.0/rayvision_houdini/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2022-09-06 03:45:31.000000 rayvision_houdini-1.5.0/rayvision_houdini/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      849 2023-05-19 09:50:53.000000 rayvision_houdini-1.5.0/rayvision_houdini/tests/test_analyze_houdini.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/rayvision_houdini.egg-info/
--rw-r--r--   0 root         (0) root         (0)      472 2023-12-25 11:40:55.000000 rayvision_houdini-1.5.0/rayvision_houdini.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1946 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/rayvision_houdini.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-25 11:40:55.000000 rayvision_houdini-1.5.0/rayvision_houdini.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-12-25 11:40:55.000000 rayvision_houdini-1.5.0/rayvision_houdini.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-12-25 11:40:55.000000 rayvision_houdini-1.5.0/rayvision_houdini.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-28 04:38:46.000000 rayvision_houdini-1.5.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-12-25 11:40:56.000000 rayvision_houdini-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-12-25 10:48:05.000000 rayvision_houdini-1.5.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3073 2023-05-05 06:19:19.000000 rayvision_houdini-1.5.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      187 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      259 2022-09-06 06:16:59.000000 rayvision_houdini-1.5.1/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      664 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       44 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/dev_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5357 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/docs/rayvision_houdini/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/docs/rayvision_houdini/core/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/rayvision_houdini/core/cg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      296 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/rayvision_houdini/core/constants.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/rayvision_houdini/first_look.rst
+-rw-rw-rw-   0 root         (0) root         (0)      854 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/rayvision_houdini/installation_guide.rst
+-rw-rw-rw-   0 root         (0) root         (0)      128 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/docs/rayvision_houdini/modules.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/help/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/help/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/help/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/help/doc/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     8755 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/help/doc/docs/Configuration Documentation--Maya.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/help/doc/docs_zh/
+-rw-rw-rw-   0 root         (0) root         (0)     8250 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/help/doc/docs_zh/配置文件文档之Maya.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/help/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/help/examples/houdini_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/help/examples/only_analyze.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/help/scenes/
+-rw-rw-rw-   0 root         (0) root         (0)   277555 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/help/scenes/sphere.hip
+-rw-rw-rw-   0 root         (0) root         (0)      452 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/init_pycharm_setup.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini/
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-09-06 06:16:59.000000 rayvision_houdini-1.5.1/rayvision_houdini/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15635 2023-12-25 06:33:16.000000 rayvision_houdini-1.5.1/rayvision_houdini/analyze_houdini.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/rayvision_houdini/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/
+-rw-rw-rw-   0 root         (0) root         (0)      498 2022-09-06 06:09:27.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py27/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py27/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   614400 2024-05-15 03:09:17.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py27/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  4217104 2023-05-10 11:23:49.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py27/hanalyse.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py310/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-15 03:09:17.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py310/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   705536 2024-05-15 03:09:17.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py310/hanalyse.pyd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py37/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py37/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   643072 2024-05-15 03:09:17.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py37/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  5355088 2023-05-10 11:23:49.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py37/hanalyse.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py39/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py39/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   645120 2024-05-15 03:09:17.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py39/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  5511584 2023-05-10 11:23:50.000000 rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py39/hanalyse.so
+-rw-rw-rw-   0 root         (0) root         (0)      787 2022-09-06 04:23:37.000000 rayvision_houdini-1.5.1/rayvision_houdini/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2021-11-25 02:46:16.000000 rayvision_houdini-1.5.1/rayvision_houdini/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2022-09-06 03:45:31.000000 rayvision_houdini-1.5.1/rayvision_houdini/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2023-05-19 09:50:53.000000 rayvision_houdini-1.5.1/rayvision_houdini/tests/test_analyze_houdini.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2411 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/rayvision_houdini.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-28 04:38:46.000000 rayvision_houdini-1.5.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-15 08:29:30.000000 rayvision_houdini-1.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-12-25 10:48:05.000000 rayvision_houdini-1.5.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3059 2024-05-15 06:45:02.000000 rayvision_houdini-1.5.1/tox.ini
```

### Comparing `rayvision_houdini-1.5.0/.pre-commit-config.yaml` & `rayvision_houdini-1.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/README.md` & `rayvision_houdini-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/docs/Makefile` & `rayvision_houdini-1.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/docs/conf.py` & `rayvision_houdini-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/docs/index.rst` & `rayvision_houdini-1.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/docs/make.bat` & `rayvision_houdini-1.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/docs/rayvision_houdini/first_look.rst` & `rayvision_houdini-1.5.1/docs/rayvision_houdini/first_look.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/docs/rayvision_houdini/installation_guide.rst` & `rayvision_houdini-1.5.1/docs/rayvision_houdini/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/help/doc/docs/Configuration Documentation--Maya.md` & `rayvision_houdini-1.5.1/help/doc/docs/Configuration Documentation--Maya.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/help/doc/docs_zh/配置文件文档之Maya.md` & `rayvision_houdini-1.5.1/help/doc/docs_zh/配置文件文档之Maya.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/help/examples/houdini_demo.py` & `rayvision_houdini-1.5.1/help/examples/houdini_demo.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/help/scenes/sphere.hip` & `rayvision_houdini-1.5.1/help/scenes/sphere.hip`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/rayvision_houdini/analyze_houdini.py` & `rayvision_houdini-1.5.1/rayvision_houdini/analyze_houdini.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py27/hanalyse.so` & `rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py27/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py37/hanalyse.so` & `rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py37/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/rayvision_houdini/hanalyse/py39/hanalyse.so` & `rayvision_houdini-1.5.1/rayvision_houdini/hanalyse/py39/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/rayvision_houdini/run.py` & `rayvision_houdini-1.5.1/rayvision_houdini/run.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/rayvision_houdini/tests/conftest.py` & `rayvision_houdini-1.5.1/rayvision_houdini/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/rayvision_houdini/tests/test_analyze_houdini.py` & `rayvision_houdini-1.5.1/rayvision_houdini/tests/test_analyze_houdini.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/rayvision_houdini.egg-info/SOURCES.txt` & `rayvision_houdini-1.5.1/rayvision_houdini.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,24 @@
 ./help/__init__.py
 ./rayvision_houdini/__init__.py
 ./rayvision_houdini/analyze_houdini.py
 ./rayvision_houdini/constants.py
 ./rayvision_houdini/run.py
 ./rayvision_houdini/hanalyse/__init__.py
 ./rayvision_houdini/hanalyse/py27/__init__.py
+./rayvision_houdini/hanalyse/py27/hanalyse.pyd
+./rayvision_houdini/hanalyse/py27/hanalyse.so
+./rayvision_houdini/hanalyse/py310/__init__.py
+./rayvision_houdini/hanalyse/py310/hanalyse.pyd
 ./rayvision_houdini/hanalyse/py37/__init__.py
+./rayvision_houdini/hanalyse/py37/hanalyse.pyd
+./rayvision_houdini/hanalyse/py37/hanalyse.so
 ./rayvision_houdini/hanalyse/py39/__init__.py
+./rayvision_houdini/hanalyse/py39/hanalyse.pyd
+./rayvision_houdini/hanalyse/py39/hanalyse.so
 ./rayvision_houdini/tests/__init__.py
 ./rayvision_houdini/tests/conftest.py
 ./rayvision_houdini/tests/test_analyze_houdini.py
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
@@ -45,14 +53,16 @@
 rayvision_houdini.egg-info/dependency_links.txt
 rayvision_houdini.egg-info/requires.txt
 rayvision_houdini.egg-info/top_level.txt
 rayvision_houdini/hanalyse/__init__.py
 rayvision_houdini/hanalyse/py27/__init__.py
 rayvision_houdini/hanalyse/py27/hanalyse.pyd
 rayvision_houdini/hanalyse/py27/hanalyse.so
+rayvision_houdini/hanalyse/py310/__init__.py
+rayvision_houdini/hanalyse/py310/hanalyse.pyd
 rayvision_houdini/hanalyse/py37/__init__.py
 rayvision_houdini/hanalyse/py37/hanalyse.pyd
 rayvision_houdini/hanalyse/py37/hanalyse.so
 rayvision_houdini/hanalyse/py39/__init__.py
 rayvision_houdini/hanalyse/py39/hanalyse.pyd
 rayvision_houdini/hanalyse/py39/hanalyse.so
 rayvision_houdini/tests/__init__.py
```

### Comparing `rayvision_houdini-1.5.0/setup.py` & `rayvision_houdini-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.5.0/tox.ini` & `rayvision_houdini-1.5.1/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,19 @@
   PYTHONHASHSEED=0
   PYCURL_SSL_LIBRARY=openssl
 whitelist_externals =
   bash
   pylint
   flake8
   ray-gitlab-ci
+allowlist_externals =
+  bash
+  pylint
+  flake8
+  ray-gitlab-ci
 install_command = {env:RAYVISION_PIP_COMMAND}
 depends =
   {py27,py36}: clean
   report: py27,py36
 
 # Support env list.
 [testenv:clean]
@@ -57,25 +62,23 @@
 [testenv:test]
 description = Run pytest.
 deps =
     -r{toxinidir}/requirements.txt
     pytest
     pytest-cov
     pytest-mock
-    sqlit
-
 commands =
   pytest --cov={env:CI_PROJECT_NAME} --cov-append {posargs}
 
 [testenv:deploy]
 deps =
     twine
 commands =
     pip install requests==2.28.2
-    python setup.py bdist_wheel register -r rayvision_pip upload -r rayvision_pip
+    python setup.py bdist_wheel
     python setup.py sdist
     twine upload --repository pypi dist/*
 
 [testenv:pre-commit]
 skip_install = true
 deps =  pre-commit
 commands =
@@ -88,23 +91,22 @@
 exclude = .venv,.tox,dist,doc,*egg,build,*.pyc
 show_source = true
 enable-extensions = G
 application-import-names = {env:CI_PROJECT_NAME}.
 format = pylint
 max-line-length = 79
 toutput-format = text
-files_to_ignore = HfsSql.py,analyze.py
+ignore = I100,I202,W503
 
 
 [pylint]
 accepted-code-rate = 9
 max-line-length = 80
 
 
-
 [coverage:report]
 include =
   {env:CI_PROJECT_NAME}/*
 skip_covered = True
 show_missing = True
 precision = 2
 exclude_lines =
```

