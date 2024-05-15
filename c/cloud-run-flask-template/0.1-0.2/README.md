# Comparing `tmp/cloud_run_flask_template-0.1.tar.gz` & `tmp/cloud_run_flask_template-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_run_flask_template-0.1.tar", last modified: Wed May 15 12:40:16 2024, max compression
+gzip compressed data, was "cloud_run_flask_template-0.2.tar", last modified: Wed May 15 12:53:58 2024, max compression
```

## Comparing `cloud_run_flask_template-0.1.tar` & `cloud_run_flask_template-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:40:16.962110 cloud_run_flask_template-0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2024-05-15 12:35:36.000000 cloud_run_flask_template-0.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      572 2024-05-15 12:40:16.962110 cloud_run_flask_template-0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2024-05-15 12:35:36.000000 cloud_run_flask_template-0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:40:16.962110 cloud_run_flask_template-0.1/cloud_run_flask_template/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:37:37.000000 cloud_run_flask_template-0.1/cloud_run_flask_template/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3884 2024-05-15 12:38:04.000000 cloud_run_flask_template-0.1/cloud_run_flask_template/generator.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:40:16.962110 cloud_run_flask_template-0.1/cloud_run_flask_template.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      572 2024-05-15 12:40:16.000000 cloud_run_flask_template-0.1/cloud_run_flask_template.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-05-15 12:40:16.000000 cloud_run_flask_template-0.1/cloud_run_flask_template.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 12:40:16.000000 cloud_run_flask_template-0.1/cloud_run_flask_template.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       97 2024-05-15 12:40:16.000000 cloud_run_flask_template-0.1/cloud_run_flask_template.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2024-05-15 12:40:16.000000 cloud_run_flask_template-0.1/cloud_run_flask_template.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-15 12:40:16.000000 cloud_run_flask_template-0.1/cloud_run_flask_template.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-15 12:40:16.962110 cloud_run_flask_template-0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      876 2024-05-15 12:38:29.000000 cloud_run_flask_template-0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:53:58.646081 cloud_run_flask_template-0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2024-05-15 12:35:36.000000 cloud_run_flask_template-0.2/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2508 2024-05-15 12:53:58.646081 cloud_run_flask_template-0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1959 2024-05-15 12:50:36.000000 cloud_run_flask_template-0.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:53:58.642081 cloud_run_flask_template-0.2/cloud_run_flask_template/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:37:37.000000 cloud_run_flask_template-0.2/cloud_run_flask_template/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3884 2024-05-15 12:38:04.000000 cloud_run_flask_template-0.2/cloud_run_flask_template/generator.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:53:58.642081 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2508 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       97 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-15 12:53:58.000000 cloud_run_flask_template-0.2/cloud_run_flask_template.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-15 12:53:58.646081 cloud_run_flask_template-0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1008 2024-05-15 12:53:22.000000 cloud_run_flask_template-0.2/setup.py
```

### Comparing `cloud_run_flask_template-0.1/LICENSE` & `cloud_run_flask_template-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud_run_flask_template-0.1/cloud_run_flask_template/generator.py` & `cloud_run_flask_template-0.2/cloud_run_flask_template/generator.py`

 * *Files identical despite different names*

### Comparing `cloud_run_flask_template-0.1/setup.py` & `cloud_run_flask_template-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup, find_packages
 
+# Read the contents of your README file
+with open('README.md', 'r') as f:
+    long_description = f.read()
+
 setup(
     name='cloud_run_flask_template',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'cloud_run_flask_template = cloud_run_flask_template.generator:generate_project'
         ]
     },
     install_requires=[
         'Flask==3.0.3',
         'gunicorn==22.0.0',
         'Werkzeug==3.0.3'
     ],
     author='Your Name',
     author_email='your.email@example.com',
     description='A template for Google Cloud Run Flask development',
-    long_description=open('README.md').read(),
+    long_description=long_description,  # Set the long description here
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cloud_run_flask_template',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

