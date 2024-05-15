# Comparing `tmp/binpolar-0.7.tar.gz` & `tmp/binpolar-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binpolar-0.7.tar", last modified: Mon May 13 07:36:38 2024, max compression
+gzip compressed data, was "binpolar-1.3.tar", last modified: Wed May 15 07:02:23 2024, max compression
```

## Comparing `binpolar-0.7.tar` & `binpolar-1.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 07:36:38.197363 binpolar-0.7/
--rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 07:36:38.197154 binpolar-0.7/PKG-INFO
--rw-r--r--   0 joycelee   (501) staff       (20)        3 2024-05-13 03:33:09.000000 binpolar-0.7/README.md
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 07:36:38.196152 binpolar-0.7/binpolar/
--rw-r--r--   0 joycelee   (501) staff       (20)       54 2024-05-13 06:21:47.000000 binpolar-0.7/binpolar/__init__.py
--rw-r--r--   0 joycelee   (501) staff       (20)     1348 2024-05-13 07:36:28.000000 binpolar-0.7/binpolar/polarity_detector.py
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 07:36:38.196962 binpolar-0.7/binpolar.egg-info/
--rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 07:36:38.000000 binpolar-0.7/binpolar.egg-info/PKG-INFO
--rw-r--r--   0 joycelee   (501) staff       (20)      228 2024-05-13 07:36:38.000000 binpolar-0.7/binpolar.egg-info/SOURCES.txt
--rw-r--r--   0 joycelee   (501) staff       (20)        1 2024-05-13 07:36:38.000000 binpolar-0.7/binpolar.egg-info/dependency_links.txt
--rw-r--r--   0 joycelee   (501) staff       (20)       13 2024-05-13 07:36:38.000000 binpolar-0.7/binpolar.egg-info/requires.txt
--rw-r--r--   0 joycelee   (501) staff       (20)        9 2024-05-13 07:36:38.000000 binpolar-0.7/binpolar.egg-info/top_level.txt
--rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-13 07:36:38.197412 binpolar-0.7/setup.cfg
--rw-r--r--   0 joycelee   (501) staff       (20)      853 2024-05-13 07:36:31.000000 binpolar-0.7/setup.py
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-15 07:02:23.012143 binpolar-1.3/
+-rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-15 07:02:00.000000 binpolar-1.3/MANIFEST.in
+-rw-r--r--   0 joycelee   (501) staff       (20)      698 2024-05-15 07:02:23.011934 binpolar-1.3/PKG-INFO
+-rw-r--r--   0 joycelee   (501) staff       (20)        3 2024-05-13 03:33:09.000000 binpolar-1.3/README.md
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-15 07:02:23.009203 binpolar-1.3/binpolar/
+-rw-r--r--   0 joycelee   (501) staff       (20)       46 2024-05-13 21:36:13.000000 binpolar-1.3/binpolar/__init__.py
+-rw-r--r--   0 joycelee   (501) staff       (20)      998 2024-05-15 07:02:17.000000 binpolar-1.3/binpolar/polarity_detector.py
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-15 07:02:23.010381 binpolar-1.3/binpolar/tokenizer/
+-rw-r--r--   0 joycelee   (501) staff       (20)      125 2024-05-12 08:02:08.000000 binpolar-1.3/binpolar/tokenizer/special_tokens_map.json
+-rw-r--r--   0 joycelee   (501) staff       (20)      372 2024-05-12 08:02:08.000000 binpolar-1.3/binpolar/tokenizer/tokenizer_config.json
+-rw-r--r--   0 joycelee   (501) staff       (20)   231508 2024-05-12 08:02:08.000000 binpolar-1.3/binpolar/tokenizer/vocab.txt
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-15 07:02:23.011728 binpolar-1.3/binpolar.egg-info/
+-rw-r--r--   0 joycelee   (501) staff       (20)      698 2024-05-15 07:02:23.000000 binpolar-1.3/binpolar.egg-info/PKG-INFO
+-rw-r--r--   0 joycelee   (501) staff       (20)      353 2024-05-15 07:02:23.000000 binpolar-1.3/binpolar.egg-info/SOURCES.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)        1 2024-05-15 07:02:23.000000 binpolar-1.3/binpolar.egg-info/dependency_links.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)       29 2024-05-15 07:02:23.000000 binpolar-1.3/binpolar.egg-info/requires.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)        9 2024-05-15 07:02:23.000000 binpolar-1.3/binpolar.egg-info/top_level.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-15 07:02:23.012194 binpolar-1.3/setup.cfg
+-rw-r--r--   0 joycelee   (501) staff       (20)      987 2024-05-15 06:45:14.000000 binpolar-1.3/setup.py
```

### Comparing `binpolar-0.7/PKG-INFO` & `binpolar-1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: binpolar
-Version: 0.7
+Version: 1.3
 Summary: Binary polarity detection
 Author: Joyce Lee
 Author-email: <leejoy1610@gmail.com>
 Keywords: python,text,polarity
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: transformers
+Requires-Dist: huggingface_hub
 
 A fine-tuned DistilBERT model for binary polarity detection in text.
+                        Returns 1 if detected positive; 0 if detected negative.
```

### Comparing `binpolar-0.7/binpolar.egg-info/PKG-INFO` & `binpolar-1.3/binpolar.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: binpolar
-Version: 0.7
+Version: 1.3
 Summary: Binary polarity detection
 Author: Joyce Lee
 Author-email: <leejoy1610@gmail.com>
 Keywords: python,text,polarity
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: transformers
+Requires-Dist: huggingface_hub
 
 A fine-tuned DistilBERT model for binary polarity detection in text.
+                        Returns 1 if detected positive; 0 if detected negative.
```

### Comparing `binpolar-0.7/setup.py` & `binpolar-1.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.7'
+VERSION = '1.3'
 DESCRIPTION = 'Binary polarity detection'
-LONG_DESCRIPTION = 'A fine-tuned DistilBERT model for binary polarity detection in text.'
+LONG_DESCRIPTION = '''A fine-tuned DistilBERT model for binary polarity detection in text.
+                        Returns 1 if detected positive; 0 if detected negative.'''
 
 # Setting up
 setup(
     name="binpolar",
     version=VERSION,
     author="Joyce Lee",
     author_email="<leejoy1610@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['transformers'],
+    include_package_data=True,
+    install_requires=['transformers', 'huggingface_hub'],
     keywords=['python', 'text', 'polarity'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

