# Comparing `tmp/wild_code-0.4.4.tar.gz` & `tmp/wild_code-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_code-0.4.4.tar", last modified: Tue May 14 20:08:52 2024, max compression
+gzip compressed data, was "wild_code-0.4.5.tar", last modified: Wed May 15 19:36:56 2024, max compression
```

## Comparing `wild_code-0.4.4.tar` & `wild_code-0.4.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:12.539648 wild_code-0.4.4/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-14 19:57:47.000000 wild_code-0.4.4/.dockerignore
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.730029 wild_code-0.4.4/.github/
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.729630 wild_code-0.4.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-14 19:57:47.000000 wild_code-0.4.4/.github/ISSUE_TEMPLATE/buggy_contract.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-14 19:57:47.000000 wild_code-0.4.4/.github/ISSUE_TEMPLATE/buggy_test.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-14 19:57:47.000000 wild_code-0.4.4/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-14 19:57:47.000000 wild_code-0.4.4/.github/ISSUE_TEMPLATE/model_eval_request.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-14 19:57:47.000000 wild_code-0.4.4/.gitignore
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-14 19:57:47.000000 wild_code-0.4.4/.pre-commit-config.yaml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-14 19:57:47.000000 wild_code-0.4.4/CITATION.cff
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      757 2024-05-14 19:57:47.000000 wild_code-0.4.4/Dockerfile
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-14 19:57:47.000000 wild_code-0.4.4/LICENSE
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-14 19:57:47.000000 wild_code-0.4.4/MANIFEST.in
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10932 2024-05-14 20:06:12.534059 wild_code-0.4.4/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9819 2024-05-14 19:57:47.000000 wild_code-0.4.4/README.md
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-14 19:57:47.000000 wild_code-0.4.4/pyproject.toml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-14 20:05:59.000000 wild_code-0.4.4/release.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      156 2024-05-14 19:57:47.000000 wild_code-0.4.4/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1348 2024-05-14 19:57:47.000000 wild_code-0.4.4/run.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1237 2024-05-14 20:06:12.551049 wild_code-0.4.4/setup.cfg
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.735305 wild_code-0.4.4/tests/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-14 19:57:47.000000 wild_code-0.4.4/tests/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-14 19:57:47.000000 wild_code-0.4.4/tests/test_legacy_sanitizer.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-14 19:57:47.000000 wild_code-0.4.4/tests/test_treesitter_sanitizer.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:12.516879 wild_code-0.4.4/wild_code.egg-info/
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10932 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/SOURCES.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/dependency_links.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/entry_points.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/requires.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/top_level.txt
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.772721 wild_code-0.4.4/wildcode/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-14 20:06:11.000000 wild_code-0.4.4/wildcode/_version.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.757082 wild_code-0.4.4/wildcode/data/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/data/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/data/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1612 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/data/wildcodebench.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.764430 wild_code-0.4.4/wildcode/eval/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7216 2024-05-14 19:58:38.000000 wild_code-0.4.4/wildcode/eval/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/eval/_special_oracle.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7110 2024-05-14 19:59:36.000000 wild_code-0.4.4/wildcode/eval/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8190 2024-05-14 20:01:25.000000 wild_code-0.4.4/wildcode/evaluate.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.782491 wild_code-0.4.4/wildcode/gen/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/gen/__init__.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.781970 wild_code-0.4.4/wildcode/gen/util/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2202 2024-05-14 20:00:46.000000 wild_code-0.4.4/wildcode/gen/util/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/gen/util/anthropic_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/gen/util/openai_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5558 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/generate.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/inspect.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/lecacy_sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14089 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/model.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7991 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/syncheck.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.991880 wild_code-0.4.5/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-15 18:58:13.000000 wild_code-0.4.5/.dockerignore
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.156472 wild_code-0.4.5/.github/
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.156041 wild_code-0.4.5/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-15 15:44:35.000000 wild_code-0.4.5/.github/ISSUE_TEMPLATE/buggy_contract.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-15 15:44:35.000000 wild_code-0.4.5/.github/ISSUE_TEMPLATE/buggy_test.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-15 15:44:35.000000 wild_code-0.4.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-15 15:44:35.000000 wild_code-0.4.5/.github/ISSUE_TEMPLATE/model_eval_request.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-15 15:44:35.000000 wild_code-0.4.5/.gitignore
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-15 15:44:35.000000 wild_code-0.4.5/.pre-commit-config.yaml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-15 15:44:35.000000 wild_code-0.4.5/CITATION.cff
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      764 2024-05-15 18:38:24.000000 wild_code-0.4.5/Dockerfile
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-15 15:44:35.000000 wild_code-0.4.5/LICENSE
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-15 15:44:35.000000 wild_code-0.4.5/MANIFEST.in
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10853 2024-05-15 19:34:15.987412 wild_code-0.4.5/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9819 2024-05-15 15:44:35.000000 wild_code-0.4.5/README.md
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-15 15:44:35.000000 wild_code-0.4.5/pyproject.toml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-15 15:44:35.000000 wild_code-0.4.5/release.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      156 2024-05-15 15:44:35.000000 wild_code-0.4.5/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      777 2024-05-15 18:34:15.000000 wild_code-0.4.5/run.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1210 2024-05-15 19:34:16.007014 wild_code-0.4.5/setup.cfg
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.160993 wild_code-0.4.5/tests/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-15 15:44:35.000000 wild_code-0.4.5/tests/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-15 15:44:35.000000 wild_code-0.4.5/tests/test_legacy_sanitizer.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-15 15:44:35.000000 wild_code-0.4.5/tests/test_treesitter_sanitizer.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.972909 wild_code-0.4.5/wild_code.egg-info/
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10853 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-15 19:34:15.000000 wild_code-0.4.5/wild_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/entry_points.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/requires.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/top_level.txt
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.188645 wild_code-0.4.5/wildcode/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-15 19:34:14.000000 wild_code-0.4.5/wildcode/_version.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.179066 wild_code-0.4.5/wildcode/data/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/data/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/data/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1612 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/data/wildcodebench.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.184183 wild_code-0.4.5/wildcode/eval/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7216 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/eval/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/eval/_special_oracle.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7110 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/eval/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8190 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/evaluate.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.197276 wild_code-0.4.5/wildcode/gen/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/gen/__init__.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.196851 wild_code-0.4.5/wildcode/gen/util/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2202 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/gen/util/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/gen/util/anthropic_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/gen/util/openai_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5592 2024-05-15 18:12:27.000000 wild_code-0.4.5/wildcode/generate.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/inspect.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/lecacy_sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    16130 2024-05-15 18:32:02.000000 wild_code-0.4.5/wildcode/model.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7991 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/syncheck.py
```

### Comparing `wild_code-0.4.4/.dockerignore` & `wild_code-0.4.5/.dockerignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/.github/ISSUE_TEMPLATE/buggy_contract.yml` & `wild_code-0.4.5/.github/ISSUE_TEMPLATE/buggy_contract.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/.github/ISSUE_TEMPLATE/buggy_test.yml` & `wild_code-0.4.5/.github/ISSUE_TEMPLATE/buggy_test.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/.github/ISSUE_TEMPLATE/model_eval_request.yml` & `wild_code-0.4.5/.github/ISSUE_TEMPLATE/model_eval_request.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/.gitignore` & `wild_code-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/Dockerfile` & `wild_code-0.4.5/Dockerfile`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Better use newer Python as generated code can use new features
 FROM python:3.10-slim
 
 # install git, g++ and python3-tk
-RUN apt-get update && apt-get install -y git g++ python3-tk zip unzip procps
+RUN apt-get update && apt-get install -y git g++ python3-tk zip unzip procps r-base
 
 # upgrade to latest pip
 RUN pip install --upgrade pip
 
 # Add a new user "wildcodeuser"
 RUN adduser --disabled-password --gecos "" wildcodeuser
```

### Comparing `wild_code-0.4.4/LICENSE` & `wild_code-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/PKG-INFO` & `wild_code-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.4.4
+Version: 0.4.5
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,25 +16,23 @@
 Requires-Dist: multipledispatch>=0.6.0
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: numpy>=1.19.5
 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0
 Requires-Dist: fire>=0.6.0
 Requires-Dist: openai>=1.11.1
-Requires-Dist: openai
-Requires-Dist: rich
+Requires-Dist: rich>=12.3.0
+Requires-Dist: tree_sitter_languages>=1.10.2
+Requires-Dist: tree-sitter==0.21.3
 Requires-Dist: accelerate
 Requires-Dist: vllm
 Requires-Dist: anthropic
 Requires-Dist: mistralai
 Requires-Dist: stop-sequencer
-Provides-Extra: perf
-Requires-Dist: Pympler>=1.0.1; extra == "perf"
-Requires-Dist: rich>=12.3.0; extra == "perf"
-Requires-Dist: tree_sitter_languages>=1.10.2; extra == "perf"
+Requires-Dist: Pympler>=1.0.1
 
 # 🌳WildCodeBench
 
 > [!WARNING] 
 > The project is under active development. Please check back later for more updates.
 
 > [!WARNING]
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.4.4 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.4.5 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
 appdirs>=1.4.4 Requires-Dist: numpy>=1.19.5 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0 Requires-Dist: fire>=0.6.0 Requires-Dist:
-openai>=1.11.1 Requires-Dist: openai Requires-Dist: rich Requires-Dist:
+openai>=1.11.1 Requires-Dist: rich>=12.3.0 Requires-Dist:
+tree_sitter_languages>=1.10.2 Requires-Dist: tree-sitter==0.21.3 Requires-Dist:
 accelerate Requires-Dist: vllm Requires-Dist: anthropic Requires-Dist:
-mistralai Requires-Dist: stop-sequencer Provides-Extra: perf Requires-Dist:
-Pympler>=1.0.1; extra == "perf" Requires-Dist: rich>=12.3.0; extra == "perf"
-Requires-Dist: tree_sitter_languages>=1.10.2; extra == "perf" #
+mistralai Requires-Dist: stop-sequencer Requires-Dist: Pympler>=1.0.1 #
 ð³WildCodeBench > [!WARNING] > The project is under active development.
 Please check back later for more updates. > [!WARNING] > Please use WildCode
 with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus),
 WildCode has a much less constrained execution environment to support tasks
 with diverse library dependencies. This may lead to security risks. We
 recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/
 ) to run the evaluation. > [!WARNING] > WildCode framework currently only
```

### Comparing `wild_code-0.4.4/README.md` & `wild_code-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/release.sh` & `wild_code-0.4.5/release.sh`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/setup.cfg` & `wild_code-0.4.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -22,33 +22,30 @@
 	multipledispatch>=0.6.0
 	appdirs>=1.4.4
 	numpy>=1.19.5
 	tqdm>=4.56.0
 	termcolor>=2.0.0
 	fire>=0.6.0
 	openai>=1.11.1
-	openai
-	rich
+	rich>=12.3.0
+	tree_sitter_languages>=1.10.2
+	tree-sitter==0.21.3
 	accelerate
 	vllm
 	anthropic
 	mistralai
 	stop-sequencer
+	Pympler>=1.0.1
 
 [options.entry_points]
 console_scripts = 
 	wildcode.evaluate = wildcode.evaluate:main
 	wildcode.sanitize = wildcode.sanitize:main
 	wildcode.syncheck = wildcode.syncheck:main
 	wildcode.legacy_sanitize = wildcode.legacy_sanitize:main
 	wildcode.generate = wildcode.generate:main
 	wildcode.inspect = wildcode.inspect:main
 
-[options.extras_require]
-perf = Pympler>=1.0.1
-	rich>=12.3.0
-	tree_sitter_languages >= 1.10.2
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wild_code-0.4.4/tests/test_legacy_sanitizer.py` & `wild_code-0.4.5/tests/test_legacy_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/tests/test_treesitter_sanitizer.py` & `wild_code-0.4.5/tests/test_treesitter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wild_code.egg-info/PKG-INFO` & `wild_code-0.4.5/wild_code.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.4.4
+Version: 0.4.5
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,25 +16,23 @@
 Requires-Dist: multipledispatch>=0.6.0
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: numpy>=1.19.5
 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0
 Requires-Dist: fire>=0.6.0
 Requires-Dist: openai>=1.11.1
-Requires-Dist: openai
-Requires-Dist: rich
+Requires-Dist: rich>=12.3.0
+Requires-Dist: tree_sitter_languages>=1.10.2
+Requires-Dist: tree-sitter==0.21.3
 Requires-Dist: accelerate
 Requires-Dist: vllm
 Requires-Dist: anthropic
 Requires-Dist: mistralai
 Requires-Dist: stop-sequencer
-Provides-Extra: perf
-Requires-Dist: Pympler>=1.0.1; extra == "perf"
-Requires-Dist: rich>=12.3.0; extra == "perf"
-Requires-Dist: tree_sitter_languages>=1.10.2; extra == "perf"
+Requires-Dist: Pympler>=1.0.1
 
 # 🌳WildCodeBench
 
 > [!WARNING] 
 > The project is under active development. Please check back later for more updates.
 
 > [!WARNING]
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.4.4 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.4.5 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
 appdirs>=1.4.4 Requires-Dist: numpy>=1.19.5 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0 Requires-Dist: fire>=0.6.0 Requires-Dist:
-openai>=1.11.1 Requires-Dist: openai Requires-Dist: rich Requires-Dist:
+openai>=1.11.1 Requires-Dist: rich>=12.3.0 Requires-Dist:
+tree_sitter_languages>=1.10.2 Requires-Dist: tree-sitter==0.21.3 Requires-Dist:
 accelerate Requires-Dist: vllm Requires-Dist: anthropic Requires-Dist:
-mistralai Requires-Dist: stop-sequencer Provides-Extra: perf Requires-Dist:
-Pympler>=1.0.1; extra == "perf" Requires-Dist: rich>=12.3.0; extra == "perf"
-Requires-Dist: tree_sitter_languages>=1.10.2; extra == "perf" #
+mistralai Requires-Dist: stop-sequencer Requires-Dist: Pympler>=1.0.1 #
 ð³WildCodeBench > [!WARNING] > The project is under active development.
 Please check back later for more updates. > [!WARNING] > Please use WildCode
 with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus),
 WildCode has a much less constrained execution environment to support tasks
 with diverse library dependencies. This may lead to security risks. We
 recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/
 ) to run the evaluation. > [!WARNING] > WildCode framework currently only
```

### Comparing `wild_code-0.4.4/wild_code.egg-info/SOURCES.txt` & `wild_code-0.4.5/wild_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/data/utils.py` & `wild_code-0.4.5/wildcode/data/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/data/wildcodebench.py` & `wild_code-0.4.5/wildcode/data/wildcodebench.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/eval/__init__.py` & `wild_code-0.4.5/wildcode/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/eval/utils.py` & `wild_code-0.4.5/wildcode/eval/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/evaluate.py` & `wild_code-0.4.5/wildcode/evaluate.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/gen/__init__.py` & `wild_code-0.4.5/wildcode/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/gen/util/__init__.py` & `wild_code-0.4.5/wildcode/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/gen/util/anthropic_request.py` & `wild_code-0.4.5/wildcode/gen/util/anthropic_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/gen/util/openai_request.py` & `wild_code-0.4.5/wildcode/gen/util/openai_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/generate.py` & `wild_code-0.4.5/wildcode/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     parser.add_argument("--backend", default="vllm", type=str)
     parser.add_argument("--base_url", default=None, type=str)
     parser.add_argument("--tp", default=1, type=int)
     args = parser.parse_args()
     
     
     assert args.dataset in ["wildcodebench"], f"Invalid dataset {args.dataset}"
-    assert args.backend in ["vllm", "hf", "openai"]
+    assert args.backend in ["vllm", "hf", "openai", "mistral", "anthropic", "google"]
 
     if args.greedy and (args.temperature != 0 or args.bs != 1 or args.n_samples != 1)\
         or (args.temperature == 0 and args.n_samples == 1):
         args.temperature = 0
         args.bs = 1
         args.n_samples = 1
         args.greedy = True
```

### Comparing `wild_code-0.4.4/wildcode/inspect.py` & `wild_code-0.4.5/wildcode/inspect.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/lecacy_sanitize.py` & `wild_code-0.4.5/wildcode/lecacy_sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/model.py` & `wild_code-0.4.5/wildcode/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 # mistral.ai
 try:
     from mistralai.client import MistralClient
     from mistralai.models.chat_completion import ChatMessage
 except ImportError:
     warn("MistralAI decoder will not work. Fix by `pip install mistralai`")
 
+try:
+    import google.generativeai as genai
+except ImportError:
+    warn("GoogleGenAI decoder will not work. Fix by `pip install google-generativeai`")
+
 import torch
 from stop_sequencer import StopSequencer
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 try:
     from vllm import LLM, SamplingParams
 except ImportError:
@@ -331,15 +336,15 @@
         outputs = []
         for _ in range(batch_size):
             ret = self.client.chat(
                 model=self.name,
                 messages=[
                     ChatMessage(
                         role="user",
-                        content="Please generate code to solve the following problem in a Python markdown block:"
+                        content="Please generate self-contained code to solve the following problem in a Python markdown block:"
                         + f"\n```python\n{prompt.strip()}\n```",
                     )
                 ],
                 max_tokens=self.max_new_tokens,
                 **kwargs,
             )
 
@@ -360,42 +365,92 @@
         return False
 
 
 class AnthropicMessageDecoder(AnthropicDecoder):
     def codegen(
         self, prompt: str, do_sample: bool = True, num_samples: int = 200
     ) -> List[str]:
+        kwargs = {}
         if do_sample:
             assert self.temperature > 0, "Temperature must be positive for sampling"
+            kwargs["top_p"] = 0.95
+            kwargs["temperature"] = self.temperature
+        else:
+            self.temperature = 0
 
         batch_size = min(self.batch_size, num_samples)
         if not do_sample:
             assert batch_size == 1, "Sampling only supports batch size of 1"
 
         outputs = []
         for _ in range(batch_size):
             message = anthropic_request.make_auto_request(
                 client=self.client,
                 model=self.name,
                 messages=[
                     {
                         "role": "user",
-                        "content": "Please generate code to complete the following problem wrapped in a Python markdown block:"
+                        "content": "Please generate self-contained code to complete the following problem wrapped in a Python markdown block:"
                         + f"\n```python\n{prompt.strip()}\n```\n",
                     }
                 ],
                 max_tokens=self.max_new_tokens,
-                temperature=self.temperature,
                 stop_sequences=["\n```\n", "\nif "],
+                **kwargs,
             )
             outputs.append(message.content[0].text)
 
         return outputs
 
 
+class GoogleGenAIDecoder(DecoderBase, ABC):
+    def __init__(self, name: str, **kwargs) -> None:
+        super().__init__(name, **kwargs)
+        genai.configure(api_key=os.environ['GOOGLE_API_KEY'])
+
+    def is_direct_completion(self) -> bool:
+        return False
+    
+
+class GeminiDecoder(GoogleGenAIDecoder):
+    def codegen(
+        self, prompt: str, do_sample: bool = True, num_samples: int = 200
+    ) -> List[str]:
+        kwargs = {}
+        if do_sample:
+            assert self.temperature > 0, "Temperature must be positive for sampling"
+            kwargs["top_p"] = 0.95
+            kwargs["temperature"] = self.temperature
+        else:
+            self.temperature = 0
+
+        batch_size = min(self.batch_size, num_samples)
+        if not do_sample:
+            assert batch_size == 1, "Sampling only supports batch size of 1"
+
+        genai_config = genai.GenerationConfig(
+            max_output_tokens=self.max_new_tokens,
+            **kwargs,
+        )
+    
+        model = genai.GenerativeModel(model_name=self.name, generation_config=genai_config)
+
+        
+        outputs = []
+        for _ in range(batch_size):
+            message = model.generate_content(
+                "Please generate self-contained code to complete the following problem wrapped in a Python markdown block:"
+                + f"\n```python\n{prompt.strip()}\n```",
+                generation_config=genai_config
+            )
+            outputs.append(message.text)
+
+        return outputs
+
+
 def make_model(
     model: str,
     backend: str,
     dataset: str,
     batch_size: int = 1,
     temperature: float = 0.0,
     tp=1,
@@ -430,8 +485,14 @@
             temperature=temperature,
         )
     elif backend == "anthropic":
         return AnthropicMessageDecoder(
             name=model,
             batch_size=batch_size,
             temperature=temperature,
+        )
+    elif backend == "google":
+        return GeminiDecoder(
+            name=model,
+            batch_size=batch_size,
+            temperature=temperature,
         )
```

### Comparing `wild_code-0.4.4/wildcode/sanitize.py` & `wild_code-0.4.5/wildcode/sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.4/wildcode/syncheck.py` & `wild_code-0.4.5/wildcode/syncheck.py`

 * *Files identical despite different names*

