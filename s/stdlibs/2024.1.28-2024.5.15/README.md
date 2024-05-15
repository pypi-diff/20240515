# Comparing `tmp/stdlibs-2024.1.28.tar.gz` & `tmp/stdlibs-2024.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdlibs-2024.1.28.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "stdlibs-2024.5.15.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `stdlibs-2024.1.28.tar` & `stdlibs-2024.5.15.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      180 2022-08-24 05:13:25.634188 stdlibs-2024.1.28/.flake8
--rw-r--r--   0        0        0     1806 2022-08-24 05:13:25.634813 stdlibs-2024.1.28/.gitignore
--rw-r--r--   0        0        0       50 2023-11-03 01:19:26.980010 stdlibs-2024.1.28/.mailmap
--rw-r--r--   0        0        0      195 2024-01-28 22:57:50.551240 stdlibs-2024.1.28/.readthedocs.yml
--rw-r--r--   0        0        0     2509 2024-01-28 22:58:56.149789 stdlibs-2024.1.28/CHANGELOG.md
--rw-r--r--   0        0        0     3216 2022-08-24 05:13:45.669813 stdlibs-2024.1.28/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1071 2022-08-24 05:13:45.673821 stdlibs-2024.1.28/LICENSE
--rw-r--r--   0        0        0     3737 2024-01-28 22:26:12.303643 stdlibs-2024.1.28/README.md
--rw-r--r--   0        0        0      360 2022-08-24 05:13:25.636019 stdlibs-2024.1.28/docs/_static/custom.css
--rw-r--r--   0        0        0      342 2022-08-24 05:13:25.636234 stdlibs-2024.1.28/docs/_templates/badges.html
--rw-r--r--   0        0        0      934 2022-08-24 05:13:25.636389 stdlibs-2024.1.28/docs/_templates/omnilib.html
--rw-r--r--   0        0        0     1819 2023-12-16 03:47:01.283708 stdlibs-2024.1.28/docs/api.rst
--rw-r--r--   0        0        0       70 2022-08-24 05:13:45.684712 stdlibs-2024.1.28/docs/changelog.rst
--rw-r--r--   0        0        0     2870 2022-08-24 05:13:45.687958 stdlibs-2024.1.28/docs/conf.py
--rw-r--r--   0        0        0       96 2022-08-24 05:13:45.690961 stdlibs-2024.1.28/docs/index.rst
--rw-r--r--   0        0        0      742 2024-01-28 22:57:50.551455 stdlibs-2024.1.28/makefile
--rw-r--r--   0        0        0     1405 2024-01-28 22:57:50.551604 stdlibs-2024.1.28/pyproject.toml
--rw-r--r--   0        0        0     1490 2022-08-24 05:13:45.727531 stdlibs-2024.1.28/stdlibs/__init__.py
--rw-r--r--   0        0        0      160 2024-01-28 22:58:56.155709 stdlibs-2024.1.28/stdlibs/__version__.py
--rw-r--r--   0        0        0    11074 2023-12-16 03:47:01.284125 stdlibs-2024.1.28/stdlibs/fetch.py
--rw-r--r--   0        0        0     1902 2023-12-16 03:47:01.284323 stdlibs-2024.1.28/stdlibs/fetch_releases.py
--rw-r--r--   0        0        0      411 2023-12-16 03:47:01.284568 stdlibs-2024.1.28/stdlibs/known.py
--rw-r--r--   0        0        0    11972 2024-01-28 22:16:24.590951 stdlibs-2024.1.28/stdlibs/py.py
--rw-r--r--   0        0        0        0 2022-10-10 04:57:02.876861 stdlibs-2024.1.28/stdlibs/py.typed
--rw-r--r--   0        0        0     9704 2023-12-16 03:16:55.434256 stdlibs-2024.1.28/stdlibs/py2.py
--rw-r--r--   0        0        0     8140 2023-12-16 03:16:51.493368 stdlibs-2024.1.28/stdlibs/py23.py
--rw-r--r--   0        0        0     8482 2023-12-16 03:16:51.632202 stdlibs-2024.1.28/stdlibs/py24.py
--rw-r--r--   0        0        0     8453 2023-12-16 03:16:51.804899 stdlibs-2024.1.28/stdlibs/py25.py
--rw-r--r--   0        0        0     8800 2023-12-16 03:16:52.016657 stdlibs-2024.1.28/stdlibs/py26.py
--rw-r--r--   0        0        0     8959 2023-12-16 03:16:52.315470 stdlibs-2024.1.28/stdlibs/py27.py
--rw-r--r--   0        0        0     7493 2024-01-28 22:16:24.591456 stdlibs-2024.1.28/stdlibs/py3.py
--rw-r--r--   0        0        0     5462 2023-12-16 03:16:52.491158 stdlibs-2024.1.28/stdlibs/py30.py
--rw-r--r--   0        0        0     5476 2023-12-16 03:16:52.690710 stdlibs-2024.1.28/stdlibs/py31.py
--rw-r--r--   0        0        0     6437 2023-12-16 03:47:01.285430 stdlibs-2024.1.28/stdlibs/py310.py
--rw-r--r--   0        0        0     6559 2023-12-16 03:16:55.265029 stdlibs-2024.1.28/stdlibs/py311.py
--rw-r--r--   0        0        0     6517 2023-12-16 03:16:55.350499 stdlibs-2024.1.28/stdlibs/py312.py
--rw-r--r--   0        0        0     6262 2024-01-28 22:16:24.591600 stdlibs-2024.1.28/stdlibs/py313.py
--rw-r--r--   0        0        0     5674 2023-12-16 03:16:52.909143 stdlibs-2024.1.28/stdlibs/py32.py
--rw-r--r--   0        0        0     5867 2023-12-16 03:16:53.173983 stdlibs-2024.1.28/stdlibs/py33.py
--rw-r--r--   0        0        0     6055 2023-12-16 03:16:53.432910 stdlibs-2024.1.28/stdlibs/py34.py
--rw-r--r--   0        0        0     6221 2023-12-16 03:16:53.685645 stdlibs-2024.1.28/stdlibs/py35.py
--rw-r--r--   0        0        0     6220 2023-12-16 03:16:53.972545 stdlibs-2024.1.28/stdlibs/py36.py
--rw-r--r--   0        0        0     6323 2023-12-16 03:16:54.232794 stdlibs-2024.1.28/stdlibs/py37.py
--rw-r--r--   0        0        0     6409 2023-12-16 03:16:54.504300 stdlibs-2024.1.28/stdlibs/py38.py
--rw-r--r--   0        0        0     6514 2023-12-16 03:16:54.783255 stdlibs-2024.1.28/stdlibs/py39.py
--rw-r--r--   0        0        0     1390 2024-01-28 22:16:24.592099 stdlibs-2024.1.28/stdlibs/releases.toml
--rw-r--r--   0        0        0     2058 2024-01-28 22:44:34.440583 stdlibs-2024.1.28/stdlibs/tests/__init__.py
--rw-r--r--   0        0        0      185 2022-08-24 05:13:45.721395 stdlibs-2024.1.28/stdlibs/tests/__main__.py
--rw-r--r--   0        0        0     4883 1970-01-01 00:00:00.000000 stdlibs-2024.1.28/PKG-INFO
+-rw-r--r--   0        0        0      180 2024-05-15 20:24:50.525751 stdlibs-2024.5.15/.flake8
+-rw-r--r--   0        0        0     1806 2024-05-15 20:24:50.526194 stdlibs-2024.5.15/.gitignore
+-rw-r--r--   0        0        0       50 2024-05-15 20:25:40.735329 stdlibs-2024.5.15/.mailmap
+-rw-r--r--   0        0        0      195 2024-05-15 20:25:40.735423 stdlibs-2024.5.15/.readthedocs.yml
+-rw-r--r--   0        0        0     2706 2024-05-15 21:07:25.407804 stdlibs-2024.5.15/CHANGELOG.md
+-rw-r--r--   0        0        0     3216 2024-05-15 20:24:50.526494 stdlibs-2024.5.15/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1071 2024-05-15 20:24:50.526594 stdlibs-2024.5.15/LICENSE
+-rw-r--r--   0        0        0     3737 2024-05-15 20:25:40.735665 stdlibs-2024.5.15/README.md
+-rw-r--r--   0        0        0      360 2024-05-15 20:24:50.526923 stdlibs-2024.5.15/docs/_static/custom.css
+-rw-r--r--   0        0        0      342 2024-05-15 20:24:50.527072 stdlibs-2024.5.15/docs/_templates/badges.html
+-rw-r--r--   0        0        0      934 2024-05-15 20:24:50.527166 stdlibs-2024.5.15/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0     1819 2024-05-15 20:25:40.735757 stdlibs-2024.5.15/docs/api.rst
+-rw-r--r--   0        0        0       70 2024-05-15 20:24:50.527503 stdlibs-2024.5.15/docs/changelog.rst
+-rw-r--r--   0        0        0     2870 2024-05-15 20:24:50.527664 stdlibs-2024.5.15/docs/conf.py
+-rw-r--r--   0        0        0       96 2024-05-15 20:24:50.527750 stdlibs-2024.5.15/docs/index.rst
+-rw-r--r--   0        0        0      742 2024-05-15 20:25:40.735842 stdlibs-2024.5.15/makefile
+-rw-r--r--   0        0        0     1412 2024-05-15 21:06:39.430703 stdlibs-2024.5.15/pyproject.toml
+-rw-r--r--   0        0        0     1490 2024-05-15 20:24:50.528322 stdlibs-2024.5.15/stdlibs/__init__.py
+-rw-r--r--   0        0        0      160 2024-05-15 21:07:25.417011 stdlibs-2024.5.15/stdlibs/__version__.py
+-rw-r--r--   0        0        0    11074 2024-05-15 20:25:40.736163 stdlibs-2024.5.15/stdlibs/fetch.py
+-rw-r--r--   0        0        0     1902 2024-05-15 20:25:40.736220 stdlibs-2024.5.15/stdlibs/fetch_releases.py
+-rw-r--r--   0        0        0      411 2024-05-15 20:25:40.736312 stdlibs-2024.5.15/stdlibs/known.py
+-rw-r--r--   0        0        0    12177 2024-05-15 20:25:40.736462 stdlibs-2024.5.15/stdlibs/py.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:25:40.736487 stdlibs-2024.5.15/stdlibs/py.typed
+-rw-r--r--   0        0        0     9704 2024-05-15 20:24:50.529728 stdlibs-2024.5.15/stdlibs/py2.py
+-rw-r--r--   0        0        0     8140 2024-05-15 20:24:50.529941 stdlibs-2024.5.15/stdlibs/py23.py
+-rw-r--r--   0        0        0     8482 2024-05-15 20:24:50.530061 stdlibs-2024.5.15/stdlibs/py24.py
+-rw-r--r--   0        0        0     8453 2024-05-15 20:24:50.530179 stdlibs-2024.5.15/stdlibs/py25.py
+-rw-r--r--   0        0        0     8800 2024-05-15 20:24:50.530294 stdlibs-2024.5.15/stdlibs/py26.py
+-rw-r--r--   0        0        0     8959 2024-05-15 20:24:50.530419 stdlibs-2024.5.15/stdlibs/py27.py
+-rw-r--r--   0        0        0     7698 2024-05-15 20:25:40.736605 stdlibs-2024.5.15/stdlibs/py3.py
+-rw-r--r--   0        0        0     5462 2024-05-15 20:24:50.530724 stdlibs-2024.5.15/stdlibs/py30.py
+-rw-r--r--   0        0        0     5476 2024-05-15 20:24:50.530840 stdlibs-2024.5.15/stdlibs/py31.py
+-rw-r--r--   0        0        0     6437 2024-05-15 20:25:40.736701 stdlibs-2024.5.15/stdlibs/py310.py
+-rw-r--r--   0        0        0     6559 2024-05-15 20:25:40.736853 stdlibs-2024.5.15/stdlibs/py311.py
+-rw-r--r--   0        0        0     6517 2024-05-15 20:25:40.736966 stdlibs-2024.5.15/stdlibs/py312.py
+-rw-r--r--   0        0        0     6408 2024-05-15 20:25:40.737049 stdlibs-2024.5.15/stdlibs/py313.py
+-rw-r--r--   0        0        0     5674 2024-05-15 20:24:50.531222 stdlibs-2024.5.15/stdlibs/py32.py
+-rw-r--r--   0        0        0     5867 2024-05-15 20:24:50.531364 stdlibs-2024.5.15/stdlibs/py33.py
+-rw-r--r--   0        0        0     6055 2024-05-15 20:24:50.531508 stdlibs-2024.5.15/stdlibs/py34.py
+-rw-r--r--   0        0        0     6221 2024-05-15 20:25:40.737164 stdlibs-2024.5.15/stdlibs/py35.py
+-rw-r--r--   0        0        0     6220 2024-05-15 20:25:40.737265 stdlibs-2024.5.15/stdlibs/py36.py
+-rw-r--r--   0        0        0     6323 2024-05-15 20:25:40.737363 stdlibs-2024.5.15/stdlibs/py37.py
+-rw-r--r--   0        0        0     6409 2024-05-15 20:25:40.737465 stdlibs-2024.5.15/stdlibs/py38.py
+-rw-r--r--   0        0        0     6514 2024-05-15 20:25:40.737558 stdlibs-2024.5.15/stdlibs/py39.py
+-rw-r--r--   0        0        0     1390 2024-05-15 20:25:40.737621 stdlibs-2024.5.15/stdlibs/releases.toml
+-rw-r--r--   0        0        0     2058 2024-05-15 20:25:40.737732 stdlibs-2024.5.15/stdlibs/tests/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-15 20:24:50.532431 stdlibs-2024.5.15/stdlibs/tests/__main__.py
+-rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 stdlibs-2024.5.15/PKG-INFO
```

### Comparing `stdlibs-2024.1.28/.gitignore` & `stdlibs-2024.5.15/.gitignore`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/CHANGELOG.md` & `stdlibs-2024.5.15/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 stdlibs
 =======
 
 [![Generated by attribution][attribution-badge]][attribution-url]
 
 
+v2024.5.15
+----------
+
+Maintenance release
+
+- Update stdlibs for 3.13b1 (#91)
+
+```text
+$ git shortlog -s v2024.1.28...v2024.5.15
+     1	Amethyst Reese
+     1	Tim Hatch
+     9	dependabot[bot]
+```
+
+
 v2024.1.28
 ----------
 
 Maintenance release
 
 - Update stdlibs for 3.13a3 (#76)
 - Update doctest usage (#77)
```

### Comparing `stdlibs-2024.1.28/CODE_OF_CONDUCT.md` & `stdlibs-2024.5.15/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/LICENSE` & `stdlibs-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/README.md` & `stdlibs-2024.5.15/README.md`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/docs/_templates/omnilib.html` & `stdlibs-2024.5.15/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/docs/api.rst` & `stdlibs-2024.5.15/docs/api.rst`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/docs/conf.py` & `stdlibs-2024.5.15/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/makefile` & `stdlibs-2024.5.15/makefile`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/pyproject.toml` & `stdlibs-2024.5.15/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,27 +18,27 @@
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 dependencies = []
 
 [project.optional-dependencies]
 dev = [
-    "attribution==1.6.2",
-    "black==24.1.1",
-    "coverage==7.4.1",
+    "attribution==1.7.1",
+    "black==24.4.2",
+    "coverage==7.5.1",
     "flake8==7.0.0",
     "flit==3.9.0",
-    "mypy==1.8.0",
-    "packaging==23.2",
-    "ufmt==2.3.0",
-    "usort==1.0.7",
+    "mypy==1.10.0",
+    "packaging==24.0",
+    "ufmt==2.6.0",
+    "usort==1.0.8.post1",
 ]
 docs = [
-    "sphinx==7.2.6",
-    "sphinx-mdinclude==0.5.3",
+    "sphinx==7.3.7",
+    "sphinx-mdinclude==0.6.0",
 ]
 
 [project.urls]
 Homepage = "https://stdlibs.omnilib.dev"
 Documentation = "https://stdlibs.omnilib.dev/en/latest/"
 Github = "https://github.com/omnilib/stdlibs"
```

### Comparing `stdlibs-2024.1.28/stdlibs/__init__.py` & `stdlibs-2024.5.15/stdlibs/__init__.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/fetch.py` & `stdlibs-2024.5.15/stdlibs/fetch.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/fetch_releases.py` & `stdlibs-2024.5.15/stdlibs/fetch_releases.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py.py` & `stdlibs-2024.5.15/stdlibs/py.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         "__hello_alias__",
         "__hello_only__",
         "__phello__",
         "__phello_alias__",
         "_abc",
         "_abcoll",
         "_aix_support",
+        "_android_support",
         "_ast",
         "_asyncio",
         "_bisect",
         "_blake2",
         "_bootlocale",
         "_bootsubprocess",
         "_bsddb",
@@ -125,14 +126,15 @@
         "_codecs_hk",
         "_codecs_iso2022",
         "_codecs_jp",
         "_codecs_kr",
         "_codecs_tw",
         "_collections",
         "_collections_abc",
+        "_colorize",
         "_compat_pickle",
         "_compression",
         "_contextvars",
         "_crypt",
         "_csv",
         "_ctypes",
         "_ctypes_test",
@@ -150,15 +152,19 @@
         "_functools",
         "_gdbm",
         "_gestalt",
         "_hashlib",
         "_heapq",
         "_hotshot",
         "_imp",
+        "_interpchannels",
+        "_interpqueues",
+        "_interpreters",
         "_io",
+        "_ios_support",
         "_json",
         "_locale",
         "_lsprof",
         "_lzma",
         "_markupbase",
         "_md5",
         "_msi",
@@ -174,14 +180,15 @@
         "_posixshmem",
         "_posixsubprocess",
         "_py_abc",
         "_pydatetime",
         "_pydecimal",
         "_pyio",
         "_pylong",
+        "_pyrepl",
         "_queue",
         "_random",
         "_scproxy",
         "_sha",
         "_sha1",
         "_sha2",
         "_sha256",
@@ -204,16 +211,18 @@
         "_symtable",
         "_sysconfig",
         "_testbuffer",
         "_testcapi",
         "_testclinic",
         "_testclinic_limited",
         "_testconsole",
+        "_testexternalinspection",
         "_testimportmultiple",
         "_testinternalcapi",
+        "_testlimitedcapi",
         "_testmultiphase",
         "_testsinglephase",
         "_thread",
         "_threading_local",
         "_tkinter",
         "_tokenize",
         "_tracemalloc",
@@ -222,15 +231,14 @@
         "_uuid",
         "_warnings",
         "_weakref",
         "_weakrefset",
         "_winapi",
         "_winreg",
         "_xxinterpchannels",
-        "_xxinterpqueues",
         "_xxsubinterpreters",
         "_xxtestfuzz",
         "_zoneinfo",
         "abc",
         "addpack",
         "aepack",
         "aetools",
```

### Comparing `stdlibs-2024.1.28/stdlibs/py2.py` & `stdlibs-2024.5.15/stdlibs/py2.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py23.py` & `stdlibs-2024.5.15/stdlibs/py23.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py24.py` & `stdlibs-2024.5.15/stdlibs/py24.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py25.py` & `stdlibs-2024.5.15/stdlibs/py25.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py26.py` & `stdlibs-2024.5.15/stdlibs/py26.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py27.py` & `stdlibs-2024.5.15/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py3.py` & `stdlibs-2024.5.15/stdlibs/py3.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         "__hello_alias__",
         "__hello_only__",
         "__phello__",
         "__phello_alias__",
         "_abc",
         "_abcoll",
         "_aix_support",
+        "_android_support",
         "_ast",
         "_asyncio",
         "_bisect",
         "_blake2",
         "_bootlocale",
         "_bootsubprocess",
         "_bytesio",
@@ -36,14 +37,15 @@
         "_codecs_hk",
         "_codecs_iso2022",
         "_codecs_jp",
         "_codecs_kr",
         "_codecs_tw",
         "_collections",
         "_collections_abc",
+        "_colorize",
         "_compat_pickle",
         "_compression",
         "_contextvars",
         "_crypt",
         "_csv",
         "_ctypes",
         "_ctypes_test",
@@ -60,15 +62,19 @@
         "_frozen_importlib_external",
         "_functools",
         "_gdbm",
         "_gestalt",
         "_hashlib",
         "_heapq",
         "_imp",
+        "_interpchannels",
+        "_interpqueues",
+        "_interpreters",
         "_io",
+        "_ios_support",
         "_json",
         "_locale",
         "_lsprof",
         "_lzma",
         "_markupbase",
         "_md5",
         "_msi",
@@ -84,14 +90,15 @@
         "_posixshmem",
         "_posixsubprocess",
         "_py_abc",
         "_pydatetime",
         "_pydecimal",
         "_pyio",
         "_pylong",
+        "_pyrepl",
         "_queue",
         "_random",
         "_scproxy",
         "_sha1",
         "_sha2",
         "_sha256",
         "_sha3",
@@ -113,31 +120,32 @@
         "_symtable",
         "_sysconfig",
         "_testbuffer",
         "_testcapi",
         "_testclinic",
         "_testclinic_limited",
         "_testconsole",
+        "_testexternalinspection",
         "_testimportmultiple",
         "_testinternalcapi",
+        "_testlimitedcapi",
         "_testmultiphase",
         "_testsinglephase",
         "_thread",
         "_threading_local",
         "_tkinter",
         "_tokenize",
         "_tracemalloc",
         "_typing",
         "_uuid",
         "_warnings",
         "_weakref",
         "_weakrefset",
         "_winapi",
         "_xxinterpchannels",
-        "_xxinterpqueues",
         "_xxsubinterpreters",
         "_xxtestfuzz",
         "_zoneinfo",
         "abc",
         "aifc",
         "antigravity",
         "argparse",
```

### Comparing `stdlibs-2024.1.28/stdlibs/py30.py` & `stdlibs-2024.5.15/stdlibs/py30.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py31.py` & `stdlibs-2024.5.15/stdlibs/py31.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py310.py` & `stdlibs-2024.5.15/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py311.py` & `stdlibs-2024.5.15/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py312.py` & `stdlibs-2024.5.15/stdlibs/py312.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py313.py` & `stdlibs-2024.5.15/stdlibs/py313.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,30 @@
         "__hello__",
         "__hello_alias__",
         "__hello_only__",
         "__phello__",
         "__phello_alias__",
         "_abc",
         "_aix_support",
+        "_android_support",
         "_ast",
         "_asyncio",
         "_bisect",
         "_blake2",
         "_bz2",
         "_codecs",
         "_codecs_cn",
         "_codecs_hk",
         "_codecs_iso2022",
         "_codecs_jp",
         "_codecs_kr",
         "_codecs_tw",
         "_collections",
         "_collections_abc",
+        "_colorize",
         "_compat_pickle",
         "_compression",
         "_contextvars",
         "_csv",
         "_ctypes",
         "_ctypes_test",
         "_curses",
@@ -44,15 +46,19 @@
         "_frozen_importlib",
         "_frozen_importlib_external",
         "_functools",
         "_gdbm",
         "_hashlib",
         "_heapq",
         "_imp",
+        "_interpchannels",
+        "_interpqueues",
+        "_interpreters",
         "_io",
+        "_ios_support",
         "_json",
         "_locale",
         "_lsprof",
         "_lzma",
         "_markupbase",
         "_md5",
         "_multibytecodec",
@@ -66,14 +72,15 @@
         "_posixshmem",
         "_posixsubprocess",
         "_py_abc",
         "_pydatetime",
         "_pydecimal",
         "_pyio",
         "_pylong",
+        "_pyrepl",
         "_queue",
         "_random",
         "_scproxy",
         "_sha1",
         "_sha2",
         "_sha3",
         "_signal",
@@ -91,32 +98,31 @@
         "_symtable",
         "_sysconfig",
         "_testbuffer",
         "_testcapi",
         "_testclinic",
         "_testclinic_limited",
         "_testconsole",
+        "_testexternalinspection",
         "_testimportmultiple",
         "_testinternalcapi",
+        "_testlimitedcapi",
         "_testmultiphase",
         "_testsinglephase",
         "_thread",
         "_threading_local",
         "_tkinter",
         "_tokenize",
         "_tracemalloc",
         "_typing",
         "_uuid",
         "_warnings",
         "_weakref",
         "_weakrefset",
         "_winapi",
-        "_xxinterpchannels",
-        "_xxinterpqueues",
-        "_xxsubinterpreters",
         "_xxtestfuzz",
         "_zoneinfo",
         "abc",
         "antigravity",
         "argparse",
         "array",
         "ast",
```

### Comparing `stdlibs-2024.1.28/stdlibs/py32.py` & `stdlibs-2024.5.15/stdlibs/py32.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py33.py` & `stdlibs-2024.5.15/stdlibs/py33.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py34.py` & `stdlibs-2024.5.15/stdlibs/py34.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py35.py` & `stdlibs-2024.5.15/stdlibs/py35.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py36.py` & `stdlibs-2024.5.15/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py37.py` & `stdlibs-2024.5.15/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py38.py` & `stdlibs-2024.5.15/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/py39.py` & `stdlibs-2024.5.15/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/stdlibs/releases.toml` & `stdlibs-2024.5.15/stdlibs/releases.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 "3.1" = "https://www.python.org/ftp/python/3.1.5/Python-3.1.5.tgz"
 "3.2" = "https://www.python.org/ftp/python/3.2.6/Python-3.2.6.tgz"
 "3.3" = "https://www.python.org/ftp/python/3.3.7/Python-3.3.7.tgz"
 "3.4" = "https://www.python.org/ftp/python/3.4.10/Python-3.4.10.tgz"
 "3.5" = "https://www.python.org/ftp/python/3.5.10/Python-3.5.10.tgz"
 "3.6" = "https://www.python.org/ftp/python/3.6.15/Python-3.6.15.tgz"
 "3.7" = "https://www.python.org/ftp/python/3.7.17/Python-3.7.17.tgz"
-"3.8" = "https://www.python.org/ftp/python/3.8.18/Python-3.8.18.tgz"
-"3.9" = "https://www.python.org/ftp/python/3.9.18/Python-3.9.18.tgz"
-"3.10" = "https://www.python.org/ftp/python/3.10.13/Python-3.10.13.tgz"
-"3.11" = "https://www.python.org/ftp/python/3.11.7/Python-3.11.7.tgz"
-"3.12" = "https://www.python.org/ftp/python/3.12.1/Python-3.12.1.tgz"
-"3.13" = "https://www.python.org/ftp/python/3.13.0/Python-3.13.0a3.tgz"
+"3.8" = "https://www.python.org/ftp/python/3.8.19/Python-3.8.19.tgz"
+"3.9" = "https://www.python.org/ftp/python/3.9.19/Python-3.9.19.tgz"
+"3.10" = "https://www.python.org/ftp/python/3.10.14/Python-3.10.14.tgz"
+"3.11" = "https://www.python.org/ftp/python/3.11.9/Python-3.11.9.tgz"
+"3.12" = "https://www.python.org/ftp/python/3.12.3/Python-3.12.3.tgz"
+"3.13" = "https://www.python.org/ftp/python/3.13.0/Python-3.13.0b1.tgz"
```

### Comparing `stdlibs-2024.1.28/stdlibs/tests/__init__.py` & `stdlibs-2024.5.15/stdlibs/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `stdlibs-2024.1.28/PKG-INFO` & `stdlibs-2024.5.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: stdlibs
-Version: 2024.1.28
+Version: 2024.5.15
 Summary: List of packages in the stdlib
 Author-email: Amethyst Reese <amy@n7.gg>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: attribution==1.6.2 ; extra == "dev"
-Requires-Dist: black==24.1.1 ; extra == "dev"
-Requires-Dist: coverage==7.4.1 ; extra == "dev"
+Requires-Dist: attribution==1.7.1 ; extra == "dev"
+Requires-Dist: black==24.4.2 ; extra == "dev"
+Requires-Dist: coverage==7.5.1 ; extra == "dev"
 Requires-Dist: flake8==7.0.0 ; extra == "dev"
 Requires-Dist: flit==3.9.0 ; extra == "dev"
-Requires-Dist: mypy==1.8.0 ; extra == "dev"
-Requires-Dist: packaging==23.2 ; extra == "dev"
-Requires-Dist: ufmt==2.3.0 ; extra == "dev"
-Requires-Dist: usort==1.0.7 ; extra == "dev"
-Requires-Dist: sphinx==7.2.6 ; extra == "docs"
-Requires-Dist: sphinx-mdinclude==0.5.3 ; extra == "docs"
+Requires-Dist: mypy==1.10.0 ; extra == "dev"
+Requires-Dist: packaging==24.0 ; extra == "dev"
+Requires-Dist: ufmt==2.6.0 ; extra == "dev"
+Requires-Dist: usort==1.0.8.post1 ; extra == "dev"
+Requires-Dist: sphinx==7.3.7 ; extra == "docs"
+Requires-Dist: sphinx-mdinclude==0.6.0 ; extra == "docs"
 Project-URL: Documentation, https://stdlibs.omnilib.dev/en/latest/
 Project-URL: Github, https://github.com/omnilib/stdlibs
 Project-URL: Homepage, https://stdlibs.omnilib.dev
 Provides-Extra: dev
 Provides-Extra: docs
 
 # stdlibs
```

