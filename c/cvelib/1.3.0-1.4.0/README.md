# Comparing `tmp/cvelib-1.3.0.tar.gz` & `tmp/cvelib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvelib-1.3.0.tar", last modified: Fri Jan 26 20:11:30 2024, max compression
+gzip compressed data, was "cvelib-1.4.0.tar", last modified: Wed May 15 18:10:52 2024, max compression
```

## Comparing `cvelib-1.3.0.tar` & `cvelib-1.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-01-26 20:11:30.925505 cvelib-1.3.0/
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     4279 2024-01-26 20:11:12.000000 cvelib-1.3.0/CHANGELOG.md
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1070 2023-06-13 00:28:29.000000 cvelib-1.3.0/LICENSE
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      153 2023-06-13 00:28:29.000000 cvelib-1.3.0/MANIFEST.in
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     9693 2024-01-26 20:11:30.924505 cvelib-1.3.0/PKG-INFO
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     8451 2024-01-26 20:11:12.000000 cvelib-1.3.0/README.md
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      498 2023-06-13 00:28:29.000000 cvelib-1.3.0/SECURITY.md
-drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-01-26 20:11:30.920505 cvelib-1.3.0/cvelib/
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)       22 2024-01-26 20:11:12.000000 cvelib-1.3.0/cvelib/__init__.py
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)    40200 2024-01-26 19:29:07.000000 cvelib-1.3.0/cvelib/cli.py
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)    12870 2024-01-17 13:19:40.000000 cvelib-1.3.0/cvelib/cve_api.py
-drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-01-26 20:11:30.921505 cvelib-1.3.0/cvelib/schemas/
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)    84947 2023-06-13 00:28:29.000000 cvelib-1.3.0/cvelib/schemas/CVE_JSON_5.0_bundled_5.0.0.json
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      541 2023-06-13 00:28:29.000000 cvelib-1.3.0/cvelib/schemas/README.md
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)    69013 2023-06-13 00:28:29.000000 cvelib-1.3.0/cvelib/schemas/adp_container_5.0.0.json
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     3607 2023-06-13 00:28:29.000000 cvelib-1.3.0/cvelib/schemas/extract_container_schemas.py
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)    70092 2023-06-13 00:28:29.000000 cvelib-1.3.0/cvelib/schemas/published_cna_container_5.0.0.json
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     6968 2023-06-13 00:28:29.000000 cvelib-1.3.0/cvelib/schemas/rejected_cna_container_5.0.0.json
-drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-01-26 20:11:30.924505 cvelib-1.3.0/cvelib.egg-info/
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     9693 2024-01-26 20:11:30.000000 cvelib-1.3.0/cvelib.egg-info/PKG-INFO
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1071 2024-01-26 20:11:30.000000 cvelib-1.3.0/cvelib.egg-info/SOURCES.txt
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)        1 2024-01-26 20:11:30.000000 cvelib-1.3.0/cvelib.egg-info/dependency_links.txt
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)       39 2024-01-26 20:11:30.000000 cvelib-1.3.0/cvelib.egg-info/entry_points.txt
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      151 2024-01-26 20:11:30.000000 cvelib-1.3.0/cvelib.egg-info/requires.txt
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)       27 2024-01-26 20:11:30.000000 cvelib-1.3.0/cvelib.egg-info/top_level.txt
-drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-01-26 20:11:30.923505 cvelib-1.3.0/man/
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      782 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-list.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      344 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-org-users.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      428 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-org.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      223 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-ping.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1358 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-publish-adp.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1585 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-publish.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      565 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-quota.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1583 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-reject.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      985 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-reserve.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      617 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-show.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      328 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-undo-reject.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      676 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-user-create.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      581 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-user-reset-key.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      812 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-user-update.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      808 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve-user.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     2359 2024-01-26 19:10:52.000000 cvelib-1.3.0/man/cve.1
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      403 2023-06-13 00:28:29.000000 cvelib-1.3.0/pyproject.toml
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)       38 2024-01-26 20:11:30.925505 cvelib-1.3.0/setup.cfg
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1775 2024-01-26 20:11:12.000000 cvelib-1.3.0/setup.py
-drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-01-26 20:11:30.923505 cvelib-1.3.0/tests/
-drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-01-26 20:11:30.924505 cvelib-1.3.0/tests/data/
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     9998 2023-06-13 00:28:29.000000 cvelib-1.3.0/tests/data/CVEv5_advanced-example.json
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1555 2023-06-13 00:28:29.000000 cvelib-1.3.0/tests/data/CVEv5_basic-example.json
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)      618 2023-07-20 13:23:25.000000 cvelib-1.3.0/tests/data/README.md
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     8472 2023-07-20 13:23:25.000000 cvelib-1.3.0/tests/data/container-advanced-example.json
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1065 2023-07-20 13:23:25.000000 cvelib-1.3.0/tests/data/container-basic-example.json
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)    28284 2023-07-20 13:23:25.000000 cvelib-1.3.0/tests/test_cli.py
--rw-r--r--   0 mprpic    (1000) mprpic    (1000)     2158 2023-06-13 00:28:29.000000 cvelib-1.3.0/tests/test_cve_api.py
+drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-05-15 18:10:52.774517 cvelib-1.4.0/
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     4479 2024-05-15 18:10:39.000000 cvelib-1.4.0/CHANGELOG.md
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1070 2023-06-13 00:28:29.000000 cvelib-1.4.0/LICENSE
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      153 2023-06-13 00:28:29.000000 cvelib-1.4.0/MANIFEST.in
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     9719 2024-05-15 18:10:52.774517 cvelib-1.4.0/PKG-INFO
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     8477 2024-05-15 18:10:39.000000 cvelib-1.4.0/README.md
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      498 2023-06-13 00:28:29.000000 cvelib-1.4.0/SECURITY.md
+drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-05-15 18:10:52.769517 cvelib-1.4.0/cvelib/
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)       22 2024-05-15 18:10:39.000000 cvelib-1.4.0/cvelib/__init__.py
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)    40200 2024-01-26 19:29:07.000000 cvelib-1.4.0/cvelib/cli.py
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)    12888 2024-05-15 17:58:22.000000 cvelib-1.4.0/cvelib/cve_api.py
+drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-05-15 18:10:52.770517 cvelib-1.4.0/cvelib/schemas/
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)    92428 2024-05-15 17:58:22.000000 cvelib-1.4.0/cvelib/schemas/CVE_JSON_adpContainer_5.1.0.json
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)   108815 2024-05-15 17:58:22.000000 cvelib-1.4.0/cvelib/schemas/CVE_JSON_bundled_5.1.0.json
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)    93506 2024-05-15 17:58:22.000000 cvelib-1.4.0/cvelib/schemas/CVE_JSON_cnaPublishedContainer_5.1.0.json
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     7351 2024-05-15 17:58:22.000000 cvelib-1.4.0/cvelib/schemas/CVE_JSON_cnaRejectedContainer_5.1.0.json
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      494 2024-05-15 17:58:22.000000 cvelib-1.4.0/cvelib/schemas/README.md
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     3500 2024-05-15 17:58:22.000000 cvelib-1.4.0/cvelib/schemas/extract_container_schemas.py
+drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-05-15 18:10:52.773517 cvelib-1.4.0/cvelib.egg-info/
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     9719 2024-05-15 18:10:52.000000 cvelib-1.4.0/cvelib.egg-info/PKG-INFO
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1089 2024-05-15 18:10:52.000000 cvelib-1.4.0/cvelib.egg-info/SOURCES.txt
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)        1 2024-05-15 18:10:52.000000 cvelib-1.4.0/cvelib.egg-info/dependency_links.txt
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)       39 2024-05-15 18:10:52.000000 cvelib-1.4.0/cvelib.egg-info/entry_points.txt
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      151 2024-05-15 18:10:52.000000 cvelib-1.4.0/cvelib.egg-info/requires.txt
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)       27 2024-05-15 18:10:52.000000 cvelib-1.4.0/cvelib.egg-info/top_level.txt
+drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-05-15 18:10:52.772517 cvelib-1.4.0/man/
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      782 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-list.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      344 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-org-users.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      428 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-org.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      223 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-ping.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1358 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-publish-adp.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1585 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-publish.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      565 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-quota.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1583 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-reject.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      985 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-reserve.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      617 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-show.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      328 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-undo-reject.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      676 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-user-create.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      581 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-user-reset-key.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      812 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-user-update.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      808 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve-user.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     2359 2024-05-15 18:10:39.000000 cvelib-1.4.0/man/cve.1
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      421 2024-05-15 17:58:22.000000 cvelib-1.4.0/pyproject.toml
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)       38 2024-05-15 18:10:52.774517 cvelib-1.4.0/setup.cfg
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1775 2024-01-26 20:11:12.000000 cvelib-1.4.0/setup.py
+drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-05-15 18:10:52.772517 cvelib-1.4.0/tests/
+drwxr-xr-x   0 mprpic    (1000) mprpic    (1000)        0 2024-05-15 18:10:52.773517 cvelib-1.4.0/tests/data/
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)    10218 2024-05-15 17:58:22.000000 cvelib-1.4.0/tests/data/CVEv5_advanced-example.json
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1454 2024-05-15 17:58:22.000000 cvelib-1.4.0/tests/data/CVEv5_basic-example.json
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)      563 2024-05-15 17:58:22.000000 cvelib-1.4.0/tests/data/README.md
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     8675 2024-05-15 17:58:22.000000 cvelib-1.4.0/tests/data/container-advanced-example.json
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     1065 2024-04-24 18:00:05.000000 cvelib-1.4.0/tests/data/container-basic-example.json
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)    28284 2023-07-20 13:23:25.000000 cvelib-1.4.0/tests/test_cli.py
+-rw-r--r--   0 mprpic    (1000) mprpic    (1000)     2158 2023-06-13 00:28:29.000000 cvelib-1.4.0/tests/test_cve_api.py
```

### Comparing `cvelib-1.3.0/CHANGELOG.md` & `cvelib-1.4.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## [1.4.0](https://github.com/RedHatProductSecurity/cvelib/compare/1.3.0...1.4.0) (May 15, 2024)
+
+* Updated CVE JSON schema to version 5.1.0, which makes it compatible with CVE Services 2.3.x (#79).
+
 ## [1.3.0](https://github.com/RedHatProductSecurity/cvelib/compare/1.2.1...1.3.0) (Jan 26, 2024)
 
 * Fixed displaying timestamps for older records (#66).
 * Added auto-completion of sub-commands (#73).
 * Added support for ADP containers (#70):
   * A new `publish-adp` command is added that allows publishing of ADP containers into an existing CVE record (this is
     only possible if a CVE is in the published state).
```

### Comparing `cvelib-1.3.0/LICENSE` & `cvelib-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvelib-1.3.0/PKG-INFO` & `cvelib-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvelib
-Version: 1.3.0
+Version: 1.4.0
 Summary: A library and command line interface for the CVE Project services.
 Home-page: https://github.com/RedHatProductSecurity/cvelib
 Author: Red Hat Product Security
 Author-email: secalert@redhat.com
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
@@ -32,19 +32,19 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # cvelib
 
 A library and a command line interface for the CVE Services API.
 
-**Note**: version 1.3.0 of cvelib is compatible with CVE Services 2.2.0.
+**Note**: version 1.4.0 of cvelib is compatible with CVE Services 2.3.1 and CVE JSON schema 5.1.0.
 
 ## Requirements
 
-- Python version 3.7 or greater
+- Python version 3.8 or greater
 - [pip](https://pypi.org/project/pip/)
 
 ## Installation
 
 ### Linux, MacOS, Windows
 
 ```bash
```

### Comparing `cvelib-1.3.0/README.md` & `cvelib-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # cvelib
 
 A library and a command line interface for the CVE Services API.
 
-**Note**: version 1.3.0 of cvelib is compatible with CVE Services 2.2.0.
+**Note**: version 1.4.0 of cvelib is compatible with CVE Services 2.3.1 and CVE JSON schema 5.1.0.
 
 ## Requirements
 
-- Python version 3.7 or greater
+- Python version 3.8 or greater
 - [pip](https://pypi.org/project/pip/)
 
 ## Installation
 
 ### Linux, MacOS, Windows
 
 ```bash
```

### Comparing `cvelib-1.3.0/cvelib/cli.py` & `cvelib-1.4.0/cvelib/cli.py`

 * *Files identical despite different names*

### Comparing `cvelib-1.3.0/cvelib/cve_api.py` & `cvelib-1.4.0/cvelib/cve_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 
     def __reduce__(self):
         return CveRecordValidationError, (self.args,)
 
 
 class CveRecord:
     class Schemas(Constants):
-        CNA_PUBLISHED = next(SCHEMA_DIR.glob("published_cna_container_*.json"))
-        CNA_REJECTED = next(SCHEMA_DIR.glob("rejected_cna_container_*.json"))
-        ADP = next(SCHEMA_DIR.glob("adp_container_*.json"))
-        V5_SCHEMA = next(SCHEMA_DIR.glob("CVE_JSON_5.0_bundled_*.json"))
+        CNA_PUBLISHED = next(SCHEMA_DIR.glob("CVE_JSON_cnaPublishedContainer_*.json"))
+        CNA_REJECTED = next(SCHEMA_DIR.glob("CVE_JSON_cnaRejectedContainer_*.json"))
+        ADP = next(SCHEMA_DIR.glob("CVE_JSON_adpContainer_*.json"))
+        V5_SCHEMA = next(SCHEMA_DIR.glob("CVE_JSON_bundled_*.json"))
 
     @classmethod
     def validate(cls, cve_json: dict, schema_path: Optional[str] = None) -> None:
         """Validate a CVE record against a JSON schema.
 
         Optionally, specify a path to a JSON schema file with which to validate the record; if not
         specified, the Published CNA container schema bundled in cvelib/schemas/ is used. All
```

### Comparing `cvelib-1.3.0/cvelib/schemas/CVE_JSON_5.0_bundled_5.0.0.json` & `cvelib-1.4.0/cvelib/schemas/CVE_JSON_adpContainer_5.1.0.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2968406866471879%*

 * *Differences: {"'$comment'": "'The character . is restricted in names allowed by patternProperties to "*

 * *               "work-around naming limitations in some common implementations.'",*

 * * "'additionalProperties'": 'False',*

 * * "'definitions'": "{'reference': {'additionalProperties': False}, 'timestamp': {'description': "*

 * *                  '"Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone '*

 * *                  "in the format 'yyyy-MM-ddTHH:mm:ss[+-]ZH:ZM'. If timezone offset is not given, "*

 * *         […]*

```diff
@@ -1,83 +1,12 @@
 {
-    "$id": "https://cve.org/cve/record/v5_00/",
+    "$comment": "The character . is restricted in names allowed by patternProperties to work-around naming limitations in some common implementations.",
     "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": false,
     "definitions": {
-        "adpContainer": {
-            "additionalProperties": false,
-            "description": "An object containing the vulnerability information provided by an Authorized Data Publisher (ADP). Since multiple ADPs can provide information for a CVE ID, an ADP container must indicate which ADP is the source of the information in the object.",
-            "minProperties": 2,
-            "patternProperties": {
-                "^x_[^.]*$": {}
-            },
-            "properties": {
-                "affected": {
-                    "$ref": "#/definitions/affected"
-                },
-                "configurations": {
-                    "$ref": "#/definitions/configurations"
-                },
-                "credits": {
-                    "$ref": "#/definitions/credits"
-                },
-                "datePublic": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "If known, the date/time the vulnerability was disclosed publicly."
-                },
-                "descriptions": {
-                    "$ref": "#/definitions/descriptions"
-                },
-                "exploits": {
-                    "$ref": "#/definitions/exploits"
-                },
-                "impacts": {
-                    "$ref": "#/definitions/impacts"
-                },
-                "metrics": {
-                    "$ref": "#/definitions/metrics"
-                },
-                "problemTypes": {
-                    "$ref": "#/definitions/problemTypes"
-                },
-                "providerMetadata": {
-                    "$ref": "#/definitions/providerMetadata"
-                },
-                "references": {
-                    "$ref": "#/definitions/references"
-                },
-                "solutions": {
-                    "$ref": "#/definitions/solutions"
-                },
-                "source": {
-                    "$ref": "#/definitions/source"
-                },
-                "tags": {
-                    "$ref": "#/definitions/adpTags"
-                },
-                "taxonomyMappings": {
-                    "$ref": "#/definitions/taxonomyMappings"
-                },
-                "timeline": {
-                    "$ref": "#/definitions/timeline"
-                },
-                "title": {
-                    "description": "A title, headline, or a brief phrase summarizing the information in an ADP container.",
-                    "maxLength": 256,
-                    "minLength": 1,
-                    "type": "string"
-                },
-                "workarounds": {
-                    "$ref": "#/definitions/workarounds"
-                }
-            },
-            "required": [
-                "providerMetadata"
-            ],
-            "type": "object"
-        },
         "adpTags": {
             "description": "Tags provided by an ADP describing the CVE Record.",
             "items": {
                 "oneOf": [
                     {
                         "$ref": "#/definitions/tagExtension"
                     },
@@ -100,158 +29,27 @@
             "description": "List of affected products.",
             "items": {
                 "$ref": "#/definitions/product"
             },
             "minItems": 1,
             "type": "array"
         },
-        "cnaPublishedContainer": {
-            "additionalProperties": false,
-            "description": "An object containing the vulnerability information provided by a CVE Numbering Authority (CNA) for a published CVE ID. There can only be one CNA container per CVE record since there can only be one assigning CNA. The CNA container must include the required information defined in the CVE Rules, which includes a product, version, problem type, prose description, and a reference.",
-            "patternProperties": {
-                "^x_[^.]*$": {}
-            },
-            "properties": {
-                "affected": {
-                    "$ref": "#/definitions/affected"
-                },
-                "configurations": {
-                    "$ref": "#/definitions/configurations"
-                },
-                "credits": {
-                    "$ref": "#/definitions/credits"
-                },
-                "dateAssigned": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "The date/time this CVE ID was associated with a vulnerability by a CNA."
-                },
-                "datePublic": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "If known, the date/time the vulnerability was disclosed publicly."
-                },
-                "descriptions": {
-                    "$ref": "#/definitions/descriptions"
-                },
-                "exploits": {
-                    "$ref": "#/definitions/exploits"
-                },
-                "impacts": {
-                    "$ref": "#/definitions/impacts"
-                },
-                "metrics": {
-                    "$ref": "#/definitions/metrics"
-                },
-                "problemTypes": {
-                    "$ref": "#/definitions/problemTypes"
-                },
-                "providerMetadata": {
-                    "$ref": "#/definitions/providerMetadata"
-                },
-                "references": {
-                    "$ref": "#/definitions/references"
-                },
-                "solutions": {
-                    "$ref": "#/definitions/solutions"
-                },
-                "source": {
-                    "$ref": "#/definitions/source"
-                },
-                "tags": {
-                    "$ref": "#/definitions/cnaTags"
-                },
-                "taxonomyMappings": {
-                    "$ref": "#/definitions/taxonomyMappings"
-                },
-                "timeline": {
-                    "$ref": "#/definitions/timeline"
-                },
-                "title": {
-                    "description": "A title, headline, or a brief phrase summarizing the CVE record. Eg., Buffer overflow in Example Soft.",
-                    "maxLength": 256,
-                    "minLength": 1,
-                    "type": "string"
-                },
-                "workarounds": {
-                    "$ref": "#/definitions/workarounds"
-                }
-            },
-            "required": [
-                "providerMetadata",
-                "descriptions",
-                "affected",
-                "references"
-            ],
-            "type": "object"
-        },
-        "cnaRejectedContainer": {
-            "additionalProperties": false,
-            "description": "An object containing the vulnerability information provided by a CVE Numbering Authority (CNA) for a rejected CVE ID. There can only be one CNA container per CVE record since there can only be one assigning CNA.",
-            "patternProperties": {
-                "^x_[^.]*$": {}
-            },
-            "properties": {
-                "providerMetadata": {
-                    "$ref": "#/definitions/providerMetadata"
-                },
-                "rejectedReasons": {
-                    "$ref": "#/definitions/descriptions",
-                    "description": "Reasons for rejecting this CVE Record."
-                },
-                "replacedBy": {
-                    "description": "Contains an array of CVE IDs that this CVE ID was rejected in favor of because this CVE ID was assigned to the vulnerabilities.",
-                    "items": {
-                        "$ref": "#/definitions/cveId"
-                    },
-                    "minItems": 1,
-                    "type": "array",
-                    "uniqueItems": true
-                }
-            },
-            "required": [
-                "providerMetadata",
-                "rejectedReasons"
-            ],
-            "type": "object"
-        },
-        "cnaTags": {
-            "description": "Tags provided by a CNA describing the CVE Record.",
-            "items": {
-                "oneOf": [
-                    {
-                        "$ref": "#/definitions/tagExtension"
-                    },
-                    {
-                        "$id": "https://cve.mitre.org/cve/v5_00/tags/cna/",
-                        "$schema": "http://json-schema.org/draft-07/schema#",
-                        "description": "exclusively-hosted-service: All known software and/or hardware affected by this CVE Record is known to exist only in the affected hosted service. If the vulnerability affects both hosted and on-prem software and/or hardware, then the tag should not be used.\n\nunsupported-when-assigned: Used by the assigning CNA to indicate that when a request for a CVE assignment was received, the product was already end-of-life (EOL) or a product or specific version was deemed not to be supported by the vendor. This tag should only be applied to a CVE Record when all affected products or version lines referenced in the CVE-Record are EOL.\n\ndisputed: When one party disagrees with another party's assertion that a particular issue in software is a vulnerability, a CVE Record assigned to that issue may be tagged as being 'disputed'.",
-                        "enum": [
-                            "unsupported-when-assigned",
-                            "exclusively-hosted-service",
-                            "disputed"
-                        ],
-                        "type": "string"
-                    }
-                ]
-            },
-            "minItems": 1,
-            "type": "array",
-            "uniqueItems": true
-        },
         "configurations": {
             "description": "Configurations required for exploiting this vulnerability.",
             "items": {
                 "$ref": "#/definitions/description"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "credits": {
             "description": "Statements acknowledging specific people, organizations, or tools recognizing the work done in researching, discovering, remediating or helping with activities related to this CVE.",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "lang": {
                         "$ref": "#/definitions/language",
                         "description": "The language used when describing the credits. The language field is included so that CVE Records can support translations. The value must be a BCP 47 language code."
                     },
                     "type": {
                         "default": "finder",
@@ -286,152 +84,25 @@
                 ],
                 "type": "object"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
-        "cveId": {
-            "pattern": "^CVE-[0-9]{4}-[0-9]{4,19}$",
-            "type": "string"
-        },
-        "cveMetadataPublished": {
-            "additionalProperties": false,
-            "description": "This is meta data about the CVE ID such as the CVE ID, who requested it, who assigned it, when it was requested, the current state (PUBLISHED, REJECTED, etc.) and so on.  These fields are controlled by the CVE Services.",
-            "properties": {
-                "assignerOrgId": {
-                    "$ref": "#/definitions/orgId",
-                    "description": "The UUID for the organization to which the CVE ID was originally assigned. This UUID can be used to lookup the organization record in the user registry service."
-                },
-                "assignerShortName": {
-                    "$ref": "#/definitions/shortName",
-                    "description": "The short name for the organization to which the CVE ID was originally assigned."
-                },
-                "cveId": {
-                    "$ref": "#/definitions/cveId",
-                    "description": "The CVE identifier that this record pertains to."
-                },
-                "datePublished": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "The date/time the CVE Record was first published in the CVE List."
-                },
-                "dateReserved": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "The date/time this CVE ID was reserved in the CVE automation workgroup services system. Disclaimer: This date reflects when the CVE ID was reserved, and does not necessarily indicate when this vulnerability was discovered, shared with the affected vendor, publicly disclosed, or updated in CVE."
-                },
-                "dateUpdated": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "The date/time the record was last updated."
-                },
-                "requesterUserId": {
-                    "$ref": "#/definitions/userId",
-                    "description": "The user that requested the CVE identifier."
-                },
-                "serial": {
-                    "description": "The system of record causes this to start at 1, and increment by 1 each time a submission from a data provider changes this CVE Record. The incremented value moves to the Rejected schema upon a PUBLISHED->REJECTED transition, and moves to the Published schema upon a REJECTED->PUBLISHED transition.",
-                    "minimum": 1,
-                    "type": "integer"
-                },
-                "state": {
-                    "description": "State of CVE - PUBLISHED, REJECTED.",
-                    "enum": [
-                        "PUBLISHED"
-                    ],
-                    "type": "string"
-                }
-            },
-            "required": [
-                "cveId",
-                "assignerOrgId",
-                "state"
-            ],
-            "type": "object"
-        },
-        "cveMetadataRejected": {
-            "additionalProperties": false,
-            "description": "This is meta data about the CVE ID such as the CVE ID, who requested it, who assigned it, when it was requested, the current state (PUBLISHED, REJECTED, etc.) and so on.  These fields are controlled by the CVE Services.",
-            "properties": {
-                "assignerOrgId": {
-                    "$ref": "#/definitions/orgId",
-                    "description": "The UUID for the organization to which the CVE ID was originally assigned."
-                },
-                "assignerShortName": {
-                    "$ref": "#/definitions/shortName",
-                    "description": "The short name for the organization to which the CVE ID was originally assigned."
-                },
-                "cveId": {
-                    "$ref": "#/definitions/cveId",
-                    "description": "The CVE identifier that this record pertains to."
-                },
-                "datePublished": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "The date/time the CVE Record was first published in the CVE List."
-                },
-                "dateRejected": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "The date/time the CVE ID was rejected."
-                },
-                "dateReserved": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "The date/time this CVE ID was reserved in the CVE automation workgroup services system. Disclaimer: This date reflects when the CVE ID was reserved, and does not necessarily indicate when this vulnerability was discovered, shared with the affected vendor, publicly disclosed, or updated in CVE."
-                },
-                "dateUpdated": {
-                    "$ref": "#/definitions/timestamp",
-                    "description": "The date/time the record was last updated."
-                },
-                "serial": {
-                    "description": "The system of record causes this to start at 1, and increment by 1 each time a submission from a data provider changes this CVE Record. The incremented value moves to the Rejected schema upon a PUBLISHED->REJECTED transition, and moves to the Published schema upon a REJECTED->PUBLISHED transition.",
-                    "minimum": 1,
-                    "type": "integer"
-                },
-                "state": {
-                    "description": "State of CVE - PUBLISHED, REJECTED.",
-                    "enum": [
-                        "REJECTED"
-                    ],
-                    "type": "string"
-                }
-            },
-            "required": [
-                "cveId",
-                "assignerOrgId",
-                "state"
-            ],
-            "type": "object"
-        },
-        "dataType": {
-            "description": "Indicates the type of information represented in the JSON instance.",
-            "enum": [
-                "CVE_RECORD"
-            ],
-            "type": "string"
-        },
-        "dataVersion": {
-            "description": "The version of the schema being used. Used to support multiple versions of this format.",
-            "enum": [
-                "5.0"
-            ],
-            "type": "string"
-        },
-        "datestamp": {
-            "description": "Date/time format based on RFC3339 and ISO ISO8601.",
-            "format": "date",
-            "pattern": "^((2000|2400|2800|(19|2[0-9](0[48]|[2468][048]|[13579][26])))-02-29)|(((19|2[0-9])[0-9]{2})-02-(0[1-9]|1[0-9]|2[0-8]))|(((19|2[0-9])[0-9]{2})-(0[13578]|10|12)-(0[1-9]|[12][0-9]|3[01]))|(((19|2[0-9])[0-9]{2})-(0[469]|11)-(0[1-9]|[12][0-9]|30))$",
-            "type": "string"
-        },
         "description": {
             "additionalProperties": false,
             "description": "Text in a particular language with optional alternate markup or formatted representation (e.g., Markdown) or embedded media.",
             "properties": {
                 "lang": {
                     "$ref": "#/definitions/language"
                 },
                 "supportingMedia": {
                     "description": "Supporting media data for the description such as markdown, diagrams, .. (optional). Similar to RFC 2397 each media object has three main parts: media type, media data value, and an optional boolean flag to indicate if the media data is base64 encoded.",
                     "items": {
+                        "additionalProperties": false,
                         "properties": {
                             "base64": {
                                 "default": false,
                                 "description": "If true then the value field contains the media data encoded in base64. If false then the value field contains the UTF-8 media content.",
                                 "title": "Encoding",
                                 "type": "boolean"
                             },
@@ -494,14 +165,15 @@
         },
         "englishLanguage": {
             "description": "BCP 47 language code, language-region, required to be English.",
             "pattern": "^en([_-][A-Za-z]{4})?([_-]([A-Za-z]{2}|[0-9]{3}))?$",
             "type": "string"
         },
         "englishLanguageDescription": {
+            "$comment": "Cannot use additionalProperties: false here, as this prevents the other properties used by /definitions/description.",
             "description": "A description with lang set to an English language (en, en_US, en_UK, and so on).",
             "properties": {
                 "lang": {
                     "$ref": "#/definitions/englishLanguage"
                 }
             },
             "required": [
@@ -517,14 +189,15 @@
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "impacts": {
             "description": "Collection of impacts of this vulnerability.",
             "items": {
+                "additionalProperties": false,
                 "description": "This is impact type information (e.g. a text description.",
                 "properties": {
                     "capecId": {
                         "description": "CAPEC ID that best relates to this impact.",
                         "maxLength": 11,
                         "minLength": 7,
                         "pattern": "^CAPEC-[1-9][0-9]{0,4}$",
@@ -549,17 +222,23 @@
             "description": "BCP 47 language code, language-region.",
             "pattern": "^[A-Za-z]{2,4}([_-][A-Za-z]{4})?([_-]([A-Za-z]{2}|[0-9]{3}))?$",
             "type": "string"
         },
         "metrics": {
             "description": "Collection of impact scores with attribution.",
             "items": {
+                "additionalProperties": false,
                 "anyOf": [
                     {
                         "required": [
+                            "cvssV4_0"
+                        ]
+                    },
+                    {
+                        "required": [
                             "cvssV3_1"
                         ]
                     },
                     {
                         "required": [
                             "cvssV3_0"
                         ]
@@ -571,18 +250,19 @@
                     },
                     {
                         "required": [
                             "other"
                         ]
                     }
                 ],
-                "description": "This is impact type information (e.g. a text description, CVSSv2, CVSSv3, etc.). Must contain: At least one entry, can be text, CVSSv2, CVSSv3, others may be added.",
+                "description": "This is impact type information (e.g. a text description, CVSSv2, CVSSv3, CVSSV4, etc.). Must contain: At least one entry, can be text, CVSSv2, CVSSv3, others may be added.",
                 "properties": {
                     "cvssV2_0": {
                         "$schema": "http://json-schema.org/draft-04/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "accessComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "MEDIUM",
                                     "LOW"
                                 ],
@@ -747,14 +427,15 @@
                             "baseScore"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 2.0",
                         "type": "object"
                     },
                     "cvssV3_0": {
                         "$schema": "http://json-schema.org/draft-04/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "attackComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "LOW"
                                 ],
                                 "type": "string"
@@ -1008,14 +689,15 @@
                             "baseSeverity"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 3.0",
                         "type": "object"
                     },
                     "cvssV3_1": {
                         "$schema": "http://json-schema.org/draft-07/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "attackComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "LOW"
                                 ],
                                 "type": "string"
@@ -1267,24 +949,592 @@
                             "vectorString",
                             "baseScore",
                             "baseSeverity"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 3.1",
                         "type": "object"
                     },
+                    "cvssV4_0": {
+                        "$schema": "http://json-schema.org/draft-07/schema#",
+                        "additionalProperties": false,
+                        "allOf": [
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            },
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            },
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            }
+                        ],
+                        "definitions": {
+                            "attackComplexityType": {
+                                "enum": [
+                                    "HIGH",
+                                    "LOW"
+                                ],
+                                "type": "string"
+                            },
+                            "attackRequirementsType": {
+                                "enum": [
+                                    "NONE",
+                                    "PRESENT"
+                                ],
+                                "type": "string"
+                            },
+                            "attackVectorType": {
+                                "enum": [
+                                    "NETWORK",
+                                    "ADJACENT",
+                                    "LOCAL",
+                                    "PHYSICAL"
+                                ],
+                                "type": "string"
+                            },
+                            "automatableType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NO",
+                                    "YES",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "ciaRequirementType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "LOW",
+                                    "MEDIUM",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "criticalScoreType": {
+                                "maximum": 10,
+                                "minimum": 9,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "criticalSeverityType": {
+                                "const": "CRITICAL"
+                            },
+                            "exploitMaturityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "UNREPORTED",
+                                    "PROOF_OF_CONCEPT",
+                                    "ATTACKED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "highScoreType": {
+                                "maximum": 8.9,
+                                "minimum": 7,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "highSeverityType": {
+                                "const": "HIGH"
+                            },
+                            "lowScoreType": {
+                                "maximum": 3.9,
+                                "minimum": 0.1,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "lowSeverityType": {
+                                "const": "LOW"
+                            },
+                            "mediumScoreType": {
+                                "maximum": 6.9,
+                                "minimum": 4,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "mediumSeverityType": {
+                                "const": "MEDIUM"
+                            },
+                            "modifiedAttackComplexityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedAttackRequirementsType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "PRESENT",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedAttackVectorType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NETWORK",
+                                    "ADJACENT",
+                                    "LOCAL",
+                                    "PHYSICAL",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedPrivilegesRequiredType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NONE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedSubCType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedSubIaType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "SAFETY",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedUserInteractionType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "PASSIVE",
+                                    "ACTIVE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedVulnCiaType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "noneScoreType": {
+                                "maximum": 0,
+                                "minimum": 0,
+                                "type": "number"
+                            },
+                            "noneSeverityType": {
+                                "const": "NONE"
+                            },
+                            "privilegesRequiredType": {
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NONE"
+                                ],
+                                "type": "string"
+                            },
+                            "providerUrgencyType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "CLEAR",
+                                    "GREEN",
+                                    "AMBER",
+                                    "RED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "recoveryType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "AUTOMATIC",
+                                    "USER",
+                                    "IRRECOVERABLE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "safetyType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NEGLIGIBLE",
+                                    "PRESENT",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "scoreType": {
+                                "maximum": 10,
+                                "minimum": 0,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "severityType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "MEDIUM",
+                                    "HIGH",
+                                    "CRITICAL"
+                                ],
+                                "type": "string"
+                            },
+                            "subCiaType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH"
+                                ],
+                                "type": "string"
+                            },
+                            "userInteractionType": {
+                                "enum": [
+                                    "NONE",
+                                    "PASSIVE",
+                                    "ACTIVE"
+                                ],
+                                "type": "string"
+                            },
+                            "valueDensityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "DIFFUSE",
+                                    "CONCENTRATED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnCiaType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnerabilityResponseEffortType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "LOW",
+                                    "MODERATE",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            }
+                        },
+                        "properties": {
+                            "Automatable": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/automatableType"
+                            },
+                            "Recovery": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/recoveryType"
+                            },
+                            "Safety": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/safetyType"
+                            },
+                            "attackComplexity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackComplexityType"
+                            },
+                            "attackRequirements": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackRequirementsType"
+                            },
+                            "attackVector": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackVectorType"
+                            },
+                            "availabilityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "baseScore": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/scoreType"
+                            },
+                            "baseSeverity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/severityType"
+                            },
+                            "confidentialityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "exploitMaturity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/exploitMaturityType"
+                            },
+                            "integrityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "modifiedAttackComplexity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackComplexityType"
+                            },
+                            "modifiedAttackRequirements": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackRequirementsType"
+                            },
+                            "modifiedAttackVector": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackVectorType"
+                            },
+                            "modifiedPrivilegesRequired": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedPrivilegesRequiredType"
+                            },
+                            "modifiedSubAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubIaType"
+                            },
+                            "modifiedSubConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubCType"
+                            },
+                            "modifiedSubIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubIaType"
+                            },
+                            "modifiedUserInteraction": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedUserInteractionType"
+                            },
+                            "modifiedVulnAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "modifiedVulnConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "modifiedVulnIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "privilegesRequired": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/privilegesRequiredType"
+                            },
+                            "providerUrgency": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/providerUrgencyType"
+                            },
+                            "subAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "subConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "subIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "userInteraction": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/userInteractionType"
+                            },
+                            "valueDensity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/valueDensityType"
+                            },
+                            "vectorString": {
+                                "pattern": "^CVSS:4[.]0/AV:[NALP]/AC:[LH]/AT:[NP]/PR:[NLH]/UI:[NPA]/VC:[HLN]/VI:[HLN]/VA:[HLN]/SC:[HLN]/SI:[HLN]/SA:[HLN](/E:[XAPU])?(/CR:[XHML])?(/IR:[XHML])?(/AR:[XHML])?(/MAV:[XNALP])?(/MAC:[XLH])?(/MAT:[XNP])?(/MPR:[XNLH])?(/MUI:[XNPA])?(/MVC:[XNLH])?(/MVI:[XNLH])?(/MVA:[XNLH])?(/MSC:[XNLH])?(/MSI:[XNLHS])?(/MSA:[XNLHS])?(/S:[XNP])?(/AU:[XNY])?(/R:[XAUI])?(/V:[XDC])?(/RE:[XLMH])?(/U:(X|Clear|Green|Amber|Red))?$",
+                                "type": "string"
+                            },
+                            "version": {
+                                "description": "CVSS Version",
+                                "enum": [
+                                    "4.0"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnerabilityResponseEffort": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnerabilityResponseEffortType"
+                            }
+                        },
+                        "required": [
+                            "version",
+                            "vectorString",
+                            "baseScore",
+                            "baseSeverity"
+                        ],
+                        "title": "JSON Schema for Common Vulnerability Scoring System version 4.0",
+                        "type": "object"
+                    },
                     "format": {
                         "description": "Name of the scoring format. This provides a bit of future proofing. Additional properties are not prohibited, so this will support the inclusion of proprietary formats. It also provides an easy future conversion mechanism when future score formats become part of the schema. example: cvssV44, format = 'cvssV44', other = cvssV4_4 JSON object. In the future, the other properties can be converted to score properties when they become part of the schema.",
                         "maxLength": 64,
                         "minLength": 1,
                         "type": "string"
                     },
                     "other": {
+                        "additionalProperties": false,
                         "description": "A non-standard impact description, may be prose or JSON block.",
                         "properties": {
                             "content": {
+                                "$comment": "additionalProperties are allowed here, since this construct supports arbitrary JSON.",
                                 "description": "JSON object not covered by another metrics format.",
                                 "minProperties": 1,
                                 "type": "object"
                             },
                             "type": {
                                 "description": "Name of the non-standard impact metrics format used.",
                                 "maxLength": 128,
@@ -1297,14 +1547,15 @@
                             "content"
                         ],
                         "type": "object"
                     },
                     "scenarios": {
                         "description": "Description of the scenarios this metrics object applies to. If no specific scenario is given, GENERAL is used as the default and applies when no more specific metric matches.",
                         "items": {
+                            "additionalProperties": false,
                             "properties": {
                                 "lang": {
                                     "$ref": "#/definitions/language"
                                 },
                                 "value": {
                                     "default": "GENERAL",
                                     "description": "Description of the scenario this metrics object applies to. If no specific scenario is given, GENERAL is used as the default and applies when no more specific metric matches.",
@@ -1333,17 +1584,19 @@
         "orgId": {
             "$ref": "#/definitions/uuidType",
             "description": "A UUID for an organization participating in the CVE program. This UUID can be used to lookup the organization record in the user registry service."
         },
         "problemTypes": {
             "description": "This is problem type information (e.g. CWE identifier). Must contain: At least one entry, can be text, OWASP, CWE, please note that while only one is required you can use more than one (or indeed all three) as long as they are correct). (CNA requirement: [PROBLEMTYPE]).",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "descriptions": {
                         "items": {
+                            "additionalProperties": false,
                             "properties": {
                                 "cweId": {
                                     "description": "CWE ID of the CWE that best describes this problemType entry.",
                                     "maxLength": 9,
                                     "minLength": 5,
                                     "pattern": "^CWE-[1-9][0-9]*$",
                                     "type": "string"
@@ -1566,14 +1819,15 @@
                     },
                     "type": "array",
                     "uniqueItems": true
                 },
                 "programRoutines": {
                     "description": "A list of the affected source code functions, methods, subroutines, or procedures (optional).",
                     "items": {
+                        "additionalProperties": false,
                         "description": "An object describing program routine.",
                         "properties": {
                             "name": {
                                 "description": "Name of the affected source code file, function, method, subroutine, or procedure.",
                                 "maxLength": 4096,
                                 "minLength": 1,
                                 "type": "string"
@@ -1596,47 +1850,54 @@
                     "maxLength": 512,
                     "minLength": 1,
                     "type": "string"
                 },
                 "versions": {
                     "description": "Set of product versions or version ranges related to the vulnerability. The versions satisfy the CNA Rules [8.1.2 requirement](https://cve.mitre.org/cve/cna/rules.html#section_8-1_cve_entry_information_requirements). Versions or defaultStatus may be omitted, but not both.",
                     "items": {
+                        "additionalProperties": false,
                         "description": "A single version or a range of versions, with vulnerability status.\n\nAn entry with only 'version' and 'status' indicates the status of a single version.\n\nOtherwise, an entry describes a range; it must include the 'versionType' property, to define the version numbering semantics in use, and 'limit', to indicate the non-inclusive upper limit of the range. The object describes the status for versions V such that 'version' <= V and V < 'limit', using the <= and < semantics defined for the specific kind of 'versionType'. Status changes within the range can be specified by an optional 'changes' list.\n\nThe algorithm to decide the status specified for a version V is:\n\n\tfor entry in product.versions {\n\t\tif entry.lessThan is not present and entry.lessThanOrEqual is not present and v == entry.version {\n\t\t\treturn entry.status\n\t\t}\n\t\tif (entry.lessThan is present and entry.version <= v and v < entry.lessThan) or\n\t\t   (entry.lessThanOrEqual is present and entry.version <= v and v <= entry.lessThanOrEqual) { // <= and < defined by entry.versionType\n\t\t\tstatus = entry.status\n\t\t\tfor change in entry.changes {\n\t\t\t\tif change.at <= v {\n\t\t\t\t\tstatus = change.status\n\t\t\t\t}\n\t\t\t}\n\t\t\treturn status\n\t\t}\n\t}\n\treturn product.defaultStatus\n\n.",
                         "oneOf": [
                             {
                                 "maxProperties": 2,
                                 "required": [
                                     "version",
                                     "status"
                                 ]
                             },
                             {
-                                "oneOf": [
-                                    {
-                                        "required": [
-                                            "lessThan"
-                                        ]
-                                    },
-                                    {
-                                        "required": [
-                                            "lessThanOrEqual"
-                                        ]
-                                    }
-                                ],
+                                "maxProperties": 3,
                                 "required": [
                                     "version",
                                     "status",
                                     "versionType"
                                 ]
+                            },
+                            {
+                                "required": [
+                                    "version",
+                                    "status",
+                                    "versionType",
+                                    "lessThan"
+                                ]
+                            },
+                            {
+                                "required": [
+                                    "version",
+                                    "status",
+                                    "versionType",
+                                    "lessThanOrEqual"
+                                ]
                             }
                         ],
                         "properties": {
                             "changes": {
                                 "description": "A list of status changes that take place during the range. The array should be sorted in increasing order by the 'at' field, according to the versionType, but clients must re-sort the list themselves rather than assume it is sorted.",
                                 "items": {
+                                    "additionalProperties": false,
                                     "description": "The start of a single status change during the range.",
                                     "properties": {
                                         "at": {
                                             "$ref": "#/definitions/version",
                                             "description": "The version at which a status change occurs."
                                         },
                                         "status": {
@@ -1691,14 +1952,15 @@
                     "type": "array",
                     "uniqueItems": true
                 }
             },
             "type": "object"
         },
         "providerMetadata": {
+            "additionalProperties": false,
             "description": "Details related to the information container provider (CNA or ADP).",
             "properties": {
                 "dateUpdated": {
                     "$ref": "#/definitions/timestamp",
                     "description": "Timestamp to be set by the system of record at time of submission. If dateUpdated is provided to the system of record it will be replaced by the current timestamp at the time of submission."
                 },
                 "orgId": {
@@ -1712,14 +1974,15 @@
             },
             "required": [
                 "orgId"
             ],
             "type": "object"
         },
         "reference": {
+            "additionalProperties": false,
             "properties": {
                 "name": {
                     "description": "User created name for the reference, often the title of the page.",
                     "maxLength": 512,
                     "minLength": 1,
                     "type": "string"
                 },
@@ -1809,34 +2072,37 @@
                 "affected",
                 "unaffected",
                 "unknown"
             ],
             "type": "string"
         },
         "tagExtension": {
+            "$comment": "These values are not used as JSON property names, so there is not a need to work-around property naming limitations in some common implementations.",
             "maxLength": 128,
             "minLength": 2,
             "pattern": "^x_.*$",
             "type": "string"
         },
         "taxonomyMappings": {
             "description": "List of taxonomy items related to the vulnerability.",
             "items": {
-                "description": "",
+                "additionalProperties": false,
+                "description": "A taxonomy mapping object identifies the taxonomy by a name and version (eg., ATT&CK v13.1, CVSS 3.1, CWE 4.12) along with a list of relations relevant to this CVE.",
                 "properties": {
                     "taxonomyName": {
-                        "description": "The name of the taxonomy.",
+                        "description": "The name of the taxonomy, eg., ATT&CK, D3FEND, CWE, CVSS",
                         "maxLength": 128,
                         "minLength": 1,
                         "type": "string"
                     },
                     "taxonomyRelations": {
-                        "description": "",
+                        "description": "List of relationships to the taxonomy for the vulnerability.",
                         "items": {
-                            "description": "List of relationships to the taxonomy for the vulnerability.  Relationships can be between the taxonomy and the CVE or two taxonomy items.",
+                            "additionalProperties": false,
+                            "description": "A relationship between the taxonomy and the CVE or two taxonomy items.",
                             "properties": {
                                 "relationshipName": {
                                     "description": "A description of the relationship.",
                                     "maxLength": 128,
                                     "minLength": 1,
                                     "type": "string"
                                 },
@@ -1880,22 +2146,23 @@
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "timeline": {
             "description": "This is timeline information for significant events about this vulnerability or changes to the CVE Record.",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "lang": {
                         "$ref": "#/definitions/language",
                         "description": "The language used in the description of the event. The language field is included so that CVE Records can support translations. The value must be a BCP 47 language code."
                     },
                     "time": {
                         "$ref": "#/definitions/timestamp",
-                        "description": "Timestamp representing when the event in the timeline occurred. The timestamp format is based on RFC3339 and ISO ISO8601, with an optional timezone. yyyy-MM-ddTHH:mm:ssZZZZ - if the timezone offset is not given, GMT (0000) is assumed."
+                        "description": "Timestamp representing when the event in the timeline occurred. The timestamp format is based on RFC3339 and ISO ISO8601, with an optional timezone. yyyy-MM-ddTHH:mm:ss[+-]ZH:ZM - if the timezone offset is not given, GMT (+00:00) is assumed."
                     },
                     "value": {
                         "description": "A summary of the event.",
                         "maxLength": 4096,
                         "minLength": 1,
                         "type": "string"
                     }
@@ -1908,30 +2175,26 @@
                 "type": "object"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "timestamp": {
-            "description": "Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone in the format 'yyyy-MM-ddTHH:mm:ssZZZZ'. If timezone offset is not given, GMT (0000) is assumed.",
+            "description": "Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone in the format 'yyyy-MM-ddTHH:mm:ss[+-]ZH:ZM'. If timezone offset is not given, GMT (+00:00) is assumed.",
             "format": "date-time",
             "pattern": "^(((2000|2400|2800|(19|2[0-9](0[48]|[2468][048]|[13579][26])))-02-29)|(((19|2[0-9])[0-9]{2})-02-(0[1-9]|1[0-9]|2[0-8]))|(((19|2[0-9])[0-9]{2})-(0[13578]|10|12)-(0[1-9]|[12][0-9]|3[01]))|(((19|2[0-9])[0-9]{2})-(0[469]|11)-(0[1-9]|[12][0-9]|30)))T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\\.[0-9]+)?(Z|[+-][0-9]{2}:[0-9]{2})?$",
             "type": "string"
         },
         "uriType": {
             "description": "A universal resource identifier (URI), according to [RFC 3986](https://tools.ietf.org/html/rfc3986).",
             "format": "uri",
             "maxLength": 2048,
             "minLength": 1,
             "type": "string"
         },
-        "userId": {
-            "$ref": "#/definitions/uuidType",
-            "description": "A UUID for a user participating in the CVE program. This UUID can be used to lookup the user record in the user registry service."
-        },
         "uuidType": {
             "description": "A version 4 (random) universally unique identifier (UUID) as defined by [RFC 4122](https://tools.ietf.org/html/rfc4122#section-4.1.3).",
             "pattern": "^[0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-4[0-9A-Fa-f]{3}-[89ABab][0-9A-Fa-f]{3}-[0-9A-Fa-f]{12}$",
             "type": "string"
         },
         "version": {
             "description": "A single version of a product, as expressed in its own version numbering scheme.",
@@ -1945,91 +2208,78 @@
                 "$ref": "#/definitions/description"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         }
     },
-    "description": "cve-schema specifies the CVE JSON record format. This is the blueprint for a rich set of JSON data that can be submitted by CVE Numbering Authorities (CNAs) and Authorized Data Publishers (ADPs) to describe a CVE Record. Some examples of CVE Record data include CVE ID number, affected product(s), affected version(s), and public references. While those specific items are required when assigning a CVE, there are many other optional data in the schema that can be used to enrich CVE Records for community benefit. Learn more about the CVE program at [the official website](https://cve.mitre.org). This CVE JSON record format is defined using JSON Schema. Learn more about JSON Schema [here](https://json-schema.org/).",
-    "oneOf": [
-        {
-            "additionalProperties": false,
-            "description": "When a CNA populates the data associated with a CVE ID as a CVE Record, the state of the CVE Record is Published.",
-            "properties": {
-                "containers": {
-                    "additionalProperties": false,
-                    "description": "A set of structures (called containers) used to store vulnerability information related to a specific CVE ID provided by a specific organization participating in the CVE program. Each container includes information provided by a different source.\n\nAt a minimum, a 'cna' container containing the vulnerability information provided by the CNA who initially assigned the CVE ID must be included.\n\nThere can only be one 'cna' container, as there can only be one assigning CNA. However, there can be multiple 'adp' containers, allowing multiple organizations participating in the CVE program to add additional information related to the vulnerability. For the most part, the 'cna' and 'adp' containers contain the same properties. The main differences are the source of the information. The 'cna' container requires the CNA to include certain fields, while the 'adp' container does not.",
-                    "properties": {
-                        "adp": {
-                            "items": {
-                                "$ref": "#/definitions/adpContainer"
-                            },
-                            "minItems": 1,
-                            "type": "array",
-                            "uniqueItems": true
-                        },
-                        "cna": {
-                            "$ref": "#/definitions/cnaPublishedContainer"
-                        }
-                    },
-                    "required": [
-                        "cna"
-                    ],
-                    "type": "object"
-                },
-                "cveMetadata": {
-                    "$ref": "#/definitions/cveMetadataPublished"
-                },
-                "dataType": {
-                    "$ref": "#/definitions/dataType"
-                },
-                "dataVersion": {
-                    "$ref": "#/definitions/dataVersion"
-                }
-            },
-            "required": [
-                "dataType",
-                "dataVersion",
-                "cveMetadata",
-                "containers"
-            ],
-            "title": "Published"
+    "description": "An object containing the vulnerability information provided by an Authorized Data Publisher (ADP). Since multiple ADPs can provide information for a CVE ID, an ADP container must indicate which ADP is the source of the information in the object.",
+    "minProperties": 2,
+    "patternProperties": {
+        "^x_[^.]*$": {}
+    },
+    "properties": {
+        "affected": {
+            "$ref": "#/definitions/affected"
         },
-        {
-            "additionalProperties": false,
-            "description": "If the CVE ID and associated CVE Record should no longer be used, the CVE Record is placed in the Rejected state. A Rejected CVE Record remains on the CVE List so that users can know when it is invalid.",
-            "properties": {
-                "containers": {
-                    "additionalProperties": false,
-                    "description": "A set of structures (called containers) used to store vulnerability information related to a specific CVE ID provided by a specific organization participating in the CVE program. Each container includes information provided by a different source.\n\nAt minimum, a 'cna' container containing the vulnerability information provided by the CNA who initially assigned the CVE ID must be included.\n\nThere can only be one 'cna' container, as there can only be one assigning CNA.",
-                    "properties": {
-                        "cna": {
-                            "$ref": "#/definitions/cnaRejectedContainer"
-                        }
-                    },
-                    "required": [
-                        "cna"
-                    ],
-                    "type": "object"
-                },
-                "cveMetadata": {
-                    "$ref": "#/definitions/cveMetadataRejected"
-                },
-                "dataType": {
-                    "$ref": "#/definitions/dataType"
-                },
-                "dataVersion": {
-                    "$ref": "#/definitions/dataVersion"
-                }
-            },
-            "required": [
-                "dataType",
-                "dataVersion",
-                "cveMetadata",
-                "containers"
-            ],
-            "title": "Rejected"
+        "configurations": {
+            "$ref": "#/definitions/configurations"
+        },
+        "credits": {
+            "$ref": "#/definitions/credits"
+        },
+        "datePublic": {
+            "$ref": "#/definitions/timestamp",
+            "description": "If known, the date/time the vulnerability was disclosed publicly."
+        },
+        "descriptions": {
+            "$ref": "#/definitions/descriptions"
+        },
+        "exploits": {
+            "$ref": "#/definitions/exploits"
+        },
+        "impacts": {
+            "$ref": "#/definitions/impacts"
+        },
+        "metrics": {
+            "$ref": "#/definitions/metrics"
+        },
+        "problemTypes": {
+            "$ref": "#/definitions/problemTypes"
+        },
+        "providerMetadata": {
+            "$ref": "#/definitions/providerMetadata"
+        },
+        "references": {
+            "$ref": "#/definitions/references"
+        },
+        "solutions": {
+            "$ref": "#/definitions/solutions"
+        },
+        "source": {
+            "$ref": "#/definitions/source"
+        },
+        "tags": {
+            "$ref": "#/definitions/adpTags"
+        },
+        "taxonomyMappings": {
+            "$ref": "#/definitions/taxonomyMappings"
+        },
+        "timeline": {
+            "$ref": "#/definitions/timeline"
+        },
+        "title": {
+            "description": "A title, headline, or a brief phrase summarizing the information in an ADP container.",
+            "maxLength": 256,
+            "minLength": 1,
+            "type": "string"
+        },
+        "workarounds": {
+            "$ref": "#/definitions/workarounds"
         }
+    },
+    "required": [
+        "providerMetadata"
     ],
-    "title": "CVE JSON record format",
+    "title": "CVE_JSON_adpContainer_5.1.0",
     "type": "object"
 }
```

### Comparing `cvelib-1.3.0/cvelib/schemas/adp_container_5.0.0.json` & `cvelib-1.4.0/cvelib/schemas/CVE_JSON_cnaPublishedContainer_5.1.0.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6862767222836967%*

 * *Differences: {"'$comment'": "'The character . is restricted in names allowed by patternProperties to "*

 * *               "work-around naming limitations in some common implementations.'",*

 * * "'definitions'": "{'credits': {'items': {'additionalProperties': False}}, 'description': "*

 * *                  "{'properties': {'supportingMedia': {'items': {'additionalProperties': "*

 * *                  "False}}}}, 'englishLanguageDescription': {'$comment': 'Cannot use "*

 * *                  'additionalProperties: false here, as this prevents  […]*

```diff
@@ -1,53 +1,57 @@
 {
+    "$comment": "The character . is restricted in names allowed by patternProperties to work-around naming limitations in some common implementations.",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "definitions": {
-        "adpTags": {
-            "description": "Tags provided by an ADP describing the CVE Record.",
+        "affected": {
+            "description": "List of affected products.",
+            "items": {
+                "$ref": "#/definitions/product"
+            },
+            "minItems": 1,
+            "type": "array"
+        },
+        "cnaTags": {
+            "description": "Tags provided by a CNA describing the CVE Record.",
             "items": {
                 "oneOf": [
                     {
                         "$ref": "#/definitions/tagExtension"
                     },
                     {
-                        "$id": "https://cve.mitre.org/cve/v5_00/tags/adp/",
+                        "$id": "https://cve.mitre.org/cve/v5_00/tags/cna/",
                         "$schema": "http://json-schema.org/draft-07/schema#",
-                        "description": "disputed: When one party disagrees with another party's assertion that a particular issue in software is a vulnerability, a CVE Record assigned to that issue may be tagged as being 'disputed'.",
+                        "description": "exclusively-hosted-service: All known software and/or hardware affected by this CVE Record is known to exist only in the affected hosted service. If the vulnerability affects both hosted and on-prem software and/or hardware, then the tag should not be used.\n\nunsupported-when-assigned: Used by the assigning CNA to indicate that when a request for a CVE assignment was received, the product was already end-of-life (EOL) or a product or specific version was deemed not to be supported by the vendor. This tag should only be applied to a CVE Record when all affected products or version lines referenced in the CVE-Record are EOL.\n\ndisputed: When one party disagrees with another party's assertion that a particular issue in software is a vulnerability, a CVE Record assigned to that issue may be tagged as being 'disputed'.",
                         "enum": [
+                            "unsupported-when-assigned",
+                            "exclusively-hosted-service",
                             "disputed"
                         ],
                         "type": "string"
                     }
                 ]
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
-        "affected": {
-            "description": "List of affected products.",
-            "items": {
-                "$ref": "#/definitions/product"
-            },
-            "minItems": 1,
-            "type": "array"
-        },
         "configurations": {
             "description": "Configurations required for exploiting this vulnerability.",
             "items": {
                 "$ref": "#/definitions/description"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "credits": {
             "description": "Statements acknowledging specific people, organizations, or tools recognizing the work done in researching, discovering, remediating or helping with activities related to this CVE.",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "lang": {
                         "$ref": "#/definitions/language",
                         "description": "The language used when describing the credits. The language field is included so that CVE Records can support translations. The value must be a BCP 47 language code."
                     },
                     "type": {
                         "default": "finder",
@@ -92,14 +96,15 @@
             "properties": {
                 "lang": {
                     "$ref": "#/definitions/language"
                 },
                 "supportingMedia": {
                     "description": "Supporting media data for the description such as markdown, diagrams, .. (optional). Similar to RFC 2397 each media object has three main parts: media type, media data value, and an optional boolean flag to indicate if the media data is base64 encoded.",
                     "items": {
+                        "additionalProperties": false,
                         "properties": {
                             "base64": {
                                 "default": false,
                                 "description": "If true then the value field contains the media data encoded in base64. If false then the value field contains the UTF-8 media content.",
                                 "title": "Encoding",
                                 "type": "boolean"
                             },
@@ -162,14 +167,15 @@
         },
         "englishLanguage": {
             "description": "BCP 47 language code, language-region, required to be English.",
             "pattern": "^en([_-][A-Za-z]{4})?([_-]([A-Za-z]{2}|[0-9]{3}))?$",
             "type": "string"
         },
         "englishLanguageDescription": {
+            "$comment": "Cannot use additionalProperties: false here, as this prevents the other properties used by /definitions/description.",
             "description": "A description with lang set to an English language (en, en_US, en_UK, and so on).",
             "properties": {
                 "lang": {
                     "$ref": "#/definitions/englishLanguage"
                 }
             },
             "required": [
@@ -185,14 +191,15 @@
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "impacts": {
             "description": "Collection of impacts of this vulnerability.",
             "items": {
+                "additionalProperties": false,
                 "description": "This is impact type information (e.g. a text description.",
                 "properties": {
                     "capecId": {
                         "description": "CAPEC ID that best relates to this impact.",
                         "maxLength": 11,
                         "minLength": 7,
                         "pattern": "^CAPEC-[1-9][0-9]{0,4}$",
@@ -217,17 +224,23 @@
             "description": "BCP 47 language code, language-region.",
             "pattern": "^[A-Za-z]{2,4}([_-][A-Za-z]{4})?([_-]([A-Za-z]{2}|[0-9]{3}))?$",
             "type": "string"
         },
         "metrics": {
             "description": "Collection of impact scores with attribution.",
             "items": {
+                "additionalProperties": false,
                 "anyOf": [
                     {
                         "required": [
+                            "cvssV4_0"
+                        ]
+                    },
+                    {
+                        "required": [
                             "cvssV3_1"
                         ]
                     },
                     {
                         "required": [
                             "cvssV3_0"
                         ]
@@ -239,18 +252,19 @@
                     },
                     {
                         "required": [
                             "other"
                         ]
                     }
                 ],
-                "description": "This is impact type information (e.g. a text description, CVSSv2, CVSSv3, etc.). Must contain: At least one entry, can be text, CVSSv2, CVSSv3, others may be added.",
+                "description": "This is impact type information (e.g. a text description, CVSSv2, CVSSv3, CVSSV4, etc.). Must contain: At least one entry, can be text, CVSSv2, CVSSv3, others may be added.",
                 "properties": {
                     "cvssV2_0": {
                         "$schema": "http://json-schema.org/draft-04/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "accessComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "MEDIUM",
                                     "LOW"
                                 ],
@@ -415,14 +429,15 @@
                             "baseScore"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 2.0",
                         "type": "object"
                     },
                     "cvssV3_0": {
                         "$schema": "http://json-schema.org/draft-04/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "attackComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "LOW"
                                 ],
                                 "type": "string"
@@ -676,14 +691,15 @@
                             "baseSeverity"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 3.0",
                         "type": "object"
                     },
                     "cvssV3_1": {
                         "$schema": "http://json-schema.org/draft-07/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "attackComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "LOW"
                                 ],
                                 "type": "string"
@@ -935,24 +951,592 @@
                             "vectorString",
                             "baseScore",
                             "baseSeverity"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 3.1",
                         "type": "object"
                     },
+                    "cvssV4_0": {
+                        "$schema": "http://json-schema.org/draft-07/schema#",
+                        "additionalProperties": false,
+                        "allOf": [
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            },
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            },
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            }
+                        ],
+                        "definitions": {
+                            "attackComplexityType": {
+                                "enum": [
+                                    "HIGH",
+                                    "LOW"
+                                ],
+                                "type": "string"
+                            },
+                            "attackRequirementsType": {
+                                "enum": [
+                                    "NONE",
+                                    "PRESENT"
+                                ],
+                                "type": "string"
+                            },
+                            "attackVectorType": {
+                                "enum": [
+                                    "NETWORK",
+                                    "ADJACENT",
+                                    "LOCAL",
+                                    "PHYSICAL"
+                                ],
+                                "type": "string"
+                            },
+                            "automatableType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NO",
+                                    "YES",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "ciaRequirementType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "LOW",
+                                    "MEDIUM",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "criticalScoreType": {
+                                "maximum": 10,
+                                "minimum": 9,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "criticalSeverityType": {
+                                "const": "CRITICAL"
+                            },
+                            "exploitMaturityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "UNREPORTED",
+                                    "PROOF_OF_CONCEPT",
+                                    "ATTACKED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "highScoreType": {
+                                "maximum": 8.9,
+                                "minimum": 7,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "highSeverityType": {
+                                "const": "HIGH"
+                            },
+                            "lowScoreType": {
+                                "maximum": 3.9,
+                                "minimum": 0.1,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "lowSeverityType": {
+                                "const": "LOW"
+                            },
+                            "mediumScoreType": {
+                                "maximum": 6.9,
+                                "minimum": 4,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "mediumSeverityType": {
+                                "const": "MEDIUM"
+                            },
+                            "modifiedAttackComplexityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedAttackRequirementsType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "PRESENT",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedAttackVectorType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NETWORK",
+                                    "ADJACENT",
+                                    "LOCAL",
+                                    "PHYSICAL",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedPrivilegesRequiredType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NONE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedSubCType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedSubIaType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "SAFETY",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedUserInteractionType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "PASSIVE",
+                                    "ACTIVE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedVulnCiaType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "noneScoreType": {
+                                "maximum": 0,
+                                "minimum": 0,
+                                "type": "number"
+                            },
+                            "noneSeverityType": {
+                                "const": "NONE"
+                            },
+                            "privilegesRequiredType": {
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NONE"
+                                ],
+                                "type": "string"
+                            },
+                            "providerUrgencyType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "CLEAR",
+                                    "GREEN",
+                                    "AMBER",
+                                    "RED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "recoveryType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "AUTOMATIC",
+                                    "USER",
+                                    "IRRECOVERABLE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "safetyType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NEGLIGIBLE",
+                                    "PRESENT",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "scoreType": {
+                                "maximum": 10,
+                                "minimum": 0,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "severityType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "MEDIUM",
+                                    "HIGH",
+                                    "CRITICAL"
+                                ],
+                                "type": "string"
+                            },
+                            "subCiaType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH"
+                                ],
+                                "type": "string"
+                            },
+                            "userInteractionType": {
+                                "enum": [
+                                    "NONE",
+                                    "PASSIVE",
+                                    "ACTIVE"
+                                ],
+                                "type": "string"
+                            },
+                            "valueDensityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "DIFFUSE",
+                                    "CONCENTRATED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnCiaType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnerabilityResponseEffortType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "LOW",
+                                    "MODERATE",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            }
+                        },
+                        "properties": {
+                            "Automatable": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/automatableType"
+                            },
+                            "Recovery": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/recoveryType"
+                            },
+                            "Safety": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/safetyType"
+                            },
+                            "attackComplexity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackComplexityType"
+                            },
+                            "attackRequirements": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackRequirementsType"
+                            },
+                            "attackVector": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackVectorType"
+                            },
+                            "availabilityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "baseScore": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/scoreType"
+                            },
+                            "baseSeverity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/severityType"
+                            },
+                            "confidentialityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "exploitMaturity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/exploitMaturityType"
+                            },
+                            "integrityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "modifiedAttackComplexity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackComplexityType"
+                            },
+                            "modifiedAttackRequirements": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackRequirementsType"
+                            },
+                            "modifiedAttackVector": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackVectorType"
+                            },
+                            "modifiedPrivilegesRequired": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedPrivilegesRequiredType"
+                            },
+                            "modifiedSubAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubIaType"
+                            },
+                            "modifiedSubConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubCType"
+                            },
+                            "modifiedSubIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubIaType"
+                            },
+                            "modifiedUserInteraction": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedUserInteractionType"
+                            },
+                            "modifiedVulnAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "modifiedVulnConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "modifiedVulnIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "privilegesRequired": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/privilegesRequiredType"
+                            },
+                            "providerUrgency": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/providerUrgencyType"
+                            },
+                            "subAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "subConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "subIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "userInteraction": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/userInteractionType"
+                            },
+                            "valueDensity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/valueDensityType"
+                            },
+                            "vectorString": {
+                                "pattern": "^CVSS:4[.]0/AV:[NALP]/AC:[LH]/AT:[NP]/PR:[NLH]/UI:[NPA]/VC:[HLN]/VI:[HLN]/VA:[HLN]/SC:[HLN]/SI:[HLN]/SA:[HLN](/E:[XAPU])?(/CR:[XHML])?(/IR:[XHML])?(/AR:[XHML])?(/MAV:[XNALP])?(/MAC:[XLH])?(/MAT:[XNP])?(/MPR:[XNLH])?(/MUI:[XNPA])?(/MVC:[XNLH])?(/MVI:[XNLH])?(/MVA:[XNLH])?(/MSC:[XNLH])?(/MSI:[XNLHS])?(/MSA:[XNLHS])?(/S:[XNP])?(/AU:[XNY])?(/R:[XAUI])?(/V:[XDC])?(/RE:[XLMH])?(/U:(X|Clear|Green|Amber|Red))?$",
+                                "type": "string"
+                            },
+                            "version": {
+                                "description": "CVSS Version",
+                                "enum": [
+                                    "4.0"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnerabilityResponseEffort": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnerabilityResponseEffortType"
+                            }
+                        },
+                        "required": [
+                            "version",
+                            "vectorString",
+                            "baseScore",
+                            "baseSeverity"
+                        ],
+                        "title": "JSON Schema for Common Vulnerability Scoring System version 4.0",
+                        "type": "object"
+                    },
                     "format": {
                         "description": "Name of the scoring format. This provides a bit of future proofing. Additional properties are not prohibited, so this will support the inclusion of proprietary formats. It also provides an easy future conversion mechanism when future score formats become part of the schema. example: cvssV44, format = 'cvssV44', other = cvssV4_4 JSON object. In the future, the other properties can be converted to score properties when they become part of the schema.",
                         "maxLength": 64,
                         "minLength": 1,
                         "type": "string"
                     },
                     "other": {
+                        "additionalProperties": false,
                         "description": "A non-standard impact description, may be prose or JSON block.",
                         "properties": {
                             "content": {
+                                "$comment": "additionalProperties are allowed here, since this construct supports arbitrary JSON.",
                                 "description": "JSON object not covered by another metrics format.",
                                 "minProperties": 1,
                                 "type": "object"
                             },
                             "type": {
                                 "description": "Name of the non-standard impact metrics format used.",
                                 "maxLength": 128,
@@ -965,14 +1549,15 @@
                             "content"
                         ],
                         "type": "object"
                     },
                     "scenarios": {
                         "description": "Description of the scenarios this metrics object applies to. If no specific scenario is given, GENERAL is used as the default and applies when no more specific metric matches.",
                         "items": {
+                            "additionalProperties": false,
                             "properties": {
                                 "lang": {
                                     "$ref": "#/definitions/language"
                                 },
                                 "value": {
                                     "default": "GENERAL",
                                     "description": "Description of the scenario this metrics object applies to. If no specific scenario is given, GENERAL is used as the default and applies when no more specific metric matches.",
@@ -1001,17 +1586,19 @@
         "orgId": {
             "$ref": "#/definitions/uuidType",
             "description": "A UUID for an organization participating in the CVE program. This UUID can be used to lookup the organization record in the user registry service."
         },
         "problemTypes": {
             "description": "This is problem type information (e.g. CWE identifier). Must contain: At least one entry, can be text, OWASP, CWE, please note that while only one is required you can use more than one (or indeed all three) as long as they are correct). (CNA requirement: [PROBLEMTYPE]).",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "descriptions": {
                         "items": {
+                            "additionalProperties": false,
                             "properties": {
                                 "cweId": {
                                     "description": "CWE ID of the CWE that best describes this problemType entry.",
                                     "maxLength": 9,
                                     "minLength": 5,
                                     "pattern": "^CWE-[1-9][0-9]*$",
                                     "type": "string"
@@ -1234,14 +1821,15 @@
                     },
                     "type": "array",
                     "uniqueItems": true
                 },
                 "programRoutines": {
                     "description": "A list of the affected source code functions, methods, subroutines, or procedures (optional).",
                     "items": {
+                        "additionalProperties": false,
                         "description": "An object describing program routine.",
                         "properties": {
                             "name": {
                                 "description": "Name of the affected source code file, function, method, subroutine, or procedure.",
                                 "maxLength": 4096,
                                 "minLength": 1,
                                 "type": "string"
@@ -1264,47 +1852,54 @@
                     "maxLength": 512,
                     "minLength": 1,
                     "type": "string"
                 },
                 "versions": {
                     "description": "Set of product versions or version ranges related to the vulnerability. The versions satisfy the CNA Rules [8.1.2 requirement](https://cve.mitre.org/cve/cna/rules.html#section_8-1_cve_entry_information_requirements). Versions or defaultStatus may be omitted, but not both.",
                     "items": {
+                        "additionalProperties": false,
                         "description": "A single version or a range of versions, with vulnerability status.\n\nAn entry with only 'version' and 'status' indicates the status of a single version.\n\nOtherwise, an entry describes a range; it must include the 'versionType' property, to define the version numbering semantics in use, and 'limit', to indicate the non-inclusive upper limit of the range. The object describes the status for versions V such that 'version' <= V and V < 'limit', using the <= and < semantics defined for the specific kind of 'versionType'. Status changes within the range can be specified by an optional 'changes' list.\n\nThe algorithm to decide the status specified for a version V is:\n\n\tfor entry in product.versions {\n\t\tif entry.lessThan is not present and entry.lessThanOrEqual is not present and v == entry.version {\n\t\t\treturn entry.status\n\t\t}\n\t\tif (entry.lessThan is present and entry.version <= v and v < entry.lessThan) or\n\t\t   (entry.lessThanOrEqual is present and entry.version <= v and v <= entry.lessThanOrEqual) { // <= and < defined by entry.versionType\n\t\t\tstatus = entry.status\n\t\t\tfor change in entry.changes {\n\t\t\t\tif change.at <= v {\n\t\t\t\t\tstatus = change.status\n\t\t\t\t}\n\t\t\t}\n\t\t\treturn status\n\t\t}\n\t}\n\treturn product.defaultStatus\n\n.",
                         "oneOf": [
                             {
                                 "maxProperties": 2,
                                 "required": [
                                     "version",
                                     "status"
                                 ]
                             },
                             {
-                                "oneOf": [
-                                    {
-                                        "required": [
-                                            "lessThan"
-                                        ]
-                                    },
-                                    {
-                                        "required": [
-                                            "lessThanOrEqual"
-                                        ]
-                                    }
-                                ],
+                                "maxProperties": 3,
                                 "required": [
                                     "version",
                                     "status",
                                     "versionType"
                                 ]
+                            },
+                            {
+                                "required": [
+                                    "version",
+                                    "status",
+                                    "versionType",
+                                    "lessThan"
+                                ]
+                            },
+                            {
+                                "required": [
+                                    "version",
+                                    "status",
+                                    "versionType",
+                                    "lessThanOrEqual"
+                                ]
                             }
                         ],
                         "properties": {
                             "changes": {
                                 "description": "A list of status changes that take place during the range. The array should be sorted in increasing order by the 'at' field, according to the versionType, but clients must re-sort the list themselves rather than assume it is sorted.",
                                 "items": {
+                                    "additionalProperties": false,
                                     "description": "The start of a single status change during the range.",
                                     "properties": {
                                         "at": {
                                             "$ref": "#/definitions/version",
                                             "description": "The version at which a status change occurs."
                                         },
                                         "status": {
@@ -1359,14 +1954,15 @@
                     "type": "array",
                     "uniqueItems": true
                 }
             },
             "type": "object"
         },
         "providerMetadata": {
+            "additionalProperties": false,
             "description": "Details related to the information container provider (CNA or ADP).",
             "properties": {
                 "dateUpdated": {
                     "$ref": "#/definitions/timestamp",
                     "description": "Timestamp to be set by the system of record at time of submission. If dateUpdated is provided to the system of record it will be replaced by the current timestamp at the time of submission."
                 },
                 "orgId": {
@@ -1380,14 +1976,15 @@
             },
             "required": [
                 "orgId"
             ],
             "type": "object"
         },
         "reference": {
+            "additionalProperties": false,
             "properties": {
                 "name": {
                     "description": "User created name for the reference, often the title of the page.",
                     "maxLength": 512,
                     "minLength": 1,
                     "type": "string"
                 },
@@ -1477,34 +2074,37 @@
                 "affected",
                 "unaffected",
                 "unknown"
             ],
             "type": "string"
         },
         "tagExtension": {
+            "$comment": "These values are not used as JSON property names, so there is not a need to work-around property naming limitations in some common implementations.",
             "maxLength": 128,
             "minLength": 2,
             "pattern": "^x_.*$",
             "type": "string"
         },
         "taxonomyMappings": {
             "description": "List of taxonomy items related to the vulnerability.",
             "items": {
-                "description": "",
+                "additionalProperties": false,
+                "description": "A taxonomy mapping object identifies the taxonomy by a name and version (eg., ATT&CK v13.1, CVSS 3.1, CWE 4.12) along with a list of relations relevant to this CVE.",
                 "properties": {
                     "taxonomyName": {
-                        "description": "The name of the taxonomy.",
+                        "description": "The name of the taxonomy, eg., ATT&CK, D3FEND, CWE, CVSS",
                         "maxLength": 128,
                         "minLength": 1,
                         "type": "string"
                     },
                     "taxonomyRelations": {
-                        "description": "",
+                        "description": "List of relationships to the taxonomy for the vulnerability.",
                         "items": {
-                            "description": "List of relationships to the taxonomy for the vulnerability.  Relationships can be between the taxonomy and the CVE or two taxonomy items.",
+                            "additionalProperties": false,
+                            "description": "A relationship between the taxonomy and the CVE or two taxonomy items.",
                             "properties": {
                                 "relationshipName": {
                                     "description": "A description of the relationship.",
                                     "maxLength": 128,
                                     "minLength": 1,
                                     "type": "string"
                                 },
@@ -1548,22 +2148,23 @@
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "timeline": {
             "description": "This is timeline information for significant events about this vulnerability or changes to the CVE Record.",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "lang": {
                         "$ref": "#/definitions/language",
                         "description": "The language used in the description of the event. The language field is included so that CVE Records can support translations. The value must be a BCP 47 language code."
                     },
                     "time": {
                         "$ref": "#/definitions/timestamp",
-                        "description": "Timestamp representing when the event in the timeline occurred. The timestamp format is based on RFC3339 and ISO ISO8601, with an optional timezone. yyyy-MM-ddTHH:mm:ssZZZZ - if the timezone offset is not given, GMT (0000) is assumed."
+                        "description": "Timestamp representing when the event in the timeline occurred. The timestamp format is based on RFC3339 and ISO ISO8601, with an optional timezone. yyyy-MM-ddTHH:mm:ss[+-]ZH:ZM - if the timezone offset is not given, GMT (+00:00) is assumed."
                     },
                     "value": {
                         "description": "A summary of the event.",
                         "maxLength": 4096,
                         "minLength": 1,
                         "type": "string"
                     }
@@ -1576,15 +2177,15 @@
                 "type": "object"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "timestamp": {
-            "description": "Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone in the format 'yyyy-MM-ddTHH:mm:ssZZZZ'. If timezone offset is not given, GMT (0000) is assumed.",
+            "description": "Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone in the format 'yyyy-MM-ddTHH:mm:ss[+-]ZH:ZM'. If timezone offset is not given, GMT (+00:00) is assumed.",
             "format": "date-time",
             "pattern": "^(((2000|2400|2800|(19|2[0-9](0[48]|[2468][048]|[13579][26])))-02-29)|(((19|2[0-9])[0-9]{2})-02-(0[1-9]|1[0-9]|2[0-8]))|(((19|2[0-9])[0-9]{2})-(0[13578]|10|12)-(0[1-9]|[12][0-9]|3[01]))|(((19|2[0-9])[0-9]{2})-(0[469]|11)-(0[1-9]|[12][0-9]|30)))T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\\.[0-9]+)?(Z|[+-][0-9]{2}:[0-9]{2})?$",
             "type": "string"
         },
         "uriType": {
             "description": "A universal resource identifier (URI), according to [RFC 3986](https://tools.ietf.org/html/rfc3986).",
             "format": "uri",
@@ -1609,29 +2210,32 @@
                 "$ref": "#/definitions/description"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         }
     },
-    "description": "An object containing the vulnerability information provided by an Authorized Data Publisher (ADP). Since multiple ADPs can provide information for a CVE ID, an ADP container must indicate which ADP is the source of the information in the object.",
-    "minProperties": 2,
+    "description": "An object containing the vulnerability information provided by a CVE Numbering Authority (CNA) for a published CVE ID. There can only be one CNA container per CVE record since there can only be one assigning CNA. The CNA container must include the required information defined in the CVE Rules, which includes a product, version, problem type, prose description, and a reference.",
     "patternProperties": {
         "^x_[^.]*$": {}
     },
     "properties": {
         "affected": {
             "$ref": "#/definitions/affected"
         },
         "configurations": {
             "$ref": "#/definitions/configurations"
         },
         "credits": {
             "$ref": "#/definitions/credits"
         },
+        "dateAssigned": {
+            "$ref": "#/definitions/timestamp",
+            "description": "The date/time this CVE ID was associated with a vulnerability by a CNA."
+        },
         "datePublic": {
             "$ref": "#/definitions/timestamp",
             "description": "If known, the date/time the vulnerability was disclosed publicly."
         },
         "descriptions": {
             "$ref": "#/definitions/descriptions"
         },
@@ -1656,31 +2260,34 @@
         "solutions": {
             "$ref": "#/definitions/solutions"
         },
         "source": {
             "$ref": "#/definitions/source"
         },
         "tags": {
-            "$ref": "#/definitions/adpTags"
+            "$ref": "#/definitions/cnaTags"
         },
         "taxonomyMappings": {
             "$ref": "#/definitions/taxonomyMappings"
         },
         "timeline": {
             "$ref": "#/definitions/timeline"
         },
         "title": {
-            "description": "A title, headline, or a brief phrase summarizing the information in an ADP container.",
+            "description": "A title, headline, or a brief phrase summarizing the CVE record. Eg., Buffer overflow in Example Soft.",
             "maxLength": 256,
             "minLength": 1,
             "type": "string"
         },
         "workarounds": {
             "$ref": "#/definitions/workarounds"
         }
     },
     "required": [
-        "providerMetadata"
+        "providerMetadata",
+        "descriptions",
+        "affected",
+        "references"
     ],
-    "title": "adp_container_5.0.0",
+    "title": "CVE_JSON_cnaPublishedContainer_5.1.0",
     "type": "object"
 }
```

### Comparing `cvelib-1.3.0/cvelib/schemas/extract_container_schemas.py` & `cvelib-1.4.0/cvelib/schemas/extract_container_schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 SCHEMAS_DIR = Path(__file__).parent
 
 
 def load_full_schema():
     try:
-        schema_file = next(SCHEMAS_DIR.glob("CVE_JSON_5.0_bundled_*.json"))
+        schema_file = next(SCHEMAS_DIR.glob("CVE_JSON_bundled_*.json"))
     except StopIteration:
         print("ERROR: No schema file found in the schemas directory!")
         sys.exit(1)
     with open(schema_file) as f:
         data = json.load(f)
 
     version = str(schema_file).rpartition("_")[2].removesuffix(".json")
@@ -74,25 +74,23 @@
     for attr in ("cveMetadataRejected", "cveMetadataPublished", "dataType", "dataVersion"):
         full_schema["definitions"].pop(attr)
 
     # Remove global oneOf attribute that sets up the full record schema. The container-level
     # schema of a specific container is placed in the global context below.
     full_schema.pop("oneOf")
 
-    container_to_filename = {
-        "cnaRejectedContainer": "rejected_cna_container",
-        "cnaPublishedContainer": "published_cna_container",
-        "adpContainer": "adp_container",
-    }
-    for object_name, file_name in container_to_filename.items():
+    container_names = ("cnaRejectedContainer", "cnaPublishedContainer", "adpContainer")
+    for container_name in container_names:
         # Save the objects from which we'll create the subschema
-        container_object = full_schema["definitions"].pop(object_name)
+        container_object = full_schema["definitions"].pop(container_name)
 
         # Create a copy of the full schema
         object_schema = copy.deepcopy(full_schema)
 
         # Wipe out the other two objects (provide default of None for the object that we already
         # popped above).
-        for attr in container_to_filename.keys():
+        for attr in container_names:
             object_schema["definitions"].pop(attr, None)
 
-        create_sub_schema(object_schema, container_object, f"{file_name}_{schema_version}.json")
+        create_sub_schema(
+            object_schema, container_object, f"CVE_JSON_{container_name}_{schema_version}.json"
+        )
```

### Comparing `cvelib-1.3.0/cvelib/schemas/published_cna_container_5.0.0.json` & `cvelib-1.4.0/cvelib/schemas/CVE_JSON_bundled_5.1.0.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2599026296739493%*

 * *Differences: {"'$id'": "'https://cveproject.github.io/cve-schema/schema/v5.0/docs/CVE_JSON_bundled.json'",*

 * * "'definitions'": "{'credits': {'items': {'additionalProperties': False}}, 'description': "*

 * *                  "{'properties': {'supportingMedia': {'items': {'additionalProperties': "*

 * *                  "False}}}}, 'englishLanguageDescription': {'$comment': 'Cannot use "*

 * *                  'additionalProperties: false here, as this prevents the other properties used by '*

 * *                  "/definitions/description.'}, […]*

```diff
@@ -1,19 +1,224 @@
 {
+    "$id": "https://cveproject.github.io/cve-schema/schema/v5.0/docs/CVE_JSON_bundled.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": false,
     "definitions": {
+        "adpContainer": {
+            "$comment": "The character . is restricted in names allowed by patternProperties to work-around naming limitations in some common implementations.",
+            "additionalProperties": false,
+            "description": "An object containing the vulnerability information provided by an Authorized Data Publisher (ADP). Since multiple ADPs can provide information for a CVE ID, an ADP container must indicate which ADP is the source of the information in the object.",
+            "minProperties": 2,
+            "patternProperties": {
+                "^x_[^.]*$": {}
+            },
+            "properties": {
+                "affected": {
+                    "$ref": "#/definitions/affected"
+                },
+                "configurations": {
+                    "$ref": "#/definitions/configurations"
+                },
+                "credits": {
+                    "$ref": "#/definitions/credits"
+                },
+                "datePublic": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "If known, the date/time the vulnerability was disclosed publicly."
+                },
+                "descriptions": {
+                    "$ref": "#/definitions/descriptions"
+                },
+                "exploits": {
+                    "$ref": "#/definitions/exploits"
+                },
+                "impacts": {
+                    "$ref": "#/definitions/impacts"
+                },
+                "metrics": {
+                    "$ref": "#/definitions/metrics"
+                },
+                "problemTypes": {
+                    "$ref": "#/definitions/problemTypes"
+                },
+                "providerMetadata": {
+                    "$ref": "#/definitions/providerMetadata"
+                },
+                "references": {
+                    "$ref": "#/definitions/references"
+                },
+                "solutions": {
+                    "$ref": "#/definitions/solutions"
+                },
+                "source": {
+                    "$ref": "#/definitions/source"
+                },
+                "tags": {
+                    "$ref": "#/definitions/adpTags"
+                },
+                "taxonomyMappings": {
+                    "$ref": "#/definitions/taxonomyMappings"
+                },
+                "timeline": {
+                    "$ref": "#/definitions/timeline"
+                },
+                "title": {
+                    "description": "A title, headline, or a brief phrase summarizing the information in an ADP container.",
+                    "maxLength": 256,
+                    "minLength": 1,
+                    "type": "string"
+                },
+                "workarounds": {
+                    "$ref": "#/definitions/workarounds"
+                }
+            },
+            "required": [
+                "providerMetadata"
+            ],
+            "type": "object"
+        },
+        "adpTags": {
+            "description": "Tags provided by an ADP describing the CVE Record.",
+            "items": {
+                "oneOf": [
+                    {
+                        "$ref": "#/definitions/tagExtension"
+                    },
+                    {
+                        "$id": "https://cve.mitre.org/cve/v5_00/tags/adp/",
+                        "$schema": "http://json-schema.org/draft-07/schema#",
+                        "description": "disputed: When one party disagrees with another party's assertion that a particular issue in software is a vulnerability, a CVE Record assigned to that issue may be tagged as being 'disputed'.",
+                        "enum": [
+                            "disputed"
+                        ],
+                        "type": "string"
+                    }
+                ]
+            },
+            "minItems": 1,
+            "type": "array",
+            "uniqueItems": true
+        },
         "affected": {
             "description": "List of affected products.",
             "items": {
                 "$ref": "#/definitions/product"
             },
             "minItems": 1,
             "type": "array"
         },
+        "cnaPublishedContainer": {
+            "$comment": "The character . is restricted in names allowed by patternProperties to work-around naming limitations in some common implementations.",
+            "additionalProperties": false,
+            "description": "An object containing the vulnerability information provided by a CVE Numbering Authority (CNA) for a published CVE ID. There can only be one CNA container per CVE record since there can only be one assigning CNA. The CNA container must include the required information defined in the CVE Rules, which includes a product, version, problem type, prose description, and a reference.",
+            "patternProperties": {
+                "^x_[^.]*$": {}
+            },
+            "properties": {
+                "affected": {
+                    "$ref": "#/definitions/affected"
+                },
+                "configurations": {
+                    "$ref": "#/definitions/configurations"
+                },
+                "credits": {
+                    "$ref": "#/definitions/credits"
+                },
+                "dateAssigned": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "The date/time this CVE ID was associated with a vulnerability by a CNA."
+                },
+                "datePublic": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "If known, the date/time the vulnerability was disclosed publicly."
+                },
+                "descriptions": {
+                    "$ref": "#/definitions/descriptions"
+                },
+                "exploits": {
+                    "$ref": "#/definitions/exploits"
+                },
+                "impacts": {
+                    "$ref": "#/definitions/impacts"
+                },
+                "metrics": {
+                    "$ref": "#/definitions/metrics"
+                },
+                "problemTypes": {
+                    "$ref": "#/definitions/problemTypes"
+                },
+                "providerMetadata": {
+                    "$ref": "#/definitions/providerMetadata"
+                },
+                "references": {
+                    "$ref": "#/definitions/references"
+                },
+                "solutions": {
+                    "$ref": "#/definitions/solutions"
+                },
+                "source": {
+                    "$ref": "#/definitions/source"
+                },
+                "tags": {
+                    "$ref": "#/definitions/cnaTags"
+                },
+                "taxonomyMappings": {
+                    "$ref": "#/definitions/taxonomyMappings"
+                },
+                "timeline": {
+                    "$ref": "#/definitions/timeline"
+                },
+                "title": {
+                    "description": "A title, headline, or a brief phrase summarizing the CVE record. Eg., Buffer overflow in Example Soft.",
+                    "maxLength": 256,
+                    "minLength": 1,
+                    "type": "string"
+                },
+                "workarounds": {
+                    "$ref": "#/definitions/workarounds"
+                }
+            },
+            "required": [
+                "providerMetadata",
+                "descriptions",
+                "affected",
+                "references"
+            ],
+            "type": "object"
+        },
+        "cnaRejectedContainer": {
+            "$comment": "The character . is restricted in names allowed by patternProperties to work-around naming limitations in some common implementations.",
+            "additionalProperties": false,
+            "description": "An object containing the vulnerability information provided by a CVE Numbering Authority (CNA) for a rejected CVE ID. There can only be one CNA container per CVE record since there can only be one assigning CNA.",
+            "patternProperties": {
+                "^x_[^.]*$": {}
+            },
+            "properties": {
+                "providerMetadata": {
+                    "$ref": "#/definitions/providerMetadata"
+                },
+                "rejectedReasons": {
+                    "$ref": "#/definitions/descriptions",
+                    "description": "Reasons for rejecting this CVE Record."
+                },
+                "replacedBy": {
+                    "description": "Contains an array of CVE IDs that this CVE ID was rejected in favor of because this CVE ID was assigned to the vulnerabilities.",
+                    "items": {
+                        "$ref": "#/definitions/cveId"
+                    },
+                    "minItems": 1,
+                    "type": "array",
+                    "uniqueItems": true
+                }
+            },
+            "required": [
+                "providerMetadata",
+                "rejectedReasons"
+            ],
+            "type": "object"
+        },
         "cnaTags": {
             "description": "Tags provided by a CNA describing the CVE Record.",
             "items": {
                 "oneOf": [
                     {
                         "$ref": "#/definitions/tagExtension"
                     },
@@ -42,14 +247,15 @@
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "credits": {
             "description": "Statements acknowledging specific people, organizations, or tools recognizing the work done in researching, discovering, remediating or helping with activities related to this CVE.",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "lang": {
                         "$ref": "#/definitions/language",
                         "description": "The language used when describing the credits. The language field is included so that CVE Records can support translations. The value must be a BCP 47 language code."
                     },
                     "type": {
                         "default": "finder",
@@ -84,24 +290,152 @@
                 ],
                 "type": "object"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
+        "cveId": {
+            "pattern": "^CVE-[0-9]{4}-[0-9]{4,19}$",
+            "type": "string"
+        },
+        "cveMetadataPublished": {
+            "additionalProperties": false,
+            "description": "This is meta data about the CVE ID such as the CVE ID, who requested it, who assigned it, when it was requested, the current state (PUBLISHED, REJECTED, etc.) and so on.  These fields are controlled by the CVE Services.",
+            "properties": {
+                "assignerOrgId": {
+                    "$ref": "#/definitions/orgId",
+                    "description": "The UUID for the organization to which the CVE ID was originally assigned. This UUID can be used to lookup the organization record in the user registry service."
+                },
+                "assignerShortName": {
+                    "$ref": "#/definitions/shortName",
+                    "description": "The short name for the organization to which the CVE ID was originally assigned."
+                },
+                "cveId": {
+                    "$ref": "#/definitions/cveId",
+                    "description": "The CVE identifier that this record pertains to."
+                },
+                "datePublished": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "The date/time the CVE Record was first published in the CVE List."
+                },
+                "dateReserved": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "The date/time this CVE ID was reserved in the CVE automation workgroup services system. Disclaimer: This date reflects when the CVE ID was reserved, and does not necessarily indicate when this vulnerability was discovered, shared with the affected vendor, publicly disclosed, or updated in CVE."
+                },
+                "dateUpdated": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "The date/time the record was last updated."
+                },
+                "requesterUserId": {
+                    "$ref": "#/definitions/userId",
+                    "description": "The user that requested the CVE identifier."
+                },
+                "serial": {
+                    "description": "The system of record causes this to start at 1, and increment by 1 each time a submission from a data provider changes this CVE Record. The incremented value moves to the Rejected schema upon a PUBLISHED->REJECTED transition, and moves to the Published schema upon a REJECTED->PUBLISHED transition.",
+                    "minimum": 1,
+                    "type": "integer"
+                },
+                "state": {
+                    "description": "State of CVE - PUBLISHED, REJECTED.",
+                    "enum": [
+                        "PUBLISHED"
+                    ],
+                    "type": "string"
+                }
+            },
+            "required": [
+                "cveId",
+                "assignerOrgId",
+                "state"
+            ],
+            "type": "object"
+        },
+        "cveMetadataRejected": {
+            "additionalProperties": false,
+            "description": "This is meta data about the CVE ID such as the CVE ID, who requested it, who assigned it, when it was requested, the current state (PUBLISHED, REJECTED, etc.) and so on.  These fields are controlled by the CVE Services.",
+            "properties": {
+                "assignerOrgId": {
+                    "$ref": "#/definitions/orgId",
+                    "description": "The UUID for the organization to which the CVE ID was originally assigned."
+                },
+                "assignerShortName": {
+                    "$ref": "#/definitions/shortName",
+                    "description": "The short name for the organization to which the CVE ID was originally assigned."
+                },
+                "cveId": {
+                    "$ref": "#/definitions/cveId",
+                    "description": "The CVE identifier that this record pertains to."
+                },
+                "datePublished": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "The date/time the CVE Record was first published in the CVE List."
+                },
+                "dateRejected": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "The date/time the CVE ID was rejected."
+                },
+                "dateReserved": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "The date/time this CVE ID was reserved in the CVE automation workgroup services system. Disclaimer: This date reflects when the CVE ID was reserved, and does not necessarily indicate when this vulnerability was discovered, shared with the affected vendor, publicly disclosed, or updated in CVE."
+                },
+                "dateUpdated": {
+                    "$ref": "#/definitions/timestamp",
+                    "description": "The date/time the record was last updated."
+                },
+                "serial": {
+                    "description": "The system of record causes this to start at 1, and increment by 1 each time a submission from a data provider changes this CVE Record. The incremented value moves to the Rejected schema upon a PUBLISHED->REJECTED transition, and moves to the Published schema upon a REJECTED->PUBLISHED transition.",
+                    "minimum": 1,
+                    "type": "integer"
+                },
+                "state": {
+                    "description": "State of CVE - PUBLISHED, REJECTED.",
+                    "enum": [
+                        "REJECTED"
+                    ],
+                    "type": "string"
+                }
+            },
+            "required": [
+                "cveId",
+                "assignerOrgId",
+                "state"
+            ],
+            "type": "object"
+        },
+        "dataType": {
+            "description": "Indicates the type of information represented in the JSON instance.",
+            "enum": [
+                "CVE_RECORD"
+            ],
+            "type": "string"
+        },
+        "dataVersion": {
+            "default": "5.1.0",
+            "description": "The version of the CVE schema used for validating this record. Used to support multiple versions of this format.",
+            "pattern": "^5\\.(0|[1-9][0-9]*)(\\.(0|[1-9][0-9]*))?$",
+            "type": "string"
+        },
+        "datestamp": {
+            "description": "Date/time format based on RFC3339 and ISO ISO8601.",
+            "format": "date",
+            "pattern": "^((2000|2400|2800|(19|2[0-9](0[48]|[2468][048]|[13579][26])))-02-29)|(((19|2[0-9])[0-9]{2})-02-(0[1-9]|1[0-9]|2[0-8]))|(((19|2[0-9])[0-9]{2})-(0[13578]|10|12)-(0[1-9]|[12][0-9]|3[01]))|(((19|2[0-9])[0-9]{2})-(0[469]|11)-(0[1-9]|[12][0-9]|30))$",
+            "type": "string"
+        },
         "description": {
             "additionalProperties": false,
             "description": "Text in a particular language with optional alternate markup or formatted representation (e.g., Markdown) or embedded media.",
             "properties": {
                 "lang": {
                     "$ref": "#/definitions/language"
                 },
                 "supportingMedia": {
                     "description": "Supporting media data for the description such as markdown, diagrams, .. (optional). Similar to RFC 2397 each media object has three main parts: media type, media data value, and an optional boolean flag to indicate if the media data is base64 encoded.",
                     "items": {
+                        "additionalProperties": false,
                         "properties": {
                             "base64": {
                                 "default": false,
                                 "description": "If true then the value field contains the media data encoded in base64. If false then the value field contains the UTF-8 media content.",
                                 "title": "Encoding",
                                 "type": "boolean"
                             },
@@ -164,14 +498,15 @@
         },
         "englishLanguage": {
             "description": "BCP 47 language code, language-region, required to be English.",
             "pattern": "^en([_-][A-Za-z]{4})?([_-]([A-Za-z]{2}|[0-9]{3}))?$",
             "type": "string"
         },
         "englishLanguageDescription": {
+            "$comment": "Cannot use additionalProperties: false here, as this prevents the other properties used by /definitions/description.",
             "description": "A description with lang set to an English language (en, en_US, en_UK, and so on).",
             "properties": {
                 "lang": {
                     "$ref": "#/definitions/englishLanguage"
                 }
             },
             "required": [
@@ -187,14 +522,15 @@
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "impacts": {
             "description": "Collection of impacts of this vulnerability.",
             "items": {
+                "additionalProperties": false,
                 "description": "This is impact type information (e.g. a text description.",
                 "properties": {
                     "capecId": {
                         "description": "CAPEC ID that best relates to this impact.",
                         "maxLength": 11,
                         "minLength": 7,
                         "pattern": "^CAPEC-[1-9][0-9]{0,4}$",
@@ -219,17 +555,23 @@
             "description": "BCP 47 language code, language-region.",
             "pattern": "^[A-Za-z]{2,4}([_-][A-Za-z]{4})?([_-]([A-Za-z]{2}|[0-9]{3}))?$",
             "type": "string"
         },
         "metrics": {
             "description": "Collection of impact scores with attribution.",
             "items": {
+                "additionalProperties": false,
                 "anyOf": [
                     {
                         "required": [
+                            "cvssV4_0"
+                        ]
+                    },
+                    {
+                        "required": [
                             "cvssV3_1"
                         ]
                     },
                     {
                         "required": [
                             "cvssV3_0"
                         ]
@@ -241,18 +583,19 @@
                     },
                     {
                         "required": [
                             "other"
                         ]
                     }
                 ],
-                "description": "This is impact type information (e.g. a text description, CVSSv2, CVSSv3, etc.). Must contain: At least one entry, can be text, CVSSv2, CVSSv3, others may be added.",
+                "description": "This is impact type information (e.g. a text description, CVSSv2, CVSSv3, CVSSV4, etc.). Must contain: At least one entry, can be text, CVSSv2, CVSSv3, others may be added.",
                 "properties": {
                     "cvssV2_0": {
                         "$schema": "http://json-schema.org/draft-04/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "accessComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "MEDIUM",
                                     "LOW"
                                 ],
@@ -417,14 +760,15 @@
                             "baseScore"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 2.0",
                         "type": "object"
                     },
                     "cvssV3_0": {
                         "$schema": "http://json-schema.org/draft-04/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "attackComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "LOW"
                                 ],
                                 "type": "string"
@@ -678,14 +1022,15 @@
                             "baseSeverity"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 3.0",
                         "type": "object"
                     },
                     "cvssV3_1": {
                         "$schema": "http://json-schema.org/draft-07/schema#",
+                        "additionalProperties": false,
                         "definitions": {
                             "attackComplexityType": {
                                 "enum": [
                                     "HIGH",
                                     "LOW"
                                 ],
                                 "type": "string"
@@ -937,24 +1282,592 @@
                             "vectorString",
                             "baseScore",
                             "baseSeverity"
                         ],
                         "title": "JSON Schema for Common Vulnerability Scoring System version 3.1",
                         "type": "object"
                     },
+                    "cvssV4_0": {
+                        "$schema": "http://json-schema.org/draft-07/schema#",
+                        "additionalProperties": false,
+                        "allOf": [
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "baseScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "baseSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            },
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "threatScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "threatSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            },
+                            {
+                                "anyOf": [
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/noneSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/lowSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/mediumSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/highSeverityType"
+                                            }
+                                        }
+                                    },
+                                    {
+                                        "properties": {
+                                            "environmentalScore": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalScoreType"
+                                            },
+                                            "environmentalSeverity": {
+                                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/criticalSeverityType"
+                                            }
+                                        }
+                                    }
+                                ]
+                            }
+                        ],
+                        "definitions": {
+                            "attackComplexityType": {
+                                "enum": [
+                                    "HIGH",
+                                    "LOW"
+                                ],
+                                "type": "string"
+                            },
+                            "attackRequirementsType": {
+                                "enum": [
+                                    "NONE",
+                                    "PRESENT"
+                                ],
+                                "type": "string"
+                            },
+                            "attackVectorType": {
+                                "enum": [
+                                    "NETWORK",
+                                    "ADJACENT",
+                                    "LOCAL",
+                                    "PHYSICAL"
+                                ],
+                                "type": "string"
+                            },
+                            "automatableType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NO",
+                                    "YES",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "ciaRequirementType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "LOW",
+                                    "MEDIUM",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "criticalScoreType": {
+                                "maximum": 10,
+                                "minimum": 9,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "criticalSeverityType": {
+                                "const": "CRITICAL"
+                            },
+                            "exploitMaturityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "UNREPORTED",
+                                    "PROOF_OF_CONCEPT",
+                                    "ATTACKED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "highScoreType": {
+                                "maximum": 8.9,
+                                "minimum": 7,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "highSeverityType": {
+                                "const": "HIGH"
+                            },
+                            "lowScoreType": {
+                                "maximum": 3.9,
+                                "minimum": 0.1,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "lowSeverityType": {
+                                "const": "LOW"
+                            },
+                            "mediumScoreType": {
+                                "maximum": 6.9,
+                                "minimum": 4,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "mediumSeverityType": {
+                                "const": "MEDIUM"
+                            },
+                            "modifiedAttackComplexityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedAttackRequirementsType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "PRESENT",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedAttackVectorType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NETWORK",
+                                    "ADJACENT",
+                                    "LOCAL",
+                                    "PHYSICAL",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedPrivilegesRequiredType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NONE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedSubCType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedSubIaType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "SAFETY",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedUserInteractionType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "PASSIVE",
+                                    "ACTIVE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "modifiedVulnCiaType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "noneScoreType": {
+                                "maximum": 0,
+                                "minimum": 0,
+                                "type": "number"
+                            },
+                            "noneSeverityType": {
+                                "const": "NONE"
+                            },
+                            "privilegesRequiredType": {
+                                "enum": [
+                                    "HIGH",
+                                    "LOW",
+                                    "NONE"
+                                ],
+                                "type": "string"
+                            },
+                            "providerUrgencyType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "CLEAR",
+                                    "GREEN",
+                                    "AMBER",
+                                    "RED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "recoveryType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "AUTOMATIC",
+                                    "USER",
+                                    "IRRECOVERABLE",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "safetyType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "NEGLIGIBLE",
+                                    "PRESENT",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "scoreType": {
+                                "maximum": 10,
+                                "minimum": 0,
+                                "multipleOf": 0.1,
+                                "type": "number"
+                            },
+                            "severityType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "MEDIUM",
+                                    "HIGH",
+                                    "CRITICAL"
+                                ],
+                                "type": "string"
+                            },
+                            "subCiaType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH"
+                                ],
+                                "type": "string"
+                            },
+                            "userInteractionType": {
+                                "enum": [
+                                    "NONE",
+                                    "PASSIVE",
+                                    "ACTIVE"
+                                ],
+                                "type": "string"
+                            },
+                            "valueDensityType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "DIFFUSE",
+                                    "CONCENTRATED",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnCiaType": {
+                                "enum": [
+                                    "NONE",
+                                    "LOW",
+                                    "HIGH"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnerabilityResponseEffortType": {
+                                "default": "NOT_DEFINED",
+                                "enum": [
+                                    "LOW",
+                                    "MODERATE",
+                                    "HIGH",
+                                    "NOT_DEFINED"
+                                ],
+                                "type": "string"
+                            }
+                        },
+                        "properties": {
+                            "Automatable": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/automatableType"
+                            },
+                            "Recovery": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/recoveryType"
+                            },
+                            "Safety": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/safetyType"
+                            },
+                            "attackComplexity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackComplexityType"
+                            },
+                            "attackRequirements": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackRequirementsType"
+                            },
+                            "attackVector": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/attackVectorType"
+                            },
+                            "availabilityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "baseScore": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/scoreType"
+                            },
+                            "baseSeverity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/severityType"
+                            },
+                            "confidentialityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "exploitMaturity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/exploitMaturityType"
+                            },
+                            "integrityRequirement": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/ciaRequirementType"
+                            },
+                            "modifiedAttackComplexity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackComplexityType"
+                            },
+                            "modifiedAttackRequirements": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackRequirementsType"
+                            },
+                            "modifiedAttackVector": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedAttackVectorType"
+                            },
+                            "modifiedPrivilegesRequired": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedPrivilegesRequiredType"
+                            },
+                            "modifiedSubAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubIaType"
+                            },
+                            "modifiedSubConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubCType"
+                            },
+                            "modifiedSubIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedSubIaType"
+                            },
+                            "modifiedUserInteraction": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedUserInteractionType"
+                            },
+                            "modifiedVulnAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "modifiedVulnConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "modifiedVulnIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/modifiedVulnCiaType"
+                            },
+                            "privilegesRequired": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/privilegesRequiredType"
+                            },
+                            "providerUrgency": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/providerUrgencyType"
+                            },
+                            "subAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "subConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "subIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/subCiaType"
+                            },
+                            "userInteraction": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/userInteractionType"
+                            },
+                            "valueDensity": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/valueDensityType"
+                            },
+                            "vectorString": {
+                                "pattern": "^CVSS:4[.]0/AV:[NALP]/AC:[LH]/AT:[NP]/PR:[NLH]/UI:[NPA]/VC:[HLN]/VI:[HLN]/VA:[HLN]/SC:[HLN]/SI:[HLN]/SA:[HLN](/E:[XAPU])?(/CR:[XHML])?(/IR:[XHML])?(/AR:[XHML])?(/MAV:[XNALP])?(/MAC:[XLH])?(/MAT:[XNP])?(/MPR:[XNLH])?(/MUI:[XNPA])?(/MVC:[XNLH])?(/MVI:[XNLH])?(/MVA:[XNLH])?(/MSC:[XNLH])?(/MSI:[XNLHS])?(/MSA:[XNLHS])?(/S:[XNP])?(/AU:[XNY])?(/R:[XAUI])?(/V:[XDC])?(/RE:[XLMH])?(/U:(X|Clear|Green|Amber|Red))?$",
+                                "type": "string"
+                            },
+                            "version": {
+                                "description": "CVSS Version",
+                                "enum": [
+                                    "4.0"
+                                ],
+                                "type": "string"
+                            },
+                            "vulnAvailabilityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnConfidentialityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnIntegrityImpact": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnCiaType"
+                            },
+                            "vulnerabilityResponseEffort": {
+                                "$ref": "#/definitions/metrics/items/properties/cvssV4_0/definitions/vulnerabilityResponseEffortType"
+                            }
+                        },
+                        "required": [
+                            "version",
+                            "vectorString",
+                            "baseScore",
+                            "baseSeverity"
+                        ],
+                        "title": "JSON Schema for Common Vulnerability Scoring System version 4.0",
+                        "type": "object"
+                    },
                     "format": {
                         "description": "Name of the scoring format. This provides a bit of future proofing. Additional properties are not prohibited, so this will support the inclusion of proprietary formats. It also provides an easy future conversion mechanism when future score formats become part of the schema. example: cvssV44, format = 'cvssV44', other = cvssV4_4 JSON object. In the future, the other properties can be converted to score properties when they become part of the schema.",
                         "maxLength": 64,
                         "minLength": 1,
                         "type": "string"
                     },
                     "other": {
+                        "additionalProperties": false,
                         "description": "A non-standard impact description, may be prose or JSON block.",
                         "properties": {
                             "content": {
+                                "$comment": "additionalProperties are allowed here, since this construct supports arbitrary JSON.",
                                 "description": "JSON object not covered by another metrics format.",
                                 "minProperties": 1,
                                 "type": "object"
                             },
                             "type": {
                                 "description": "Name of the non-standard impact metrics format used.",
                                 "maxLength": 128,
@@ -967,14 +1880,15 @@
                             "content"
                         ],
                         "type": "object"
                     },
                     "scenarios": {
                         "description": "Description of the scenarios this metrics object applies to. If no specific scenario is given, GENERAL is used as the default and applies when no more specific metric matches.",
                         "items": {
+                            "additionalProperties": false,
                             "properties": {
                                 "lang": {
                                     "$ref": "#/definitions/language"
                                 },
                                 "value": {
                                     "default": "GENERAL",
                                     "description": "Description of the scenario this metrics object applies to. If no specific scenario is given, GENERAL is used as the default and applies when no more specific metric matches.",
@@ -1003,17 +1917,19 @@
         "orgId": {
             "$ref": "#/definitions/uuidType",
             "description": "A UUID for an organization participating in the CVE program. This UUID can be used to lookup the organization record in the user registry service."
         },
         "problemTypes": {
             "description": "This is problem type information (e.g. CWE identifier). Must contain: At least one entry, can be text, OWASP, CWE, please note that while only one is required you can use more than one (or indeed all three) as long as they are correct). (CNA requirement: [PROBLEMTYPE]).",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "descriptions": {
                         "items": {
+                            "additionalProperties": false,
                             "properties": {
                                 "cweId": {
                                     "description": "CWE ID of the CWE that best describes this problemType entry.",
                                     "maxLength": 9,
                                     "minLength": 5,
                                     "pattern": "^CWE-[1-9][0-9]*$",
                                     "type": "string"
@@ -1236,14 +2152,15 @@
                     },
                     "type": "array",
                     "uniqueItems": true
                 },
                 "programRoutines": {
                     "description": "A list of the affected source code functions, methods, subroutines, or procedures (optional).",
                     "items": {
+                        "additionalProperties": false,
                         "description": "An object describing program routine.",
                         "properties": {
                             "name": {
                                 "description": "Name of the affected source code file, function, method, subroutine, or procedure.",
                                 "maxLength": 4096,
                                 "minLength": 1,
                                 "type": "string"
@@ -1266,47 +2183,54 @@
                     "maxLength": 512,
                     "minLength": 1,
                     "type": "string"
                 },
                 "versions": {
                     "description": "Set of product versions or version ranges related to the vulnerability. The versions satisfy the CNA Rules [8.1.2 requirement](https://cve.mitre.org/cve/cna/rules.html#section_8-1_cve_entry_information_requirements). Versions or defaultStatus may be omitted, but not both.",
                     "items": {
+                        "additionalProperties": false,
                         "description": "A single version or a range of versions, with vulnerability status.\n\nAn entry with only 'version' and 'status' indicates the status of a single version.\n\nOtherwise, an entry describes a range; it must include the 'versionType' property, to define the version numbering semantics in use, and 'limit', to indicate the non-inclusive upper limit of the range. The object describes the status for versions V such that 'version' <= V and V < 'limit', using the <= and < semantics defined for the specific kind of 'versionType'. Status changes within the range can be specified by an optional 'changes' list.\n\nThe algorithm to decide the status specified for a version V is:\n\n\tfor entry in product.versions {\n\t\tif entry.lessThan is not present and entry.lessThanOrEqual is not present and v == entry.version {\n\t\t\treturn entry.status\n\t\t}\n\t\tif (entry.lessThan is present and entry.version <= v and v < entry.lessThan) or\n\t\t   (entry.lessThanOrEqual is present and entry.version <= v and v <= entry.lessThanOrEqual) { // <= and < defined by entry.versionType\n\t\t\tstatus = entry.status\n\t\t\tfor change in entry.changes {\n\t\t\t\tif change.at <= v {\n\t\t\t\t\tstatus = change.status\n\t\t\t\t}\n\t\t\t}\n\t\t\treturn status\n\t\t}\n\t}\n\treturn product.defaultStatus\n\n.",
                         "oneOf": [
                             {
                                 "maxProperties": 2,
                                 "required": [
                                     "version",
                                     "status"
                                 ]
                             },
                             {
-                                "oneOf": [
-                                    {
-                                        "required": [
-                                            "lessThan"
-                                        ]
-                                    },
-                                    {
-                                        "required": [
-                                            "lessThanOrEqual"
-                                        ]
-                                    }
-                                ],
+                                "maxProperties": 3,
                                 "required": [
                                     "version",
                                     "status",
                                     "versionType"
                                 ]
+                            },
+                            {
+                                "required": [
+                                    "version",
+                                    "status",
+                                    "versionType",
+                                    "lessThan"
+                                ]
+                            },
+                            {
+                                "required": [
+                                    "version",
+                                    "status",
+                                    "versionType",
+                                    "lessThanOrEqual"
+                                ]
                             }
                         ],
                         "properties": {
                             "changes": {
                                 "description": "A list of status changes that take place during the range. The array should be sorted in increasing order by the 'at' field, according to the versionType, but clients must re-sort the list themselves rather than assume it is sorted.",
                                 "items": {
+                                    "additionalProperties": false,
                                     "description": "The start of a single status change during the range.",
                                     "properties": {
                                         "at": {
                                             "$ref": "#/definitions/version",
                                             "description": "The version at which a status change occurs."
                                         },
                                         "status": {
@@ -1361,14 +2285,15 @@
                     "type": "array",
                     "uniqueItems": true
                 }
             },
             "type": "object"
         },
         "providerMetadata": {
+            "additionalProperties": false,
             "description": "Details related to the information container provider (CNA or ADP).",
             "properties": {
                 "dateUpdated": {
                     "$ref": "#/definitions/timestamp",
                     "description": "Timestamp to be set by the system of record at time of submission. If dateUpdated is provided to the system of record it will be replaced by the current timestamp at the time of submission."
                 },
                 "orgId": {
@@ -1382,14 +2307,15 @@
             },
             "required": [
                 "orgId"
             ],
             "type": "object"
         },
         "reference": {
+            "additionalProperties": false,
             "properties": {
                 "name": {
                     "description": "User created name for the reference, often the title of the page.",
                     "maxLength": 512,
                     "minLength": 1,
                     "type": "string"
                 },
@@ -1479,34 +2405,37 @@
                 "affected",
                 "unaffected",
                 "unknown"
             ],
             "type": "string"
         },
         "tagExtension": {
+            "$comment": "These values are not used as JSON property names, so there is not a need to work-around property naming limitations in some common implementations.",
             "maxLength": 128,
             "minLength": 2,
             "pattern": "^x_.*$",
             "type": "string"
         },
         "taxonomyMappings": {
             "description": "List of taxonomy items related to the vulnerability.",
             "items": {
-                "description": "",
+                "additionalProperties": false,
+                "description": "A taxonomy mapping object identifies the taxonomy by a name and version (eg., ATT&CK v13.1, CVSS 3.1, CWE 4.12) along with a list of relations relevant to this CVE.",
                 "properties": {
                     "taxonomyName": {
-                        "description": "The name of the taxonomy.",
+                        "description": "The name of the taxonomy, eg., ATT&CK, D3FEND, CWE, CVSS",
                         "maxLength": 128,
                         "minLength": 1,
                         "type": "string"
                     },
                     "taxonomyRelations": {
-                        "description": "",
+                        "description": "List of relationships to the taxonomy for the vulnerability.",
                         "items": {
-                            "description": "List of relationships to the taxonomy for the vulnerability.  Relationships can be between the taxonomy and the CVE or two taxonomy items.",
+                            "additionalProperties": false,
+                            "description": "A relationship between the taxonomy and the CVE or two taxonomy items.",
                             "properties": {
                                 "relationshipName": {
                                     "description": "A description of the relationship.",
                                     "maxLength": 128,
                                     "minLength": 1,
                                     "type": "string"
                                 },
@@ -1550,22 +2479,23 @@
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "timeline": {
             "description": "This is timeline information for significant events about this vulnerability or changes to the CVE Record.",
             "items": {
+                "additionalProperties": false,
                 "properties": {
                     "lang": {
                         "$ref": "#/definitions/language",
                         "description": "The language used in the description of the event. The language field is included so that CVE Records can support translations. The value must be a BCP 47 language code."
                     },
                     "time": {
                         "$ref": "#/definitions/timestamp",
-                        "description": "Timestamp representing when the event in the timeline occurred. The timestamp format is based on RFC3339 and ISO ISO8601, with an optional timezone. yyyy-MM-ddTHH:mm:ssZZZZ - if the timezone offset is not given, GMT (0000) is assumed."
+                        "description": "Timestamp representing when the event in the timeline occurred. The timestamp format is based on RFC3339 and ISO ISO8601, with an optional timezone. yyyy-MM-ddTHH:mm:ss[+-]ZH:ZM - if the timezone offset is not given, GMT (+00:00) is assumed."
                     },
                     "value": {
                         "description": "A summary of the event.",
                         "maxLength": 4096,
                         "minLength": 1,
                         "type": "string"
                     }
@@ -1578,26 +2508,30 @@
                 "type": "object"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
         "timestamp": {
-            "description": "Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone in the format 'yyyy-MM-ddTHH:mm:ssZZZZ'. If timezone offset is not given, GMT (0000) is assumed.",
+            "description": "Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone in the format 'yyyy-MM-ddTHH:mm:ss[+-]ZH:ZM'. If timezone offset is not given, GMT (+00:00) is assumed.",
             "format": "date-time",
             "pattern": "^(((2000|2400|2800|(19|2[0-9](0[48]|[2468][048]|[13579][26])))-02-29)|(((19|2[0-9])[0-9]{2})-02-(0[1-9]|1[0-9]|2[0-8]))|(((19|2[0-9])[0-9]{2})-(0[13578]|10|12)-(0[1-9]|[12][0-9]|3[01]))|(((19|2[0-9])[0-9]{2})-(0[469]|11)-(0[1-9]|[12][0-9]|30)))T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\\.[0-9]+)?(Z|[+-][0-9]{2}:[0-9]{2})?$",
             "type": "string"
         },
         "uriType": {
             "description": "A universal resource identifier (URI), according to [RFC 3986](https://tools.ietf.org/html/rfc3986).",
             "format": "uri",
             "maxLength": 2048,
             "minLength": 1,
             "type": "string"
         },
+        "userId": {
+            "$ref": "#/definitions/uuidType",
+            "description": "A UUID for a user participating in the CVE program. This UUID can be used to lookup the user record in the user registry service."
+        },
         "uuidType": {
             "description": "A version 4 (random) universally unique identifier (UUID) as defined by [RFC 4122](https://tools.ietf.org/html/rfc4122#section-4.1.3).",
             "pattern": "^[0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-4[0-9A-Fa-f]{3}-[89ABab][0-9A-Fa-f]{3}-[0-9A-Fa-f]{12}$",
             "type": "string"
         },
         "version": {
             "description": "A single version of a product, as expressed in its own version numbering scheme.",
@@ -1611,84 +2545,92 @@
                 "$ref": "#/definitions/description"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         }
     },
-    "description": "An object containing the vulnerability information provided by a CVE Numbering Authority (CNA) for a published CVE ID. There can only be one CNA container per CVE record since there can only be one assigning CNA. The CNA container must include the required information defined in the CVE Rules, which includes a product, version, problem type, prose description, and a reference.",
-    "patternProperties": {
-        "^x_[^.]*$": {}
-    },
-    "properties": {
-        "affected": {
-            "$ref": "#/definitions/affected"
-        },
-        "configurations": {
-            "$ref": "#/definitions/configurations"
-        },
-        "credits": {
-            "$ref": "#/definitions/credits"
-        },
-        "dateAssigned": {
-            "$ref": "#/definitions/timestamp",
-            "description": "The date/time this CVE ID was associated with a vulnerability by a CNA."
-        },
-        "datePublic": {
-            "$ref": "#/definitions/timestamp",
-            "description": "If known, the date/time the vulnerability was disclosed publicly."
-        },
-        "descriptions": {
-            "$ref": "#/definitions/descriptions"
-        },
-        "exploits": {
-            "$ref": "#/definitions/exploits"
-        },
-        "impacts": {
-            "$ref": "#/definitions/impacts"
-        },
-        "metrics": {
-            "$ref": "#/definitions/metrics"
-        },
-        "problemTypes": {
-            "$ref": "#/definitions/problemTypes"
-        },
-        "providerMetadata": {
-            "$ref": "#/definitions/providerMetadata"
-        },
-        "references": {
-            "$ref": "#/definitions/references"
-        },
-        "solutions": {
-            "$ref": "#/definitions/solutions"
-        },
-        "source": {
-            "$ref": "#/definitions/source"
-        },
-        "tags": {
-            "$ref": "#/definitions/cnaTags"
-        },
-        "taxonomyMappings": {
-            "$ref": "#/definitions/taxonomyMappings"
-        },
-        "timeline": {
-            "$ref": "#/definitions/timeline"
-        },
-        "title": {
-            "description": "A title, headline, or a brief phrase summarizing the CVE record. Eg., Buffer overflow in Example Soft.",
-            "maxLength": 256,
-            "minLength": 1,
-            "type": "string"
+    "description": "cve-schema specifies the CVE JSON record format. This is the blueprint for a rich set of JSON data that can be submitted by CVE Numbering Authorities (CNAs) and Authorized Data Publishers (ADPs) to describe a CVE Record. Some examples of CVE Record data include CVE ID number, affected product(s), affected version(s), and public references. While those specific items are required when assigning a CVE, there are many other optional data in the schema that can be used to enrich CVE Records for community benefit. Learn more about the CVE program at [the official website](https://cve.mitre.org). This CVE JSON record format is defined using JSON Schema. Learn more about JSON Schema [here](https://json-schema.org/).",
+    "oneOf": [
+        {
+            "additionalProperties": false,
+            "description": "When a CNA populates the data associated with a CVE ID as a CVE Record, the state of the CVE Record is Published.",
+            "properties": {
+                "containers": {
+                    "additionalProperties": false,
+                    "description": "A set of structures (called containers) used to store vulnerability information related to a specific CVE ID provided by a specific organization participating in the CVE program. Each container includes information provided by a different source.\n\nAt a minimum, a 'cna' container containing the vulnerability information provided by the CNA who initially assigned the CVE ID must be included.\n\nThere can only be one 'cna' container, as there can only be one assigning CNA. However, there can be multiple 'adp' containers, allowing multiple organizations participating in the CVE program to add additional information related to the vulnerability. For the most part, the 'cna' and 'adp' containers contain the same properties. The main differences are the source of the information. The 'cna' container requires the CNA to include certain fields, while the 'adp' container does not.",
+                    "properties": {
+                        "adp": {
+                            "items": {
+                                "$ref": "#/definitions/adpContainer"
+                            },
+                            "minItems": 1,
+                            "type": "array",
+                            "uniqueItems": true
+                        },
+                        "cna": {
+                            "$ref": "#/definitions/cnaPublishedContainer"
+                        }
+                    },
+                    "required": [
+                        "cna"
+                    ],
+                    "type": "object"
+                },
+                "cveMetadata": {
+                    "$ref": "#/definitions/cveMetadataPublished"
+                },
+                "dataType": {
+                    "$ref": "#/definitions/dataType"
+                },
+                "dataVersion": {
+                    "$ref": "#/definitions/dataVersion"
+                }
+            },
+            "required": [
+                "dataType",
+                "dataVersion",
+                "cveMetadata",
+                "containers"
+            ],
+            "title": "Published",
+            "type": "object"
         },
-        "workarounds": {
-            "$ref": "#/definitions/workarounds"
+        {
+            "additionalProperties": false,
+            "description": "If the CVE ID and associated CVE Record should no longer be used, the CVE Record is placed in the Rejected state. A Rejected CVE Record remains on the CVE List so that users can know when it is invalid.",
+            "properties": {
+                "containers": {
+                    "additionalProperties": false,
+                    "description": "A set of structures (called containers) used to store vulnerability information related to a specific CVE ID provided by a specific organization participating in the CVE program. Each container includes information provided by a different source.\n\nAt minimum, a 'cna' container containing the vulnerability information provided by the CNA who initially assigned the CVE ID must be included.\n\nThere can only be one 'cna' container, as there can only be one assigning CNA.",
+                    "properties": {
+                        "cna": {
+                            "$ref": "#/definitions/cnaRejectedContainer"
+                        }
+                    },
+                    "required": [
+                        "cna"
+                    ],
+                    "type": "object"
+                },
+                "cveMetadata": {
+                    "$ref": "#/definitions/cveMetadataRejected"
+                },
+                "dataType": {
+                    "$ref": "#/definitions/dataType"
+                },
+                "dataVersion": {
+                    "$ref": "#/definitions/dataVersion"
+                }
+            },
+            "required": [
+                "dataType",
+                "dataVersion",
+                "cveMetadata",
+                "containers"
+            ],
+            "title": "Rejected",
+            "type": "object"
         }
-    },
-    "required": [
-        "providerMetadata",
-        "descriptions",
-        "affected",
-        "references"
     ],
-    "title": "published_cna_container_5.0.0",
-    "type": "object"
+    "title": "CVE JSON record format"
 }
```

### Comparing `cvelib-1.3.0/cvelib/schemas/rejected_cna_container_5.0.0.json` & `cvelib-1.4.0/cvelib/schemas/CVE_JSON_cnaRejectedContainer_5.1.0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8488060290404039%*

 * *Differences: {"'$comment'": "'The character . is restricted in names allowed by patternProperties to "*

 * *               "work-around naming limitations in some common implementations.'",*

 * * "'definitions'": "{'description': {'properties': {'supportingMedia': {'items': "*

 * *                  "{'additionalProperties': False}}}}, 'englishLanguageDescription': {'$comment': "*

 * *                  "'Cannot use additionalProperties: false here, as this prevents the other "*

 * *                  "properties used by /definitions/description.' […]*

```diff
@@ -1,8 +1,9 @@
 {
+    "$comment": "The character . is restricted in names allowed by patternProperties to work-around naming limitations in some common implementations.",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "definitions": {
         "cveId": {
             "pattern": "^CVE-[0-9]{4}-[0-9]{4,19}$",
             "type": "string"
         },
@@ -12,14 +13,15 @@
             "properties": {
                 "lang": {
                     "$ref": "#/definitions/language"
                 },
                 "supportingMedia": {
                     "description": "Supporting media data for the description such as markdown, diagrams, .. (optional). Similar to RFC 2397 each media object has three main parts: media type, media data value, and an optional boolean flag to indicate if the media data is base64 encoded.",
                     "items": {
+                        "additionalProperties": false,
                         "properties": {
                             "base64": {
                                 "default": false,
                                 "description": "If true then the value field contains the media data encoded in base64. If false then the value field contains the UTF-8 media content.",
                                 "title": "Encoding",
                                 "type": "boolean"
                             },
@@ -82,14 +84,15 @@
         },
         "englishLanguage": {
             "description": "BCP 47 language code, language-region, required to be English.",
             "pattern": "^en([_-][A-Za-z]{4})?([_-]([A-Za-z]{2}|[0-9]{3}))?$",
             "type": "string"
         },
         "englishLanguageDescription": {
+            "$comment": "Cannot use additionalProperties: false here, as this prevents the other properties used by /definitions/description.",
             "description": "A description with lang set to an English language (en, en_US, en_UK, and so on).",
             "properties": {
                 "lang": {
                     "$ref": "#/definitions/englishLanguage"
                 }
             },
             "required": [
@@ -104,14 +107,15 @@
             "type": "string"
         },
         "orgId": {
             "$ref": "#/definitions/uuidType",
             "description": "A UUID for an organization participating in the CVE program. This UUID can be used to lookup the organization record in the user registry service."
         },
         "providerMetadata": {
+            "additionalProperties": false,
             "description": "Details related to the information container provider (CNA or ADP).",
             "properties": {
                 "dateUpdated": {
                     "$ref": "#/definitions/timestamp",
                     "description": "Timestamp to be set by the system of record at time of submission. If dateUpdated is provided to the system of record it will be replaced by the current timestamp at the time of submission."
                 },
                 "orgId": {
@@ -131,15 +135,15 @@
         "shortName": {
             "description": "A 2-32 character name that can be used to complement an organization's UUID.",
             "maxLength": 32,
             "minLength": 2,
             "type": "string"
         },
         "timestamp": {
-            "description": "Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone in the format 'yyyy-MM-ddTHH:mm:ssZZZZ'. If timezone offset is not given, GMT (0000) is assumed.",
+            "description": "Date/time format based on RFC3339 and ISO ISO8601, with an optional timezone in the format 'yyyy-MM-ddTHH:mm:ss[+-]ZH:ZM'. If timezone offset is not given, GMT (+00:00) is assumed.",
             "format": "date-time",
             "pattern": "^(((2000|2400|2800|(19|2[0-9](0[48]|[2468][048]|[13579][26])))-02-29)|(((19|2[0-9])[0-9]{2})-02-(0[1-9]|1[0-9]|2[0-8]))|(((19|2[0-9])[0-9]{2})-(0[13578]|10|12)-(0[1-9]|[12][0-9]|3[01]))|(((19|2[0-9])[0-9]{2})-(0[469]|11)-(0[1-9]|[12][0-9]|30)))T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\\.[0-9]+)?(Z|[+-][0-9]{2}:[0-9]{2})?$",
             "type": "string"
         },
         "uuidType": {
             "description": "A version 4 (random) universally unique identifier (UUID) as defined by [RFC 4122](https://tools.ietf.org/html/rfc4122#section-4.1.3).",
             "pattern": "^[0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-4[0-9A-Fa-f]{3}-[89ABab][0-9A-Fa-f]{3}-[0-9A-Fa-f]{12}$",
@@ -168,10 +172,10 @@
             "uniqueItems": true
         }
     },
     "required": [
         "providerMetadata",
         "rejectedReasons"
     ],
-    "title": "rejected_cna_container_5.0.0",
+    "title": "CVE_JSON_cnaRejectedContainer_5.1.0",
     "type": "object"
 }
```

### Comparing `cvelib-1.3.0/cvelib.egg-info/PKG-INFO` & `cvelib-1.4.0/cvelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvelib
-Version: 1.3.0
+Version: 1.4.0
 Summary: A library and command line interface for the CVE Project services.
 Home-page: https://github.com/RedHatProductSecurity/cvelib
 Author: Red Hat Product Security
 Author-email: secalert@redhat.com
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
@@ -32,19 +32,19 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # cvelib
 
 A library and a command line interface for the CVE Services API.
 
-**Note**: version 1.3.0 of cvelib is compatible with CVE Services 2.2.0.
+**Note**: version 1.4.0 of cvelib is compatible with CVE Services 2.3.1 and CVE JSON schema 5.1.0.
 
 ## Requirements
 
-- Python version 3.7 or greater
+- Python version 3.8 or greater
 - [pip](https://pypi.org/project/pip/)
 
 ## Installation
 
 ### Linux, MacOS, Windows
 
 ```bash
```

### Comparing `cvelib-1.3.0/cvelib.egg-info/SOURCES.txt` & `cvelib-1.4.0/cvelib.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 cvelib/cve_api.py
 cvelib.egg-info/PKG-INFO
 cvelib.egg-info/SOURCES.txt
 cvelib.egg-info/dependency_links.txt
 cvelib.egg-info/entry_points.txt
 cvelib.egg-info/requires.txt
 cvelib.egg-info/top_level.txt
-cvelib/schemas/CVE_JSON_5.0_bundled_5.0.0.json
+cvelib/schemas/CVE_JSON_adpContainer_5.1.0.json
+cvelib/schemas/CVE_JSON_bundled_5.1.0.json
+cvelib/schemas/CVE_JSON_cnaPublishedContainer_5.1.0.json
+cvelib/schemas/CVE_JSON_cnaRejectedContainer_5.1.0.json
 cvelib/schemas/README.md
-cvelib/schemas/adp_container_5.0.0.json
 cvelib/schemas/extract_container_schemas.py
-cvelib/schemas/published_cna_container_5.0.0.json
-cvelib/schemas/rejected_cna_container_5.0.0.json
 man/cve-list.1
 man/cve-org-users.1
 man/cve-org.1
 man/cve-ping.1
 man/cve-publish-adp.1
 man/cve-publish.1
 man/cve-quota.1
```

### Comparing `cvelib-1.3.0/man/cve-list.1` & `cvelib-1.4.0/man/cve-list.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE LIST" "1" "2024-01-26" "1.3.0" "cve list Manual"
+.TH "CVE LIST" "1" "2024-05-15" "1.4.0" "cve list Manual"
 .SH NAME
 cve\-list \- Filter and list reserved CVE IDs owned by...
 .SH SYNOPSIS
 .B cve list
 [OPTIONS]
 .SH DESCRIPTION
 Filter and list reserved CVE IDs owned by your CNA.
```

### Comparing `cvelib-1.3.0/man/cve-publish-adp.1` & `cvelib-1.4.0/man/cve-publish-adp.1`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE PUBLISH-ADP" "1" "2024-01-26" "1.3.0" "cve publish-adp Manual"
+.TH "CVE PUBLISH-ADP" "1" "2024-05-15" "1.4.0" "cve publish-adp Manual"
 .SH NAME
 cve\-publish-adp \- Add or update an ADP container in a CVE...
 .SH SYNOPSIS
 .B cve publish-adp
 [OPTIONS] CVE_ID
 .SH DESCRIPTION
 Add or update an ADP container in a CVE record for a published CVE ID.
```

### Comparing `cvelib-1.3.0/man/cve-publish.1` & `cvelib-1.4.0/man/cve-publish.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE PUBLISH" "1" "2024-01-26" "1.3.0" "cve publish Manual"
+.TH "CVE PUBLISH" "1" "2024-05-15" "1.4.0" "cve publish Manual"
 .SH NAME
 cve\-publish \- Publish a CNA container of a CVE record...
 .SH SYNOPSIS
 .B cve publish
 [OPTIONS] CVE_ID
 .SH DESCRIPTION
 Publish a CNA container of a CVE record for a reserved (or rejected) CVE ID.
```

### Comparing `cvelib-1.3.0/man/cve-quota.1` & `cvelib-1.4.0/man/cve-quota.1`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE QUOTA" "1" "2024-01-26" "1.3.0" "cve quota Manual"
+.TH "CVE QUOTA" "1" "2024-05-15" "1.4.0" "cve quota Manual"
 .SH NAME
 cve\-quota \- Display the available CVE ID quota for...
 .SH SYNOPSIS
 .B cve quota
 [OPTIONS]
 .SH DESCRIPTION
 Display the available CVE ID quota for your CNA.
```

### Comparing `cvelib-1.3.0/man/cve-reject.1` & `cvelib-1.4.0/man/cve-reject.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE REJECT" "1" "2024-01-26" "1.3.0" "cve reject Manual"
+.TH "CVE REJECT" "1" "2024-05-15" "1.4.0" "cve reject Manual"
 .SH NAME
 cve\-reject \- Reject a CVE record for a reserved or...
 .SH SYNOPSIS
 .B cve reject
 [OPTIONS] CVE_ID
 .SH DESCRIPTION
 Reject a CVE record for a reserved or published CVE ID.
```

### Comparing `cvelib-1.3.0/man/cve-reserve.1` & `cvelib-1.4.0/man/cve-reserve.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE RESERVE" "1" "2024-01-26" "1.3.0" "cve reserve Manual"
+.TH "CVE RESERVE" "1" "2024-05-15" "1.4.0" "cve reserve Manual"
 .SH NAME
 cve\-reserve \- Reserve one or more CVE IDs.
 .SH SYNOPSIS
 .B cve reserve
 [OPTIONS] [COUNT]
 .SH DESCRIPTION
 Reserve one or more CVE IDs. COUNT is the number of CVEs to reserve; defaults to 1.
```

### Comparing `cvelib-1.3.0/man/cve-show.1` & `cvelib-1.4.0/man/cve-show.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE SHOW" "1" "2024-01-26" "1.3.0" "cve show Manual"
+.TH "CVE SHOW" "1" "2024-05-15" "1.4.0" "cve show Manual"
 .SH NAME
 cve\-show \- Display a specific CVE ID (and optionally...
 .SH SYNOPSIS
 .B cve show
 [OPTIONS] CVE_ID
 .SH DESCRIPTION
 Display a specific CVE ID (and optionally its record) owned by your CNA.
```

### Comparing `cvelib-1.3.0/man/cve-user-create.1` & `cvelib-1.4.0/man/cve-user-create.1`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE USER CREATE" "1" "2024-01-26" "1.3.0" "cve user create Manual"
+.TH "CVE USER CREATE" "1" "2024-05-15" "1.4.0" "cve user create Manual"
 .SH NAME
 cve\-user\-create \- Create a user in your organization.
 .SH SYNOPSIS
 .B cve user create
 [OPTIONS]
 .SH DESCRIPTION
 Create a user in your organization.
```

### Comparing `cvelib-1.3.0/man/cve-user.1` & `cvelib-1.4.0/man/cve-user.1`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE USER" "1" "2024-01-26" "1.3.0" "cve user Manual"
+.TH "CVE USER" "1" "2024-05-15" "1.4.0" "cve user Manual"
 .SH NAME
 cve\-user \- Show information about a user.
 .SH SYNOPSIS
 .B cve user
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 Show information about a user.
```

### Comparing `cvelib-1.3.0/man/cve.1` & `cvelib-1.4.0/man/cve.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "CVE" "1" "2024-01-26" "1.3.0" "cve Manual"
+.TH "CVE" "1" "2024-05-15" "1.4.0" "cve Manual"
 .SH NAME
 cve \- A CLI interface for the CVE Services API.
 .SH SYNOPSIS
 .B cve
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 A CLI interface for the CVE Services API.
```

### Comparing `cvelib-1.3.0/setup.py` & `cvelib-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `cvelib-1.3.0/tests/data/CVEv5_advanced-example.json` & `cvelib-1.4.0/tests/data/CVEv5_advanced-example.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8747702205882353%*

 * *Differences: {"'containers'": "{'cna': {'metrics': {0: {'cvssV4_0': OrderedDict([('baseScore', 7.8), "*

 * *                 "('baseSeverity', 'HIGH'), ('vectorString', "*

 * *                 "'CVSS:4.0/AV:N/AC:L/AT:N/PR:N/UI:N/VC:N/VI:N/VA:N/SC:H/SI:L/SA:L'), ('version', "*

 * *                 "'4.0')])}}}}",*

 * * "'dataVersion'": "'5.1'"}*

```diff
@@ -148,14 +148,20 @@
                         "integrityImpact": "HIGH",
                         "privilegesRequired": "NONE",
                         "scope": "UNCHANGED",
                         "userInteraction": "NONE",
                         "vectorString": "CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H",
                         "version": "3.1"
                     },
+                    "cvssV4_0": {
+                        "baseScore": 7.8,
+                        "baseSeverity": "HIGH",
+                        "vectorString": "CVSS:4.0/AV:N/AC:L/AT:N/PR:N/UI:N/VC:N/VI:N/VA:N/SC:H/SI:L/SA:L",
+                        "version": "4.0"
+                    },
                     "format": "CVSS",
                     "scenarios": [
                         {
                             "lang": "en",
                             "value": "GENERAL"
                         }
                     ]
@@ -302,9 +308,9 @@
         "assignerShortName": "example",
         "cveId": "CVE-1337-1234",
         "requesterUserId": "b3476cb9-2e3d-41a6-98d0-0f47421a65b6",
         "serial": 1,
         "state": "PUBLISHED"
     },
     "dataType": "CVE_RECORD",
-    "dataVersion": "5.0"
+    "dataVersion": "5.1"
 }
```

### Comparing `cvelib-1.3.0/tests/data/CVEv5_basic-example.json` & `cvelib-1.4.0/tests/data/CVEv5_basic-example.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'dataVersion'": "'5.1'"}*

```diff
@@ -44,9 +44,9 @@
     },
     "cveMetadata": {
         "assignerOrgId": "b3476cb9-2e3d-41a6-98d0-0f47421a65b6",
         "cveId": "CVE-1337-1234",
         "state": "PUBLISHED"
     },
     "dataType": "CVE_RECORD",
-    "dataVersion": "5.0"
+    "dataVersion": "5.1"
 }
```

### Comparing `cvelib-1.3.0/tests/data/container-advanced-example.json` & `cvelib-1.4.0/tests/data/container-advanced-example.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963235294117647%*

 * *Differences: {"'metrics'": "{0: {'cvssV4_0': OrderedDict([('baseScore', 7.8), ('baseSeverity', 'HIGH'), "*

 * *              "('vectorString', "*

 * *              "'CVSS:4.0/AV:N/AC:L/AT:N/PR:N/UI:N/VC:N/VI:N/VA:N/SC:H/SI:L/SA:L'), ('version', "*

 * *              "'4.0')])}}"}*

```diff
@@ -146,14 +146,20 @@
                 "integrityImpact": "HIGH",
                 "privilegesRequired": "NONE",
                 "scope": "UNCHANGED",
                 "userInteraction": "NONE",
                 "vectorString": "CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H",
                 "version": "3.1"
             },
+            "cvssV4_0": {
+                "baseScore": 7.8,
+                "baseSeverity": "HIGH",
+                "vectorString": "CVSS:4.0/AV:N/AC:L/AT:N/PR:N/UI:N/VC:N/VI:N/VA:N/SC:H/SI:L/SA:L",
+                "version": "4.0"
+            },
             "format": "CVSS",
             "scenarios": [
                 {
                     "lang": "en",
                     "value": "GENERAL"
                 }
             ]
```

### Comparing `cvelib-1.3.0/tests/data/container-basic-example.json` & `cvelib-1.4.0/tests/data/container-basic-example.json`

 * *Files identical despite different names*

### Comparing `cvelib-1.3.0/tests/test_cli.py` & `cvelib-1.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cvelib-1.3.0/tests/test_cve_api.py` & `cvelib-1.4.0/tests/test_cve_api.py`

 * *Files identical despite different names*

