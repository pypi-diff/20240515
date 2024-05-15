# Comparing `tmp/crudfastapi-0.0.3.tar.gz` & `tmp/crudfastapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crudfastapi-0.0.3.tar", max compression
+gzip compressed data, was "crudfastapi-0.0.4.tar", max compression
```

## Comparing `crudfastapi-0.0.3.tar` & `crudfastapi-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/crud/__init__.py
--rw-r--r--   0        0        0    71690 2024-05-14 07:48:13.635983 crudfastapi-0.0.3/CRUDFastAPI/crud/fast_crud.py
--rw-r--r--   0        0        0     6087 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/crud/helper.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/endpoint/__init__.py
--rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/endpoint/crud_router.py
--rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/endpoint/endpoint_creator.py
--rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/endpoint/helper.py
--rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/exceptions/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/exceptions/http_exceptions.py
--rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/paginated/__init__.py
--rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/paginated/helper.py
--rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/paginated/response.py
--rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/paginated/schemas.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/CRUDFastAPI/py.typed
--rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/LICENSE
--rw-r--r--   0        0        0     1498 2024-05-14 07:49:24.935201 crudfastapi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.3/README.md
--rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/crud/__init__.py
+-rw-r--r--   0        0        0    72803 2024-05-15 05:36:35.751891 crudfastapi-0.0.4/CRUDFastAPI/crud/fast_crud.py
+-rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.4/CRUDFastAPI/crud/helper.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/endpoint/__init__.py
+-rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/endpoint/crud_router.py
+-rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/endpoint/endpoint_creator.py
+-rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/endpoint/helper.py
+-rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/exceptions/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/paginated/__init__.py
+-rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/paginated/helper.py
+-rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/paginated/response.py
+-rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/paginated/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/py.typed
+-rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1498 2024-05-15 05:37:08.847450 crudfastapi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/README.md
+-rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.4/PKG-INFO
```

### Comparing `crudfastapi-0.0.3/CRUDFastAPI/crud/fast_crud.py` & `crudfastapi-0.0.4/CRUDFastAPI/crud/fast_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Generic, TypeVar, Union, Optional
 from datetime import datetime, timezone
 
 from pydantic import BaseModel, ValidationError
-from sqlalchemy import select, update, delete, func, inspect, asc, desc
+from sqlalchemy import select, update, delete, func, inspect, asc, desc, or_
 from sqlalchemy.exc import ArgumentError, MultipleResultsFound, NoResultFound
 from sqlalchemy.sql import Join
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.engine.row import Row
 from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy.orm.util import AliasedClass
 from sqlalchemy.sql.elements import BinaryExpression
@@ -209,15 +209,18 @@
     ) -> None:
         self.model = model
         self.is_deleted_column = is_deleted_column
         self.deleted_at_column = deleted_at_column
         self.updated_at_column = updated_at_column
 
     def _parse_filters(
-        self, model: Optional[Union[type[ModelType], AliasedClass]] = None, **kwargs
+        self,
+        model: Optional[Union[type[ModelType], AliasedClass]] = None,
+        or_filter: bool = False,
+        **kwargs,
     ) -> list[BinaryExpression]:
         model = model or self.model
         filters = []
 
         for key, value in kwargs.items():
             if "__" in key:
                 field_name, op = key.rsplit("__", 1)
@@ -231,15 +234,18 @@
                 else:
                     raise ValueError(f"Unsupported filter operation: {op}")
             else:
                 column = getattr(model, key, None)
                 if column is not None:
                     filters.append(column == value)
 
-        return filters
+        if or_filter:
+            return [or_(*filters)]
+        else:
+            return filters
 
     def _apply_sorting(
         self,
         stmt: Select,
         sort_columns: Union[str, list[str]],
         sort_orders: Optional[Union[str, list[str]]] = None,
     ) -> Select:
@@ -321,40 +327,44 @@
         """
         Applies joins to the given SQL statement based on a list of JoinConfig objects.
 
         Args:
             stmt: The initial SQL statement.
             joins_config: Configurations for all joins.
             use_temporary_prefix: Whether to use or not an aditional prefix for joins. Default False.
-
+            or_filter: Whether to filter based on and/or. Default False so filter based on and
         Returns:
             Select: The modified SQL statement with joins applied.
         """
+        conditions = []
         for join in joins_config:
             model = join.alias or join.model
             join_select = _extract_matching_columns_from_schema(
                 model,
                 join.schema_to_select,
                 join.join_prefix,
                 join.alias,
                 use_temporary_prefix,
             )
             joined_model_filters = self._parse_filters(
-                model=model, **(join.filters or {})
+                model=model, **(join.filters or {}), or_filter=join.join_or_filter
             )
 
             if join.join_type == "left":
                 stmt = stmt.outerjoin(model, join.join_on).add_columns(*join_select)
             elif join.join_type == "inner":
                 stmt = stmt.join(model, join.join_on).add_columns(*join_select)
             else:
                 raise ValueError(f"Unsupported join type: {join.join_type}.")
             if joined_model_filters:
-                stmt = stmt.filter(*joined_model_filters)
-
+                conditions.append(
+                    or_(*joined_model_filters)
+                ) if join.join_or_filter else conditions.append(joined_model_filters)
+        if conditions:
+            stmt = stmt.filter(*conditions)
         return stmt
 
     async def create(
         self, db: AsyncSession, object: CreateSchemaType, commit: bool = True
     ) -> ModelType:
         """
         Create a new record in the database.
@@ -556,14 +566,15 @@
         result = await db.execute(stmt)
         return result.first() is not None
 
     async def count(
         self,
         db: AsyncSession,
         joins_config: Optional[list[JoinConfig]] = None,
+        join_or_filter: bool = False,
         **kwargs: Any,
     ) -> int:
         """
         Counts records that match specified filters, supporting advanced filtering through comparison operators:
             '__gt' (greater than),
             '__lt' (less than),
             '__gte' (greater than or equal to),
@@ -572,14 +583,15 @@
             '__not_in' (not included in [tuple, list or set]),
             '__startswith' (start with)
         Can also count records based on a configuration of joins, useful for complex queries involving relationships.
 
         Args:
             db: The database session to use for the operation.
             joins_config: Optional configuration for applying joins in the count query.
+            join_or_filter: Whether to filter based on and/or. Default False so filter based on and
             **kwargs: Filters to apply for the count, including field names for equality checks or with comparison operators for advanced queries.
 
         Returns:
             The total number of records matching the filter conditions.
 
         Examples:
             Count users by ID:
@@ -628,15 +640,15 @@
                     join_type="inner",
                     filters={'name': 'Jane Doe'}
                 )
             ]
             count = await crud.count(db, joins_config=joins_config)
             ```
         """
-        primary_filters = self._parse_filters(**kwargs)
+        primary_filters = self._parse_filters(or_filter=join_or_filter, **kwargs)
 
         if joins_config is not None:
             primary_keys = [p.name for p in _get_primary_keys(self.model)]
             if not any(primary_keys):  # pragma: no cover
                 raise ValueError(
                     f"The model '{self.model.__name__}' does not have a primary key defined, which is required for counting with joins."
                 )
@@ -644,15 +656,17 @@
                 getattr(self.model, pk).label(f"distinct_{pk}") for pk in primary_keys
             ]
             base_query = select(*to_select)
 
             for join in joins_config:
                 join_model = join.alias or join.model
                 join_filters = (
-                    self._parse_filters(model=join_model, **join.filters)
+                    self._parse_filters(
+                        model=join_model, or_filter=join.join_or_filter, **join.filters
+                    )
                     if join.filters
                     else []
                 )
 
                 if join.join_type == "inner":
                     base_query = base_query.join(join_model, join.join_on)
                 else:
@@ -661,20 +675,22 @@
                 if join_filters:
                     base_query = base_query.where(*join_filters)
 
             if primary_filters:
                 base_query = base_query.where(*primary_filters)
 
             subquery = base_query.subquery()
+            print(base_query, subquery)
             count_query = select(func.count()).select_from(subquery)
         else:
             count_query = select(func.count()).select_from(self.model)
             if primary_filters:
                 count_query = count_query.where(*primary_filters)
 
+        print(count_query)
         total_count: Optional[int] = await db.scalar(count_query)
         if total_count is None:
             raise ValueError("Could not find the count.")
 
         return total_count
 
     async def get_multi(
@@ -1037,14 +1053,15 @@
         join_model: Optional[type[ModelType]] = None,
         join_on: Optional[Any] = None,
         join_prefix: Optional[str] = None,
         join_schema_to_select: Optional[type[BaseModel]] = None,
         join_type: str = "left",
         alias: Optional[AliasedClass[Any]] = None,
         join_filters: Optional[dict] = None,
+        join_or_filter: bool = False,
         nest_joins: bool = False,
         offset: int = 0,
         limit: Optional[int] = 100,
         sort_columns: Optional[Union[str, list[str]]] = None,
         sort_orders: Optional[Union[str, list[str]]] = None,
         return_as_model: bool = False,
         joins_config: Optional[list[JoinConfig]] = None,
@@ -1069,14 +1086,15 @@
             join_model: The model to join with.
             join_on: SQLAlchemy Join object for specifying the ON clause of the join. If None, the join condition is auto-detected based on foreign keys.
             join_prefix: Optional prefix to be added to all columns of the joined model. If None, no prefix is added.
             join_schema_to_select: Pydantic schema for selecting specific columns from the joined model.
             join_type: Specifies the type of join operation to perform. Can be "left" for a left outer join or "inner" for an inner join.
             alias: An instance of `AliasedClass` for the join model, useful for self-joins or multiple joins on the same model. Result of `aliased(join_model)`.
             join_filters: Filters applied to the joined model, specified as a dictionary mapping column names to their expected values.
+            join_or_filter: A boolean field indicating whether the join is based on and/or. Default False which means join basedon and
             nest_joins: If True, nested data structures will be returned where joined model data are nested under the join_prefix as a dictionary.
             offset: The offset (number of records to skip) for pagination.
             limit: Maximum number of records to fetch in one call. Use `None` for "no limit", fetching all matching rows. Note that in order to use `limit=None`, you'll have to provide a custom endpoint to facilitate it, which you should only do if you really seriously want to allow the user to get all the data at once.
             sort_columns: A single column name or a list of column names on which to apply sorting.
             sort_orders: A single sort order ('asc' or 'desc') or a list of sort orders corresponding to the columns in sort_columns. If not provided, defaults to 'asc' for each column.
             return_as_model: If True, converts the fetched data to Pydantic models based on schema_to_select. Defaults to False.
             joins_config: List of JoinConfig instances for specifying multiple joins. Each instance defines a model to join with, join condition, optional prefix for column names, schema for selecting specific columns, and join type.
@@ -1290,15 +1308,14 @@
                 "Cannot use both single join parameters and joins_config simultaneously."
             )
         elif not joins_config and not join_model:
             raise ValueError("You need one of join_model or joins_config.")
 
         if (limit is not None and limit < 0) or offset < 0:
             raise ValueError("Limit and offset must be non-negative.")
-
         if join_on is None:
             join_on = _auto_detect_join_condition(self.model, join_model)
 
         primary_select = _extract_matching_columns_from_schema(
             model=self.model, schema=schema_to_select
         )
         stmt: Select = select(*primary_select)
@@ -1310,33 +1327,33 @@
                     model=join_model,
                     join_on=join_on,
                     join_prefix=join_prefix,
                     schema_to_select=join_schema_to_select,
                     join_type=join_type,
                     alias=alias,
                     filters=join_filters,
+                    join_or_filter=join_or_filter,
                 )
             )
 
         stmt = self._prepare_and_apply_joins(
             stmt=stmt, joins_config=join_definitions, use_temporary_prefix=nest_joins
         )
 
-        primary_filters = self._parse_filters(**kwargs)
+        primary_filters = self._parse_filters(or_filter=join_or_filter, **kwargs)
         if primary_filters:
             stmt = stmt.filter(*primary_filters)
 
         if sort_columns:
             stmt = self._apply_sorting(stmt, sort_columns, sort_orders)
 
         if offset:
             stmt = stmt.offset(offset)
         if limit is not None:
             stmt = stmt.limit(limit)
-
         result = await db.execute(stmt)
         data: list[Union[dict, BaseModel]] = []
         for row in result.mappings().all():
             row_dict = dict(row)
 
             if nest_joins:
                 row_dict = _nest_join_data(row_dict, join_definitions)
@@ -1356,18 +1373,20 @@
             else:
                 data.append(row_dict)
 
         response: dict[str, Any] = {"data": data}
 
         if return_total_count:
             total_count: int = await self.count(
-                db=db, joins_config=joins_config, **kwargs
+                db=db,
+                joins_config=join_definitions,
+                join_or_filter=join_or_filter,
+                **kwargs,
             )
             response["total_count"] = total_count
-
         return response
 
     async def get_multi_by_cursor(
         self,
         db: AsyncSession,
         cursor: Any = None,
         limit: int = 100,
```

### Comparing `crudfastapi-0.0.3/CRUDFastAPI/crud/helper.py` & `crudfastapi-0.0.4/CRUDFastAPI/crud/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     model: Any
     join_on: Any
     join_prefix: Optional[str] = None
     schema_to_select: Optional[type[BaseModel]] = None
     join_type: str = "left"
     alias: Optional[AliasedClass] = None
     filters: Optional[dict] = None
+    join_or_filter: bool = False
 
 
 def _extract_matching_columns_from_schema(
     model: Union[type[DeclarativeBase], AliasedClass],
     schema: Optional[type[BaseModel]],
     prefix: Optional[str] = None,
     alias: Optional[AliasedClass] = None,
```

### Comparing `crudfastapi-0.0.3/CRUDFastAPI/endpoint/crud_router.py` & `crudfastapi-0.0.4/CRUDFastAPI/endpoint/crud_router.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.3/CRUDFastAPI/endpoint/endpoint_creator.py` & `crudfastapi-0.0.4/CRUDFastAPI/endpoint/endpoint_creator.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.3/CRUDFastAPI/endpoint/helper.py` & `crudfastapi-0.0.4/CRUDFastAPI/endpoint/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.3/CRUDFastAPI/exceptions/http_exceptions.py` & `crudfastapi-0.0.4/CRUDFastAPI/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.3/CRUDFastAPI/paginated/helper.py` & `crudfastapi-0.0.4/CRUDFastAPI/paginated/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.3/CRUDFastAPI/paginated/response.py` & `crudfastapi-0.0.4/CRUDFastAPI/paginated/response.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.3/LICENSE` & `crudfastapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.3/pyproject.toml` & `crudfastapi-0.0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CRUDFastAPI"
-version = "0.0.3"
+version = "0.0.4"
 description = "CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities."
 authors = ["Mithun Thomas <mithunthomas003@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mithun2003/CRUDFastAPI"
 include = ["LICENSE"]
```

### Comparing `crudfastapi-0.0.3/README.md` & `crudfastapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.3/PKG-INFO` & `crudfastapi-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRUDFastAPI
-Version: 0.0.3
+Version: 0.0.4
 Summary: CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities.
 Home-page: https://github.com/mithun2003/CRUDFastAPI
 License: MIT
 Keywords: fastapi,crud,async,sqlalchemy,pydantic,fastcrud,crudfastapi
 Author: Mithun Thomas
 Author-email: mithunthomas003@gmail.com
 Requires-Python: >=3.9,<4.0
```

