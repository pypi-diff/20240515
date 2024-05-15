# Comparing `tmp/crudfastapi-0.0.2.tar.gz` & `tmp/crudfastapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crudfastapi-0.0.2.tar", max compression
+gzip compressed data, was "crudfastapi-0.0.3.tar", max compression
```

## Comparing `crudfastapi-0.0.2.tar` & `crudfastapi-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/crud/__init__.py
--rw-r--r--   0        0        0    71660 2024-05-14 03:11:28.107402 crudfastapi-0.0.2/CRUDFastAPI/crud/fast_crud.py
--rw-r--r--   0        0        0     6087 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/crud/helper.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/endpoint/__init__.py
--rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/endpoint/crud_router.py
--rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/endpoint/endpoint_creator.py
--rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/endpoint/helper.py
--rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/exceptions/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/exceptions/http_exceptions.py
--rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/paginated/__init__.py
--rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/paginated/helper.py
--rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/paginated/response.py
--rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/paginated/schemas.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/CRUDFastAPI/py.typed
--rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/LICENSE
--rw-r--r--   0        0        0     1498 2024-05-14 02:56:02.573204 crudfastapi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.2/README.md
--rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/crud/__init__.py
+-rw-r--r--   0        0        0    71690 2024-05-14 07:48:13.635983 crudfastapi-0.0.3/CRUDFastAPI/crud/fast_crud.py
+-rw-r--r--   0        0        0     6087 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/crud/helper.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/endpoint/__init__.py
+-rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/endpoint/crud_router.py
+-rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/endpoint/endpoint_creator.py
+-rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/endpoint/helper.py
+-rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/exceptions/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/paginated/__init__.py
+-rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/paginated/helper.py
+-rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/paginated/response.py
+-rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/paginated/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/py.typed
+-rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1498 2024-05-14 07:49:24.935201 crudfastapi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/README.md
+-rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.3/PKG-INFO
```

### Comparing `crudfastapi-0.0.2/CRUDFastAPI/crud/fast_crud.py` & `crudfastapi-0.0.3/CRUDFastAPI/crud/fast_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1291,26 +1291,28 @@
             )
         elif not joins_config and not join_model:
             raise ValueError("You need one of join_model or joins_config.")
 
         if (limit is not None and limit < 0) or offset < 0:
             raise ValueError("Limit and offset must be non-negative.")
 
+        if join_on is None:
+            join_on = _auto_detect_join_condition(self.model, join_model)
+
         primary_select = _extract_matching_columns_from_schema(
             model=self.model, schema=schema_to_select
         )
         stmt: Select = select(*primary_select)
 
         join_definitions = joins_config if joins_config else []
         if join_model:
             join_definitions.append(
                 JoinConfig(
                     model=join_model,
-                    join_on=join_on
-                    or _auto_detect_join_condition(self.model, join_model),
+                    join_on=join_on,
                     join_prefix=join_prefix,
                     schema_to_select=join_schema_to_select,
                     join_type=join_type,
                     alias=alias,
                     filters=join_filters,
                 )
             )
```

### Comparing `crudfastapi-0.0.2/CRUDFastAPI/crud/helper.py` & `crudfastapi-0.0.3/CRUDFastAPI/crud/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/CRUDFastAPI/endpoint/crud_router.py` & `crudfastapi-0.0.3/CRUDFastAPI/endpoint/crud_router.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/CRUDFastAPI/endpoint/endpoint_creator.py` & `crudfastapi-0.0.3/CRUDFastAPI/endpoint/endpoint_creator.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/CRUDFastAPI/endpoint/helper.py` & `crudfastapi-0.0.3/CRUDFastAPI/endpoint/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/CRUDFastAPI/exceptions/http_exceptions.py` & `crudfastapi-0.0.3/CRUDFastAPI/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/CRUDFastAPI/paginated/helper.py` & `crudfastapi-0.0.3/CRUDFastAPI/paginated/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/CRUDFastAPI/paginated/response.py` & `crudfastapi-0.0.3/CRUDFastAPI/paginated/response.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/LICENSE` & `crudfastapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/pyproject.toml` & `crudfastapi-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CRUDFastAPI"
-version = "0.0.2"
+version = "0.0.3"
 description = "CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities."
 authors = ["Mithun Thomas <mithunthomas003@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mithun2003/CRUDFastAPI"
 include = ["LICENSE"]
```

### Comparing `crudfastapi-0.0.2/README.md` & `crudfastapi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.2/PKG-INFO` & `crudfastapi-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRUDFastAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities.
 Home-page: https://github.com/mithun2003/CRUDFastAPI
 License: MIT
 Keywords: fastapi,crud,async,sqlalchemy,pydantic,fastcrud,crudfastapi
 Author: Mithun Thomas
 Author-email: mithunthomas003@gmail.com
 Requires-Python: >=3.9,<4.0
```

