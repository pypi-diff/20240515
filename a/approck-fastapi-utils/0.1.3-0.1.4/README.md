# Comparing `tmp/approck_fastapi_utils-0.1.3.tar.gz` & `tmp/approck_fastapi_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_fastapi_utils-0.1.3.tar", max compression
+gzip compressed data, was "approck_fastapi_utils-0.1.4.tar", max compression
```

## Comparing `approck_fastapi_utils-0.1.3.tar` & `approck_fastapi_utils-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        0 2024-03-03 22:23:31.626673 approck_fastapi_utils-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-03-03 22:23:31.627673 approck_fastapi_utils-0.1.3/approck_fastapi_utils/__init__.py
--rw-r--r--   0        0        0      271 2024-03-03 22:23:31.603672 approck_fastapi_utils-0.1.3/approck_fastapi_utils/auth.py
--rw-r--r--   0        0        0     1130 2024-03-03 22:23:31.603672 approck_fastapi_utils-0.1.3/approck_fastapi_utils/exception_handlers.py
--rw-r--r--   0        0        0      180 2024-03-03 22:23:31.604672 approck_fastapi_utils-0.1.3/approck_fastapi_utils/exceptions.py
--rw-r--r--   0        0        0      325 2024-03-03 22:23:31.604672 approck_fastapi_utils-0.1.3/approck_fastapi_utils/jwt.py
--rw-r--r--   0        0        0      212 2024-03-03 22:23:31.604672 approck_fastapi_utils-0.1.3/approck_fastapi_utils/response.py
--rw-r--r--   0        0        0     1991 2024-03-03 22:23:31.604672 approck_fastapi_utils-0.1.3/approck_fastapi_utils/responses.py
--rw-r--r--   0        0        0        0 2024-03-03 22:23:31.627673 approck_fastapi_utils-0.1.3/approck_fastapi_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      637 2024-03-03 22:23:31.604672 approck_fastapi_utils-0.1.3/approck_fastapi_utils/sqlalchemy/exception_handlers.py
--rw-r--r--   0        0        0      407 2024-03-03 22:23:31.604672 approck_fastapi_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 approck_fastapi_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-15 11:09:37.638882 approck_fastapi_utils-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 11:09:37.639883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/__init__.py
+-rw-r--r--   0        0        0      271 2024-05-15 11:09:37.607883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/auth.py
+-rw-r--r--   0        0        0     1130 2024-05-15 11:09:37.607883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/exception_handlers.py
+-rw-r--r--   0        0        0      180 2024-05-15 11:09:37.608883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/exceptions.py
+-rw-r--r--   0        0        0      325 2024-05-15 11:09:37.608883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/jwt.py
+-rw-r--r--   0        0        0      212 2024-05-15 11:09:37.608883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/response.py
+-rw-r--r--   0        0        0     1991 2024-05-15 11:09:37.608883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/responses.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:09:37.639883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-15 11:09:37.608883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/sqlalchemy/exception_handlers.py
+-rw-r--r--   0        0        0     1350 2024-05-15 11:09:37.608883 approck_fastapi_utils-0.1.4/approck_fastapi_utils/types.py
+-rw-r--r--   0        0        0      426 2024-05-15 11:09:37.609883 approck_fastapi_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 approck_fastapi_utils-0.1.4/PKG-INFO
```

### Comparing `approck_fastapi_utils-0.1.3/approck_fastapi_utils/exception_handlers.py` & `approck_fastapi_utils-0.1.4/approck_fastapi_utils/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `approck_fastapi_utils-0.1.3/approck_fastapi_utils/responses.py` & `approck_fastapi_utils-0.1.4/approck_fastapi_utils/responses.py`

 * *Files identical despite different names*

### Comparing `approck_fastapi_utils-0.1.3/approck_fastapi_utils/sqlalchemy/exception_handlers.py` & `approck_fastapi_utils-0.1.4/approck_fastapi_utils/sqlalchemy/exception_handlers.py`

 * *Files identical despite different names*

