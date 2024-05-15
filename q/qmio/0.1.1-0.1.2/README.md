# Comparing `tmp/qmio-0.1.1.tar.gz` & `tmp/qmio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmio-0.1.1.tar", last modified: Wed May 15 10:48:21 2024, max compression
+gzip compressed data, was "qmio-0.1.2.tar", last modified: Wed May 15 15:57:04 2024, max compression
```

## Comparing `qmio-0.1.1.tar` & `qmio-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 10:48:21.528248 qmio-0.1.1/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)    11358 2024-05-08 07:55:18.000000 qmio-0.1.1/LICENSE
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     7834 2024-05-15 10:48:21.528248 qmio-0.1.1/PKG-INFO
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     7418 2024-05-08 07:55:18.000000 qmio-0.1.1/README.md
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 10:48:21.524248 qmio-0.1.1/config/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       50 2024-05-08 10:14:51.000000 qmio-0.1.1/config/__init__.py
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 10:48:21.524248 qmio-0.1.1/qmio/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       63 2024-05-08 09:58:54.000000 qmio-0.1.1/qmio/__init__.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     2255 2024-05-08 09:56:22.000000 qmio-0.1.1/qmio/backends.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      346 2024-05-08 09:53:14.000000 qmio-0.1.1/qmio/circuits.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     1511 2024-05-08 10:12:16.000000 qmio-0.1.1/qmio/clients.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     1092 2024-05-08 07:55:18.000000 qmio-0.1.1/qmio/qmio.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      275 2024-05-08 07:55:18.000000 qmio-0.1.1/qmio/services.py
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 10:48:21.528248 qmio-0.1.1/qmio.egg-info/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     7834 2024-05-15 10:48:21.000000 qmio-0.1.1/qmio.egg-info/PKG-INFO
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      380 2024-05-15 10:48:21.000000 qmio-0.1.1/qmio.egg-info/SOURCES.txt
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)        1 2024-05-15 10:48:21.000000 qmio-0.1.1/qmio.egg-info/dependency_links.txt
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       21 2024-05-15 10:48:21.000000 qmio-0.1.1/qmio.egg-info/requires.txt
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       18 2024-05-15 10:48:21.000000 qmio-0.1.1/qmio.egg-info/top_level.txt
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      630 2024-05-15 10:48:21.528248 qmio-0.1.1/setup.cfg
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       38 2024-05-08 07:55:18.000000 qmio-0.1.1/setup.py
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 10:48:21.528248 qmio-0.1.1/tests/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)        0 2024-05-08 07:55:18.000000 qmio-0.1.1/tests/__init__.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      834 2024-05-08 07:55:18.000000 qmio-0.1.1/tests/test_backends.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      412 2024-05-08 07:55:18.000000 qmio-0.1.1/tests/test_services.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       35 2024-05-08 07:55:18.000000 qmio-0.1.1/tests/test_zmq_client.py
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)    11358 2024-05-08 07:55:18.000000 qmio-0.1.2/LICENSE
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      828 2024-05-15 15:57:04.200924 qmio-0.1.2/PKG-INFO
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      412 2024-05-15 15:53:18.000000 qmio-0.1.2/README.md
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/config/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       50 2024-05-08 10:14:51.000000 qmio-0.1.2/config/__init__.py
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/qmio/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       63 2024-05-15 15:55:44.000000 qmio-0.1.2/qmio/__init__.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     2255 2024-05-08 09:56:22.000000 qmio-0.1.2/qmio/backends.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      346 2024-05-08 09:53:14.000000 qmio-0.1.2/qmio/circuits.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     1511 2024-05-08 10:12:16.000000 qmio-0.1.2/qmio/clients.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     1092 2024-05-08 07:55:18.000000 qmio-0.1.2/qmio/qmio.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      275 2024-05-08 07:55:18.000000 qmio-0.1.2/qmio/services.py
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/qmio.egg-info/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      828 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/PKG-INFO
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      380 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)        1 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       21 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/requires.txt
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       18 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/top_level.txt
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      630 2024-05-15 15:57:04.200924 qmio-0.1.2/setup.cfg
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       38 2024-05-08 07:55:18.000000 qmio-0.1.2/setup.py
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/tests/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)        0 2024-05-08 07:55:18.000000 qmio-0.1.2/tests/__init__.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      834 2024-05-08 07:55:18.000000 qmio-0.1.2/tests/test_backends.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      412 2024-05-08 07:55:18.000000 qmio-0.1.2/tests/test_services.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       35 2024-05-08 07:55:18.000000 qmio-0.1.2/tests/test_zmq_client.py
```

### Comparing `qmio-0.1.1/LICENSE` & `qmio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qmio-0.1.1/qmio/backends.py` & `qmio-0.1.2/qmio/backends.py`

 * *Files identical despite different names*

### Comparing `qmio-0.1.1/qmio/clients.py` & `qmio-0.1.2/qmio/clients.py`

 * *Files identical despite different names*

### Comparing `qmio-0.1.1/qmio/qmio.py` & `qmio-0.1.2/qmio/qmio.py`

 * *Files identical despite different names*

### Comparing `qmio-0.1.1/setup.cfg` & `qmio-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qmio
-version = 0.1.1
+version = 0.1.2
 author = 'Javier Cacheiro, Alvaro Caride'
 author_email = 'javier.cacheiro@gmail.com, a.caride.sanchez@gmail.com'
 url = https://github.com/javicacheiro/qmio
 license = Apache
 description = Helper python module to interact with the different backends available in Qmio.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `qmio-0.1.1/tests/test_backends.py` & `qmio-0.1.2/tests/test_backends.py`

 * *Files identical despite different names*

