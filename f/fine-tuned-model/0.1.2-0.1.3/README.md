# Comparing `tmp/fine-tuned-model-0.1.2.tar.gz` & `tmp/fine-tuned-model-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fine-tuned-model-0.1.2.tar", last modified: Wed May 15 18:23:41 2024, max compression
+gzip compressed data, was "fine-tuned-model-0.1.3.tar", last modified: Wed May 15 18:24:51 2024, max compression
```

## Comparing `fine-tuned-model-0.1.2.tar` & `fine-tuned-model-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 18:23:41.378451 fine-tuned-model-0.1.2/
--rw-rw-rw-   0        0        0     1090 2024-02-25 17:48:30.000000 fine-tuned-model-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      876 2024-05-15 18:23:41.377388 fine-tuned-model-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 18:23:41.374046 fine-tuned-model-0.1.2/fine_tuned_model.egg-info/
--rw-rw-rw-   0        0        0      876 2024-05-15 18:23:41.000000 fine-tuned-model-0.1.2/fine_tuned_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-15 18:23:41.000000 fine-tuned-model-0.1.2/fine_tuned_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:23:41.000000 fine-tuned-model-0.1.2/fine_tuned_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-15 18:23:41.000000 fine-tuned-model-0.1.2/fine_tuned_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:23:41.000000 fine-tuned-model-0.1.2/fine_tuned_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 18:23:41.378451 fine-tuned-model-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1154 2024-05-15 18:23:33.000000 fine-tuned-model-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:24:51.010259 fine-tuned-model-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2024-02-25 17:48:30.000000 fine-tuned-model-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      876 2024-05-15 18:24:51.009096 fine-tuned-model-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 18:24:51.006945 fine-tuned-model-0.1.3/fine_tuned_model.egg-info/
+-rw-rw-rw-   0        0        0      876 2024-05-15 18:24:50.000000 fine-tuned-model-0.1.3/fine_tuned_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-15 18:24:50.000000 fine-tuned-model-0.1.3/fine_tuned_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:24:50.000000 fine-tuned-model-0.1.3/fine_tuned_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-15 18:24:50.000000 fine-tuned-model-0.1.3/fine_tuned_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:24:50.000000 fine-tuned-model-0.1.3/fine_tuned_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 18:24:51.010765 fine-tuned-model-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1154 2024-05-15 18:24:47.000000 fine-tuned-model-0.1.3/setup.py
```

### Comparing `fine-tuned-model-0.1.2/LICENSE` & `fine-tuned-model-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fine-tuned-model-0.1.2/PKG-INFO` & `fine-tuned-model-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fine-tuned-model
-Version: 0.1.2
+Version: 0.1.3
 Summary: fine tuned model
 Home-page: https://github.com/NullpointerW/fine-tuned-model
 Author: vow1231a
 Author-email: voidmanwzp@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/NullpointerW/fine-tuned-model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fine-tuned-model-0.1.2/fine_tuned_model.egg-info/PKG-INFO` & `fine-tuned-model-0.1.3/fine_tuned_model.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fine-tuned-model
-Version: 0.1.2
+Version: 0.1.3
 Summary: fine tuned model
 Home-page: https://github.com/NullpointerW/fine-tuned-model
 Author: vow1231a
 Author-email: voidmanwzp@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/NullpointerW/fine-tuned-model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fine-tuned-model-0.1.2/setup.py` & `fine-tuned-model-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fine-tuned-model",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         # 在这里列出你的库所需的其他Python包
         'bardapi==0.1.23a0',
         'Flask==2.3.2',
         'httpx==0.24.1',
     ],
```

