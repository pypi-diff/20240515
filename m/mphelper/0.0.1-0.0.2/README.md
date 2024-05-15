# Comparing `tmp/mphelper-0.0.1.tar.gz` & `tmp/mphelper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mphelper-0.0.1.tar", last modified: Tue Apr 30 02:50:59 2024, max compression
+gzip compressed data, was "mphelper-0.0.2.tar", last modified: Wed May 15 17:25:13 2024, max compression
```

## Comparing `mphelper-0.0.1.tar` & `mphelper-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:50:59.627123 mphelper-0.0.1/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      655 2024-04-30 02:50:59.627123 mphelper-0.0.1/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       64 2024-04-30 02:48:54.000000 mphelper-0.0.1/README.md
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:50:59.625123 mphelper-0.0.1/mphelper/
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)    11007 2024-04-24 06:40:59.000000 mphelper-0.0.1/mphelper/__init__.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:50:59.627123 mphelper-0.0.1/mphelper.egg-info/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      655 2024-04-30 02:50:59.000000 mphelper-0.0.1/mphelper.egg-info/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      167 2024-04-30 02:50:59.000000 mphelper-0.0.1/mphelper.egg-info/SOURCES.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-04-30 02:50:59.000000 mphelper-0.0.1/mphelper.egg-info/dependency_links.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        9 2024-04-30 02:50:59.000000 mphelper-0.0.1/mphelper.egg-info/top_level.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-04-30 02:50:59.627123 mphelper-0.0.1/setup.cfg
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      828 2024-04-24 06:50:09.000000 mphelper-0.0.1/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-15 17:25:13.387519 mphelper-0.0.2/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      655 2024-05-15 17:25:13.387519 mphelper-0.0.2/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       64 2024-04-30 02:48:54.000000 mphelper-0.0.2/README.md
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-15 17:25:13.386519 mphelper-0.0.2/mphelper/
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)    10928 2024-05-15 16:46:00.000000 mphelper-0.0.2/mphelper/__init__.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-15 17:25:13.387519 mphelper-0.0.2/mphelper.egg-info/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      655 2024-05-15 17:25:04.000000 mphelper-0.0.2/mphelper.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      167 2024-05-15 17:25:04.000000 mphelper-0.0.2/mphelper.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-05-15 17:25:04.000000 mphelper-0.0.2/mphelper.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        9 2024-05-15 17:25:04.000000 mphelper-0.0.2/mphelper.egg-info/top_level.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-05-15 17:25:13.387519 mphelper-0.0.2/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      828 2024-05-15 16:45:40.000000 mphelper-0.0.2/setup.py
```

### Comparing `mphelper-0.0.1/PKG-INFO` & `mphelper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mphelper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for simple multi-processing support
 Home-page: https://github.com/aldenleung/mphelper/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mphelper-0.0.1/mphelper/__init__.py` & `mphelper-0.0.2/mphelper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 		
 		if not self.use_thread:
 			self.p.close()
 			self.q.close()
 		self.plock.release()
 		if self.callback is not None:
 			self.callback(self.state, self.r, self.begin_time, self.end_time, self.pid)
-			self.callback(self.state, self.r, self.begin_time, self.end_time, self.pid)
 
 
 class ProcessWrapPool():
 	'''
 	Process is not recycled. Hence this is very inefficient for running many short processes. 
 	However, it benefits from interruptable Process, and not affected by jupyter's "stop"   
 	'''
```

### Comparing `mphelper-0.0.1/mphelper.egg-info/PKG-INFO` & `mphelper-0.0.2/mphelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mphelper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for simple multi-processing support
 Home-page: https://github.com/aldenleung/mphelper/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mphelper-0.0.1/setup.py` & `mphelper-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
 requirements = []
 
 setup(
 	name="mphelper",
-	version="0.0.1",
+	version="0.0.2",
 	author="Alden Leung",
 	author_email="alden.leung@gmail.com",
 	description="A python package for simple multi-processing support",
 	long_description=readme,
 	long_description_content_type="text/markdown",
 	url="https://github.com/aldenleung/mphelper/",
 	packages=find_packages(),
```

