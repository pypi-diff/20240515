# Comparing `tmp/django_acs_email-0.0.3.tar.gz` & `tmp/django_acs_email-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_acs_email-0.0.3.tar", last modified: Sun Feb 12 17:35:39 2023, max compression
+gzip compressed data, was "django_acs_email-0.0.4.tar", last modified: Wed May 15 04:52:30 2024, max compression
```

## Comparing `django_acs_email-0.0.3.tar` & `django_acs_email-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2023-02-12 17:35:39.931952 django_acs_email-0.0.3/
--rw-r--r--   0 juan       (501) staff       (20)      648 2023-02-12 17:35:39.931680 django_acs_email-0.0.3/PKG-INFO
--rw-r--r--   0 juan       (501) staff       (20)       38 2023-02-12 17:35:39.932034 django_acs_email-0.0.3/setup.cfg
--rw-r--r--   0 juan       (501) staff       (20)     1228 2023-02-12 17:35:37.000000 django_acs_email-0.0.3/setup.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2023-02-12 17:35:39.926640 django_acs_email-0.0.3/src/
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2023-02-12 17:35:39.928995 django_acs_email-0.0.3/src/django_acs_email/
--rw-r--r--   0 juan       (501) staff       (20)       37 2023-02-12 15:23:53.000000 django_acs_email-0.0.3/src/django_acs_email/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     4341 2023-02-12 17:25:28.000000 django_acs_email-0.0.3/src/django_acs_email/backend.py
--rw-r--r--   0 juan       (501) staff       (20)      557 2023-02-12 14:11:11.000000 django_acs_email-0.0.3/src/django_acs_email/logger.py
--rw-r--r--   0 juan       (501) staff       (20)     1734 2023-02-12 14:39:22.000000 django_acs_email-0.0.3/src/django_acs_email/mime.py
--rw-r--r--   0 juan       (501) staff       (20)      747 2023-02-12 14:40:49.000000 django_acs_email-0.0.3/src/django_acs_email/triple.py
--rw-r--r--   0 juan       (501) staff       (20)      262 2023-02-12 14:41:46.000000 django_acs_email-0.0.3/src/django_acs_email/utils.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2023-02-12 17:35:39.931292 django_acs_email-0.0.3/src/django_acs_email.egg-info/
--rw-r--r--   0 juan       (501) staff       (20)      648 2023-02-12 17:35:39.000000 django_acs_email-0.0.3/src/django_acs_email.egg-info/PKG-INFO
--rw-r--r--   0 juan       (501) staff       (20)      413 2023-02-12 17:35:39.000000 django_acs_email-0.0.3/src/django_acs_email.egg-info/SOURCES.txt
--rw-r--r--   0 juan       (501) staff       (20)        1 2023-02-12 17:35:39.000000 django_acs_email-0.0.3/src/django_acs_email.egg-info/dependency_links.txt
--rw-r--r--   0 juan       (501) staff       (20)       26 2023-02-12 17:35:39.000000 django_acs_email-0.0.3/src/django_acs_email.egg-info/requires.txt
--rw-r--r--   0 juan       (501) staff       (20)       17 2023-02-12 17:35:39.000000 django_acs_email-0.0.3/src/django_acs_email.egg-info/top_level.txt
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-05-15 04:52:30.328909 django_acs_email-0.0.4/
+-rw-r--r--   0 juan       (501) staff       (20)      698 2024-05-15 04:52:30.327616 django_acs_email-0.0.4/PKG-INFO
+-rw-r--r--   0 juan       (501) staff       (20)       38 2024-05-15 04:52:30.329080 django_acs_email-0.0.4/setup.cfg
+-rw-r--r--   0 juan       (501) staff       (20)     1237 2024-05-15 04:51:40.000000 django_acs_email-0.0.4/setup.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-05-15 04:52:30.322523 django_acs_email-0.0.4/src/
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-05-15 04:52:30.325183 django_acs_email-0.0.4/src/django_acs_email/
+-rw-r--r--   0 juan       (501) staff       (20)       37 2024-05-15 04:30:04.000000 django_acs_email-0.0.4/src/django_acs_email/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)     4341 2024-05-15 04:30:04.000000 django_acs_email-0.0.4/src/django_acs_email/backend.py
+-rw-r--r--   0 juan       (501) staff       (20)      557 2024-05-15 04:30:04.000000 django_acs_email-0.0.4/src/django_acs_email/logger.py
+-rw-r--r--   0 juan       (501) staff       (20)     1734 2024-05-15 04:30:04.000000 django_acs_email-0.0.4/src/django_acs_email/mime.py
+-rw-r--r--   0 juan       (501) staff       (20)      747 2024-05-15 04:30:04.000000 django_acs_email-0.0.4/src/django_acs_email/triple.py
+-rw-r--r--   0 juan       (501) staff       (20)      262 2024-05-15 04:30:04.000000 django_acs_email-0.0.4/src/django_acs_email/utils.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-05-15 04:52:30.327129 django_acs_email-0.0.4/src/django_acs_email.egg-info/
+-rw-r--r--   0 juan       (501) staff       (20)      698 2024-05-15 04:52:30.000000 django_acs_email-0.0.4/src/django_acs_email.egg-info/PKG-INFO
+-rw-r--r--   0 juan       (501) staff       (20)      413 2024-05-15 04:52:30.000000 django_acs_email-0.0.4/src/django_acs_email.egg-info/SOURCES.txt
+-rw-r--r--   0 juan       (501) staff       (20)        1 2024-05-15 04:52:30.000000 django_acs_email-0.0.4/src/django_acs_email.egg-info/dependency_links.txt
+-rw-r--r--   0 juan       (501) staff       (20)       35 2024-05-15 04:52:30.000000 django_acs_email-0.0.4/src/django_acs_email.egg-info/requires.txt
+-rw-r--r--   0 juan       (501) staff       (20)       17 2024-05-15 04:52:30.000000 django_acs_email-0.0.4/src/django_acs_email.egg-info/top_level.txt
```

### Comparing `django_acs_email-0.0.3/PKG-INFO` & `django_acs_email-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django_acs_email
-Version: 0.0.3
+Version: 0.0.4
 Summary: Azure Comunication Service Email Backend for Django
 Author: Juan Carlos Espinoza Zurita
 Author-email: carlos_jcez@hotmail.com
 Keywords: python,django,azure,communication,service,email,backend
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django :: 4.0
 Requires-Python: >=3.6
+Requires-Dist: azure-communication-email==1.0.0b1
 
 Package to send emails using Azure Communication Service from Django using a BackendEmail.
```

### Comparing `django_acs_email-0.0.3/setup.py` & `django_acs_email-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "Azure Comunication Service Email Backend for Django"
 LONG_DESCRIPTION = "Package to send emails using Azure Communication Service from Django using a BackendEmail."
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="django_acs_email",
@@ -12,15 +12,15 @@
     author="Juan Carlos Espinoza Zurita",
     author_email="carlos_jcez@hotmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.6",
-    install_requires=["azure-communication-email"],  # add any additional packages that
+    install_requires=["azure-communication-email==1.0.0b1"],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
     keywords=[
         "python",
         "django",
         "azure",
         "communication",
         "service",
```

### Comparing `django_acs_email-0.0.3/src/django_acs_email/backend.py` & `django_acs_email-0.0.4/src/django_acs_email/backend.py`

 * *Files identical despite different names*

### Comparing `django_acs_email-0.0.3/src/django_acs_email/logger.py` & `django_acs_email-0.0.4/src/django_acs_email/logger.py`

 * *Files identical despite different names*

### Comparing `django_acs_email-0.0.3/src/django_acs_email/mime.py` & `django_acs_email-0.0.4/src/django_acs_email/mime.py`

 * *Files identical despite different names*

### Comparing `django_acs_email-0.0.3/src/django_acs_email/triple.py` & `django_acs_email-0.0.4/src/django_acs_email/triple.py`

 * *Files identical despite different names*

### Comparing `django_acs_email-0.0.3/src/django_acs_email.egg-info/PKG-INFO` & `django_acs_email-0.0.4/src/django_acs_email.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django-acs-email
-Version: 0.0.3
+Version: 0.0.4
 Summary: Azure Comunication Service Email Backend for Django
 Author: Juan Carlos Espinoza Zurita
 Author-email: carlos_jcez@hotmail.com
 Keywords: python,django,azure,communication,service,email,backend
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django :: 4.0
 Requires-Python: >=3.6
+Requires-Dist: azure-communication-email==1.0.0b1
 
 Package to send emails using Azure Communication Service from Django using a BackendEmail.
```

