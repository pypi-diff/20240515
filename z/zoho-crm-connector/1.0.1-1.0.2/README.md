# Comparing `tmp/zoho_crm_connector-1.0.1.tar.gz` & `tmp/zoho_crm_connector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho_crm_connector-1.0.1.tar", last modified: Tue May 14 05:02:19 2024, max compression
+gzip compressed data, was "zoho_crm_connector-1.0.2.tar", last modified: Tue May 14 05:09:43 2024, max compression
```

## Comparing `zoho_crm_connector-1.0.1.tar` & `zoho_crm_connector-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1064 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.1/LICENCE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       19 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.1/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)     7744 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     7193 2024-05-14 03:29:42.000000 zoho_crm_connector-1.0.1/README.md
--rw-rw-r--   0 tim       (1000) tim       (1000)       63 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)     1467 2024-05-14 03:28:56.000000 zoho_crm_connector-1.0.1/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/zoho_crm_connector/
--rw-rw-r--   0 tim       (1000) tim       (1000)       35 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.1/zoho_crm_connector/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    21233 2024-05-13 13:11:27.000000 zoho_crm_connector-1.0.1/zoho_crm_connector/zoho_crm_api.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)     7744 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      327 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        9 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       19 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:09:43.769149 zoho_crm_connector-1.0.2/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1064 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.2/LICENCE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       19 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.2/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)     7865 2024-05-14 05:09:43.769149 zoho_crm_connector-1.0.2/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7309 2024-05-14 05:08:54.000000 zoho_crm_connector-1.0.2/README.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)       63 2024-05-14 05:09:43.769149 zoho_crm_connector-1.0.2/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1472 2024-05-14 05:08:17.000000 zoho_crm_connector-1.0.2/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:09:43.765149 zoho_crm_connector-1.0.2/zoho_crm_connector/
+-rw-rw-r--   0 tim       (1000) tim       (1000)       35 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.2/zoho_crm_connector/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21233 2024-05-13 13:11:27.000000 zoho_crm_connector-1.0.2/zoho_crm_connector/zoho_crm_api.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:09:43.769149 zoho_crm_connector-1.0.2/zoho_crm_connector.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)     7865 2024-05-14 05:09:43.000000 zoho_crm_connector-1.0.2/zoho_crm_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      327 2024-05-14 05:09:43.000000 zoho_crm_connector-1.0.2/zoho_crm_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-05-14 05:09:43.000000 zoho_crm_connector-1.0.2/zoho_crm_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        9 2024-05-14 05:09:43.000000 zoho_crm_connector-1.0.2/zoho_crm_connector.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       19 2024-05-14 05:09:43.000000 zoho_crm_connector-1.0.2/zoho_crm_connector.egg-info/top_level.txt
```

### Comparing `zoho_crm_connector-1.0.1/LICENCE.txt` & `zoho_crm_connector-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zoho_crm_connector-1.0.1/PKG-INFO` & `zoho_crm_connector-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zoho_crm_connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Zoho CRM connector
 Home-page: https://github.com/timrichardson/zoho_crm_package
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MIT
 Keywords: zoho crm
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: requests
 
 Zoho CRM Connector for Python
 ==================
@@ -168,19 +168,21 @@
     and also set a Zoho user id as the default user (ZOHOCRM_DEFAULT_USERID). This is an internal Zoho id value, not a user name.
 
 
 Uploading
 =========
 ```
 python3 setup.py sdist bdist_wheel
-python3 -m twine upload --skip-existing dist/*
+python3 -m twine upload --skip-existing dist/*python3 -m twine upload --skip-existing dist/*
 ```
 
 Changes
 ========
+v1.0.2 Metadata updates in the package, promote to Production/Stable
+
 v1.0.1 Fixed bug with get_users(): now all pages are returned, and the usertype filter works.
 
 v1.0.0 It works well enough to be v1
 
 v0.4.6. Add a message to Quota Exceeded exception
 
 v0.4.5. Raise Runtime exception if token refresh fails to return a valid token
```

### Comparing `zoho_crm_connector-1.0.1/README.md` & `zoho_crm_connector-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -150,19 +150,21 @@
     and also set a Zoho user id as the default user (ZOHOCRM_DEFAULT_USERID). This is an internal Zoho id value, not a user name.
 
 
 Uploading
 =========
 ```
 python3 setup.py sdist bdist_wheel
-python3 -m twine upload --skip-existing dist/*
+python3 -m twine upload --skip-existing dist/*python3 -m twine upload --skip-existing dist/*
 ```
 
 Changes
 ========
+v1.0.2 Metadata updates in the package, promote to Production/Stable
+
 v1.0.1 Fixed bug with get_users(): now all pages are returned, and the usertype filter works.
 
 v1.0.0 It works well enough to be v1
 
 v0.4.6. Add a message to Quota Exceeded exception
 
 v0.4.5. Raise Runtime exception if token refresh fails to return a valid token
```

### Comparing `zoho_crm_connector-1.0.1/setup.py` & `zoho_crm_connector-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 cmdclass = {'build_sphinx': BuildDoc}
 
 # https://pypi.org/classifiers/
 
 name = 'zoho_crm_connector'
 keywords = 'zoho crm'
-version = '1.0.1'
+version = '1.0.2'
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=name,
@@ -22,18 +22,18 @@
     packages=['zoho_crm_connector'],
     python_requires='>=3.6',
     install_requires=['requests',
                       ],
     setup_requires=["pytest-runner", ],
     tests_require=["pytest", ],
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
-        'Topic :: Text Processing :: Linguistic',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Internet :: WWW/HTTP',
     ],
     url='https://github.com/timrichardson/zoho_crm_package',
     license='MIT',
     author='Tim Richardson',
     author_email='tim@growthpath.com.au',
     description='Zoho CRM connector',
     long_description=long_description,
```

### Comparing `zoho_crm_connector-1.0.1/zoho_crm_connector/zoho_crm_api.py` & `zoho_crm_connector-1.0.2/zoho_crm_connector/zoho_crm_api.py`

 * *Files identical despite different names*

### Comparing `zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/PKG-INFO` & `zoho_crm_connector-1.0.2/zoho_crm_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zoho-crm-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Zoho CRM connector
 Home-page: https://github.com/timrichardson/zoho_crm_package
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MIT
 Keywords: zoho crm
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: requests
 
 Zoho CRM Connector for Python
 ==================
@@ -168,19 +168,21 @@
     and also set a Zoho user id as the default user (ZOHOCRM_DEFAULT_USERID). This is an internal Zoho id value, not a user name.
 
 
 Uploading
 =========
 ```
 python3 setup.py sdist bdist_wheel
-python3 -m twine upload --skip-existing dist/*
+python3 -m twine upload --skip-existing dist/*python3 -m twine upload --skip-existing dist/*
 ```
 
 Changes
 ========
+v1.0.2 Metadata updates in the package, promote to Production/Stable
+
 v1.0.1 Fixed bug with get_users(): now all pages are returned, and the usertype filter works.
 
 v1.0.0 It works well enough to be v1
 
 v0.4.6. Add a message to Quota Exceeded exception
 
 v0.4.5. Raise Runtime exception if token refresh fails to return a valid token
```

