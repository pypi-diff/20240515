# Comparing `tmp/mowaki-2.0.tar.gz` & `tmp/mowaki-2.0a2.tar.gz`

## Comparing `mowaki-2.0.tar` & `mowaki-2.0a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 mowaki-2.0/.travis.yml
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mowaki-2.0/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/__init__.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/config.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/context.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/crypto.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/database.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/email_composer.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/jwt.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/emailer/__init__.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/emailer/base.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/emailer/dummy.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/emailer/smtp.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/storage/__init__.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/storage/base.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/storage/storage_file.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/storage/storage_memory.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/storage/storage_s3.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 mowaki-2.0/mowaki/storage/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mowaki-2.0/tests/__init__.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 mowaki-2.0/tests/test_config.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 mowaki-2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mowaki-2.0/LICENSE
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mowaki-2.0/README.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 mowaki-2.0/pyproject.toml
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 mowaki-2.0/PKG-INFO
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 mowaki-2.0a2/.travis.yml
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mowaki-2.0a2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/__init__.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/config.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/context.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/crypto.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/database.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/email_composer.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/jwt.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/emailer/__init__.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/emailer/base.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/emailer/dummy.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/emailer/smtp.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/__init__.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/base.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/storage_file.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/storage_memory.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/storage_s3.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mowaki-2.0a2/tests/__init__.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 mowaki-2.0a2/tests/test_config.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 mowaki-2.0a2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mowaki-2.0a2/LICENSE
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mowaki-2.0a2/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 mowaki-2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 mowaki-2.0a2/PKG-INFO
```

### Comparing `mowaki-2.0/setup.py` & `mowaki-2.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/config.py` & `mowaki-2.0a2/mowaki/config.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/crypto.py` & `mowaki-2.0a2/mowaki/crypto.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/database.py` & `mowaki-2.0a2/mowaki/database.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/email_composer.py` & `mowaki-2.0a2/mowaki/email_composer.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/jwt.py` & `mowaki-2.0a2/mowaki/jwt.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/emailer/__init__.py` & `mowaki-2.0a2/mowaki/emailer/__init__.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/emailer/dummy.py` & `mowaki-2.0a2/mowaki/emailer/dummy.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/emailer/smtp.py` & `mowaki-2.0a2/mowaki/emailer/smtp.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/storage/__init__.py` & `mowaki-2.0a2/mowaki/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/storage/base.py` & `mowaki-2.0a2/mowaki/storage/base.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/storage/storage_file.py` & `mowaki-2.0a2/mowaki/storage/storage_file.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/storage/storage_memory.py` & `mowaki-2.0a2/mowaki/storage/storage_memory.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/storage/storage_s3.py` & `mowaki-2.0a2/mowaki/storage/storage_s3.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/mowaki/storage/types.py` & `mowaki-2.0a2/mowaki/storage/types.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/tests/test_config.py` & `mowaki-2.0a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/.gitignore` & `mowaki-2.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/LICENSE` & `mowaki-2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/pyproject.toml` & `mowaki-2.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mowaki-2.0/PKG-INFO` & `mowaki-2.0a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mowaki
-Version: 2.0
+Version: 2.0a2
 Summary: Utilities for MoWaKi (and other) apps
 Project-URL: Homepage, https://www.mowaki.org
 Project-URL: Repository, https://github.com/rshk/mowaki-py
 Project-URL: Issues, https://github.com/rshk/mowaki-py/issues
 Author-email: Sam Santi <samuele@samuelesanti.com>
 License: MIT License
```

