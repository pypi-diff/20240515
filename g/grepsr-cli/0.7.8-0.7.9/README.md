# Comparing `tmp/grepsr_cli-0.7.8.tar.gz` & `tmp/grepsr_cli-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grepsr_cli-0.7.8.tar", last modified: Wed May 15 11:02:33 2024, max compression
+gzip compressed data, was "grepsr_cli-0.7.9.tar", last modified: Wed May 15 11:03:08 2024, max compression
```

## Comparing `grepsr_cli-0.7.8.tar` & `grepsr_cli-0.7.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/.version
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1240 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/CHANGELOG.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/LICENSE.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/MANIFEST.in
--rw-r--r--   0 zznix     (1000) zznix     (1000)     3475 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2943 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/README.md
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/grepsr_cli.egg-info/
--rw-r--r--   0 zznix     (1000) zznix     (1000)     3475 2024-05-15 11:02:33.000000 grepsr_cli-0.7.8/grepsr_cli.egg-info/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1264 2024-05-15 11:02:33.000000 grepsr_cli-0.7.8/grepsr_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2024-05-15 11:02:33.000000 grepsr_cli-0.7.8/grepsr_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2024-05-15 11:02:33.000000 grepsr_cli-0.7.8/grepsr_cli.egg-info/entry_points.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2024-05-15 11:02:33.000000 grepsr_cli-0.7.8/grepsr_cli.egg-info/requires.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2024-05-15 11:02:33.000000 grepsr_cli-0.7.8/grepsr_cli.egg-info/top_level.txt
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.072779 grepsr_cli-0.7.8/grepsrcli/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.072779 grepsr_cli-0.7.8/grepsrcli/controllers/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/controllers/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2023-06-06 11:43:01.000000 grepsr_cli-0.7.8/grepsrcli/controllers/base.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    18775 2024-05-15 10:59:50.000000 grepsr_cli-0.7.8/grepsrcli/controllers/crawler.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/controllers/generate.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/controllers/report.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/grepsrcli/core/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/core/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr_cli-0.7.8/grepsrcli/core/aws_s3.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-06-05 10:31:03.000000 grepsr_cli-0.7.8/grepsrcli/core/config.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/core/exc.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/core/input_prompts.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr_cli-0.7.8/grepsrcli/core/message_log.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/core/report_api.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-09-06 03:15:01.000000 grepsr_cli-0.7.8/grepsrcli/core/sdk_setup.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     5713 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/grepsrcli/core/test_local.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    16013 2024-05-15 10:59:50.000000 grepsr_cli-0.7.8/grepsrcli/core/utils.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/grepsrcli/ext/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/ext/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2169 2024-04-25 17:32:12.000000 grepsr_cli-0.7.8/grepsrcli/main.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/grepsrcli/plugins/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/plugins/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/grepsrcli/templates/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/templates/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/templates/autocomplete.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/templates/autocomplete_zsh.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/templates/composer.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/templates/node_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2084 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/grepsrcli/templates/php_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3458 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/grepsrcli/templates/php_brp_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2087 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/grepsrcli/templates/php_vc_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/grepsrcli/templates/py_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/requirements-dev.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/requirements.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/setup.cfg
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr_cli-0.7.8/setup.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:02:33.076779 grepsr_cli-0.7.8/tests/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      615 2024-05-07 09:17:11.000000 grepsr_cli-0.7.8/tests/test_grepsrcli.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      932 2024-04-25 17:32:12.000000 grepsr_cli-0.7.8/tests/test_unit.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.395675 grepsr_cli-0.7.9/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2024-05-15 11:03:00.000000 grepsr_cli-0.7.9/.version
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1240 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/CHANGELOG.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/LICENSE.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/MANIFEST.in
+-rw-r--r--   0 zznix     (1000) zznix     (1000)     3475 2024-05-15 11:03:08.395675 grepsr_cli-0.7.9/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2943 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/README.md
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.395675 grepsr_cli-0.7.9/grepsr_cli.egg-info/
+-rw-r--r--   0 zznix     (1000) zznix     (1000)     3475 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1264 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/requires.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/top_level.txt
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/controllers/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/controllers/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2023-06-06 11:43:01.000000 grepsr_cli-0.7.9/grepsrcli/controllers/base.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    18775 2024-05-15 10:59:50.000000 grepsr_cli-0.7.9/grepsrcli/controllers/crawler.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/controllers/generate.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/controllers/report.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/core/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/core/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr_cli-0.7.9/grepsrcli/core/aws_s3.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-06-05 10:31:03.000000 grepsr_cli-0.7.9/grepsrcli/core/config.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/core/exc.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/core/input_prompts.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr_cli-0.7.9/grepsrcli/core/message_log.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/core/report_api.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-09-06 03:15:01.000000 grepsr_cli-0.7.9/grepsrcli/core/sdk_setup.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     5713 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/grepsrcli/core/test_local.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    16013 2024-05-15 10:59:50.000000 grepsr_cli-0.7.9/grepsrcli/core/utils.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/ext/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/ext/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2169 2024-04-25 17:32:12.000000 grepsr_cli-0.7.9/grepsrcli/main.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/plugins/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/plugins/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/templates/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/autocomplete.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/autocomplete_zsh.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/composer.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/node_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2084 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/grepsrcli/templates/php_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3458 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/grepsrcli/templates/php_brp_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2087 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/grepsrcli/templates/php_vc_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/py_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/requirements-dev.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/requirements.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2024-05-15 11:03:08.395675 grepsr_cli-0.7.9/setup.cfg
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/setup.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/tests/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      615 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/tests/test_grepsrcli.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      932 2024-04-25 17:32:12.000000 grepsr_cli-0.7.9/tests/test_unit.py
```

### Comparing `grepsr_cli-0.7.8/CHANGELOG.md` & `grepsr_cli-0.7.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/PKG-INFO` & `grepsr_cli-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `grepsr_cli-0.7.8/README.md` & `grepsr_cli-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsr_cli.egg-info/PKG-INFO` & `grepsr_cli-0.7.9/grepsr_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `grepsr_cli-0.7.8/grepsr_cli.egg-info/SOURCES.txt` & `grepsr_cli-0.7.9/grepsr_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/controllers/base.py` & `grepsr_cli-0.7.9/grepsrcli/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/controllers/crawler.py` & `grepsr_cli-0.7.9/grepsrcli/controllers/crawler.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/controllers/generate.py` & `grepsr_cli-0.7.9/grepsrcli/controllers/generate.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/controllers/report.py` & `grepsr_cli-0.7.9/grepsrcli/controllers/report.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/core/aws_s3.py` & `grepsr_cli-0.7.9/grepsrcli/core/aws_s3.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/core/config.py` & `grepsr_cli-0.7.9/grepsrcli/core/config.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/core/message_log.py` & `grepsr_cli-0.7.9/grepsrcli/core/message_log.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/core/report_api.py` & `grepsr_cli-0.7.9/grepsrcli/core/report_api.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/core/sdk_setup.py` & `grepsr_cli-0.7.9/grepsrcli/core/sdk_setup.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/core/test_local.py` & `grepsr_cli-0.7.9/grepsrcli/core/test_local.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/core/utils.py` & `grepsr_cli-0.7.9/grepsrcli/core/utils.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/main.py` & `grepsr_cli-0.7.9/grepsrcli/main.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/templates/autocomplete_zsh.jinja2` & `grepsr_cli-0.7.9/grepsrcli/templates/autocomplete_zsh.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/templates/node_boilerplate.jinja2` & `grepsr_cli-0.7.9/grepsrcli/templates/node_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/templates/php_boilerplate.jinja2` & `grepsr_cli-0.7.9/grepsrcli/templates/php_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/templates/php_brp_boilerplate.jinja2` & `grepsr_cli-0.7.9/grepsrcli/templates/php_brp_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/templates/php_vc_boilerplate.jinja2` & `grepsr_cli-0.7.9/grepsrcli/templates/php_vc_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/grepsrcli/templates/py_boilerplate.jinja2` & `grepsr_cli-0.7.9/grepsrcli/templates/py_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/setup.py` & `grepsr_cli-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/tests/test_grepsrcli.py` & `grepsr_cli-0.7.9/tests/test_grepsrcli.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.8/tests/test_unit.py` & `grepsr_cli-0.7.9/tests/test_unit.py`

 * *Files identical despite different names*

