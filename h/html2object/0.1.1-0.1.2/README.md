# Comparing `tmp/html2object-0.1.1.tar.gz` & `tmp/html2object-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2object-0.1.1.tar", last modified: Tue May 14 19:45:50 2024, max compression
+gzip compressed data, was "html2object-0.1.2.tar", last modified: Tue May 14 20:20:22 2024, max compression
```

## Comparing `html2object-0.1.1.tar` & `html2object-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:45:50.202280 html2object-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 19:45:41.000000 html2object-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 19:45:50.202280 html2object-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-14 19:45:41.000000 html2object-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:45:50.202280 html2object-0.1.1/html2object.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 19:45:50.000000 html2object-0.1.1/html2object.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-14 19:45:50.000000 html2object-0.1.1/html2object.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:45:50.000000 html2object-0.1.1/html2object.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:45:50.000000 html2object-0.1.1/html2object.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:45:50.202280 html2object-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-14 19:45:41.000000 html2object-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:45:50.202280 html2object-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:45:41.000000 html2object-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-14 19:45:41.000000 html2object-0.1.1/tests/test_html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:22.862776 html2object-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 20:20:14.000000 html2object-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-14 20:20:22.862776 html2object-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-14 20:20:14.000000 html2object-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:22.858776 html2object-0.1.2/html2object/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 20:20:14.000000 html2object-0.1.2/html2object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-14 20:20:14.000000 html2object-0.1.2/html2object/html2object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-14 20:20:14.000000 html2object-0.1.2/html2object/html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:22.862776 html2object-0.1.2/html2object.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-14 20:20:22.000000 html2object-0.1.2/html2object.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 20:20:22.000000 html2object-0.1.2/html2object.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:20:22.000000 html2object-0.1.2/html2object.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 20:20:22.000000 html2object-0.1.2/html2object.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:20:22.862776 html2object-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-14 20:20:14.000000 html2object-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:22.858776 html2object-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:14.000000 html2object-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-14 20:20:14.000000 html2object-0.1.2/tests/test_html_element.py
```

### Comparing `html2object-0.1.1/LICENSE` & `html2object-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `html2object-0.1.1/PKG-INFO` & `html2object-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2object
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools to handle the CRUD of .html files as objects.
 Home-page: https://github.com/boterop/html2object
 Author: boterop
 Author-email: boterop22@gmail.com
 Keywords: html,utils,html_utils,html_element,html_parser,html_writer,html_reader,html_crud,html_object,html_file,html_utils.py,html_element.py,html_parser.py,html_writer.py,html_reader.py,html_crud.py,html_object.py,html_file.py,html2object,html2object.py,html2object.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,29 +21,28 @@
 
 [![Coverage Status](https://coveralls.io/repos/github/boterop/html2object/badge.svg?branch=main)](https://coveralls.io/github/boterop/html2object?branch=main)
 
 # HTML 2 Object
 
 Tools to handle the CRUD of .html files as objects.
 
-## Table of Contents
+## Install
 
-- [Installation](#installation)
-- [Usage](#usage)
-- [Contributing](#contributing)
-- [License](#license)
+```sh
+pip install html2object
+```
 
 ## Usage
 
 This project provides a way to manipulate HTML files and update them dynamically. Here's how you can use it:
 
 First, import the necessary classes from this project:
 
 ```sh
-from html_element import HtmlElement
+from html2object import HtmlElement
 ```
 
 read your html file and create an `HtmlElement()`
 
 ```sh
 html = open(<path>, "r").read("bin/gui/index.html")
 document = HtmlElement(html)
@@ -76,15 +75,15 @@
 
 save the html file running
 
 ```sh
 open(path, "w").write(str(document)).close()
 ```
 
-## Installation
+## Local setup
 
 Instructions on how to install and set up your project. Include any dependencies that need to be installed.
 
 1. Clone the repository
 2. Navigate to the project directory:
 
 ```sh
```

### Comparing `html2object-0.1.1/README.md` & `html2object-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [![Coverage Status](https://coveralls.io/repos/github/boterop/html2object/badge.svg?branch=main)](https://coveralls.io/github/boterop/html2object?branch=main)
 
 # HTML 2 Object
 
 Tools to handle the CRUD of .html files as objects.
 
-## Table of Contents
+## Install
 
-- [Installation](#installation)
-- [Usage](#usage)
-- [Contributing](#contributing)
-- [License](#license)
+```sh
+pip install html2object
+```
 
 ## Usage
 
 This project provides a way to manipulate HTML files and update them dynamically. Here's how you can use it:
 
 First, import the necessary classes from this project:
 
 ```sh
-from html_element import HtmlElement
+from html2object import HtmlElement
 ```
 
 read your html file and create an `HtmlElement()`
 
 ```sh
 html = open(<path>, "r").read("bin/gui/index.html")
 document = HtmlElement(html)
@@ -55,15 +54,15 @@
 
 save the html file running
 
 ```sh
 open(path, "w").write(str(document)).close()
 ```
 
-## Installation
+## Local setup
 
 Instructions on how to install and set up your project. Include any dependencies that need to be installed.
 
 1. Clone the repository
 2. Navigate to the project directory:
 
 ```sh
```

### Comparing `html2object-0.1.1/html2object.egg-info/PKG-INFO` & `html2object-0.1.2/html2object.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2object
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools to handle the CRUD of .html files as objects.
 Home-page: https://github.com/boterop/html2object
 Author: boterop
 Author-email: boterop22@gmail.com
 Keywords: html,utils,html_utils,html_element,html_parser,html_writer,html_reader,html_crud,html_object,html_file,html_utils.py,html_element.py,html_parser.py,html_writer.py,html_reader.py,html_crud.py,html_object.py,html_file.py,html2object,html2object.py,html2object.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,29 +21,28 @@
 
 [![Coverage Status](https://coveralls.io/repos/github/boterop/html2object/badge.svg?branch=main)](https://coveralls.io/github/boterop/html2object?branch=main)
 
 # HTML 2 Object
 
 Tools to handle the CRUD of .html files as objects.
 
-## Table of Contents
+## Install
 
-- [Installation](#installation)
-- [Usage](#usage)
-- [Contributing](#contributing)
-- [License](#license)
+```sh
+pip install html2object
+```
 
 ## Usage
 
 This project provides a way to manipulate HTML files and update them dynamically. Here's how you can use it:
 
 First, import the necessary classes from this project:
 
 ```sh
-from html_element import HtmlElement
+from html2object import HtmlElement
 ```
 
 read your html file and create an `HtmlElement()`
 
 ```sh
 html = open(<path>, "r").read("bin/gui/index.html")
 document = HtmlElement(html)
@@ -76,15 +75,15 @@
 
 save the html file running
 
 ```sh
 open(path, "w").write(str(document)).close()
 ```
 
-## Installation
+## Local setup
 
 Instructions on how to install and set up your project. Include any dependencies that need to be installed.
 
 1. Clone the repository
 2. Navigate to the project directory:
 
 ```sh
```

### Comparing `html2object-0.1.1/setup.py` & `html2object-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="html2object",
-    version="0.1.1",
+    version="0.1.2",
     author="boterop",
     author_email="boterop22@gmail.com",
     description="Tools to handle the CRUD of .html files as objects.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/boterop/html2object",
     packages=find_packages(),
```

### Comparing `html2object-0.1.1/tests/test_html_element.py` & `html2object-0.1.2/tests/test_html_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from html_element import HtmlElement
+from html2object.html_element import HtmlElement
 
 
 class TestHtmlElement(unittest.TestCase):
 
     def test_init(self):
         element = HtmlElement()
         self.assertEqual(element.name, "")
```

