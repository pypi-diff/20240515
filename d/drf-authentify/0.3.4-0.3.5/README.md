# Comparing `tmp/drf_authentify-0.3.4.tar.gz` & `tmp/drf_authentify-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_authentify-0.3.4.tar", last modified: Sat Apr 20 20:42:14 2024, max compression
+gzip compressed data, was "drf_authentify-0.3.5.tar", last modified: Wed May 15 06:43:46 2024, max compression
```

## Comparing `drf_authentify-0.3.4.tar` & `drf_authentify-0.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:42:14.562536 drf_authentify-0.3.4/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1501 2024-04-20 20:41:52.000000 drf_authentify-0.3.4/LICENSE
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       33 2024-04-20 20:41:52.000000 drf_authentify-0.3.4/MANIFEST.in
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8193 2024-04-20 20:42:14.562536 drf_authentify-0.3.4/PKG-INFO
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     4727 2024-04-20 20:41:53.000000 drf_authentify-0.3.4/README.md
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:42:14.554534 drf_authentify-0.3.4/drf_authentify/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/__init__.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1687 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/admin.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      159 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/apps.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1806 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/auth.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      185 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/choices.py
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:42:14.558535 drf_authentify-0.3.4/drf_authentify/migrations/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1193 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/migrations/0001_initial.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/migrations/__init__.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     2425 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/models.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      651 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/settings.py
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:42:14.558535 drf_authentify-0.3.4/drf_authentify/tests/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/tests/__init__.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/tests/test_auth.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     9566 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/tests/test_models.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     2731 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/tests/test_utils.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      208 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/urls.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      888 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/utils.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       63 2024-04-20 20:41:42.000000 drf_authentify-0.3.4/drf_authentify/views.py
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:42:14.558535 drf_authentify-0.3.4/drf_authentify.egg-info/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8193 2024-04-20 20:42:14.000000 drf_authentify-0.3.4/drf_authentify.egg-info/PKG-INFO
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      697 2024-04-20 20:42:14.000000 drf_authentify-0.3.4/drf_authentify.egg-info/SOURCES.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        1 2024-04-20 20:42:14.000000 drf_authentify-0.3.4/drf_authentify.egg-info/dependency_links.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       37 2024-04-20 20:42:14.000000 drf_authentify-0.3.4/drf_authentify.egg-info/requires.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       15 2024-04-20 20:42:14.000000 drf_authentify-0.3.4/drf_authentify.egg-info/top_level.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1793 2024-04-20 20:41:53.000000 drf_authentify-0.3.4/pyproject.toml
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       38 2024-04-20 20:42:14.562536 drf_authentify-0.3.4/setup.cfg
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:43:46.884263 drf_authentify-0.3.5/
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1501 2024-05-15 06:35:42.000000 drf_authentify-0.3.5/LICENSE
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       33 2024-05-15 06:35:42.000000 drf_authentify-0.3.5/MANIFEST.in
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8196 2024-05-15 06:43:46.880262 drf_authentify-0.3.5/PKG-INFO
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     4730 2024-05-15 06:35:42.000000 drf_authentify-0.3.5/README.md
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:43:46.876263 drf_authentify-0.3.5/drf_authentify/
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/__init__.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1687 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/admin.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      159 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/apps.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1755 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/auth.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      185 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/choices.py
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:43:46.880262 drf_authentify-0.3.5/drf_authentify/migrations/
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1193 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/migrations/0001_initial.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/migrations/__init__.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     2425 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/models.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      651 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/settings.py
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:43:46.880262 drf_authentify-0.3.5/drf_authentify/tests/
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/tests/__init__.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/tests/test_auth.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     9566 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/tests/test_models.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     2731 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/tests/test_utils.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      208 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/urls.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      888 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/utils.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:35:04.000000 drf_authentify-0.3.5/drf_authentify/views.py
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-05-15 06:43:46.880262 drf_authentify-0.3.5/drf_authentify.egg-info/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8196 2024-05-15 06:43:46.000000 drf_authentify-0.3.5/drf_authentify.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      697 2024-05-15 06:43:46.000000 drf_authentify-0.3.5/drf_authentify.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        1 2024-05-15 06:43:46.000000 drf_authentify-0.3.5/drf_authentify.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       37 2024-05-15 06:43:46.000000 drf_authentify-0.3.5/drf_authentify.egg-info/requires.txt
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       15 2024-05-15 06:43:46.000000 drf_authentify-0.3.5/drf_authentify.egg-info/top_level.txt
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1793 2024-05-15 06:35:42.000000 drf_authentify-0.3.5/pyproject.toml
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       38 2024-05-15 06:43:46.884263 drf_authentify-0.3.5/setup.cfg
```

### Comparing `drf_authentify-0.3.4/LICENSE` & `drf_authentify-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/PKG-INFO` & `drf_authentify-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-authentify
-Version: 0.3.4
+Version: 0.3.5
 Summary: A simple authentication module for django rest framework
 Author: Gabriel Idenyi
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Idenyi Gabriel
         
         Redistribution and use in source and binary forms, with or without
@@ -101,15 +101,15 @@
 Then add the `drf-authentify` to your project by including the app to your `INSTALLED_APPS`.
 
 The app should preferably go somewhere after your regular apps.
 
 ```python
 INSTALLED_APPS = (
     ...
-    'drf-authentify'
+    'drf_authentify'
 )
 ```
 
 `drf-authentify` adds a model to your admin section called AuthToken, with this you can view and manage all tokens created on your applications. We already have a nice setup for you on django admin section.
 
 Finally migrate all database entries.
 
@@ -120,17 +120,17 @@
 
 ## Global Configuration
 
 For a one type fits all case, you can globally alter the following settings, or leave the default as it is.
 
 ```python
 DRF_AUTHENTIFY = {
-    ALLOWED_HEADER_PREFIXES = ["bearer", "token"] # default
-    TOKEN_EXPIRATION = 3000 # default
-    COOKIE_KEY = "token" # default
+    "ALLOWED_HEADER_PREFIXES": ["bearer", "token"] # default
+    "TOKEN_EXPIRATION": 3000 # default
+    "COOKIE_KEY": "token" # default
 }
 ```
 
 ## Customizing Tokens
 
 - ALLOWED_HEADER_PREFIXES: Here you can provide a list of prefixes that are allowed for your authentication header. We will validate this when you apply our authentication scheme `drf_authentify.auth.TokenAuthentication` as shown below.
```

### Comparing `drf_authentify-0.3.4/README.md` & `drf_authentify-0.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 Then add the `drf-authentify` to your project by including the app to your `INSTALLED_APPS`.
 
 The app should preferably go somewhere after your regular apps.
 
 ```python
 INSTALLED_APPS = (
     ...
-    'drf-authentify'
+    'drf_authentify'
 )
 ```
 
 `drf-authentify` adds a model to your admin section called AuthToken, with this you can view and manage all tokens created on your applications. We already have a nice setup for you on django admin section.
 
 Finally migrate all database entries.
 
@@ -53,17 +53,17 @@
 
 ## Global Configuration
 
 For a one type fits all case, you can globally alter the following settings, or leave the default as it is.
 
 ```python
 DRF_AUTHENTIFY = {
-    ALLOWED_HEADER_PREFIXES = ["bearer", "token"] # default
-    TOKEN_EXPIRATION = 3000 # default
-    COOKIE_KEY = "token" # default
+    "ALLOWED_HEADER_PREFIXES": ["bearer", "token"] # default
+    "TOKEN_EXPIRATION": 3000 # default
+    "COOKIE_KEY": "token" # default
 }
 ```
 
 ## Customizing Tokens
 
 - ALLOWED_HEADER_PREFIXES: Here you can provide a list of prefixes that are allowed for your authentication header. We will validate this when you apply our authentication scheme `drf_authentify.auth.TokenAuthentication` as shown below.
```

### Comparing `drf_authentify-0.3.4/drf_authentify/admin.py` & `drf_authentify-0.3.5/drf_authentify/admin.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/drf_authentify/auth.py` & `drf_authentify-0.3.5/drf_authentify/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from django.utils.translation import gettext_lazy as _
 from rest_framework.exceptions import AuthenticationFailed
 from rest_framework.authentication import BaseAuthentication
 
 from drf_authentify.choices import AUTH
 from drf_authentify.models import AuthToken
 from drf_authentify.settings import authentify_settings
 
@@ -37,15 +36,15 @@
 class CookieAuthentication(BaseAuthentication):
     """Simple cookie based authentication."""
 
     def authenticate(self, request):
         if authentify_settings.COOKIE_KEY in request.COOKIES:
             token_str = request.COOKIES[authentify_settings.COOKIE_KEY]
             if token_str:
-                token = AuthToken.verify_token(token, AUTH.COOKIE)
+                token = AuthToken.verify_token(token_str, AUTH.COOKIE)
                 if token:
                     return (token.user, token)
             raise AuthenticationFailed()
         return None
 
     def authenticate_header(self, request):
         return "Set-Cookie: token=value"
```

### Comparing `drf_authentify-0.3.4/drf_authentify/migrations/0001_initial.py` & `drf_authentify-0.3.5/drf_authentify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/drf_authentify/models.py` & `drf_authentify-0.3.5/drf_authentify/models.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/drf_authentify/settings.py` & `drf_authentify-0.3.5/drf_authentify/settings.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/drf_authentify/tests/test_models.py` & `drf_authentify-0.3.5/drf_authentify/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/drf_authentify/tests/test_utils.py` & `drf_authentify-0.3.5/drf_authentify/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/drf_authentify/utils.py` & `drf_authentify-0.3.5/drf_authentify/utils.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/drf_authentify.egg-info/PKG-INFO` & `drf_authentify-0.3.5/drf_authentify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-authentify
-Version: 0.3.4
+Version: 0.3.5
 Summary: A simple authentication module for django rest framework
 Author: Gabriel Idenyi
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Idenyi Gabriel
         
         Redistribution and use in source and binary forms, with or without
@@ -101,15 +101,15 @@
 Then add the `drf-authentify` to your project by including the app to your `INSTALLED_APPS`.
 
 The app should preferably go somewhere after your regular apps.
 
 ```python
 INSTALLED_APPS = (
     ...
-    'drf-authentify'
+    'drf_authentify'
 )
 ```
 
 `drf-authentify` adds a model to your admin section called AuthToken, with this you can view and manage all tokens created on your applications. We already have a nice setup for you on django admin section.
 
 Finally migrate all database entries.
 
@@ -120,17 +120,17 @@
 
 ## Global Configuration
 
 For a one type fits all case, you can globally alter the following settings, or leave the default as it is.
 
 ```python
 DRF_AUTHENTIFY = {
-    ALLOWED_HEADER_PREFIXES = ["bearer", "token"] # default
-    TOKEN_EXPIRATION = 3000 # default
-    COOKIE_KEY = "token" # default
+    "ALLOWED_HEADER_PREFIXES": ["bearer", "token"] # default
+    "TOKEN_EXPIRATION": 3000 # default
+    "COOKIE_KEY": "token" # default
 }
 ```
 
 ## Customizing Tokens
 
 - ALLOWED_HEADER_PREFIXES: Here you can provide a list of prefixes that are allowed for your authentication header. We will validate this when you apply our authentication scheme `drf_authentify.auth.TokenAuthentication` as shown below.
```

### Comparing `drf_authentify-0.3.4/drf_authentify.egg-info/SOURCES.txt` & `drf_authentify-0.3.5/drf_authentify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.4/pyproject.toml` & `drf_authentify-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 40.8.0"]
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "drf-authentify"
-version = "0.3.4"
+version = "0.3.5"
 description = "A simple authentication module for django rest framework"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["django", "djangorestframework", "drf", "authentication"]
 authors = [
     {name = "Gabriel Idenyi"}
 ]
```

