# Comparing `tmp/robotframework-robocop-5.0.4.tar.gz` & `tmp/robotframework_robocop-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robocop-5.0.4.tar", last modified: Wed Apr 10 07:26:03 2024, max compression
+gzip compressed data, was "robotframework_robocop-5.1.0.tar", last modified: Wed May 15 16:54:00 2024, max compression
```

## Comparing `robotframework-robocop-5.0.4.tar` & `robotframework_robocop-5.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.192041 robotframework-robocop-5.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-04-10 07:26:03.192041 robotframework-robocop-5.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.184041 robotframework-robocop-5.0.4/robocop/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.184041 robotframework-robocop-5.0.4/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/comments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.188041 robotframework-robocop-5.0.4/robocop/checkers/community_rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/community_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/community_rules/keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    18295 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    32413 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (127)    57337 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    56593 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    33738 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    24002 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.188041 robotframework-robocop-5.0.4/robocop/reports/
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/compare_runs_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/file_stats_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/json_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/return_status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/robocop_version_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/rules_by_id_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/rules_by_severity_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/sarif_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/time_taken_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/timestamp_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.188041 robotframework-robocop-5.0.4/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/variable_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/version_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.192041 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:26:03.192041 robotframework-robocop-5.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:54:00.737082 robotframework_robocop-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-05-15 16:54:00.737082 robotframework_robocop-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:54:00.729082 robotframework_robocop-5.1.0/robocop/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:54:00.733082 robotframework_robocop-5.1.0/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/comments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:54:00.733082 robotframework_robocop-5.1.0/robocop/checkers/community_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/community_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/community_rules/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18295 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32413 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57461 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56611 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34028 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:54:00.733082 robotframework_robocop-5.1.0/robocop/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/compare_runs_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/file_stats_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/json_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/return_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/robocop_version_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/rules_by_id_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/rules_by_severity_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/sarif_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/time_taken_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/reports/timestamp_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:54:00.737082 robotframework_robocop-5.1.0/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/utils/variable_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/utils/version_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:54:00.737082 robotframework_robocop-5.1.0/robotframework_robocop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-05-15 16:54:00.000000 robotframework_robocop-5.1.0/robotframework_robocop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-15 16:54:00.000000 robotframework_robocop-5.1.0/robotframework_robocop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:54:00.000000 robotframework_robocop-5.1.0/robotframework_robocop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 16:54:00.000000 robotframework_robocop-5.1.0/robotframework_robocop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 16:54:00.000000 robotframework_robocop-5.1.0/robotframework_robocop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 16:54:00.000000 robotframework_robocop-5.1.0/robotframework_robocop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:54:00.737082 robotframework_robocop-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-15 16:53:51.000000 robotframework_robocop-5.1.0/setup.py
```

### Comparing `robotframework-robocop-5.0.4/LICENSE` & `robotframework_robocop-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/PKG-INFO` & `robotframework_robocop-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 5.0.4
+Version: 5.1.0
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-5.0.4/README.md` & `robotframework_robocop-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/__init__.py` & `robotframework_robocop-5.1.0/robocop/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/comments.py` & `robotframework_robocop-5.1.0/robocop/checkers/comments.py`

 * *Files 9% similar despite different names*

```diff
@@ -247,49 +247,50 @@
     reports = (
         "ignored-data",
         "bom-encoding-in-file",
     )
     BOM = [BOM_UTF32_BE, BOM_UTF32_LE, BOM_UTF8, BOM_UTF16_LE, BOM_UTF16_BE]
     SECTION_HEADER = "***"
     ROBOCOP_HEADER = "# robocop:"
+    ROBOTIDY_HEADER = "# robotidy:"
     LANGUAGE_HEADER = "language:"
 
     def __init__(self):
         self.is_bom = False
-        self.has_language_header = False
+        self.ignore_empty_lines = False  # ignore empty lines if language header or robocop disabler is present
         super().__init__()
 
     def parse_file(self):
         self.is_bom = False
-        self.has_language_header = False
+        self.ignore_empty_lines = False
         if self.lines is not None:
             for lineno, line in enumerate(self.lines, start=1):
                 if self.check_line(line, lineno):
                     break
         else:
             self.detect_bom(self.source)
             with FileReader(self.source) as file_reader:
                 for lineno, line in enumerate(file_reader.readlines(), start=1):
                     if self.check_line(line, lineno):
                         break
 
     def check_line(self, line, lineno):
         if line.startswith(self.SECTION_HEADER):
             return True
-        if line.startswith(self.ROBOCOP_HEADER):
+        if line.startswith(self.ROBOCOP_HEADER) or line.startswith(self.ROBOTIDY_HEADER):
+            self.ignore_empty_lines = True
             return False
         if lineno == 1:
             if line.lower().startswith(self.LANGUAGE_HEADER):
-                self.has_language_header = True
+                self.ignore_empty_lines = True
                 return False
             if self.is_bom:
                 # if it's BOM encoded file, first line can be ignored
                 return "***" in line
-        if self.has_language_header and not line.strip():
-            # empty lines after language: header can be ignored
+        if self.ignore_empty_lines and not line.strip():
             return False
         self.report("ignored-data", lineno=lineno, col=1, end_col=len(line))
         return True
 
     def detect_bom(self, source):
         with open(source, "rb") as raw_file:
             first_four = raw_file.read(4)
```

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/documentation.py` & `robotframework_robocop-5.1.0/robocop/checkers/documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/duplications.py` & `robotframework_robocop-5.1.0/robocop/checkers/duplications.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/errors.py` & `robotframework_robocop-5.1.0/robocop/checkers/errors.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/lengths.py` & `robotframework_robocop-5.1.0/robocop/checkers/lengths.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/misc.py` & `robotframework_robocop-5.1.0/robocop/checkers/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1222,15 +1222,19 @@
         visit_Return
     ) = (
         visit_SuiteSetup
     ) = (
         visit_SuiteTeardown
     ) = (
         visit_TestSetup
-    ) = visit_TestTeardown = visit_Setup = visit_ResourceImport = visit_VariablesImport = visit_LibraryImport
+    ) = (
+        visit_TestTeardown
+    ) = (
+        visit_Setup
+    ) = visit_ResourceImport = visit_VariablesImport = visit_Tags = visit_Documentation = visit_LibraryImport
 
     def clear_variables_after_loop(self):
         """Remove used variables after loop finishes."""
         for index, scope in enumerate(self.variables):
             self.variables[index] = {name: variable for name, variable in scope.items() if not variable.is_used}
 
     def revisit_variables_used_in_loop(self):
@@ -1265,15 +1269,15 @@
 
     def visit_For(self, node):  # noqa
         if getattr(node.header, "errors", None):
             return node
         self.in_loop = True
         self.used_in_scope = set()
         self.ignore_overwriting = True
-        for token in node.header.get_tokens(Token.ARGUMENT):
+        for token in node.header.get_tokens(Token.ARGUMENT, "OPTION"):  # Token.Option does not exist for RF3 and RF4
             self.find_not_nested_variable(token.value, is_var=False)
         for token in node.header.get_tokens(Token.VARIABLE):
             self.handle_assign_variable(token)
         self.generic_visit(node)
         self.ignore_overwriting = False
         self.in_loop = False
         self.revisit_variables_used_in_loop()
```

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/naming.py` & `robotframework_robocop-5.1.0/robocop/checkers/naming.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,16 +873,17 @@
     def visit_File(self, node):  # noqa
         for section in node.sections:
             if isinstance(section, TestCaseSection):
                 if (ROBOT_VERSION.major < 6 and "task" in section.header.name.lower()) or (
                     ROBOT_VERSION.major >= 6 and section.header.type == Token.TASK_HEADER
                 ):
                     self.task_section = True
-            else:
-                self.task_section = False
+                    break
+        else:
+            self.task_section = False
         super().visit_File(node)
 
     def visit_Setup(self, node):  # noqa
         self.check_setting_name(node.data_tokens[0].value, node)
         self.check_settings_consistency(node.data_tokens[0].value, node)
 
     visit_SuiteSetup = (
```

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/spacing.py` & `robotframework_robocop-5.1.0/robocop/checkers/spacing.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,19 +175,27 @@
         rule_id="1012",
         name="consecutive-empty-lines",
         msg="Too many consecutive empty lines ({{ empty_lines }}/{{ allowed_empty_lines }})",
         severity=RuleSeverity.WARNING,
         docs="""
         Example of rule violation::
 
+            *** Variables ***
+            ${VAR}    value
+            
+            
+            ${VAR2}    value  # previous line will be reported with 2/1 consecutive lines
+            
+            
+            *** Keywords ***
             Keyword
                 Step 1
 
 
-                Step 2
+                Step 2  # previous line will be reported with 2/1 consecutive lines
 
         """,
         added_in_version="1.8.0",
     ),
     "1013": Rule(
         rule_id="1013",
         name="empty-lines-in-statement",
```

### Comparing `robotframework-robocop-5.0.4/robocop/checkers/tags.py` & `robotframework_robocop-5.1.0/robocop/checkers/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/config.py` & `robotframework_robocop-5.1.0/robocop/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             argfile = args.pop(0)
             argfile_path = Path(argfile)
             if argfile_path.is_file():
                 loaded_config_dir = argfile_path.parent
             else:
                 loaded_config_dir = None
             file_args = self.load_argument_file(argfile, config_dir)
-            file_args = self.resolve_arguments_paths(file_args, config_dir)
+            file_args = self.resolve_arguments_paths(file_args, loaded_config_dir)
             parsed_args += self.expand_argument_files(file_args, loaded_config_dir)
         return parsed_args
 
     def resolve_arguments_paths(self, args, root_dir):
         if root_dir is None:
             return args
         prev_option_like = False
```

### Comparing `robotframework-robocop-5.0.4/robocop/exceptions.py` & `robotframework_robocop-5.1.0/robocop/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/files.py` & `robotframework_robocop-5.1.0/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/__init__.py` & `robotframework_robocop-5.1.0/robocop/reports/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import json
 from collections import OrderedDict
 from pathlib import Path
-from typing import Dict
+from typing import Dict, List
 
 import robocop.exceptions
+from robocop import config
 from robocop.checkers import RobocopImporter
 from robocop.utils.misc import get_robocop_cache_directory
 
 ROBOCOP_CACHE_FILE = ".robocop_cache"
 
 
 class Report:
@@ -80,19 +81,32 @@
     return getattr(report, "DEFAULT", False)
 
 
 def is_report_internal(report):
     return getattr(report, "INTERNAL", False)
 
 
+def disable_external_reports_if_none(configured_reports: List[str]) -> List[str]:
+    """
+    If any reports is 'None', disable other reports other than internal reports.
+    """
+    if "None" in configured_reports:
+        if "internal_json_report" in configured_reports:
+            # TODO Improve how internal reports are handled
+            return ["return_status", "internal_json_report"]
+        return ["return_status"]
+    return configured_reports
+
+
 def get_reports(configured_reports):
     """
     Returns dictionary with list of valid, enabled reports (listed in `configured_reports` set of str).
     If `configured_reports` contains `all` then all default reports are enabled.
     """
+    configured_reports = disable_external_reports_if_none(configured_reports)
     compare_runs = "compare_runs" in configured_reports
     reports = load_reports(compare_runs)
     enabled_reports = OrderedDict()
     for report in configured_reports:
         if report == "all":
             for name, report_class in reports.items():
                 if is_report_default(report_class) and name not in enabled_reports:
```

### Comparing `robotframework-robocop-5.0.4/robocop/reports/compare_runs_report.py` & `robotframework_robocop-5.1.0/robocop/reports/compare_runs_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/file_stats_report.py` & `robotframework_robocop-5.1.0/robocop/reports/file_stats_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/json_report.py` & `robotframework_robocop-5.1.0/robocop/reports/json_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/return_status_report.py` & `robotframework_robocop-5.1.0/robocop/reports/return_status_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/robocop_version_report.py` & `robotframework_robocop-5.1.0/robocop/reports/robocop_version_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/rules_by_id_report.py` & `robotframework_robocop-5.1.0/robocop/reports/rules_by_id_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/rules_by_severity_report.py` & `robotframework_robocop-5.1.0/robocop/reports/rules_by_severity_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/sarif_report.py` & `robotframework_robocop-5.1.0/robocop/reports/sarif_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/time_taken_report.py` & `robotframework_robocop-5.1.0/robocop/reports/time_taken_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/reports/timestamp_report.py` & `robotframework_robocop-5.1.0/robocop/reports/timestamp_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/rules.py` & `robotframework_robocop-5.1.0/robocop/rules.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/run.py` & `robotframework_robocop-5.1.0/robocop/run.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/utils/__init__.py` & `robotframework_robocop-5.1.0/robocop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/utils/disablers.py` & `robotframework_robocop-5.1.0/robocop/utils/disablers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,82 @@
 """
 Collection of classes for detecting checker disablers (like # robocop: disable) in robot files
 """
 import re
 from collections import defaultdict
 from copy import deepcopy
+from typing import List, Optional
 
 from robot.api import Token
+from robot.parsing.model.blocks import CommentSection
 
 try:
     from robot.api.parsing import ModelVisitor
 except ImportError:
     from robot.parsing.model.visitor import ModelVisitor
 
 
 class DisablersInFile:  # pylint: disable=too-few-public-methods
     """Container for file disablers"""
 
-    def __init__(self):
+    def __init__(self, blocks: Optional[List] = None):
         self.lastblock = -1
         self.lines = set()
-        self.blocks = []
+        self.blocks = [] if not blocks else blocks
 
     def copy(self):
         """Used by defaultdict to create new instance for every new key in disablers container"""
         return deepcopy(self)
 
 
-class DisablersFinder(ModelVisitor):
-    """Visit and find robocop disablers in Robot Framework file."""
-
+class DisablersVisitor(ModelVisitor):
     ENABLERS = {"enable", "on"}
     DISABLERS = {"disable", "off"}
 
     def __init__(self, model):
         self.file_disabled = False
+        self.file_end = 1
+        self.is_first_comment_section = True
         self.keyword_or_test_section = False
         self.last_name_header_line = 0
-        self.rules_disabled_in_file = set()
         self.disablers_in_scope = []
         self.disabler_pattern = re.compile(r"robocop: ?(?P<disabler>disable|off|enable|on)=?(?P<rules>[\w\-,]*)")
         self.rules = defaultdict(DisablersInFile().copy)
         self.visit(model)
 
-    @property
-    def any_disabler(self):
-        return len(self.rules) != 0
-
     def visit_File(self, node):  # noqa
+        self.file_end = node.end_lineno
         self.generic_visit(node)
-        for rule in self.rules_disabled_in_file:
-            self.rules[rule].blocks.append((1, node.end_lineno))
-        self.file_disabled = self._is_file_disabled(node.end_lineno)
 
     def parse_disablers_in_node(self, node, last_line=None):
         self.disablers_in_scope.append(defaultdict(DisablersInFile().copy))
         self.generic_visit(node)
         for rule_name, rule_disabler in self.disablers_in_scope[-1].items():
-            if rule_disabler.lastblock == 1:  # disabler in first line, never enabled again -> file disabler
-                self.rules_disabled_in_file.add(rule_name)
+            if self.is_first_comment_section:
+                if rule_name == "all":
+                    self.file_disabled = True
+                self.rules[rule_name] = DisablersInFile(blocks=[(1, self.file_end)])
             else:
                 last_line = node.end_lineno if last_line is None else last_line
                 self._end_block(self.disablers_in_scope[-1], rule_name, last_line)
-            self.rules[rule_name].blocks.extend(rule_disabler.blocks)
-            self.rules[rule_name].lines.update(rule_disabler.lines)
+                self.rules[rule_name].blocks.extend(rule_disabler.blocks)
+                self.rules[rule_name].lines.update(rule_disabler.lines)
         self.disablers_in_scope.pop()
 
     def visit_KeywordSection(self, node):  # noqa
         self.keyword_or_test_section = True
         self.parse_disablers_in_node(node)
         self.keyword_or_test_section = False
 
     visit_TestCaseSection = visit_KeywordSection
 
     def visit_Section(self, node):  # noqa
+        self.is_first_comment_section = self.is_first_comment_section and isinstance(node, CommentSection)
         self.parse_disablers_in_node(node)
+        self.is_first_comment_section = False
 
     visit_TestCase = visit_Keyword = visit_Try = visit_For = visit_ForLoop = visit_While = visit_Section
 
     def visit_If(self, node):  # noqa
         last_line = node.body[-1].end_lineno if node.body else None
         self.parse_disablers_in_node(node, last_line)
 
@@ -94,35 +93,14 @@
 
     def visit_Comment(self, node):  # noqa
         for comment in node.get_tokens(Token.COMMENT):
             # Comment is only inline if it is next to test/kw name
             is_inline = comment.lineno == self.last_name_header_line
             self.parse_comment_token(comment, is_inline=is_inline)
 
-    def is_rule_disabled(self, rule_msg):
-        """
-        Check if given `rule_msg` is disabled. All takes precedence, then line disablers, then block disablers.
-        We're checking for both message id and name.
-        """
-        if not self.any_disabler:
-            return False
-        return any(
-            self.is_line_disabled(line, rule)
-            for line in (rule_msg.line, *rule_msg.extended_disablers)
-            for rule in ("all", rule_msg.rule_id, rule_msg.name)
-        )
-
-    def is_line_disabled(self, line, rule):
-        """Helper method for is_rule_disabled that check if given line is in range of any disabled block"""
-        if rule not in self.rules:
-            return False
-        if line in self.rules[rule].lines:
-            return True
-        return any(block[0] <= line <= block[1] for block in self.rules[rule].blocks)
-
     def parse_comment_token(self, token, is_inline):
         if "#" not in token.value:
             return
         if "# noqa" in token.value:
             self._add_inline_disabler("all", token.lineno)
         disabler = self.disabler_pattern.search(token.value)
         if not disabler:
@@ -144,28 +122,14 @@
                 self._end_block(scope, rule, token.lineno)
 
     def get_scope_for_disabler(self, token):
         if token.col_offset == 0 and self.keyword_or_test_section:
             return self.disablers_in_scope[0]
         return self.disablers_in_scope[-1]
 
-    def _is_file_disabled(self, last_line):
-        """
-        The file is disabled if all rules are disabled in every line - we need to iterate every block to see
-        if they are linked from first to last line without breaks.
-        """
-        if "all" not in self.rules:
-            return False
-        prev_end = 1
-        for block in self.rules["all"].blocks:
-            if prev_end != block[0]:
-                return False
-            prev_end = block[1]
-        return prev_end == last_line
-
     def _add_inline_disabler(self, rule, lineno):
         self.rules[rule].lines.add(lineno)
 
     def _start_block(self, scope, rule, lineno):
         if scope[rule].lastblock == -1:
             scope[rule].lastblock = lineno
 
@@ -180,7 +144,46 @@
             scope[rule].blocks.append(block)
 
     def _end_all_blocks(self, scope, lineno):
         for rule in scope:
             if rule == "all":
                 continue  # to avoid recursion
             self._end_block(scope, rule, lineno)
+
+
+class DisablersFinder(ModelVisitor):
+    """Visit and find robocop disablers in Robot Framework file."""
+
+    ENABLERS = {"enable", "on"}
+    DISABLERS = {"disable", "off"}
+
+    def __init__(self, model):
+        self.disabled = DisablersVisitor(model)
+
+    @property
+    def any_disabler(self):
+        return len(self.disabled.rules) != 0
+
+    @property
+    def file_disabled(self):
+        return self.disabled.file_disabled
+
+    def is_rule_disabled(self, rule_msg):
+        """
+        Check if given `rule_msg` is disabled. All takes precedence, then line disablers, then block disablers.
+        We're checking for both message id and name.
+        """
+        if not self.any_disabler:
+            return False
+        return any(
+            self.is_line_disabled(line, rule)
+            for line in (rule_msg.line, *rule_msg.extended_disablers)
+            for rule in ("all", rule_msg.rule_id, rule_msg.name)
+        )
+
+    def is_line_disabled(self, line, rule):
+        """Helper method for is_rule_disabled that check if given line is in range of any disabled block"""
+        if rule not in self.disabled.rules:
+            return False
+        if line in self.disabled.rules[rule].lines:
+            return True
+        return any(block[0] <= line <= block[1] for block in self.disabled.rules[rule].blocks)
```

### Comparing `robotframework-robocop-5.0.4/robocop/utils/file_types.py` & `robotframework_robocop-5.1.0/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/utils/misc.py` & `robotframework_robocop-5.1.0/robocop/utils/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/utils/run_keywords.py` & `robotframework_robocop-5.1.0/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/utils/variable_matcher.py` & `robotframework_robocop-5.1.0/robocop/utils/variable_matcher.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robocop/utils/version_matching.py` & `robotframework_robocop-5.1.0/robocop/utils/version_matching.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/robotframework_robocop.egg-info/PKG-INFO` & `robotframework_robocop-5.1.0/robotframework_robocop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 5.0.4
+Version: 5.1.0
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-5.0.4/robotframework_robocop.egg-info/SOURCES.txt` & `robotframework_robocop-5.1.0/robotframework_robocop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.4/setup.py` & `robotframework_robocop-5.1.0/setup.py`

 * *Files identical despite different names*

