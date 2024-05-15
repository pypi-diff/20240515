# Comparing `tmp/spdx3query-0.0.1.tar.gz` & `tmp/spdx3query-0.0.2.tar.gz`

## Comparing `spdx3query-0.0.1.tar` & `spdx3query-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 spdx3query-0.0.1/.flake8
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 spdx3query-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 spdx3query-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/__main__.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/cmd.py
--rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/main.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/name.py
--rw-r--r--   0        0        0   249528 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/spdx3.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/version.py
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/wordlist.txt
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/commands/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/commands/build.py
--rw-r--r--   0        0        0     7840 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/commands/find.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/commands/info.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/commands/load.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/commands/show.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 spdx3query-0.0.1/src/spdx3query/commands/vuln.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 spdx3query-0.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 spdx3query-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 spdx3query-0.0.1/LICENSE
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 spdx3query-0.0.1/README.md
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 spdx3query-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 spdx3query-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 spdx3query-0.0.2/.flake8
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 spdx3query-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 spdx3query-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/__main__.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/cmd.py
+-rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/main.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/name.py
+-rw-r--r--   0        0        0   249528 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/spdx3.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/version.py
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/wordlist.txt
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/commands/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/commands/build.py
+-rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/commands/find.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/commands/info.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/commands/load.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/commands/show.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 spdx3query-0.0.2/src/spdx3query/commands/vuln.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 spdx3query-0.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 spdx3query-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 spdx3query-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 spdx3query-0.0.2/README.md
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 spdx3query-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 spdx3query-0.0.2/PKG-INFO
```

### Comparing `spdx3query-0.0.1/.github/workflows/publish.yaml` & `spdx3query-0.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/.github/workflows/test.yaml` & `spdx3query-0.0.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/cmd.py` & `spdx3query-0.0.2/src/spdx3query/cmd.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/main.py` & `spdx3query-0.0.2/src/spdx3query/main.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/name.py` & `spdx3query-0.0.2/src/spdx3query/name.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/spdx3.py` & `spdx3query-0.0.2/src/spdx3query/spdx3.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/wordlist.txt` & `spdx3query-0.0.2/src/spdx3query/wordlist.txt`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/commands/build.py` & `spdx3query-0.0.2/src/spdx3query/commands/build.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/commands/find.py` & `spdx3query-0.0.2/src/spdx3query/commands/find.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         if args.subclass:
             final &= set(doc.foreach_type(args.subclass, match_subclass=True))
 
         if args.verified_using:
             objs = set()
 
             algo, val = args.verified_using
-            algo_iri = check_enum(algo, spdx3.HashAlgoritm, "hash algorithm")
+            algo_iri = check_enum(algo, spdx3.HashAlgorithm, "hash algorithm")
 
             for o in doc.foreach_type(spdx3.Element, match_subclass=True):
                 for v in o.verifiedUsing:
                     if isinstance(v, spdx3.Hash):
                         if v.algorithm == algo_iri and v.hashValue == val:
                             objs.add(o)
```

### Comparing `spdx3query-0.0.1/src/spdx3query/commands/info.py` & `spdx3query-0.0.2/src/spdx3query/commands/info.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/commands/load.py` & `spdx3query-0.0.2/src/spdx3query/commands/load.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/commands/show.py` & `spdx3query-0.0.2/src/spdx3query/commands/show.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/src/spdx3query/commands/vuln.py` & `spdx3query-0.0.2/src/spdx3query/commands/vuln.py`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/.gitignore` & `spdx3query-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/LICENSE` & `spdx3query-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spdx3query-0.0.1/pyproject.toml` & `spdx3query-0.0.2/pyproject.toml`

 * *Files identical despite different names*

