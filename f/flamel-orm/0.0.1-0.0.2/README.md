# Comparing `tmp/flamel_orm-0.0.1.tar.gz` & `tmp/flamel_orm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamel_orm-0.0.1.tar", last modified: Wed May 15 18:38:05 2024, max compression
+gzip compressed data, was "flamel_orm-0.0.2.tar", last modified: Wed May 15 18:47:42 2024, max compression
```

## Comparing `flamel_orm-0.0.1.tar` & `flamel_orm-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:38:05.077139 flamel_orm-0.0.1/
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1061 2024-05-06 19:53:28.000000 flamel_orm-0.0.1/LICENSE
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3038 2024-05-15 18:38:05.077139 flamel_orm-0.0.1/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     2690 2024-05-11 20:25:34.000000 flamel_orm-0.0.1/README.md
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:38:05.073139 flamel_orm-0.0.1/flamel/
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       22 2024-05-11 00:52:30.000000 flamel_orm-0.0.1/flamel/__init__.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     2487 2024-05-11 19:46:26.000000 flamel_orm-0.0.1/flamel/base.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     4371 2024-05-05 19:07:21.000000 flamel_orm-0.0.1/flamel/column.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1690 2024-05-11 19:54:50.000000 flamel_orm-0.0.1/flamel/dialect.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     3024 2024-05-12 19:14:23.000000 flamel_orm-0.0.1/flamel/query.py
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:38:05.077139 flamel_orm-0.0.1/flamel_orm.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3038 2024-05-15 18:38:05.000000 flamel_orm-0.0.1/flamel_orm.egg-info/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      360 2024-05-15 18:38:05.000000 flamel_orm-0.0.1/flamel_orm.egg-info/SOURCES.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-15 18:38:05.000000 flamel_orm-0.0.1/flamel_orm.egg-info/dependency_links.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        7 2024-05-15 18:38:05.000000 flamel_orm-0.0.1/flamel_orm.egg-info/top_level.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      600 2024-05-15 18:37:53.000000 flamel_orm-0.0.1/pyproject.toml
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-15 18:38:05.077139 flamel_orm-0.0.1/setup.cfg
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:38:05.077139 flamel_orm-0.0.1/tests/
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     3350 2024-05-11 18:58:02.000000 flamel_orm-0.0.1/tests/test_base.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     3412 2024-05-11 00:54:52.000000 flamel_orm-0.0.1/tests/test_column.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      588 2024-05-11 00:54:52.000000 flamel_orm-0.0.1/tests/test_dialect.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     5293 2024-05-11 19:52:40.000000 flamel_orm-0.0.1/tests/test_query.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      982 2024-05-11 00:54:52.000000 flamel_orm-0.0.1/tests/test_sqlbuilder.py
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:47:42.386389 flamel_orm-0.0.2/
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1061 2024-05-06 19:53:28.000000 flamel_orm-0.0.2/LICENSE
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     3129 2024-05-15 18:47:42.386389 flamel_orm-0.0.2/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     2697 2024-05-15 18:46:55.000000 flamel_orm-0.0.2/README.md
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:47:42.386389 flamel_orm-0.0.2/flamel/
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       22 2024-05-11 00:52:30.000000 flamel_orm-0.0.2/flamel/__init__.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     2487 2024-05-11 19:46:26.000000 flamel_orm-0.0.2/flamel/base.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     4371 2024-05-05 19:07:21.000000 flamel_orm-0.0.2/flamel/column.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1690 2024-05-11 19:54:50.000000 flamel_orm-0.0.2/flamel/dialect.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     3024 2024-05-12 19:14:23.000000 flamel_orm-0.0.2/flamel/query.py
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:47:42.386389 flamel_orm-0.0.2/flamel_orm.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     3129 2024-05-15 18:47:42.000000 flamel_orm-0.0.2/flamel_orm.egg-info/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      360 2024-05-15 18:47:42.000000 flamel_orm-0.0.2/flamel_orm.egg-info/SOURCES.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-15 18:47:42.000000 flamel_orm-0.0.2/flamel_orm.egg-info/dependency_links.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        7 2024-05-15 18:47:42.000000 flamel_orm-0.0.2/flamel_orm.egg-info/top_level.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      690 2024-05-15 18:46:39.000000 flamel_orm-0.0.2/pyproject.toml
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-15 18:47:42.386389 flamel_orm-0.0.2/setup.cfg
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:47:42.386389 flamel_orm-0.0.2/tests/
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     3350 2024-05-11 18:58:02.000000 flamel_orm-0.0.2/tests/test_base.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     3412 2024-05-11 00:54:52.000000 flamel_orm-0.0.2/tests/test_column.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      588 2024-05-11 00:54:52.000000 flamel_orm-0.0.2/tests/test_dialect.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     5293 2024-05-11 19:52:40.000000 flamel_orm-0.0.2/tests/test_query.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      982 2024-05-11 00:54:52.000000 flamel_orm-0.0.2/tests/test_sqlbuilder.py
```

### Comparing `flamel_orm-0.0.1/LICENSE` & `flamel_orm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/PKG-INFO` & `flamel_orm-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: flamel-orm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple declarative ORM for SQLite
-Author-email: test <test@test.com>
+Author-email: fernando24164 <fernando24164@gmail.com>
 License: MIT
+Project-URL: Repository, https://github.com/fernando24164/flamel
 Keywords: ORM,simple
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,15 +33,15 @@
 A declarative ORM from scratch, compatible with SQLite
 
 ## ➤ Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [your project name].
 
 ```bash
-pip install ...
+pip install flamel-orm
 ```
 
 ## 📚 Usage
 
 ```python
 from flamel.base import Base
 from flamel.column import Column, Integer, String
```

### Comparing `flamel_orm-0.0.1/README.md` & `flamel_orm-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 A declarative ORM from scratch, compatible with SQLite
 
 ## ➤ Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [your project name].
 
 ```bash
-pip install ...
+pip install flamel-orm
 ```
 
 ## 📚 Usage
 
 ```python
 from flamel.base import Base
 from flamel.column import Column, Integer, String
```

### Comparing `flamel_orm-0.0.1/flamel/base.py` & `flamel_orm-0.0.2/flamel/base.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/flamel/column.py` & `flamel_orm-0.0.2/flamel/column.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/flamel/dialect.py` & `flamel_orm-0.0.2/flamel/dialect.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/flamel/query.py` & `flamel_orm-0.0.2/flamel/query.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/flamel_orm.egg-info/PKG-INFO` & `flamel_orm-0.0.2/flamel_orm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: flamel-orm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple declarative ORM for SQLite
-Author-email: test <test@test.com>
+Author-email: fernando24164 <fernando24164@gmail.com>
 License: MIT
+Project-URL: Repository, https://github.com/fernando24164/flamel
 Keywords: ORM,simple
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,15 +33,15 @@
 A declarative ORM from scratch, compatible with SQLite
 
 ## ➤ Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [your project name].
 
 ```bash
-pip install ...
+pip install flamel-orm
 ```
 
 ## 📚 Usage
 
 ```python
 from flamel.base import Base
 from flamel.column import Column, Integer, String
```

### Comparing `flamel_orm-0.0.1/tests/test_base.py` & `flamel_orm-0.0.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/tests/test_column.py` & `flamel_orm-0.0.2/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/tests/test_dialect.py` & `flamel_orm-0.0.2/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/tests/test_query.py` & `flamel_orm-0.0.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.1/tests/test_sqlbuilder.py` & `flamel_orm-0.0.2/tests/test_sqlbuilder.py`

 * *Files identical despite different names*

