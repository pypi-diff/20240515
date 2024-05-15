# Comparing `tmp/certbot_dns_mydnsjp-1.0.0.tar.gz` & `tmp/certbot_dns_mydnsjp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot_dns_mydnsjp-1.0.0.tar", last modified: Wed May 15 08:35:17 2024, max compression
+gzip compressed data, was "certbot_dns_mydnsjp-1.0.1.tar", last modified: Wed May 15 10:05:16 2024, max compression
```

## Comparing `certbot_dns_mydnsjp-1.0.0.tar` & `certbot_dns_mydnsjp-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 08:35:17.984588 certbot_dns_mydnsjp-1.0.0/
--rw-r--r--   0 giga      (1000) giga      (1000)     4200 2024-05-15 01:11:27.000000 certbot_dns_mydnsjp-1.0.0/.dockerignore
--rw-r--r--   0 giga      (1000) giga      (1000)     4749 2024-05-08 12:47:36.000000 certbot_dns_mydnsjp-1.0.0/.gitignore
--rw-r--r--   0 giga      (1000) giga      (1000)      142 2024-05-15 07:45:12.000000 certbot_dns_mydnsjp-1.0.0/Dockerfile
--rw-r--r--   0 giga      (1000) giga      (1000)     1069 2024-05-08 12:47:36.000000 certbot_dns_mydnsjp-1.0.0/LICENSE
--rw-r--r--   0 giga      (1000) giga      (1000)       63 2024-05-09 15:13:34.000000 certbot_dns_mydnsjp-1.0.0/MANIFEST.in
--rw-r--r--   0 giga      (1000) giga      (1000)    15476 2024-05-15 08:35:17.984588 certbot_dns_mydnsjp-1.0.0/PKG-INFO
--rw-r--r--   0 giga      (1000) giga      (1000)    14507 2024-05-15 07:50:32.000000 certbot_dns_mydnsjp-1.0.0/Readme.md
-drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 08:35:17.980588 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/
--rw-r--r--   0 giga      (1000) giga      (1000)        0 2024-05-14 12:36:57.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/__init__.py
-drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 08:35:17.980588 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/cert/
--rw-r--r--   0 giga      (1000) giga      (1000)        0 2024-05-08 12:47:36.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/cert/__init__.py
--rw-r--r--   0 giga      (1000) giga      (1000)     4796 2024-05-14 14:28:21.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/cert/client.py
-drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 08:35:17.980588 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/mydnsjp/
--rw-r--r--   0 giga      (1000) giga      (1000)        0 2024-05-08 12:47:36.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/mydnsjp/__init__.py
--rw-r--r--   0 giga      (1000) giga      (1000)    19582 2024-05-15 04:07:11.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/mydnsjp/client.py
-drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 08:35:17.984588 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/
--rw-r--r--   0 giga      (1000) giga      (1000)    15476 2024-05-15 08:35:17.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/PKG-INFO
--rw-rw-r--   0 giga      (1000) giga      (1000)      573 2024-05-15 08:35:17.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/SOURCES.txt
--rw-rw-r--   0 giga      (1000) giga      (1000)        1 2024-05-15 08:35:17.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/dependency_links.txt
--rw-rw-r--   0 giga      (1000) giga      (1000)       78 2024-05-15 08:35:17.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/entry_points.txt
--rw-rw-r--   0 giga      (1000) giga      (1000)       43 2024-05-15 08:35:17.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/requires.txt
--rw-rw-r--   0 giga      (1000) giga      (1000)       20 2024-05-15 08:35:17.000000 certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/top_level.txt
--rw-r--r--   0 giga      (1000) giga      (1000)       76 2024-05-15 01:06:49.000000 certbot_dns_mydnsjp-1.0.0/requirements.txt
--rw-rw-r--   0 giga      (1000) giga      (1000)       38 2024-05-15 08:35:17.984588 certbot_dns_mydnsjp-1.0.0/setup.cfg
--rw-r--r--   0 giga      (1000) giga      (1000)     1478 2024-05-14 13:58:59.000000 certbot_dns_mydnsjp-1.0.0/setup.py
-drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 08:35:17.980588 certbot_dns_mydnsjp-1.0.0/snap/
--rw-r--r--   0 giga      (1000) giga      (1000)     1153 2024-05-14 13:59:47.000000 certbot_dns_mydnsjp-1.0.0/snap/snapcraft.yaml
--rw-r--r--   0 giga      (1000) giga      (1000)    26522 2024-05-14 12:27:36.000000 certbot_dns_mydnsjp-1.0.0/third-party-notices
+drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 10:05:16.957440 certbot_dns_mydnsjp-1.0.1/
+-rw-rw-r--   0 giga      (1000) giga      (1000)     4195 2024-05-15 10:04:12.000000 certbot_dns_mydnsjp-1.0.1/.dockerignore
+-rw-r--r--   0 giga      (1000) giga      (1000)     4749 2024-05-08 12:47:36.000000 certbot_dns_mydnsjp-1.0.1/.gitignore
+-rw-r--r--   0 giga      (1000) giga      (1000)      142 2024-05-15 07:45:12.000000 certbot_dns_mydnsjp-1.0.1/Dockerfile
+-rw-r--r--   0 giga      (1000) giga      (1000)     1069 2024-05-08 12:47:36.000000 certbot_dns_mydnsjp-1.0.1/LICENSE
+-rw-r--r--   0 giga      (1000) giga      (1000)       63 2024-05-09 15:13:34.000000 certbot_dns_mydnsjp-1.0.1/MANIFEST.in
+-rw-r--r--   0 giga      (1000) giga      (1000)    15476 2024-05-15 10:05:16.957440 certbot_dns_mydnsjp-1.0.1/PKG-INFO
+-rw-r--r--   0 giga      (1000) giga      (1000)    14507 2024-05-15 07:50:32.000000 certbot_dns_mydnsjp-1.0.1/Readme.md
+drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 10:05:16.953441 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/
+-rw-r--r--   0 giga      (1000) giga      (1000)        0 2024-05-14 12:36:57.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/__init__.py
+drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 10:05:16.953441 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/cert/
+-rw-r--r--   0 giga      (1000) giga      (1000)        0 2024-05-08 12:47:36.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/cert/__init__.py
+-rw-r--r--   0 giga      (1000) giga      (1000)     4796 2024-05-14 14:28:21.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/cert/client.py
+drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 10:05:16.953441 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/mydnsjp/
+-rw-r--r--   0 giga      (1000) giga      (1000)        0 2024-05-08 12:47:36.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/mydnsjp/__init__.py
+-rw-r--r--   0 giga      (1000) giga      (1000)    19582 2024-05-15 04:07:11.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/mydnsjp/client.py
+drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 10:05:16.953441 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/
+-rw-r--r--   0 giga      (1000) giga      (1000)    15476 2024-05-15 10:05:16.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/PKG-INFO
+-rw-rw-r--   0 giga      (1000) giga      (1000)      573 2024-05-15 10:05:16.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/SOURCES.txt
+-rw-rw-r--   0 giga      (1000) giga      (1000)        1 2024-05-15 10:05:16.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/dependency_links.txt
+-rw-rw-r--   0 giga      (1000) giga      (1000)       78 2024-05-15 10:05:16.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/entry_points.txt
+-rw-rw-r--   0 giga      (1000) giga      (1000)       43 2024-05-15 10:05:16.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/requires.txt
+-rw-rw-r--   0 giga      (1000) giga      (1000)       20 2024-05-15 10:05:16.000000 certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/top_level.txt
+-rw-r--r--   0 giga      (1000) giga      (1000)       76 2024-05-15 01:06:49.000000 certbot_dns_mydnsjp-1.0.1/requirements.txt
+-rw-rw-r--   0 giga      (1000) giga      (1000)       38 2024-05-15 10:05:16.957440 certbot_dns_mydnsjp-1.0.1/setup.cfg
+-rw-r--r--   0 giga      (1000) giga      (1000)     1478 2024-05-14 13:58:59.000000 certbot_dns_mydnsjp-1.0.1/setup.py
+drwxrwxr-x   0 giga      (1000) giga      (1000)        0 2024-05-15 10:05:16.953441 certbot_dns_mydnsjp-1.0.1/snap/
+-rw-r--r--   0 giga      (1000) giga      (1000)     1153 2024-05-14 13:59:47.000000 certbot_dns_mydnsjp-1.0.1/snap/snapcraft.yaml
+-rw-r--r--   0 giga      (1000) giga      (1000)    26522 2024-05-14 12:27:36.000000 certbot_dns_mydnsjp-1.0.1/third-party-notices
```

### Comparing `certbot_dns_mydnsjp-1.0.0/.dockerignore` & `certbot_dns_mydnsjp-1.0.1/.dockerignore`

 * *Files 6% similar despite different names*

```diff
@@ -238,9 +238,8 @@
 
 # Android studio 3.1+ serialized cache file
 .idea/caches/build_file_checksums.ser
 
 # Custom rules
 .github
 docker
-snap
 *.snap
```

### Comparing `certbot_dns_mydnsjp-1.0.0/.gitignore` & `certbot_dns_mydnsjp-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `certbot_dns_mydnsjp-1.0.0/LICENSE` & `certbot_dns_mydnsjp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot_dns_mydnsjp-1.0.0/PKG-INFO` & `certbot_dns_mydnsjp-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot_dns_mydnsjp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Authenticator plugin for certbot to handle dns-01 challenge with MyDNS.JP.
 Home-page: https://github.com/usk-johnny-s/certbot_dns_mydnsjp/
 Author: usk-johnny-s
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `certbot_dns_mydnsjp-1.0.0/Readme.md` & `certbot_dns_mydnsjp-1.0.1/Readme.md`

 * *Files identical despite different names*

### Comparing `certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/cert/client.py` & `certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/cert/client.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp/mydnsjp/client.py` & `certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp/mydnsjp/client.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/PKG-INFO` & `certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot_dns_mydnsjp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Authenticator plugin for certbot to handle dns-01 challenge with MyDNS.JP.
 Home-page: https://github.com/usk-johnny-s/certbot_dns_mydnsjp/
 Author: usk-johnny-s
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `certbot_dns_mydnsjp-1.0.0/certbot_dns_mydnsjp.egg-info/SOURCES.txt` & `certbot_dns_mydnsjp-1.0.1/certbot_dns_mydnsjp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot_dns_mydnsjp-1.0.0/setup.py` & `certbot_dns_mydnsjp-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_mydnsjp-1.0.0/snap/snapcraft.yaml` & `certbot_dns_mydnsjp-1.0.1/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `certbot_dns_mydnsjp-1.0.0/third-party-notices` & `certbot_dns_mydnsjp-1.0.1/third-party-notices`

 * *Files identical despite different names*

