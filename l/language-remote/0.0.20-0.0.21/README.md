# Comparing `tmp/language_remote-0.0.20.tar.gz` & `tmp/language_remote-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language_remote-0.0.20.tar", last modified: Tue May  7 20:37:21 2024, max compression
+gzip compressed data, was "language_remote-0.0.21.tar", last modified: Tue May 14 20:47:13 2024, max compression
```

## Comparing `language_remote-0.0.20.tar` & `language_remote-0.0.21.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:21.405856 language_remote-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 20:37:21.405856 language_remote-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-07 20:37:02.000000 language_remote-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:21.405856 language_remote-0.0.20/language_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:21.405856 language_remote-0.0.20/language_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:02.000000 language_remote-0.0.20/language_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 20:37:02.000000 language_remote-0.0.20/language_remote/src/lang_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 20:37:02.000000 language_remote-0.0.20/language_remote/src/language_code_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:21.405856 language_remote-0.0.20/language_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 20:37:02.000000 language_remote-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:37:21.405856 language_remote-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 20:37:02.000000 language_remote-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:47:13.558342 language_remote-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 20:47:13.554342 language_remote-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-14 20:46:55.000000 language_remote-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:47:13.554342 language_remote-0.0.21/language_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:47:13.554342 language_remote-0.0.21/language_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:46:55.000000 language_remote-0.0.21/language_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-14 20:46:55.000000 language_remote-0.0.21/language_remote/src/lang_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-14 20:46:55.000000 language_remote-0.0.21/language_remote/src/language_code_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:47:13.554342 language_remote-0.0.21/language_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 20:47:13.000000 language_remote-0.0.21/language_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-14 20:47:13.000000 language_remote-0.0.21/language_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:47:13.000000 language_remote-0.0.21/language_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:47:13.000000 language_remote-0.0.21/language_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 20:47:13.000000 language_remote-0.0.21/language_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 20:46:55.000000 language_remote-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:47:13.558342 language_remote-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-14 20:46:55.000000 language_remote-0.0.21/setup.py
```

### Comparing `language_remote-0.0.20/README.md` & `language_remote-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `language_remote-0.0.20/language_remote/src/lang_code.py` & `language_remote-0.0.21/language_remote/src/lang_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
                 result = f'{lang}-{country.upper()}'
                 MiniLogger.end(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"result": result})
                 return result
             else:
                 MiniLogger.end(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"result": most_common_result})
                 return most_common_result
         except LangDetectException:
-            MiniLogger.error(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"error": "LangDetectException"})
+            MiniLogger.exception(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"error": "LangDetectException"})
             MiniLogger.end(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"result": None})
             return None
 
     @staticmethod
     def detect_lang_code(text: str, attempts=3) -> 'LangCode':
         DETECT_LANG_CODE_METHOD_NAME = 'detect_lang_code'
         MiniLogger.start(message=DETECT_LANG_CODE_METHOD_NAME, object={"text": text, "attempts": attempts})
```

### Comparing `language_remote-0.0.20/language_remote/src/language_code_constants.py` & `language_remote-0.0.21/language_remote/src/language_code_constants.py`

 * *Files identical despite different names*

### Comparing `language_remote-0.0.20/setup.py` & `language_remote-0.0.21/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "language-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/language-remote
-    version='0.0.20',
+    version='0.0.21',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Language Remote",
```

