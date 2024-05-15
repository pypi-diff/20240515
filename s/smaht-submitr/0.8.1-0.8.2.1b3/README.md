# Comparing `tmp/smaht_submitr-0.8.1.tar.gz` & `tmp/smaht_submitr-0.8.2.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.8.1.tar", max compression
+gzip compressed data, was "smaht_submitr-0.8.2.1b3.tar", max compression
```

## Comparing `smaht_submitr-0.8.1.tar` & `smaht_submitr-0.8.2.1b3.tar`

### file list

```diff
@@ -1,53 +1,66 @@
--rw-r--r--   0        0        0     1098 2024-04-22 12:30:40.164081 smaht_submitr-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-22 12:30:40.164081 smaht_submitr-0.8.1/README.rst
--rw-r--r--   0        0        0     3482 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/exceptions.py
--rw-r--r--   0        0        0    11097 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/metadata_template.py
--rw-r--r--   0        0        0     2628 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/output.py
--rw-r--r--   0        0        0    10904 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4779 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     9895 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     2824 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/get_metadata_template.py
--rw-r--r--   0        0        0     1822 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5705 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    20411 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-22 12:30:40.204082 smaht_submitr-0.8.1/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   162499 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157490 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    11245 2024-04-22 12:30:40.208082 smaht_submitr-0.8.1/submitr/utils.py
--rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 smaht_submitr-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-15 11:48:03.500949 smaht_submitr-0.8.2.1b3/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-05-15 11:48:03.500949 smaht_submitr-0.8.2.1b3/README.rst
+-rw-r--r--   0        0        0     3720 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/exceptions.py
+-rw-r--r--   0        0        0    16784 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/file_for_upload.py
+-rw-r--r--   0        0        0    11097 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/metadata_template.py
+-rw-r--r--   0        0        0     2628 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/output.py
+-rw-r--r--   0        0        0      377 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/__init__.py
+-rw-r--r--   0        0        0    10830 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/rclone.py
+-rw-r--r--   0        0        0     8848 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/rclone_commands.py
+-rw-r--r--   0        0        0     6750 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/rclone_config.py
+-rw-r--r--   0        0        0     8002 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/rclone_config_amazon.py
+-rw-r--r--   0        0        0     9757 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/rclone_config_google.py
+-rw-r--r--   0        0        0     5152 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/rclone_installation.py
+-rw-r--r--   0        0        0     2608 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/rclone_utils.py
+-rw-r--r--   0        0        0    18682 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
+-rw-r--r--   0        0        0     7572 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/rclone/testing/rclone_utils_for_testing_google.py
+-rw-r--r--   0        0        0    19785 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4779 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     9895 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     2824 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/get_metadata_template.py
+-rw-r--r--   0        0        0     1822 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     4123 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/rcloner.py
+-rw-r--r--   0        0        0     6303 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    21329 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-05-15 11:48:03.540949 smaht_submitr-0.8.2.1b3/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   127817 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/submission.py
+-rw-r--r--   0        0        0    14834 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/submission_uploads.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6448 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_file_for_upload.py
+-rw-r--r--   0        0        0     1620 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    34279 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_rclone_support.py
+-rw-r--r--   0        0        0    11773 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0    37993 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     4353 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0     8667 2024-05-15 11:48:03.544949 smaht_submitr-0.8.2.1b3/submitr/utils.py
+-rw-r--r--   0        0        0     4039 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b3/PKG-INFO
```

### Comparing `smaht_submitr-0.8.1/LICENSE.txt` & `smaht_submitr-0.8.2.1b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/README.rst` & `smaht_submitr-0.8.2.1b3/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/pyproject.toml` & `smaht_submitr-0.8.2.1b3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.8.1"
+version = "0.8.2.1b3"  # TODO: To become 0.8.3
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
@@ -42,18 +42,18 @@
 ]
 include = [
   "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 
-python = ">=3.8.0,<3.12"
-awscli = ">=1.32.81"
-boto3 = "^1.34.81"
-dcicutils = "^8.8.4"
+python = ">=3.8.0,<3.13"
+awscli = ">=1.32.105"
+boto3 = "^1.34.105"
+dcicutils = "^8.8.4.1b31"
 PyYAML = "^6.0.1"
 requests = "^2.31.0"
 googleapi = "^0.1.0"
 
 [tool.poetry.dev-dependencies]
 
 # Coverage
@@ -62,14 +62,16 @@
 # Loaded manually in GA workflow for coverage because a dependency on 2to3
 # in its docopts dependency makes a problem for laoding it here in poetry. -kmp 7-Apr-2023
 # coveralls = ">=3.3.1"
 
 # Linting generally
 flake8 = ">=3.9.2"
 
+google-cloud-storage = "^2.16.0"
+
 pip-licenses = ">=3.5.5"
 
 # pygments is used by PyCharm
 pygments = ">=2.14.0"
 
 # PyTest and its auxiliary support files
 pytest = ">=7.2.1"  # ">=6.2.5"
@@ -85,14 +87,15 @@
 [tool.poetry.scripts]
 
 check-submission= "submitr.scripts.check_submission:main"
 get-metadata-template = "submitr.scripts.get_metadata_template:main"
 list-submissions= "submitr.scripts.list_submissions:main"
 make-sample-fastq-file = "submitr.scripts.make_sample_fastq_file:main"
 publish-to-pypi = "dcicutils.scripts.publish_to_pypi:main"
+rcloner= "submitr.scripts.rcloner:main"
 resume-uploads = "submitr.scripts.resume_uploads:main"
 # Covered by check-submission
 # show-submission-info = "submitr.scripts.show_upload_info:main"
 # show-upload-info = "submitr.scripts.show_upload_info:main"
 submit-genelist = "submitr.scripts.submit_genelist:main"
 submit-metadata-bundle = "submitr.scripts.submit_metadata_bundle:main"
 submit-ontology = "submitr.scripts.submit_ontology:main"
@@ -104,16 +107,20 @@
 # https://coverage.readthedocs.io/en/latest/config.html
 exclude_lines = [
   "if __name__ == .__main__.:",
   "pragma: no cover"
 ]
 
 [tool.pytest.ini_options]
+filterwarnings = [
+    "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
+]
 markers = [
-  "static: a test that tests the static form of code, not its runtime functionality"
+  "static: a test that tests the static form of code, not its runtime functionality",
+  "integration: integration tests"
 ]
 
 
 [build-system]
 
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `smaht_submitr-0.8.1/submitr/base.py` & `smaht_submitr-0.8.2.1b3/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/metadata_template.py` & `smaht_submitr-0.8.2.1b3/submitr/metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/output.py` & `smaht_submitr-0.8.2.1b3/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/check_submission.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/cli_utils.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/get_metadata_template.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/get_metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/list_submissions.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/resume_uploads.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from dcicutils.command_utils import script_catch_errors
 from dcicutils.misc_utils import PRINT
-from .cli_utils import CustomArgumentParser
-from ..base import DEFAULT_APP
-from ..submission import resume_uploads
+from submitr.base import DEFAULT_APP
+from submitr.rclone import RCloneConfigGoogle
+from submitr.submission import resume_uploads
+from submitr.scripts.cli_utils import CustomArgumentParser
 
 
 _HELP = f"""
 ===
 resume-uploads [VERSION]
 ===
 Tool to upload files referenced in a metadata file,
@@ -72,15 +73,18 @@
                         help=f"An application (default {DEFAULT_APP!r}. Only for debugging."
                              f" Normally this should not be given.")
     parser.add_argument('--bundle', help="location of the original Excel submission file")
     parser.add_argument('--keys', help="Path to keys file (rather than default ~/.smaht-keys.json).", default=None)
     parser.add_argument('--directory', help="Directory of the upload files.")
     parser.add_argument('--directory-only', help="Same as --directory but NOT recursively.", default=False)
     parser.add_argument('--upload_folder', help="Synonym for --directory.")
+    parser.add_argument('--rclone-google-source', help="Use rlcone to copy upload files from GCS.", default=None)
+    parser.add_argument('--rclone-google-credentials', help="GCS credentials (service account file).", default=None)
     parser.add_argument('--output', help="Output file for results.", default=False)
+    parser.add_argument('--verbose', action="store_true", default=False)
     parser.add_argument('--yes', action="store_true",
                         help="Suppress (yes/no) requests for user input.", default=False)
     args = parser.parse_args(args=simulated_args_for_testing)
 
     directory_only = True
     if args.directory:
         args.upload_folder = args.directory
@@ -113,14 +117,16 @@
     if not args.upload_folder and args.directory:
         args.upload_folder = args.directory
 
     if args.upload_folder and not os.path.isdir(args.upload_folder):
         PRINT(f"Specified upload directory not found: {args.upload_folder}")
         exit(1)
 
+    config_google = RCloneConfigGoogle.from_command_args(args.rclone_google_source, args.rclone_google_credentials)
+
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
         if args.env:
             env_from_env = True
 
     with script_catch_errors():
@@ -130,13 +136,15 @@
                        env_from_env=env_from_env,
                        keys_file=args.keys,
                        bundle_filename=args.bundle,
                        server=args.server,
                        upload_folder=args.upload_folder,
                        no_query=args.yes,
                        subfolders=not directory_only,
+                       rclone_config_google=config_google,
                        output_file=args.output,
-                       app=args.app)
+                       app=args.app,
+                       verbose=args.verbose)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `smaht_submitr-0.8.1/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/submit_metadata_bundle.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     _define_portal,
     _get_consortia,
     _get_submission_centers,
     _ping,
     _print_metadata_file_info,
     _pytesting
 )
+from submitr.rclone import RCloneConfigGoogle
 
 _HELP = f"""
 ===
 submit-metadata-bundle [VERSION]
 ===
 Tool to submit submission metadata and files to SMaHT Portal.
 See: {CustomArgumentParser.HELP_URL}
@@ -50,14 +51,20 @@
 --submission-center SUBMISSION-CENTER
   To specify your submission center.
   Default is to use the submission center associated with your account.
 --directory DIRECTORY
   To specify a directory containing the files to upload; in addition
   to the default of using the directory containing the submitted file;
   this directory will be searched recursively.
+--rclone-google-source GOOGLE-CLOUD-STORAGE-SOURCE
+  A Google Cloud Storage (GCS) bucket or bucket/key (foldrer)
+  from where the upload file(s) should be read.
+--rclone-google-credentials GCS-SERVICE-ACCOUNT-FILE
+  GCS credentials to use for --rclone-google-source;
+  e.g. a path to a service account file.
 --output OUTPUT-FILE
   Writes all logging output to the specified file;
   and refrains from printing lengthy content to output/stdout.
 --info
   Displays ONLY info about the specified metadata file; nothing else.
   Add --refs or --files to see (linkTo) references or (upload) files.
 --verbose
@@ -214,53 +221,49 @@
                         help="Outputs list of files from the metadata file; only with --info.", default=False)
     parser.add_argument('--output', help="Output file for results.", default=False)
     parser.add_argument('--verbose', action="store_true", help="Debug output.", default=False)
     parser.add_argument('--timeout', help="Wait timeout for server validation/submission.")
     parser.add_argument('--debug', action="store_true", help="Debug output.", default=False)
     parser.add_argument('--debug-sleep', help="Sleep on each row read for troubleshooting/testing.", default=False)
     parser.add_argument('--ping', action="store_true", help="Ping server.", default=False)
+    parser.add_argument('--rclone-google-source', help="Use rlcone to copy upload files from GCS.", default=None)
+    parser.add_argument('--rclone-google-credentials', help="GCS credentials (service account file).", default=None)
     args = parser.parse_args(args=simulated_args_for_testing)
 
     directory_only = True
     if args.directory:
         args.upload_folder = args.directory
         directory_only = False
     if args.directory_only:
         args.upload_folder = args.directory_only
         directory_only = True
 
-#   keys_file = args.keys or os.environ.get("SMAHT_KEYS")
-#   if keys_file:
-#       if not keys_file.endswith(".json"):
-#           PRINT(f"ERROR: The specified keys file is not a .json file: {keys_file}")
-#           exit(1)
-#       if not keys_file.endswith(".json") or not os.path.exists(keys_file):
-#           PRINT(f"ERROR: The --keys argument must be the name of an existing .json file: {keys_file}")
-#           exit(1)
-
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
         if args.env:
             env_from_env = True
 
+    config_google = RCloneConfigGoogle.from_command_args(args.rclone_google_source, args.rclone_google_credentials)
+
     if args.ping or (args.bundle_filename and args.bundle_filename.lower() == "ping"):
-        ping_okay = _ping(
-            env=args.env or os.environ.get("SMAHT_ENV"),
-            env_from_env=env_from_env,
-            server=args.server,
-            app=args.app,
-            keys_file=args.keys,
-            verbose=True)
-        if ping_okay:
-            PRINT("Ping success. Your connection appears to be OK.")
-            exit(0)
+        if args.env or os.environ.get("SMAHT_ENV"):
+            ping_okay = _ping(env=args.env or os.environ.get("SMAHT_ENV"), env_from_env=env_from_env,
+                              server=args.server, app=args.app, keys_file=args.keys, verbose=True)
+            if ping_okay:
+                PRINT("Portal connectivity appears to be OK ✓")
+            else:
+                PRINT("Portal connectivty appears to be problematic ✗")
         else:
-            PRINT("Ping failure. Your connection appears to be problematic.")
-            exit(1)
+            PRINT("No environment specified (via --env); skipping SMaHT Portal ping.")
+            ping_okay = True
+        ping_rclone_okay = None
+        if config_google:
+            ping_rclone_okay = config_google.verify_connectivity()
+        exit(0 if ping_okay is True and (ping_rclone_okay is not False) else 1)
 
     if args.consortia or (args.bundle_filename and args.bundle_filename.lower() == "consortia"):
         portal = _define_portal(env=args.env)
         consortia = _get_consortia(portal)
         PRINT("Known Consortia:")
         for consortium in consortia:
             if ((consortium_name := consortium.get("name")) and
@@ -307,15 +310,20 @@
             args.timeout = int(args.timeout)
 
     if args.info:
         if not os.path.exists(args.bundle_filename):
             PRINT(f"File does not exist: {args.bundle_filename}")
             exit(1)
         _print_metadata_file_info(args.bundle_filename, env=args.env,
-                                  refs=args.refs, files=args.files, output_file=args.output, verbose=args.verbose)
+                                  refs=args.refs, files=args.files,
+                                  subfolders=not directory_only,
+                                  upload_folder=args.upload_folder,
+                                  rclone_config_google=config_google,
+                                  output_file=args.output,
+                                  verbose=args.verbose)
         exit(0)
 
     with script_catch_errors():
 
         if not _sanity_check_submitted_file(args.bundle_filename):
             exit(1)
 
@@ -331,14 +339,15 @@
                              app=args.app,
                              submission_protocol=args.submission_protocol,
                              upload_folder=args.upload_folder,
                              show_details=args.details,
                              post_only=args.post_only,
                              patch_only=args.patch_only,
                              submit=args.submit,
+                             rclone_config_google=config_google,
                              validate_local_only=args.validate_local_only,
                              validate_remote_only=args.validate_remote_only,
                              validate_local_skip=args.validate_local_skip,
                              validate_remote_skip=args.validate_remote_skip,
                              noanalyze=args.noanalyze,
                              json_only=args.json_only,
                              ref_nocache=args.ref_nocache,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smaht_submitr-0.8.1/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.8.2.1b3/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/submission.py` & `smaht_submitr-0.8.2.1b3/submitr/submission.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,49 +5,45 @@
 import io
 import json
 import os
 import re
 import sys
 import time
 from typing import Any, BinaryIO, Callable, Dict, List, Optional, Tuple
-import yaml
+from typing_extensions import Literal
 
 # get_env_real_url would rely on env_utils
 # from dcicutils.env_utils import get_env_real_url
 from dcicutils.command_utils import yes_or_no
 from dcicutils.common import APP_CGAP, APP_FOURFRONT, APP_SMAHT, OrchestratedApp
 from dcicutils.data_readers import Excel
 from dcicutils.datetime_utils import format_datetime
-from dcicutils.file_utils import search_for_file
-from dcicutils.function_cache_decorator import function_cache
+from dcicutils.file_utils import (
+       compute_file_etag, compute_file_md5,
+       get_file_modified_datetime, get_file_size
+)
 from dcicutils.lang_utils import conjoined_list, disjoined_list, there_are
 from dcicutils.misc_utils import (
     environ_bool, format_duration, format_size,
-    is_uuid, url_path_join, ignorable, normalize_spaces, remove_prefix
+    is_uuid, url_path_join, normalize_spaces
 )
 from dcicutils.progress_bar import ProgressBar
-from dcicutils.s3_utils import HealthPageKey
 from dcicutils.schema_utils import EncodedSchemaConstants, JsonSchemaConstants, Schema
 from dcicutils.structured_data import Portal, StructuredDataSet
 from dcicutils.submitr.progress_constants import PROGRESS_INGESTER, PROGRESS_LOADXL, PROGRESS_PARSE
 from dcicutils.submitr.ref_lookup_strategy import ref_lookup_strategy
-from typing_extensions import Literal
-from urllib.parse import urlparse
 from submitr.base import DEFAULT_APP
 from submitr.exceptions import PortalPermissionError
+from submitr.file_for_upload import FilesForUpload
 from submitr.metadata_template import check_metadata_version, print_metadata_version_warning
 from submitr.output import PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW, get_output_file, setup_for_output_file_option
+from submitr.rclone import RCloneConfigGoogle
 from submitr.scripts.cli_utils import get_version
-from submitr.s3_utils import upload_file_to_aws_s3
-from submitr.utils import (
-    format_path,
-    get_file_checksum, get_file_md5, get_file_md5_like_aws_s3_etag,
-    get_file_modified_datetime, get_file_size, get_s3_bucket_and_key_from_s3_uri,
-    is_excel_file_name, print_boxed, keyword_as_title, tobool
-)
+from submitr.submission_uploads import do_any_uploads
+from submitr.utils import format_path, get_health_page, is_excel_file_name, print_boxed, tobool
 
 
 def set_output_file(output_file):
     if output_file:
         global PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW
         PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW = setup_for_output_file_option(output_file)
 
@@ -383,93 +379,14 @@
 
 
 PROGRESS_CHECK_INTERVAL = 7  # seconds
 ATTEMPTS_BEFORE_TIMEOUT = 100
 ATTEMPTS_BEFORE_TIMEOUT = 4
 
 
-def _get_section(res, section):
-    """
-    Given a description of an ingestion submission, returns a section name within that ingestion.
-
-    :param res: the description of an ingestion submission as a python dictionary that represents JSON data
-    :param section: the name of a section to find either in the toplevel or in additional_data.
-    :return: the section's content
-    """
-
-    return res.get(section) or res.get('additional_data', {}).get(section)
-
-
-def _show_section(res, section, caveat_outcome=None, portal=None):
-    """
-    Shows a given named section from a description of an ingestion submission.
-
-    The caveat is used when there has been an error and should be a phrase that describes the fact that output
-    shown is only up to the point of the caveat situation. Instead of a "My Heading" header the output will be
-    "My Heading (prior to <caveat>)."
-
-    :param res: the description of an ingestion submission as a python dictionary that represents JSON data
-    :param section: the name of a section to find either in the toplevel or in additional_data.
-    :param caveat_outcome: a phrase describing some caveat on the output
-    """
-
-    section_data = _get_section(res, section)
-    if caveat_outcome and not section_data:
-        # In the case of non-success, be brief unless there's data to show.
-        return
-    if caveat_outcome:
-        caveat = " (prior to %s)" % caveat_outcome
-    else:
-        caveat = ""
-    if not section_data:
-        return
-    SHOW("\n----- %s%s -----" % (keyword_as_title(section), caveat))
-    if isinstance(section_data, dict):
-        if file := section_data.get("file"):
-            PRINT(f"File: {file}")
-        if s3_file := section_data.get("s3_file"):
-            PRINT(f"S3 File: {s3_file}")
-        if details := section_data.get("details"):
-            PRINT(f"Details: {details}")
-        for item in section_data:
-            if isinstance(section_data[item], list) and section_data[item]:
-                issue_prefix = ""
-                if item == "reader":
-                    PRINT(f"Parser Warnings:")
-                    issue_prefix = "WARNING: "
-                elif item == "validation":
-                    PRINT(f"Validation Errors:")
-                    issue_prefix = "ERROR: "
-                elif item == "ref":
-                    PRINT(f"Reference (linkTo) Errors:")
-                    issue_prefix = "ERROR: "
-                elif item == "errors":
-                    PRINT(f"Other Errors:")
-                    issue_prefix = "ERROR: "
-                else:
-                    continue
-                for issue in section_data[item]:
-                    if isinstance(issue, dict):
-                        PRINT(f"- {issue_prefix}{_format_issue(issue, file)}")
-                    elif isinstance(issue, str):
-                        PRINT(f"- {issue_prefix}{issue}")
-    elif isinstance(section_data, list):
-        if section == "upload_info":
-            for info in section_data:
-                if isinstance(info, dict) and info.get("filename") and (uuid := info.get("uuid")):
-                    upload_file_accession_name, upload_file_type = _get_upload_file_info(portal, uuid)
-                    info["target"] = upload_file_accession_name
-                    info["type"] = upload_file_type
-            PRINT(yaml.dump(section_data))
-        else:
-            [SHOW(line) for line in section_data]
-    else:  # We don't expect this, but such should be shown as-is, mostly to see what it is.
-        SHOW(section_data)
-
-
 def _ingestion_submission_item_url(server, uuid):
     # Note that we use datastore=database for quicker feedback.
     return url_path_join(server, "ingestion-submissions", uuid) + "?format=json&datastore=database"
 
 
 # TRY_OLD_PROTOCOL = True
 DEBUG_PROTOCOL = environ_bool("DEBUG_PROTOCOL", default=False)
@@ -479,14 +396,15 @@
         portal: Portal,
         ingestion_filename: str,
         consortia: Optional[List[str]] = None,
         submission_centers: Optional[List[str]] = None,
         add_submission_center: Optional[str] = None,
         is_server_validation: bool = False,
         is_resume_submission: bool = False,
+        validate_remote_skip: bool = False,
         validation_ingestion_submission_object: Optional[dict] = None,
         post_only: bool = False,
         patch_only: bool = False,
         autoadd: Optional[dict] = None,
         datafile_size: Optional[Any] = None,
         datafile_checksum: Optional[Any] = None,
         user: Optional[dict] = None,
@@ -505,21 +423,22 @@
     else:
         validation_ingestion_submission_object = None
         validation_ingestion_submission_uuid = None
         validation_parameters = None
 
     submission_post_data = {
         "validate_only": is_server_validation,
+        "validate_skip": validate_remote_skip,
         "post_only": post_only,
         "patch_only": patch_only,
         "ref_nocache": False,  # Do not do this server-side at all; only client-side for testing.
         "autoadd": json.dumps(autoadd),
         "ingestion_directory": os.path.dirname(ingestion_filename) if ingestion_filename else None,
         "datafile_size": datafile_size or get_file_size(ingestion_filename),
-        "datafile_checksum": datafile_checksum or get_file_checksum(ingestion_filename),
+        "datafile_checksum": datafile_checksum or compute_file_md5(ingestion_filename),
         "submitr_version": get_version(),
         "user": json.dumps(user) if user else None
     }
 
     if validation_ingestion_submission_uuid:
         submission_post_data["validation_uuid"] = validation_ingestion_submission_uuid
     if debug_sleep:
@@ -680,14 +599,15 @@
                          add_submission_center=None,
                          app: OrchestratedApp = None,
                          upload_folder=None,
                          no_query=False,
                          subfolders=False,
                          submission_protocol=DEFAULT_SUBMISSION_PROTOCOL,
                          submit=False,
+                         rclone_config_google=None,
                          validate_local_only=False,
                          validate_remote_only=False,
                          validate_local_skip=False,
                          validate_remote_skip=False,
                          post_only=False,
                          patch_only=False,
                          keys_file=None,
@@ -751,14 +671,15 @@
                                  consortium=consortium, submission_center=submission_center)
 
     if not portal.ping():
         SHOW(f"Portal credentials do not seem to work: {portal.keys_file} ({env})")
         exit(1)
 
     user_record = _get_user_record(portal.server, auth=portal.key_pair, quiet=json_only and not verbose)
+
     # Nevermind: Too confusing for both testing and general usage
     # to have different behaviours for admin and non-admin users.
     # is_admin_user = _is_admin_user(user_record)
     exit_immediately_on_errors = True
     if validate_local_only or validate_remote_skip:
         if validate_remote_only or validate_local_skip:
             PRINT("WARNING: Skipping all validation is definitely not recommended.")
@@ -809,14 +730,17 @@
                 PRINT(f"- {known_submission_center.get('name')} ({known_submission_center.get('uuid')})")
             exit(1)
         add_submission_center = f"/submission-centers/{found_submission_centers[0]['uuid']}/"
 
     if verbose:
         SHOW(f"Metadata bundle upload bucket: {metadata_bundles_bucket}")
 
+    if rclone_config_google:
+        rclone_config_google.verify_connectivity()
+
     if not noversion:
         check_metadata_version(ingestion_filename, portal=portal)
 
     if not validate_remote_only and not validate_local_skip:
         structured_data = _validate_locally(ingestion_filename, portal,
                                             validation=validation,
                                             validate_local_only=validate_local_only,
@@ -867,40 +791,50 @@
 
         SHOW(f"Validation tracking ID: {validation_uuid}")
 
         server_validation_done, server_validation_status, server_validation_response = _monitor_ingestion_process(
                 validation_uuid, portal.server, portal.env, app=portal.app, keys_file=portal.keys_file,
                 show_details=show_details, report=False, messages=True,
                 validation=True,
+                rclone_config_google=rclone_config_google,
                 nofiles=True, noprogress=noprogress, timeout=timeout,
                 verbose=verbose, debug=debug, debug_sleep=debug_sleep)
 
         if server_validation_status != "success":
             exit(1)
 
         PRINT("Validation results (server): OK")
 
     else:
         server_validation_response = None
         PRINT("Skipping remote (server) validation (as requested via"
               f" {'--validate-local-only' if validate_local_only else '--validate-remote-skip'}).")
 
     if validation:
+        do_any_uploads(structured_data,
+                       metadata_file=ingestion_filename,
+                       main_search_directory=upload_folder,
+                       main_search_directory_recursively=subfolders,
+                       config_google=rclone_config_google,
+                       portal=portal,
+                       verbose=True,
+                       review_only=True)
         exit(0)
 
     # Server submission.
 
     SHOW(f"Ready to submit your metadata to {portal.server}: {format_path(ingestion_filename)}")
     if not yes_or_no("Continue on with the actual submission?"):
         exit(0)
 
     submission_uuid = _initiate_server_ingestion_process(
         portal=portal,
         ingestion_filename=ingestion_filename,
         is_server_validation=False,
+        validate_remote_skip=validate_remote_skip,
         validation_ingestion_submission_object=server_validation_response,
         consortia=app_args.get("consortia"),
         submission_centers=app_args.get("submission_centers"),
         add_submission_center=add_submission_center,
         post_only=post_only,
         patch_only=patch_only,
         autoadd=autoadd,
@@ -911,32 +845,33 @@
         debug_sleep=debug_sleep)
 
     SHOW(f"Submission tracking ID: {submission_uuid}")
 
     submission_done, submission_status, submission_response = _monitor_ingestion_process(
             submission_uuid, portal.server, portal.env, app=portal.app, keys_file=portal.keys_file,
             show_details=show_details, report=False, messages=True,
+            rclone_config_google=rclone_config_google,
             validation=False,
             nofiles=True, noprogress=noprogress, timeout=timeout,
             verbose=verbose, debug=debug, debug_sleep=debug_sleep)
 
     if submission_status != "success":
         exit(1)
 
     PRINT("Submission complete!")
 
     # Now that submission has successfully complete, review the files to upload and then do it.
 
-    if structured_data:
-        _review_upload_files(structured_data, ingestion_filename,
-                             validation=validation, directory=upload_folder, recursive=subfolders)
-
-    do_any_uploads(submission_response, keydict=portal.key, ingestion_filename=ingestion_filename,
-                   upload_folder=upload_folder, no_query=no_query,
-                   subfolders=subfolders, portal=portal)
+    do_any_uploads(submission_response,
+                   metadata_file=ingestion_filename,
+                   main_search_directory=upload_folder,
+                   main_search_directory_recursively=subfolders,
+                   config_google=rclone_config_google,
+                   portal=portal,
+                   verbose=verbose)
 
 
 def _get_recent_submissions(portal: Portal, count: int = 30, name: Optional[str] = None) -> List[dict]:
     url = f"/search/?type=IngestionSubmission&sort=-date_created&from=0&limit={count}"
     if name:
         # TODO: Does not seem to return the same stuff; of not great consequence yet.
         url += f"&q={name}"
@@ -1026,14 +961,15 @@
                                validation: bool = False,
                                env_from_env: bool = False,
                                report: bool = True, messages: bool = False,
                                nofiles: bool = False, noprogress: bool = False,
                                check_submission_script: bool = False,
                                upload_directory: Optional[str] = None,
                                upload_directory_recursive: bool = False,
+                               rclone_config_google: Optional[RCloneConfigGoogle] = None,
                                timeout: Optional[int] = None,
                                verbose: bool = False, debug: bool = False,
                                note: Optional[str] = None,
                                output_file: Optional[str] = None,
                                debug_sleep: Optional[int] = None) -> Tuple[bool, str, dict]:
 
     if output_file:
@@ -1189,21 +1125,26 @@
     def interrupt_exit_message(bar: ProgressBar):
         nonlocal uuid, server, env, validation, portal
         command_summary = _summarize_submission(uuid=uuid, server=server, env=env, app=portal.app)
         SHOW(f"Your {'validation' if validation else 'submission'} is still running on the server: {uuid}")
         SHOW(f"Use this command to check its status: {command_summary}")
 
     if not (uuid_metadata := portal.get_metadata(uuid, raise_exception=False)):
-        message = f"Submission ID not found: {uuid}" if uuid != "dummy" else "No submission ID specified."
-        message += "\nSome recent submission IDs below. Use list-submissions to view more."
-        if _print_recent_submissions(portal, message=message, count=4):
-            if check_submission_script:
-                exit(1)
-            return
-        raise Exception(f"Cannot find object given uuid: {uuid}")
+        found_non_suffixed_uuid = False
+        if (dot := uuid.find(".")) > 0:
+            if uuid_metadata := portal.get_metadata(uuid := uuid[:dot], raise_exception=False):
+                found_non_suffixed_uuid = True
+        if not found_non_suffixed_uuid:
+            message = f"Submission ID not found: {uuid}" if uuid != "dummy" else "No submission ID specified."
+            message += "\nSome recent submission IDs below. Use list-submissions to view more."
+            if _print_recent_submissions(portal, message=message, count=4):
+                if check_submission_script:
+                    exit(1)
+                return
+            raise Exception(f"Cannot find object given uuid: {uuid}")
     if not portal.is_schema_type(uuid_metadata, INGESTION_SUBMISSION_TYPE_NAME):
         if portal.is_schema_file_type(uuid_metadata):
             _print_upload_file_summary(portal, uuid_metadata)
             # TODO: This is for special case of check-submission UPLOAD-FILE-UUID
             return
         undesired_type = portal.get_schema_type(uuid_metadata)
         raise Exception(f"Given ID is not for a submission or validation: {uuid} ({undesired_type})"
@@ -1347,16 +1288,20 @@
                 show_details=show_details, report=False, messages=True,
                 validation=False,
                 nofiles=True, noprogress=noprogress, timeout=timeout,
                 verbose=verbose, debug=debug, debug_sleep=debug_sleep)
         if submission_status != "success":
             exit(1)
         PRINT("Submission complete!")
-        do_any_uploads(submission_response, keydict=portal.key,
-                       upload_folder=upload_directory, subfolders=upload_directory_recursive, portal=portal)
+        do_any_uploads(submission_response,
+                       main_search_directory=upload_directory,
+                       main_search_directory_recursively=upload_directory_recursive,
+                       config_google=rclone_config_google,
+                       portal=portal,
+                       verbose=verbose)
         return
 
     if check_submission_script or verbose or debug:  # or not validation
         PRINT(f"Details for this server {'validation' if validation else 'submission'} ({uuid}) below:")
         _print_submission_summary(portal, check_response,
                                   nofiles=nofiles, check_submission_script=check_submission_script,
                                   verbose=verbose, debug=debug)
@@ -1502,39 +1447,14 @@
     elif server:
         command_summary = f"check-submission --server {server} {uuid}"
     else:  # unsatisfying, but not worth raising an error
         command_summary = f"check-submission {uuid}"
     return command_summary
 
 
-def compute_s3_submission_post_data(ingestion_filename, ingestion_post_result, **other_args):
-    uuid = ingestion_post_result['uuid']
-    at_id = ingestion_post_result['@id']
-    accession = ingestion_post_result.get('accession')  # maybe not always there?
-    upload_credentials = ingestion_post_result['upload_credentials']
-    upload_urlstring = upload_credentials['upload_url']
-    upload_url = urlparse(upload_urlstring)
-    upload_key = upload_credentials['key']
-    upload_bucket = upload_url.netloc
-    # Possible sanity check, probably not needed...
-    # check_true(upload_key == remove_prefix('/', upload_url.path, required=True),
-    #            message=f"The upload_key, {upload_key!r}, did not match path of {upload_url}.")
-    submission_post_data = {
-        'datafile_uuid': uuid,
-        'datafile_accession': accession,
-        'datafile_@id': at_id,
-        'datafile_url': upload_urlstring,
-        'datafile_bucket': upload_bucket,
-        'datafile_key': upload_key,
-        'datafile_source_filename': os.path.basename(ingestion_filename),
-        **other_args  # validate_remote_only, and any of institution, project, lab, or award that caller gave us
-    }
-    return submission_post_data
-
-
 def _print_submission_summary(portal: Portal, result: dict,
                               nofiles: bool = False,
                               check_submission_script: bool = False,
                               include_errors: bool = False,
                               verbose: bool = False, debug: bool = False) -> None:
     if not result:
         return
@@ -1777,70 +1697,14 @@
     for submission_center in submission_centers:
         if result:
             result += " | "
         result += submission_center.get("display_title")
     return result
 
 
-def _show_upload_info(uuid, server=None, env=None, keydict=None, app: str = None,
-                      show_primary_result=True,
-                      show_validation_output=True,
-                      show_processing_status=True,
-                      show_datafile_url=True,
-                      show_details=True):
-    """
-    Uploads the files associated with a given ingestion submission. This is useful if you answered "no" to the query
-    about uploading your data and then later are ready to do that upload.
-
-    :param uuid: a string guid that identifies the ingestion submission
-    :param server: the server to upload to
-    :param env: the portal environment to upload to
-    :param keydict: keydict-style auth, a dictionary of 'key', 'secret', and 'server'
-    :param app: the name of the app to use
-        e.g., affects whether to expect --lab, --award, --institution, --project, --consortium or --submission_center
-        and whether to use .fourfront-keys.json, .cgap-keys.json, or .smaht-keys.json
-    :param show_primary_result: bool controls whether the primary result is shown
-    :param show_validation_output: bool controls whether to show output resulting from validation checks
-    :param show_processing_status: bool controls whether to show the current processing status
-    :param show_datafile_url: bool controls whether to show the datafile_url parameter from the parameters.
-    :param show_details: bool controls whether to show the details from the results file in S3.
-    """
-
-    if app is None:  # Better to pass explicitly, but some legacy situations might require this to default
-        app = DEFAULT_APP
-
-    portal = _define_portal(key=keydict, env=env, server=server, app=app, report=True)
-
-    if not (uuid_metadata := portal.get_metadata(uuid)):
-        raise Exception(f"Cannot find object given uuid: {uuid}")
-
-    if not portal.is_schema_type(uuid_metadata, INGESTION_SUBMISSION_TYPE_NAME):
-        undesired_type = portal.get_schema_type(uuid_metadata)
-        raise Exception(f"Given ID is not an {INGESTION_SUBMISSION_TYPE_NAME} type: {uuid} ({undesired_type})")
-
-    url = _ingestion_submission_item_url(portal.server, uuid)
-    response = portal.get(url)
-    response.raise_for_status()
-    res = response.json()
-    _show_upload_result(res,
-                        show_primary_result=show_primary_result,
-                        show_validation_output=show_validation_output,
-                        show_processing_status=show_processing_status,
-                        show_datafile_url=show_datafile_url,
-                        show_details=show_details,
-                        portal=portal)
-    if show_details:
-        metadata_bundles_bucket = get_metadata_bundles_bucket_from_health_path(key=portal.key)
-        _show_detailed_results(uuid, metadata_bundles_bucket)
-
-    if not _pytesting():
-        PRINT("")
-        _print_submission_summary(portal, res)
-
-
 @lru_cache(maxsize=256)
 def _get_upload_file_info(portal: Portal, uuid: str) -> Tuple[Optional[str], Optional[str]]:
     try:
         upload_file_info = portal.get(f"/{uuid}").json()
         upload_file_accession_based_name = upload_file_info.get("display_title")
         if upload_file_type := upload_file_info.get("data_type"):
             if isinstance(upload_file_type, list) and len(upload_file_type) > 0:
@@ -1850,576 +1714,46 @@
             if upload_file_type:
                 upload_file_type = Schema.type_name(upload_file_type)
         return upload_file_accession_based_name, upload_file_type
     except Exception:
         return None
 
 
-def _show_upload_result(result,
-                        show_primary_result=True,
-                        show_validation_output=True,
-                        show_processing_status=True,
-                        show_datafile_url=True,
-                        show_details=True,
-                        portal=None):
-
-    if show_primary_result:
-        if _get_section(result, 'upload_info'):
-            _show_section(result, 'upload_info', portal=portal)
-        else:
-            SHOW("Uploads: None")
-
-    # New March 2023 ...
-
-    if show_validation_output and _get_section(result, 'validation_output'):
-        _show_section(result, 'validation_output')
-
-    if show_processing_status and result.get('processing_status'):
-        SHOW("\n----- Processing Status -----")
-        state = result['processing_status'].get('state')
-        if state:
-            SHOW(f"State: {state.title()}")
-        outcome = result['processing_status'].get('outcome')
-        if outcome:
-            SHOW(f"Outcome: {outcome.title()}")
-        progress = result['processing_status'].get('progress')
-        if progress:
-            SHOW(f"Progress: {progress.title()}")
-
-    if show_datafile_url and result.get('parameters'):
-        datafile_url = result['parameters'].get('datafile_url')
-        if datafile_url:
-            SHOW("----- DataFile URL -----")
-            SHOW(datafile_url)
-
-
-def do_any_uploads(res, keydict, upload_folder=None, ingestion_filename=None,
-                   no_query=False, subfolders=False, portal=None):
-
-    def display_file_info(upload_file_info: dict) -> None:
-        nonlocal upload_folder, subfolders
-        file = upload_file_info.get("filename")
-        file_uuid = upload_file_info.get("uuid")
-        if file:
-            if file_paths := search_for_file(file, location=upload_folder, recursive=subfolders):
-                if len(file_paths) == 1:
-                    PRINT(f"File to upload to AWS S3: {format_path(file_paths[0])}"
-                          f" ({format_size(get_file_size(file_paths[0]))})")
-                    return True
-                else:
-                    PRINT(f"No upload attempted for file {file} because multiple"
-                          f" copies were found in folder {upload_folder}: {', '.join(file_paths)}.")
-                    return False
-            PRINT(f"WARNING: Cannot find file to upload to AWS S3: {format_path(file)} ({file_uuid})")
-        return False
-
-    upload_info = _get_section(res, 'upload_info')
-    if not upload_folder:
-        if ingestion_directory := res.get("parameters", {}).get("ingestion_directory"):
-            if os.path.isdir(ingestion_directory):
-                upload_folder = ingestion_directory
-    if not upload_folder and ingestion_filename:
-        if ingestion_directory := os.path.dirname(ingestion_filename):
-            upload_folder = ingestion_directory
-    resume_upload_commands = []
-    resume_upload_commands_missing = []
-    noupload = False
-    if upload_info:
-        files_to_upload = []
-        for upload_file_info in upload_info:
-            if display_file_info(upload_file_info):
-                files_to_upload.append(upload_file_info)
-                if portal:
-                    resume_upload_commands.append(f"resume-uploads --env {portal.env} {upload_file_info.get('uuid')}")
-            elif portal:
-                resume_upload_commands_missing.append(
-                    f"resume-uploads --env {portal.env} {upload_file_info.get('uuid')}")
-        if len(files_to_upload) == 0:
-            return
-        if no_query:
-            do_uploads(files_to_upload, auth=keydict, no_query=no_query, folder=upload_folder,
-                       subfolders=subfolders, portal=portal)
-        else:
-            message = ("Upload this file?" if len(files_to_upload) == 1
-                       else f"Upload these {len(files_to_upload)} files?")
-            if yes_or_no(message):
-                do_uploads(files_to_upload, auth=keydict,
-                           no_query=no_query, folder=upload_folder,
-                           subfolders=subfolders, portal=portal)
-            else:
-                noupload = True
-                SHOW("No uploads attempted.")
-                if resume_upload_commands:
-                    resume_upload_commands += resume_upload_commands_missing
-                    nresume_upload_commands = len(resume_upload_commands)
-                    if yes_or_no(f"Do you want to see the resume-uploads"
-                                 f" command{'s' if nresume_upload_commands != 1 else ''} to use to"
-                                 f" upload {'these' if nresume_upload_commands != 1 else 'this'} separately?"):
-                        for resume_upload_command in resume_upload_commands:
-                            PRINT(f"▶ {resume_upload_command}")
-    if not noupload and resume_upload_commands_missing:
-        nresume_upload_commands_missing = len(resume_upload_commands_missing)
-        PRINT(f"There {'were' if nresume_upload_commands_missing != 1 else 'was'}"
-              f" {nresume_upload_commands_missing} missing"
-              f" file{'s' if nresume_upload_commands_missing != 1 else ''} as mentioned above.")
-        if yes_or_no(f"Do you want to see the resume-uploads"
-                     f" command{'s' if nresume_upload_commands_missing != 1 else ''}"
-                     f" to use to upload {'these' if nresume_upload_commands_missing != 1 else 'this'} separately?"):
-            for resume_upload_command_missing in resume_upload_commands_missing:
-                PRINT(f"▶ {resume_upload_command_missing}")
-
-
 def resume_uploads(uuid, server=None, env=None, bundle_filename=None, keydict=None,
                    upload_folder=None, no_query=False, subfolders=False,
-                   output_file=None, app=None, keys_file=None, env_from_env=False):
-    """
-    Uploads the files associated with a given ingestion submission. This is useful if you answered "no" to the query
-    about uploading your data and then later are ready to do that upload.
-
-    :param uuid: a string guid that identifies the ingestion submission
-    :param server: the server to upload to
-    :param env: the portal environment to upload to
-    :param bundle_filename: the bundle file to be uploaded
-    :param keydict: keydict-style auth, a dictionary of 'key', 'secret', and 'server'
-    :param upload_folder: folder in which to find files to upload (default: same as ingestion_filename)
-    :param no_query: bool to suppress requests for user input
-    :param subfolders: bool to search subdirectories within upload_folder for files
-    """
+                   rclone_config_google=None,
+                   output_file=None, app=None, keys_file=None, env_from_env=False, verbose=False):
 
     if output_file:
         global PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW
         PRINT, PRINT_OUTPUT, PRINT_STDOUT, SHOW = setup_for_output_file_option(output_file)
 
     portal = _define_portal(key=keydict, keys_file=keys_file, env=env,
                             server=server, app=app, env_from_env=env_from_env,
                             report=True, note="Resuming File Upload")
+    if rclone_config_google:
+        rclone_config_google.verify_connectivity()
 
-    if not (response := portal.get_metadata(uuid, raise_exception=False)):
-        if accession_id := _extract_accession_id(uuid):
-            if not (response := portal.get_metadata(accession_id)):
-                raise Exception(f"Given accession ID not found: {accession_id}")
-            if (display_title := response.get("display_title")) and not (uuid == display_title):
-                raise Exception(f"Accession ID found but wrong filename: {accession_id} vs {uuid}")
-            uuid = accession_id
-        else:
-            raise Exception(f"Given ID not found: {uuid}")
-
-    if not portal.is_schema_type(response, INGESTION_SUBMISSION_TYPE_NAME):
-
-        # Subsume function of upload-item-data into resume-uploads for convenience.
-        if portal.is_schema_file_type(response):
-            _upload_item_data(item_filename=uuid, uuid=None, server=portal.server,
-                              env=portal.env, directory=upload_folder, recursive=subfolders,
-                              no_query=no_query, app=app, report=False)
-            return
-
-        undesired_type = portal.get_schema_type(response)
-        raise Exception(f"Given ID is not an {INGESTION_SUBMISSION_TYPE_NAME} type: {uuid} ({undesired_type})")
-
-    if submission_parameters := response.get("parameters", {}):
-        if tobool(submission_parameters.get("validate_only")):
-            PRINT(f"This submission ID ({uuid}) is for a validation not an actual submission.")
-            if submission_uuid := submission_parameters.get("submission_uuid"):
-                PRINT(f"▶ Perhaps you meant to use the submission ID"
-                      f" associated with this: {submission_uuid}")  # noqa
-            exit(1)
-
-    do_any_uploads(response,
-                   keydict=portal.key,
-                   ingestion_filename=bundle_filename,
-                   upload_folder=upload_folder,
-                   no_query=no_query,
-                   subfolders=subfolders,
-                   portal=portal)
-
-
-@function_cache(serialize_key=True)
-def _get_health_page(key: dict) -> dict:
-    return Portal(key).get_health().json()
+    do_any_uploads(uuid,
+                   metadata_file=bundle_filename,
+                   main_search_directory=upload_folder,
+                   main_search_directory_recursively=subfolders,
+                   config_google=rclone_config_google,
+                   portal=portal,
+                   verbose=verbose)
 
 
 def get_metadata_bundles_bucket_from_health_path(key: dict) -> str:
-    return _get_health_page(key=key).get("metadata_bundles_bucket")
-
-
-def get_s3_encrypt_key_id_from_health_page(auth):
-    try:
-        return _get_health_page(key=auth).get(HealthPageKey.S3_ENCRYPT_KEY_ID)
-    except Exception:  # pragma: no cover
-        # We don't actually unit test this section because _get_health_page realistically always returns
-        # a dictionary, and so health.get(...) always succeeds, possibly returning None, which should
-        # already be tested. Returning None here amounts to the same and needs no extra unit testing.
-        # The presence of this error clause is largely pro forma and probably not really needed.
-        return None
-
-
-def get_s3_encrypt_key_id(*, upload_credentials, auth):
-    if 's3_encrypt_key_id' in upload_credentials:
-        s3_encrypt_key_id = upload_credentials.get('s3_encrypt_key_id')
-        if DEBUG_PROTOCOL:  # pragma: no cover
-            PRINT(f"Extracted s3_encrypt_key_id from upload_credentials: {s3_encrypt_key_id}")
-    else:
-        if DEBUG_PROTOCOL:  # pragma: no cover
-            PRINT(f"No s3_encrypt_key_id entry found in upload_credentials.")
-            PRINT(f"Fetching s3_encrypt_key_id from health page.")
-        s3_encrypt_key_id = get_s3_encrypt_key_id_from_health_page(auth)
-        if DEBUG_PROTOCOL:  # pragma: no cover
-            PRINT(f" =id=> {s3_encrypt_key_id!r}")
-    return s3_encrypt_key_id
-
-
-def execute_prearranged_upload(path, upload_credentials, auth=None):
-    """
-    This performs a file upload using special credentials received from ff_utils.patch_metadata.
-
-    :param path: the name of a local file to upload
-    :param upload_credentials: a dictionary of credentials to be used for the upload,
-        containing the keys 'AccessKeyId', 'SecretAccessKey', 'SessionToken', and 'upload_url'.
-    :param auth: auth info in the form of a dictionary containing 'key', 'secret', and 'server',
-        and possibly other useful information such as an encryption key id.
-    """
-
-    if DEBUG_PROTOCOL:  # pragma: no cover
-        PRINT(f"Upload credentials contain {conjoined_list(list(upload_credentials.keys()))}.")
-    try:
-        s3_uri = upload_credentials["upload_url"]
-        aws_credentials = {
-            "AWS_ACCESS_KEY_ID": upload_credentials["AccessKeyId"],
-            "AWS_SECRET_ACCESS_KEY": upload_credentials["SecretAccessKey"],
-            "AWS_SECURITY_TOKEN": upload_credentials["SessionToken"]
-        }
-        aws_kms_key_id = get_s3_encrypt_key_id(upload_credentials=upload_credentials, auth=auth)
-    except Exception as e:
-        raise ValueError("Upload specification is not in good form. %s: %s" % (e.__class__.__name__, e))
-
-    upload_file_to_aws_s3(file=path,
-                          s3_uri=s3_uri,
-                          aws_credentials=aws_credentials,
-                          aws_kms_key_id=aws_kms_key_id,
-                          print_progress=True,
-                          print_function=PRINT,
-                          verify_upload=True,
-                          catch_interrupt=True)
-
-
-def _running_on_windows_native():
-    return os.name == 'nt'
-
-
-def compute_file_post_data(filename, context_attributes):
-    file_basename = os.path.basename(filename)
-    _, ext = os.path.splitext(file_basename)  # could probably get a nicer error message if file in bad format
-    file_format = remove_prefix('.', ext, required=True)
-    return {
-        'filename': file_basename,
-        'file_format': file_format,
-        **{attr: val for attr, val in context_attributes.items() if val}
-    }
-
-
-def upload_file_to_new_uuid(filename, schema_name, auth, **context_attributes):
-    """
-    Upload file to a target environment.
-
-    :param filename: the name of a file to upload.
-    :param schema_name: the schema_name to use when creating a new file item whose content is to be uploaded.
-    :param auth: auth info in the form of a dictionary containing 'key', 'secret', and 'server'.
-    :returns: item metadata dict or None
-    """
-
-    post_item = compute_file_post_data(filename=filename, context_attributes=context_attributes)
-
-    if DEBUG_PROTOCOL:  # pragma: no cover
-        SHOW("Creating FileOther type object ...")
-    response = Portal(auth).post_metadata(object_type=schema_name, data=post_item)
-    if DEBUG_PROTOCOL:  # pragma: no cover
-        type_object_message = f" {response.get('@graph', [{'uuid': 'not-found'}])[0].get('uuid', 'not-found')}"
-        SHOW(f"Created FileOther type object: {type_object_message}")
-
-    metadata, upload_credentials = extract_metadata_and_upload_credentials(response,
-                                                                           method='POST', schema_name=schema_name,
-                                                                           filename=filename, payload_data=post_item)
-
-    execute_prearranged_upload(filename, upload_credentials=upload_credentials, auth=auth)
-
-    return metadata
-
-
-def upload_file_to_uuid(filename, uuid, auth, first_time=False, portal=None):
-    """
-    Upload file to a target environment.
-
-    :param filename: the name of a file to upload.
-    :param uuid: the item into which the filename is to be uploaded.
-    :param auth: auth info in the form of a dictionary containing 'key', 'secret', and 'server'.
-    :returns: item metadata dict or None
-    """
-    metadata = None
-    ignorable(metadata)  # PyCharm might need this if it worries it isn't set below
-
-    # filename here should not include path
-    patch_data = {'filename': os.path.basename(filename)}
-
-    response = Portal(auth).patch_metadata(object_id=uuid, data=patch_data)
-
-    metadata, upload_credentials = extract_metadata_and_upload_credentials(response,
-                                                                           method='PATCH', uuid=uuid,
-                                                                           filename=filename,
-                                                                           payload_data=patch_data,
-                                                                           portal=portal)
-
-    if first_time:
-        if upload_url := upload_credentials.get('upload_url'):
-            s3_bucket, _ = get_s3_bucket_and_key_from_s3_uri(upload_url)
-            if s3_bucket:
-                # This assumes all files are going to the same bucket;
-                # which I think is a pretty solid assumption.
-                PRINT(f"Upload file destination AWS S3 bucket: {s3_bucket}")
-    execute_prearranged_upload(filename, upload_credentials=upload_credentials, auth=auth)
-
-    return metadata
-
-
-def extract_metadata_and_upload_credentials(response, filename, method, payload_data,
-                                            uuid=None, schema_name=None, portal=None):
-    try:
-        [metadata] = response['@graph']
-        upload_credentials = metadata['upload_credentials']
-    except Exception as e:
-        if DEBUG_PROTOCOL:  # pragma: no cover
-            PRINT(f"Problem trying to {method} to get upload credentials.")
-            PRINT(f" payload_data={payload_data}")
-            if uuid:
-                PRINT(f" uuid={uuid}")
-            if schema_name:
-                PRINT(f" schema_name={schema_name}")
-            PRINT(f" response={response}")
-            PRINT(f"Got error {type(e)}: {e}")
-        file_status = None
-        if portal and uuid:
-            try:
-                file_status = portal.get_metadata(uuid).get("status")
-            except Exception:
-                pass
-        message = f"Unable to obtain upload credentials for file {filename}."
-        if file_status:
-            message += f" File status: {file_status}"
-        raise RuntimeError(message)
-    return metadata, upload_credentials
+    return get_health_page(key=key).get("metadata_bundles_bucket")
 
 
 # This can be set to True in unusual situations, but normally will be False to avoid unnecessary querying.
 SUBMITR_SELECTIVE_UPLOADS = environ_bool("SUBMITR_SELECTIVE_UPLOADS")
 
 
-def do_uploads(upload_spec_list, auth, folder=None, no_query=False, subfolders=False, portal=None):
-    """
-    Uploads the files mentioned in the give upload_spec_list.
-
-    If any files have associated extra files, upload those as well.
-
-    :param upload_spec_list: a list of upload_spec dictionaries, each of the form {'filename': ..., 'uuid': ...},
-        representing uploads to be formed.
-    :param auth: a dictionary-form auth spec, of the form {'key': ..., 'secret': ..., 'server': ...}
-        representing destination and credentials.
-    :param folder: a string naming a folder in which to find the filenames to be uploaded.
-    :param no_query: bool to suppress requests for user input
-    :param subfolders: bool to search subdirectories within upload_folder for files
-    :return: None
-    """
-    folder = folder or os.path.curdir
-    if subfolders:
-        folder = os.path.join(folder, '**')
-    first_time = True
-    for upload_spec in upload_spec_list:
-        file_name = upload_spec["filename"]
-        if not (file_paths := search_for_file(file_name, location=folder, recursive=subfolders)) or len(file_paths) > 1:
-            if len(file_paths) > 1:
-                SHOW(f"No upload attempted for file {file_name} because multiple copies"
-                     f" were found in folder {folder}: {', '.join(file_paths)}.")
-            else:
-                SHOW(f"Upload file not found: {file_name}")
-            continue
-        file_path = file_paths[0]
-        uuid = upload_spec['uuid']
-        uploader_wrapper = UploadMessageWrapper(uuid, no_query=no_query)
-        wrapped_upload_file_to_uuid = uploader_wrapper.wrap_upload_function(
-            upload_file_to_uuid, file_path
-        )
-        file_metadata = wrapped_upload_file_to_uuid(
-            filename=file_path, uuid=uuid, auth=auth, first_time=first_time, portal=portal
-        )
-        if file_metadata:
-            extra_files_credentials = file_metadata.get("extra_files_creds", [])
-            if extra_files_credentials:
-                _upload_extra_files(
-                    extra_files_credentials,
-                    uploader_wrapper,
-                    folder,
-                    auth,
-                    recursive=subfolders,
-                )
-        first_time = False
-
-
-class UploadMessageWrapper:
-    """Class to provide consistent queries/messages to user when
-    uploading file(s) to given File UUID.
-    """
-
-    def __init__(self, uuid, no_query=False):
-        """Initialize instance for given UUID
-
-        :param uuid: UUID of File item for uploads
-        :param no_query: Whether to suppress asking for user
-            confirmation prior to upload
-        """
-        self.uuid = uuid
-        self.no_query = no_query
-
-    def wrap_upload_function(self, function, file_name):
-        """Wrap upload given function with messages conerning upload.
-
-        :param function: Upload function to wrap
-        :param file_name: File to upload
-        :returns: Wrapped function
-        """
-        def wrapper(*args, **kwargs):
-            result = None
-            perform_upload = True
-            if not self.no_query:
-                if (
-                    SUBMITR_SELECTIVE_UPLOADS
-                    and not yes_or_no(f"Upload {file_name}?")
-                ):
-                    SHOW("OK, not uploading it.")
-                    perform_upload = False
-            if perform_upload:
-                try:
-                    result = function(*args, **kwargs)
-                except Exception as e:
-                    SHOW("%s: %s" % (e.__class__.__name__, e))
-            return result
-        return wrapper
-
-
-def _upload_extra_files(
-    credentials, uploader_wrapper, folder, auth, recursive=False
-):
-    """Attempt upload of all extra files.
-
-    Similar to "do_uploads", search for each file and then call a
-    wrapped upload function. Here, since extra files do not correspond
-    to Items on the portal, no need to PATCH an Item to retrieve AWS
-    credentials; they are directly passed in from the parent File's
-    metadata.
-
-    :param credentials: AWS credentials dictionary
-    :param uploader_wrapper: UploadMessageWrapper instance
-    :param folder: Directory to search for files
-    :param auth: a portal authorization tuple
-    :param recursive: Whether to search subdirectories for file
-    """
-    for extra_file_item in credentials:
-        extra_file_name = extra_file_item.get("filename")
-        extra_file_credentials = extra_file_item.get("upload_credentials")
-        if not extra_file_name or not extra_file_credentials:
-            continue
-        if (not (extra_file_paths := search_for_file(extra_file_name, location=folder,
-                                                     recursive=recursive)) or len(extra_file_paths) > 1):
-            if len(extra_file_paths) > 1:
-                SHOW(f"No upload attempted for file {extra_file_name} because multiple"
-                     f" copies were found in folder {folder}: {', '.join(extra_file_paths)}.")
-            else:
-                SHOW(f"Upload file not found: {extra_file_name}")
-            continue
-        extra_file_path = extra_file_paths[0]
-        wrapped_execute_prearranged_upload = uploader_wrapper.wrap_upload_function(
-            execute_prearranged_upload, extra_file_path
-        )
-        wrapped_execute_prearranged_upload(extra_file_path, extra_file_credentials, auth=auth)
-
-
-def _upload_item_data(item_filename, uuid, server, env, directory=None, recursive=False,
-                      no_query=False, app=None, report=True):
-    """
-    Given a part_filename, uploads that filename to the Item specified by uuid on the given server.
-
-    Only one of server or env may be specified.
-
-    :param item_filename: the name of a file to be uploaded
-    :param uuid: the UUID of the Item with which the uploaded data is to be associated
-    :param server: the server to upload to (where the Item is defined)
-    :param env: the portal environment to upload to (where the Item is defined)
-    :param no_query: bool to suppress requests for user input
-    :return:
-    """
-
-    # Allow the given "file name" to be uuid for submitted File object, or associated accession
-    # ID (e.g. SMAFIP2PIEDG), or the (S3) accession ID based file name (e.g. SMAFIP2PIEDG.fastq).
-    if not uuid:
-        if is_uuid(item_filename) or _is_accession_id(item_filename):
-            uuid = item_filename
-            item_filename = None
-        elif accession_id := _extract_accession_id(item_filename):
-            uuid = accession_id
-            item_filename = None
-
-    portal = _define_portal(env=env, server=server, app=app, report=report)
-
-    if not (uuid_metadata := portal.get_metadata(uuid)):
-        raise Exception(f"Cannot find object given uuid: {uuid}")
-
-    if not portal.is_schema_file_type(uuid_metadata):
-        undesired_type = portal.get_schema_type(uuid_metadata)
-        raise Exception(f"Given uuid is not a file type: {uuid} ({undesired_type})")
-
-    if not item_filename:
-        if not (item_filename := uuid_metadata.get("filename")):
-            raise Exception(f"Cannot determine file name: {uuid}")
-
-    if not (item_filename_found := search_for_file(item_filename, location=directory,
-                                                   recursive=recursive, single=True)):
-        raise Exception(f"File not found: {item_filename}")
-    else:
-        PRINT(f"File to upload to AWS S3: {format_path(item_filename_found)}")
-        item_filename = item_filename_found
-
-    if not no_query:
-        file_size = format_size(get_file_size(item_filename))
-        if not yes_or_no(f"Upload {format_path(item_filename)} ({file_size}) to {server}?"):
-            SHOW("Aborting submission.")
-            exit(1)
-
-    upload_file_to_uuid(filename=item_filename, uuid=uuid, auth=portal.key, portal=portal)
-
-
-def _show_detailed_results(uuid: str, metadata_bundles_bucket: str) -> None:
-
-    PRINT(f"----- Detailed Info -----")
-
-    submission_results_location, submission_results = _fetch_submission_results(metadata_bundles_bucket, uuid)
-    exception_results_location, exception_results = _fetch_exception_results(metadata_bundles_bucket, uuid)
-
-    if not submission_results and not exception_results:
-        PRINT(f"Neither submission nor exception results found!")
-        PRINT(f"-> {submission_results_location}")
-        PRINT(f"-> {exception_results_location}")
-        return
-
-    if submission_results:
-        PRINT(f"From: {submission_results_location}")
-        PRINT(yaml.dump(submission_results))
-
-    if exception_results:
-        PRINT("Exception during schema ingestion processing:")
-        PRINT(f"From: {exception_results_location}")
-        PRINT(exception_results)
-
-
 def _fetch_submission_results(metadata_bundles_bucket: str, uuid: str) -> Optional[Tuple[str, dict]]:
     return _fetch_results(metadata_bundles_bucket, uuid, "submission.json")
 
 
 def _fetch_exception_results(metadata_bundles_bucket: str, uuid: str) -> Optional[Tuple[str, str]]:
     return _fetch_results(metadata_bundles_bucket, uuid, "traceback.txt")
 
@@ -2573,18 +1907,14 @@
         else:
             if not verbose:
                 PRINT_STDOUT()
             PRINT_STDOUT(f"Exiting with preliminary validation errors.")
             PRINT_STDOUT("Use the --output FILE option to write errors to a file.")
         exit(1)
 
-    # They don't want to present upload file info on validate, only on submit.
-    # _review_upload_files(structured_data, ingestion_filename,
-    #                      validation=validation, directory=upload_folder, recursive=subfolders)
-
     if verbose:
         _print_structured_data_verbose(portal, structured_data, ingestion_filename, upload_folder=upload_folder,
                                        recursive=subfolders, validation=validation, verbose=verbose)
     elif not quiet:
         if not noanalyze:
             _print_structured_data_status(portal, structured_data, validation=validation,
                                           report_updates_only=True, noprogress=noprogress, verbose=verbose, debug=debug)
@@ -2597,48 +1927,14 @@
     if validate_local_only:
         PRINT("Terminating as requested (per --validate-local-only).")
         exit(0 if validation_okay else 1)
 
     return structured_data
 
 
-def _review_upload_files(structured_data: StructuredDataSet, ingestion_filename: str, validation: bool = False,
-                         directory: Optional[str] = None, recursive: bool = False) -> None:
-
-    nfiles_found, file_validation_errors = _validate_files(structured_data, ingestion_filename,
-                                                           upload_folder=directory, recursive=recursive)
-    if file_validation_errors:
-        nfiles = len(file_validation_errors)
-        if nfiles_found > 0:
-            PRINT(f"WARNING: There {'is' if nfiles == 1 else 'are'} {nfiles}"
-                  f" file{'' if nfiles == 1 else 's'} referenced which are missing.")
-        else:
-            PRINT(f"WARNING: All {nfiles} file{'' if nfiles == 1 else 's'} are missing.")
-        if not (show_missing_files := (nfiles <= 3)):
-            show_missing_files = yes_or_no(f"Do you want to see a list of these {nfiles}"
-                                           f" missing file{'' if nfiles == 1 else 's'}?")
-        if show_missing_files:
-            for error in sorted(file_validation_errors):
-                PRINT(f"- {error}")
-        if nfiles_found == 0:
-            PRINT("No files found for upload.")
-            exit(1)
-        if not validation:
-            if not yes_or_no(f"Do you want to continue even with"
-                             f" {'this' if nfiles == 1 else 'these'} missing file{'' if nfiles == 1 else 's'}?"):
-                exit(1)
-        else:
-            PRINT(f"Continuing even with {'this' if nfiles == 1 else 'these'}"
-                  f" missing file{'' if nfiles == 1 else 's'} as noted above.")
-    if nfiles_found > 0:
-        PRINT(f"Files referenced for upload (and which exist): {nfiles_found}")
-    elif not file_validation_errors:
-        PRINT("No files to upload were referenced.")
-
-
 def _validate_data(structured_data: StructuredDataSet, portal: Portal, ingestion_filename: str,
                    upload_folder: str, recursive: bool, verbose: bool = False, debug: bool = False) -> bool:
     nerrors = 0
 
     if initial_validation_errors := _validate_initial(structured_data, portal):
         nerrors += len(initial_validation_errors)
 
@@ -2757,26 +2053,14 @@
                 else:
                     errors.append(f"  - ERROR: {ref_error['ref']}")
             if truncated:
                 errors.append(f"  - {truncated}")
     return errors
 
 
-def _validate_files(structured_data: StructuredDataSet, ingestion_filename: str,
-                    upload_folder: str, recursive: bool) -> Tuple[int, List[str]]:
-    file_validation_errors = []
-    if files := structured_data.upload_files_located(location=[upload_folder,
-                                                               os.path.dirname(ingestion_filename) or "."],
-                                                     recursive=recursive):
-        if files_not_found := [file for file in files if not file.get("path")]:
-            for file in sorted(files_not_found, key=lambda key: key.get("file")):
-                file_validation_errors.append(f"{file.get('file')} -> File not found ({file.get('type')})")
-    return len(files) - len(file_validation_errors), sorted(file_validation_errors)
-
-
 def _validate_initial(structured_data: StructuredDataSet, portal: Portal) -> List[str]:
     # TODO: Move this more specific "pre" validation checking to dcicutils.structured_data.
     # Just for nicer more specific (non-jsonschema) error messages for common problems.
     initial_validation_errors = []
     if not (portal and structured_data and structured_data.data):
         return initial_validation_errors
     for schema_name in structured_data.data:
@@ -2805,22 +2089,24 @@
 def _print_structured_data_verbose(portal: Portal, structured_data: StructuredDataSet, ingestion_filename: str,
                                    upload_folder: str, recursive: bool, validation: bool = False,
                                    noanalyze: bool = False, noprogress: bool = False, verbose: bool = False) -> None:
     if (reader_warnings := structured_data.reader_warnings):
         PRINT_OUTPUT(f"\n> Parser warnings:")
         for reader_warning in reader_warnings:
             PRINT_OUTPUT(f"  - {_format_issue(reader_warning, ingestion_filename)}")
-    PRINT_OUTPUT(f"\n> Types submitting:")
-    for type_name in sorted(structured_data.data):
-        PRINT_OUTPUT(f"  - {type_name}: {len(structured_data.data[type_name])}"
-                     f" object{'s' if len(structured_data.data[type_name]) != 1 else ''}")
+    if structured_data.data:
+        PRINT_OUTPUT(f"\n> Types submitting:")
+        for type_name in sorted(structured_data.data):
+            PRINT_OUTPUT(f"  - {type_name}: {len(structured_data.data[type_name])}"
+                         f" object{'s' if len(structured_data.data[type_name]) != 1 else ''}")
     if resolved_refs := structured_data.resolved_refs:
         PRINT_OUTPUT(f"\n> Resolved object (linkTo) references:")
         for resolved_ref in sorted(resolved_refs):
             PRINT_OUTPUT(f"  - {resolved_ref}")
+    # TODO: replace with FilesForUpload
     if files := structured_data.upload_files_located(location=[upload_folder,
                                                                os.path.dirname(ingestion_filename) or "."],
                                                      recursive=recursive):
         printed_header = False
         if files_found := [file for file in files if file.get("path")]:
             for file in files_found:
                 path = file.get("path")
@@ -3146,43 +2432,31 @@
         for submission_center in submission_centers:
             if ((submission_center_name := submission_center.get("identifier")) and
                 (submission_center_uuid := submission_center.get("uuid"))):  # noqa
                 results.append({"name": submission_center_name, "uuid": submission_center_uuid})
     return results
 
 
-def _is_accession_id(value: str) -> bool:
-    # See smaht-portal/.../schema_formats.py
-    return isinstance(value, str) and re.match(r"^SMA[1-9A-Z]{9}$", value) is not None
-    # return isinstance(value, str) and re.match(r"^[A-Z0-9]{12}$", value) is not None
-
-
-def _extract_accession_id(value: str) -> Optional[str]:
-    if isinstance(value, str):
-        if value.endswith(".gz"):
-            value = value[:-3]
-        value, _ = os.path.splitext(value)
-        if _is_accession_id(value):
-            return value
-
-
 def _print_metadata_file_info(file: str, env: str,
                               refs: bool = False, files: bool = False,
+                              upload_folder: Optional[str] = None,
+                              subfolders: bool = False,
+                              rclone_config_google: Optional[RCloneConfigGoogle] = None,
                               output_file: Optional[str] = None,
                               verbose: bool = False) -> None:
     if output_file:
         set_output_file(output_file)
     PRINT(f"Metadata File: {os.path.basename(file)}")
     if size := get_file_size(file):
         PRINT(f"Size: {format_size(size)} ({size})")
     if modified := get_file_modified_datetime(file):
         PRINT(f"Modified: {modified}")
-    if md5 := get_file_md5(file):
+    if md5 := compute_file_md5(file):
         PRINT(f"MD5: {md5}")
-    if (etag := get_file_md5_like_aws_s3_etag(file)) and etag != md5:
+    if (etag := compute_file_etag(file)) and etag != md5:
         PRINT(f"S3 ETag: {etag}")
     sheet_lines = []
     if is_excel_file_name(file):
         excel = Excel(file)
         nrows_total = 0
         for sheet_name in sorted(excel.sheet_names):
             nrows = excel.sheet_reader(sheet_name).nrows
@@ -3216,31 +2490,19 @@
                         for src in srcs:
                             printf(f"  - {_format_src(src)}")
                             note_output()
             unchecked_refs = structured_data.unchecked_refs
             PRINT(f"References: {len(unchecked_refs)}")
             print_refs(unchecked_refs, max_output=max_output, output_file=output_file, verbose=verbose)
         if files is True:
-            def print_files(files: List[dict], max_output: int, output_file: str, verbose: bool = False) -> None:
-                def note_output():
-                    nonlocal max_output, output_file, noutput, printf, truncated
-                    noutput += 1
-                    if noutput >= max_output and output_file and not truncated:
-                        PRINT_STDOUT(f"+ Truncated results | See your output file for full listing: {output_file}")
-                        printf = PRINT_OUTPUT
-                        truncated = True
-                printf = PRINT
-                noutput = 0
-                truncated = False
-                for file in sorted(files, key=lambda file: file["file"]):
-                    printf(f"- {file['file']} ({file['type']})")
-                    note_output()
-            upload_files = structured_data.upload_files
-            PRINT(f"Files: {len(upload_files)}")
-            print_files(upload_files, max_output=max_output, output_file=output_file, verbose=verbose)
+            files_for_upload = FilesForUpload.assemble(structured_data,
+                                                       main_search_directory=upload_folder,
+                                                       main_search_directory_recursively=subfolders,
+                                                       config_google=rclone_config_google)
+            FilesForUpload.review(files_for_upload, portal=portal, review_only=True, verbose=True, printf=PRINT)
     if not (refs is True):
         if not (files is True):
             PRINT("Note: Use --refs to view references; and --files to view files for upload.")
         else:
             PRINT("Note: Use --refs to view references (linkTo) paths.")
     elif not (files is True):
         PRINT("Note: Use --files to view files for upload.")
```

### Comparing `smaht_submitr-0.8.1/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.8.2.1b3/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.8.2.1b3/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.8.2.1b3/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.8.2.1b3/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_base.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_check_submission.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_exceptions.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_misc.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_resume_uploads.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dcicutils.tmpfile_utils import temporary_directory
 from ..scripts.resume_uploads import main as resume_uploads_main
 from ..scripts import resume_uploads as resume_uploads_module
 from .testing_helpers import system_exit_expected, argparse_errors_muffled
 
 
 @pytest.mark.parametrize("keyfile", [None, "foo.bar"])
-def test_resume_uploads_script(keyfile):
+def need_to_replace_with_new_version_resume_uploads_script(keyfile):
 
     def test_it(args_in, expect_exit_code, expect_called, expect_call_args=None, expect_output=[]):
         output = []
         with argparse_errors_muffled():
             with temporary_directory() as tmpdir:
                 open(os.path.join(tmpdir, "some.file"), "w")
                 os.mkdir(os.path.join(tmpdir, "a-folder"))
@@ -163,15 +163,15 @@
     "@type": "IngestionSubmission",
     "additional_data": {
         "upload_info": SAMPLE_UPLOAD_INFO
     }
 }
 
 
-def test_c4_383_regression_action():
+def need_to_replace_with_new_version_c4_383_regression_action():
     """
     Check that bug C4-383 is really fixed.
 
     This bug involves resume_uploads not merging the uploaded file against the current directory
     when no bundle or upload_folder is given. The present behavior is to merge against
     the parent directory.
     """
@@ -226,9 +226,10 @@
                                         joined_filename = os.path.join(current_dir, SAMPLE_UPLOAD_INFO[-1]['filename'])
                                         # Make sure this is doing what we expect.
                                         assert current_dir + "/" in joined_filename
                                         # Make sure the inner upload actually uploads to the current dir.
                                         mock_upload_file_to_uuid.assert_called_with(auth=fake_keydict,
                                                                                     filename=joined_filename,
                                                                                     uuid=SAMPLE_UPLOAD_INFO[-1]['uuid'],
+                                                                                    rclone_config_google=None,
                                                                                     first_time=False, portal=mock.ANY)
                                         assert output == []
```

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/test_utils.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/tests/testing_helpers.py` & `smaht_submitr-0.8.2.1b3/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.1/submitr/utils.py` & `smaht_submitr-0.8.2.1b3/submitr/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from collections import namedtuple
 from contextlib import contextmanager
 from datetime import datetime
 from functools import lru_cache
 import io
 from json import dumps as json_dumps, loads as json_loads
-import hashlib
 import os
 from pathlib import Path
 import pkg_resources
 import re
 import requests
 from signal import signal, SIGINT
 import string
 from typing import Any, Callable, List, Optional, Tuple
-from dcicutils.misc_utils import PRINT, str_to_bool
 from dcicutils.datetime_utils import format_datetime, parse_datetime
+from dcicutils.function_cache_decorator import function_cache
+from dcicutils.misc_utils import PRINT, str_to_bool
+from dcicutils.structured_data import Portal
 
 
 ERASE_LINE = "\033[K"
 TIMESTAMP_PATTERN = "%H:%M:%S"
 TIMESTAMP_REGEXP = "[0-2][0-9]:[0-5][0-9]:[0-5][0-9]"
 
 
@@ -108,99 +109,14 @@
 
 def format_path(path: str) -> str:
     if isinstance(path, str) and os.path.isabs(path) and path.startswith(os.path.expanduser("~")):
         path = "~/" + Path(path).relative_to(Path.home()).as_posix()
     return path
 
 
-def get_file_size(file: str) -> int:
-    try:
-        return os.path.getsize(file) if isinstance(file, str) else ""
-    except Exception:
-        return -1
-
-
-def get_file_modified_datetime(file: str) -> str:
-    try:
-        return format_datetime(datetime.fromtimestamp(os.path.getmtime(file)))
-    except Exception:
-        return ""
-
-
-def get_file_checksum(file: str) -> str:
-    return get_file_md5_like_aws_s3_etag(file)
-
-
-def get_file_md5(file: str) -> str:
-    if not isinstance(file, str):
-        return ""
-    try:
-        md5 = hashlib.md5()
-        with open(file, "rb") as file:
-            for chunk in iter(lambda: file.read(4096), b""):
-                md5.update(chunk)
-        return md5.hexdigest()
-    except Exception:
-        return ""
-
-
-def get_file_md5_like_aws_s3_etag(file: str) -> Optional[str]:
-    try:
-        with io.open(file, "rb") as f:
-            return _get_file_md5_like_aws_s3_etag(f)
-    except Exception:
-        return None
-
-
-def _get_file_md5_like_aws_s3_etag(f: io.BufferedReader) -> str:
-    """
-    Returns the AWS S3 "Etag" for the given file; this value is md5-like but
-    not the same as a normal md5. We use this to compare that a file in S3
-    appears to be the exact the same file as a local file. Adapted from:
-    https://stackoverflow.com/questions/75723647/calculate-md5-from-aws-s3-etag
-    """
-    MULTIPART_THRESHOLD = 8388608
-    MULTIPART_CHUNKSIZE = 8388608
-    # BUFFER_SIZE = 1048576
-    # Verify some assumptions are correct
-    # assert(MULTIPART_CHUNKSIZE >= MULTIPART_THRESHOLD)
-    # assert((MULTIPART_THRESHOLD % BUFFER_SIZE) == 0)
-    # assert((MULTIPART_CHUNKSIZE % BUFFER_SIZE) == 0)
-    hash = hashlib.md5()
-    read = 0
-    chunks = None
-    while True:
-        # Read some from stdin, if we're at the end, stop reading
-        bits = f.read(1048576)
-        if len(bits) == 0:
-            break
-        read += len(bits)
-        hash.update(bits)
-        if chunks is None:
-            # We're handling a multi-part upload, so switch to calculating
-            # hashes of each chunk
-            if read >= MULTIPART_THRESHOLD:
-                chunks = b''
-        if chunks is not None:
-            if (read % MULTIPART_CHUNKSIZE) == 0:
-                # Dont with a chunk, add it to the list of hashes to hash later
-                chunks += hash.digest()
-                hash = hashlib.md5()
-    if chunks is None:
-        # Normal upload, just output the MD5 hash
-        etag = hash.hexdigest()
-    else:
-        # Multipart upload, need to output the hash of the hashes
-        if (read % MULTIPART_CHUNKSIZE) != 0:
-            # Add the last part if we have a partial chunk
-            chunks += hash.digest()
-        etag = hashlib.md5(chunks).hexdigest() + "-" + str(len(chunks) // 16)
-    return etag
-
-
 def print_boxed(lines: List[str], right_justified_macro: Optional[Tuple[str, Callable]] = None,
                 printf: Optional[Callable] = PRINT) -> None:
     macro_name = None
     macro_value = None
     if right_justified_macro and (len(right_justified_macro) == 2):
         macro_name = right_justified_macro[0]
         macro_value = right_justified_macro[1]()
@@ -300,7 +216,12 @@
             if on_interrupt() is False:
                 exit(1)
     try:
         previous_interrupt_handler = signal(SIGINT, interrupt_handler)
         yield
     finally:
         signal(SIGINT, previous_interrupt_handler)
+
+
+@function_cache(serialize_key=True)
+def get_health_page(key: dict) -> dict:
+    return Portal(key).get_health().json()
```

### Comparing `smaht_submitr-0.8.1/PKG-INFO` & `smaht_submitr-0.8.2.1b3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.8.1
+Version: 0.8.2.1b3
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
-Requires-Python: >=3.8.0,<3.12
+Requires-Python: >=3.8.0,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
-Requires-Dist: awscli (>=1.32.81)
-Requires-Dist: boto3 (>=1.34.81,<2.0.0)
-Requires-Dist: dcicutils (>=8.8.4,<9.0.0)
+Requires-Dist: awscli (>=1.32.105)
+Requires-Dist: boto3 (>=1.34.105,<2.0.0)
+Requires-Dist: dcicutils (>=8.8.4.1b31,<9.0.0.0)
 Requires-Dist: googleapi (>=0.1.0,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/smaht-dac/submitr.git
 Description-Content-Type: text/x-rst
 
 
 .. image:: https://staging.smaht.org/static/img/docs/submitr_logo.png
```

