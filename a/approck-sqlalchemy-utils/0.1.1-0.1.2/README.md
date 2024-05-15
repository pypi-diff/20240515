# Comparing `tmp/approck_sqlalchemy_utils-0.1.1.tar.gz` & `tmp/approck_sqlalchemy_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_sqlalchemy_utils-0.1.1.tar", max compression
+gzip compressed data, was "approck_sqlalchemy_utils-0.1.2.tar", max compression
```

## Comparing `approck_sqlalchemy_utils-0.1.1.tar` & `approck_sqlalchemy_utils-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0        0 2024-03-09 12:03:08.160798 approck_sqlalchemy_utils-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-09 12:03:08.161798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-09 12:03:08.161798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/alembic/__init__.py
--rw-r--r--   0        0        0      621 2024-03-09 12:03:08.136798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/alembic/humanreadable.py
--rw-r--r--   0        0        0       48 2024-03-09 12:03:08.136798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-09 12:03:08.161798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/mixins/__init__.py
--rw-r--r--   0        0        0      434 2024-03-09 12:03:08.137798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/mixins/auto_now.py
--rw-r--r--   0        0        0       49 2024-03-09 12:03:08.137798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/mocks.py
--rw-r--r--   0        0        0      577 2024-03-09 12:03:08.137798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/model.py
--rw-r--r--   0        0        0     1561 2024-03-09 12:03:08.137798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/session.py
--rw-r--r--   0        0        0        0 2024-03-09 12:03:08.161798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/__init__.py
--rw-r--r--   0        0        0        0 2024-03-09 12:03:08.161798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/encrypted/__init__.py
--rw-r--r--   0        0        0    15877 2024-03-09 12:03:08.137798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/encrypted/encrypted_type.py
--rw-r--r--   0        0        0     4483 2024-03-09 12:03:08.137798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/encrypted/padding.py
--rw-r--r--   0        0        0     2123 2024-03-09 12:03:08.137798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/json.py
--rw-r--r--   0        0        0      192 2024-03-09 12:03:08.137798 approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/scalar_coercible.py
--rw-r--r--   0        0        0      779 2024-03-09 12:03:08.138798 approck_sqlalchemy_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 approck_sqlalchemy_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-15 10:35:46.937837 approck_sqlalchemy_utils-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 10:35:46.938837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:35:46.938837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/alembic/__init__.py
+-rw-r--r--   0        0        0      621 2024-05-15 10:35:46.902837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/alembic/humanreadable.py
+-rw-r--r--   0        0        0       48 2024-05-15 10:35:46.902837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:35:46.938837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/mixins/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-15 10:35:46.903837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/mixins/auto_now.py
+-rw-r--r--   0        0        0       49 2024-05-15 10:35:46.903837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/mocks.py
+-rw-r--r--   0        0        0      577 2024-05-15 10:35:46.903837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/model.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:35:46.938837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/parsers/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-15 10:35:46.903837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/parsers/order_by.py
+-rw-r--r--   0        0        0     1561 2024-05-15 10:35:46.903837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/session.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:35:46.938837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:35:46.938837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/encrypted/__init__.py
+-rw-r--r--   0        0        0    15877 2024-05-15 10:35:46.904837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/encrypted/encrypted_type.py
+-rw-r--r--   0        0        0     4483 2024-05-15 10:35:46.904837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/encrypted/padding.py
+-rw-r--r--   0        0        0     2123 2024-05-15 10:35:46.904837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/json.py
+-rw-r--r--   0        0        0      192 2024-05-15 10:35:46.904837 approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/scalar_coercible.py
+-rw-r--r--   0        0        0      707 2024-05-15 10:35:46.905837 approck_sqlalchemy_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 approck_sqlalchemy_utils-0.1.2/PKG-INFO
```

### Comparing `approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/alembic/humanreadable.py` & `approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/alembic/humanreadable.py`

 * *Files identical despite different names*

### Comparing `approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/model.py` & `approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/model.py`

 * *Files identical despite different names*

### Comparing `approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/session.py` & `approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/session.py`

 * *Files identical despite different names*

### Comparing `approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/encrypted/encrypted_type.py` & `approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/encrypted/encrypted_type.py`

 * *Files identical despite different names*

### Comparing `approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/encrypted/padding.py` & `approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/encrypted/padding.py`

 * *Files identical despite different names*

### Comparing `approck_sqlalchemy_utils-0.1.1/approck_sqlalchemy_utils/types/json.py` & `approck_sqlalchemy_utils-0.1.2/approck_sqlalchemy_utils/types/json.py`

 * *Files identical despite different names*

### Comparing `approck_sqlalchemy_utils-0.1.1/pyproject.toml` & `approck_sqlalchemy_utils-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [tool.poetry]
 name = "approck-sqlalchemy-utils"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Aleksey Dalekin <adalekin@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 alembic = "^1.13.1"
 asyncpg = { version = "^0.29.0", optional = true }
 psycopg2-binary = { version = "^2.9.3", optional = true }
 python = "^3.10"
 SQLAlchemy = { extras = ["asyncio", "mypy"], version = "^2.0.27" }
-cryptography = "^42.0.5"
+cryptography = "^42.0.7"
 
 [tool.poetry.extras]
 postgres = ["psycopg2-binary", "asyncpg"]
 cryptography = ["cryptography"]
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.1.1"
-pre-commit = "^3.1.0"
-pytest = "^7.2.2"
-pytest-asyncio = "^0.21.0"
-pytest-dotenv = "^0.5.2"
-wemake-python-styleguide = "^0.17.0"
+mypy = "^1.10.0"
+pre-commit = "^3.7.1"
+pytest = "^8.2.0"
+ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `approck_sqlalchemy_utils-0.1.1/PKG-INFO` & `approck_sqlalchemy_utils-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: approck-sqlalchemy-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Aleksey Dalekin
 Author-email: adalekin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cryptography
 Provides-Extra: postgres
 Requires-Dist: SQLAlchemy[asyncio,mypy] (>=2.0.27,<3.0.0)
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0) ; extra == "postgres"
-Requires-Dist: cryptography (>=42.0.5,<43.0.0) ; extra == "cryptography"
+Requires-Dist: cryptography (>=42.0.7,<43.0.0) ; extra == "cryptography"
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0) ; extra == "postgres"
 Description-Content-Type: text/markdown
```

