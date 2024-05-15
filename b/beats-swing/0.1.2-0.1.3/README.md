# Comparing `tmp/beats_swing-0.1.2.tar.gz` & `tmp/beats_swing-0.1.3.tar.gz`

## Comparing `beats_swing-0.1.2.tar` & `beats_swing-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 beats_swing-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 beats_swing-0.1.2/DEVELOPMENT.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 beats_swing-0.1.2/Makefile
--rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 beats_swing-0.1.2/pylintrc
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 beats_swing-0.1.2/test_requirements.txt
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 beats_swing-0.1.2/.github/workflows/build_release.yml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 beats_swing-0.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 beats_swing-0.1.2/scripts/explorer.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 beats_swing-0.1.2/scripts/first_pass.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 beats_swing-0.1.2/scripts/librosa_explorer.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 beats_swing-0.1.2/scripts/mess_around_w_librosa.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 beats_swing-0.1.2/scripts/score.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/__init__.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/cli.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/constants.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/filtering.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/shared_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/estimators/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/estimators/api.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/estimators/librosa.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/estimators/trivial.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 beats_swing-0.1.2/src/beats/estimators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.2/tests/beats/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 beats_swing-0.1.2/tests/beats/test_cli.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 beats_swing-0.1.2/tests/beats/test_smoke.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 beats_swing-0.1.2/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 beats_swing-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 beats_swing-0.1.2/README.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 beats_swing-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 beats_swing-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 beats_swing-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 beats_swing-0.1.3/DEVELOPMENT.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 beats_swing-0.1.3/Makefile
+-rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 beats_swing-0.1.3/pylintrc
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 beats_swing-0.1.3/test_requirements.txt
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 beats_swing-0.1.3/.github/workflows/build_release.yml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 beats_swing-0.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/explorer.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/first_pass.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/librosa_explorer.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/mess_around_w_librosa.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/score.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/__init__.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/cli.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/constants.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/filtering.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/shared_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/api.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/librosa.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/trivial.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.3/tests/beats/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 beats_swing-0.1.3/tests/beats/test_cli.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 beats_swing-0.1.3/tests/beats/test_smoke.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 beats_swing-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 beats_swing-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 beats_swing-0.1.3/README.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 beats_swing-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 beats_swing-0.1.3/PKG-INFO
```

### Comparing `beats_swing-0.1.2/.pre-commit-config.yaml` & `beats_swing-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/DEVELOPMENT.md` & `beats_swing-0.1.3/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/Makefile` & `beats_swing-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/pylintrc` & `beats_swing-0.1.3/pylintrc`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/test_requirements.txt` & `beats_swing-0.1.3/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/.github/workflows/build_release.yml` & `beats_swing-0.1.3/.github/workflows/build_release.yml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/.github/workflows/tests.yml` & `beats_swing-0.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/scripts/explorer.py` & `beats_swing-0.1.3/scripts/explorer.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/scripts/first_pass.py` & `beats_swing-0.1.3/scripts/first_pass.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/scripts/librosa_explorer.py` & `beats_swing-0.1.3/scripts/librosa_explorer.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/scripts/mess_around_w_librosa.py` & `beats_swing-0.1.3/scripts/mess_around_w_librosa.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/scripts/score.py` & `beats_swing-0.1.3/scripts/score.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/src/beats/cli.py` & `beats_swing-0.1.3/src/beats/cli.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/src/beats/filtering.py` & `beats_swing-0.1.3/src/beats/filtering.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/src/beats/estimators/api.py` & `beats_swing-0.1.3/src/beats/estimators/api.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/src/beats/estimators/librosa.py` & `beats_swing-0.1.3/src/beats/estimators/librosa.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/src/beats/estimators/utils.py` & `beats_swing-0.1.3/src/beats/estimators/utils.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/.gitignore` & `beats_swing-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/LICENSE.txt` & `beats_swing-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.2/README.md` & `beats_swing-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # beats
 
-![tests](https://github.com/elvijs/beats/workflows/main/badge.svg)
+![tests](https://github.com/elvijs/beats/workflows/tests/badge.svg)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # What is it?
 
 Determine the tempo of a song from its mp3. Designed for swing music. May work in other cases as well.
```

### Comparing `beats_swing-0.1.2/pyproject.toml` & `beats_swing-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "beats_swing"
-version = "0.1.2"
+version = "0.1.3"
 description = "Determine the tempo of an mp3 song. Tweaked for swing music."
 authors = [
     {name = "Elvijs Sarkans", email = "elvijs.sarkans@gmail.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `beats_swing-0.1.2/PKG-INFO` & `beats_swing-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: beats_swing
-Version: 0.1.2
+Version: 0.1.3
 Summary: Determine the tempo of an mp3 song. Tweaked for swing music.
 Project-URL: repository, https://github.com/elvijs/beats
 Project-URL: homepage, https://github.com/elvijs/beats
 Project-URL: issues, https://github.com/elvijs/beats/issues
 Author-email: Elvijs Sarkans <elvijs.sarkans@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: librosa<1,>=0.10.2
 Description-Content-Type: text/markdown
 
 # beats
 
-![tests](https://github.com/elvijs/beats/workflows/main/badge.svg)
+![tests](https://github.com/elvijs/beats/workflows/tests/badge.svg)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # What is it?
 
 Determine the tempo of a song from its mp3. Designed for swing music. May work in other cases as well.
```

