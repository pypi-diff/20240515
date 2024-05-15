# Comparing `tmp/mullai-1.0.1.tar.gz` & `tmp/mullai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mullai-1.0.1.tar", last modified: Wed May 15 20:40:35 2024, max compression
+gzip compressed data, was "mullai-1.0.2.tar", last modified: Wed May 15 20:43:29 2024, max compression
```

## Comparing `mullai-1.0.1.tar` & `mullai-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 20:40:35.454929 mullai-1.0.1/
--rw-rw-rw-   0        0        0     1082 2024-04-29 15:07:52.000000 mullai-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      845 2024-05-15 20:40:35.420776 mullai-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1693 2024-05-15 20:34:28.000000 mullai-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 20:40:35.237343 mullai-1.0.1/mullai/
--rw-rw-rw-   0        0        0        0 2024-04-25 20:07:37.000000 mullai-1.0.1/mullai/__init__.py
--rw-rw-rw-   0        0        0    17552 2024-05-11 18:26:22.000000 mullai-1.0.1/mullai/mullai.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:40:35.406175 mullai-1.0.1/mullai.egg-info/
--rw-rw-rw-   0        0        0      845 2024-05-15 20:40:35.000000 mullai-1.0.1/mullai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-15 20:40:35.000000 mullai-1.0.1/mullai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 20:40:35.000000 mullai-1.0.1/mullai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-15 20:40:35.000000 mullai-1.0.1/mullai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2024-05-15 20:40:35.000000 mullai-1.0.1/mullai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 20:40:35.000000 mullai-1.0.1/mullai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 20:40:35.455817 mullai-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1028 2024-05-15 20:31:32.000000 mullai-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:43:29.281224 mullai-1.0.2/
+-rw-rw-rw-   0        0        0     1082 2024-04-29 15:07:52.000000 mullai-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      845 2024-05-15 20:43:29.237873 mullai-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1693 2024-05-15 20:34:28.000000 mullai-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 20:43:29.072214 mullai-1.0.2/mullai/
+-rw-rw-rw-   0        0        0        0 2024-04-25 20:07:37.000000 mullai-1.0.2/mullai/__init__.py
+-rw-rw-rw-   0        0        0    17552 2024-05-11 18:26:22.000000 mullai-1.0.2/mullai/mullai.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:43:29.223185 mullai-1.0.2/mullai.egg-info/
+-rw-rw-rw-   0        0        0      845 2024-05-15 20:43:28.000000 mullai-1.0.2/mullai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-15 20:43:28.000000 mullai-1.0.2/mullai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:43:28.000000 mullai-1.0.2/mullai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-15 20:43:28.000000 mullai-1.0.2/mullai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2024-05-15 20:43:28.000000 mullai-1.0.2/mullai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 20:43:28.000000 mullai-1.0.2/mullai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:43:29.283171 mullai-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2024-05-15 20:43:17.000000 mullai-1.0.2/setup.py
```

### Comparing `mullai-1.0.1/LICENSE.txt` & `mullai-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mullai-1.0.1/PKG-INFO` & `mullai-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mullai
-Version: 1.0.1
+Version: 1.0.2
 Summary: A static site generator, that will allow you to generate content from database or remote.
 Home-page: https://github.com/whoisjeeva/mullai
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mullai-1.0.1/README.md` & `mullai-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mullai-1.0.1/mullai/mullai.py` & `mullai-1.0.2/mullai/mullai.py`

 * *Files identical despite different names*

### Comparing `mullai-1.0.1/mullai.egg-info/PKG-INFO` & `mullai-1.0.2/mullai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mullai
-Version: 1.0.1
+Version: 1.0.2
 Summary: A static site generator, that will allow you to generate content from database or remote.
 Home-page: https://github.com/whoisjeeva/mullai
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mullai-1.0.1/setup.py` & `mullai-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="mullai",
-    version="1.0.1",
+    version="1.0.2",
     description="A static site generator, that will allow you to generate content from database or remote.",
     url="https://github.com/whoisjeeva/mullai",
     author="Jeeva",
     author_email="support@gumify.me",
     license="MIT",
-    packages=["mullai"],
+    packages=find_packages(),
     install_requires=[
         "Jinja2==3.1.3",
         "Markdown==3.6",
         "MarkupSafe==2.1.5",
         "peewee==3.17.3",
         "PyMySQL==1.1.0",
         "python-slugify==8.0.4",
```

