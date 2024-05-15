# Comparing `tmp/aind_behavior_curriculum_template-0.0.2.tar.gz` & `tmp/aind_behavior_curriculum_template-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_behavior_curriculum_template-0.0.2.tar", last modified: Fri May 10 20:33:30 2024, max compression
+gzip compressed data, was "aind_behavior_curriculum_template-0.0.3.tar", last modified: Wed May 15 17:34:45 2024, max compression
```

## Comparing `aind_behavior_curriculum_template-0.0.2.tar` & `aind_behavior_curriculum_template-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.791608 aind_behavior_curriculum_template-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.783609 aind_behavior_curriculum_template-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.783609 aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/workflows/tag_publish_upload.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-10 20:33:30.791608 aind_behavior_curriculum_template-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:33:30.791608 aind_behavior_curriculum_template-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.783609 aind_behavior_curriculum_template-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 20:33:21.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.550813 aind_behavior_curriculum_template-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.546813 aind_behavior_curriculum_template-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.546813 aind_behavior_curriculum_template-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.546813 aind_behavior_curriculum_template-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/.github/workflows/tag_publish_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-15 17:34:45.550813 aind_behavior_curriculum_template-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.546813 aind_behavior_curriculum_template-0.0.3/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.546813 aind_behavior_curriculum_template-0.0.3/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.550813 aind_behavior_curriculum_template-0.0.3/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:34:45.550813 aind_behavior_curriculum_template-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.546813 aind_behavior_curriculum_template-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.550813 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.550813 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-15 17:34:45.000000 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-15 17:34:45.000000 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:34:45.000000 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 17:34:45.000000 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 17:34:45.000000 aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:34:45.550813 aind_behavior_curriculum_template-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 17:34:36.000000 aind_behavior_curriculum_template-0.0.3/tests/test_example.py
```

### Comparing `aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_behavior_curriculum_template-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_behavior_curriculum_template-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_behavior_curriculum_template-0.0.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/.github/workflows/init.yml` & `aind_behavior_curriculum_template-0.0.3/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/.github/workflows/tag_publish_upload.yml` & `aind_behavior_curriculum_template-0.0.3/.github/workflows/tag_publish_upload.yml`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
   upload_curriculum:
     needs: [tag, publish]
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: read
     env:
-      AWS_AIND_BEHAVIOR_ROLE: 'arn:aws:iam::467914378000:role/AindBehaviorCurriculumBucketGithubRole'
+      AWS_AIND_BEHAVIOR_ROLE: ${{ secrets.AIND_AWS_BEHAVIOR_CURRICULUM_ROLE }}
       AWS_BEHAVIOR_CURRICULUM_BUCKET: 'aind-behavior-curriculum-prod-o5171v'
       AWS_REGION: 'us-west-2'
       TEMP_DIR: 'temp_dir'
       S3_PREFIX: 'curriculums'
       REPO_NAME: ${{ github.repository }}
       VERSION: ${{ needs.tag.outputs.new_version }}
```

### Comparing `aind_behavior_curriculum_template-0.0.2/.github/workflows/test_and_lint.yml` & `aind_behavior_curriculum_template-0.0.3/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/.gitignore` & `aind_behavior_curriculum_template-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/LICENSE` & `aind_behavior_curriculum_template-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/PKG-INFO` & `aind_behavior_curriculum_template-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-behavior-curriculum-template
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_behavior_curriculum_template-0.0.2/README.md` & `aind_behavior_curriculum_template-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/doc_template/Makefile` & `aind_behavior_curriculum_template-0.0.3/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/doc_template/make.bat` & `aind_behavior_curriculum_template-0.0.3/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/dark-logo.svg` & `aind_behavior_curriculum_template-0.0.3/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/favicon.ico` & `aind_behavior_curriculum_template-0.0.3/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/light-logo.svg` & `aind_behavior_curriculum_template-0.0.3/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/doc_template/source/conf.py` & `aind_behavior_curriculum_template-0.0.3/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/pyproject.toml` & `aind_behavior_curriculum_template-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/PKG-INFO` & `aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-behavior-curriculum-template
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/SOURCES.txt` & `aind_behavior_curriculum_template-0.0.3/src/aind_behavior_curriculum_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

