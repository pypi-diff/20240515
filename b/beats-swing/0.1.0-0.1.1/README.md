# Comparing `tmp/beats_swing-0.1.0.tar.gz` & `tmp/beats_swing-0.1.1.tar.gz`

## Comparing `beats_swing-0.1.0.tar` & `beats_swing-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 beats_swing-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 beats_swing-0.1.0/Makefile
--rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 beats_swing-0.1.0/pylintrc
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 beats_swing-0.1.0/test_requirements.txt
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 beats_swing-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 beats_swing-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/explorer.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/first_pass.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/librosa_explorer.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/mess_around_w_librosa.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 beats_swing-0.1.0/scripts/score.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/__init__.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/cli.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/constants.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/filtering.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/shared_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/api.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/librosa.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/trivial.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 beats_swing-0.1.0/src/beats/estimators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.0/tests/beats/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 beats_swing-0.1.0/tests/beats/test_smoke.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 beats_swing-0.1.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 beats_swing-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 beats_swing-0.1.0/README.md
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 beats_swing-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 beats_swing-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 beats_swing-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 beats_swing-0.1.1/Makefile
+-rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 beats_swing-0.1.1/pylintrc
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 beats_swing-0.1.1/test_requirements.txt
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 beats_swing-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 beats_swing-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 beats_swing-0.1.1/scripts/explorer.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 beats_swing-0.1.1/scripts/first_pass.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 beats_swing-0.1.1/scripts/librosa_explorer.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 beats_swing-0.1.1/scripts/mess_around_w_librosa.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 beats_swing-0.1.1/scripts/score.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/__init__.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/cli.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/constants.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/filtering.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/shared_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/estimators/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/estimators/api.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/estimators/librosa.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/estimators/trivial.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 beats_swing-0.1.1/src/beats/estimators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.1/tests/beats/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 beats_swing-0.1.1/tests/beats/test_smoke.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 beats_swing-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 beats_swing-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 beats_swing-0.1.1/README.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 beats_swing-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 beats_swing-0.1.1/PKG-INFO
```

### Comparing `beats_swing-0.1.0/.pre-commit-config.yaml` & `beats_swing-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/Makefile` & `beats_swing-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/pylintrc` & `beats_swing-0.1.1/pylintrc`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/test_requirements.txt` & `beats_swing-0.1.1/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/.github/workflows/publish.yml` & `beats_swing-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/.github/workflows/tests.yml` & `beats_swing-0.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/scripts/explorer.py` & `beats_swing-0.1.1/scripts/explorer.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/scripts/first_pass.py` & `beats_swing-0.1.1/scripts/first_pass.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/scripts/librosa_explorer.py` & `beats_swing-0.1.1/scripts/librosa_explorer.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/scripts/mess_around_w_librosa.py` & `beats_swing-0.1.1/scripts/mess_around_w_librosa.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/scripts/score.py` & `beats_swing-0.1.1/scripts/score.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/src/beats/cli.py` & `beats_swing-0.1.1/src/beats/cli.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/src/beats/filtering.py` & `beats_swing-0.1.1/src/beats/filtering.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/src/beats/estimators/api.py` & `beats_swing-0.1.1/src/beats/estimators/api.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/src/beats/estimators/librosa.py` & `beats_swing-0.1.1/src/beats/estimators/librosa.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/src/beats/estimators/utils.py` & `beats_swing-0.1.1/src/beats/estimators/utils.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/.gitignore` & `beats_swing-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/LICENSE.txt` & `beats_swing-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.0/README.md` & `beats_swing-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # What is it?
 
 Determine the tempo of a song from its mp3. Designed for swing music. May work in other cases as well.
 
+This is essentially a thin wrapper on top of the amazing [`librosa`](https://librosa.org/doc/latest/index.html) library.
+
 # Usage
 
 ## Non-Python dependencies
 
 ```console
 $ sudo apt install ffmpeg
 ```
```

### Comparing `beats_swing-0.1.0/pyproject.toml` & `beats_swing-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 [project]
 name = "beats_swing"
-version = "0.1.0"
+version = "0.1.1"
 description = "Determine the tempo of an mp3 song. Tweaked for swing music."
 authors = [
     {name = "Elvijs Sarkans", email = "elvijs.sarkans@gmail.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 
 packages = [
     { include = "beats", from = "src" },
 ]
 
 dependencies = [
-    "pydub>=0.25.1,<1",
-    "numpy>=1.26.4,<2",
-    "matplotlib>=3.8.4,<4",
-    "plotly>=5.22.0,<6",
-    "scipy>=1.13.0,<2",
     "librosa>=0.10.2,<1",
-    "mlflow>=2,<3"
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `beats_swing-0.1.0/PKG-INFO` & `beats_swing-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 Metadata-Version: 2.3
 Name: beats_swing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Determine the tempo of an mp3 song. Tweaked for swing music.
 Project-URL: repository, https://github.com/elvijs/beats
 Project-URL: homepage, https://github.com/elvijs/beats
 Project-URL: issues, https://github.com/elvijs/beats/issues
 Author-email: Elvijs Sarkans <elvijs.sarkans@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: librosa<1,>=0.10.2
-Requires-Dist: matplotlib<4,>=3.8.4
-Requires-Dist: mlflow<3,>=2
-Requires-Dist: numpy<2,>=1.26.4
-Requires-Dist: plotly<6,>=5.22.0
-Requires-Dist: pydub<1,>=0.25.1
-Requires-Dist: scipy<2,>=1.13.0
 Description-Content-Type: text/markdown
 
 # beats
 
 ![tests](https://github.com/elvijs/beats/workflows/main/badge.svg)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # What is it?
 
 Determine the tempo of a song from its mp3. Designed for swing music. May work in other cases as well.
 
+This is essentially a thin wrapper on top of the amazing [`librosa`](https://librosa.org/doc/latest/index.html) library.
+
 # Usage
 
 ## Non-Python dependencies
 
 ```console
 $ sudo apt install ffmpeg
 ```
```

