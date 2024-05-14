# Comparing `tmp/database_mysql_local-0.0.302.tar.gz` & `tmp/database_mysql_local-0.0.303.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.302.tar", last modified: Tue May 14 09:39:57 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.303.tar", last modified: Tue May 14 23:00:48 2024, max compression
```

## Comparing `database_mysql_local-0.0.302.tar` & `database_mysql_local-0.0.303.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:39:57.313394 database_mysql_local-0.0.302/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 09:39:57.313394 database_mysql_local-0.0.302/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:39:57.309394 database_mysql_local-0.0.302/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:39:57.313394 database_mysql_local-0.0.302/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51545 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31055 2024-05-14 09:39:28.000000 database_mysql_local-0.0.302/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-14 09:39:25.000000 database_mysql_local-0.0.302/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-14 09:39:03.000000 database_mysql_local-0.0.302/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:39:57.313394 database_mysql_local-0.0.302/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 09:39:57.000000 database_mysql_local-0.0.302/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-14 09:39:57.000000 database_mysql_local-0.0.302/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:39:57.000000 database_mysql_local-0.0.302/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 09:39:57.000000 database_mysql_local-0.0.302/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 09:39:57.000000 database_mysql_local-0.0.302/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 09:39:28.000000 database_mysql_local-0.0.302/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:39:57.313394 database_mysql_local-0.0.302/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-14 09:39:28.000000 database_mysql_local-0.0.302/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:00:48.590732 database_mysql_local-0.0.303/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 23:00:48.590732 database_mysql_local-0.0.303/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:00:48.582732 database_mysql_local-0.0.303/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:00:48.590732 database_mysql_local-0.0.303/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-14 23:00:19.000000 database_mysql_local-0.0.303/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52802 2024-05-14 23:00:19.000000 database_mysql_local-0.0.303/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31055 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-14 23:00:15.000000 database_mysql_local-0.0.303/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:00:48.590732 database_mysql_local-0.0.303/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 23:00:48.000000 database_mysql_local-0.0.303/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-14 23:00:48.000000 database_mysql_local-0.0.303/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 23:00:48.000000 database_mysql_local-0.0.303/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 23:00:48.000000 database_mysql_local-0.0.303/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 23:00:48.000000 database_mysql_local-0.0.303/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 22:59:53.000000 database_mysql_local-0.0.303/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:00:48.590732 database_mysql_local-0.0.303/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-14 23:00:19.000000 database_mysql_local-0.0.303/setup.py
```

### Comparing `database_mysql_local-0.0.302/PKG-INFO` & `database_mysql_local-0.0.303/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.302
+Version: 0.0.303
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.302/README.md` & `database_mysql_local-0.0.303/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.303/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.303/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.303/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,15 @@
             data_dict=data_dict, add_created_user_id=True, schema_name=schema_name, table_name=table_name)
 
         columns, values, data_dict = process_insert_data_dict(data_dict=data_dict)
         # We removed the IGNORE from the SQL Statement as we want to return the id of the existing row
         insert_query = "INSERT " + \
                        f"INTO `{schema_name}`.`{table_name}` ({columns}) " \
                        f"VALUES ({values});"
-        # Log query without parameters
-        values_str = ', '.join(f"'{value}'" for value in data_dict.values())
-        insert_query_without_parameters = f"INSERT INTO `{schema_name}`.`{table_name}` ({columns}) VALUES ({values_str});"
-        self.logger.info("GenericCRUD.insert",
-                         object={"insert_query_without_parameters": insert_query_without_parameters})
+
         try:
             self.cursor.execute(insert_query, tuple(data_dict.values()))
             if commit_changes:
                 self.connection.commit()
             inserted_id = self.cursor.lastrowid()
         except mysql.connector.errors.IntegrityError as exception:
             if ignore_duplicate:
@@ -110,14 +106,47 @@
                 inserted_id = self._get_existing_duplicate_id(schema_name, table_name, exception)
             else:
                 raise exception
         finally:
             self.logger.debug(object=locals())
         return inserted_id
 
+    def insert_many(self, *, schema_name: str = None, table_name: str = None, data_dict: dict[str, list or tuple],
+                    commit_changes: bool = True) -> None:
+        """Inserts multiple rows into the table.
+        data_dict should be in the following format: {col1: [val1, val2], col2: [val3, val4], ...}
+        """
+        # TODO: support another format: [{col1: val1, col2: val2}, {col1: val3, col2: val4}]
+
+        schema_name = schema_name or self.default_schema_name
+        table_name = table_name or self.default_table_name
+
+        self._validate_args(args=locals())
+        # TODO: I am not sure we can use process_insert_data_dict here
+
+        len_rows = len(next(v for v in data_dict.values()))
+        data_dict = self.__add_create_updated_user_profile_ids(
+            data_dict=data_dict, add_created_user_id=True, schema_name=schema_name, table_name=table_name)
+        # Fix values from __add_create_updated_user_profile_ids
+        for k, v in data_dict.items():
+            if not isinstance(v, list) and not isinstance(v, tuple):
+                data_dict[k] = [v] * len_rows
+
+        columns = ", ".join(f"`{key}`" for key in data_dict)
+        values = ", ".join(["%s"] * len(data_dict))
+        sql_statement = f"""
+        INSERT INTO `{schema_name}`.`{table_name}` ({columns})
+        VALUES ({values});
+        """
+        sql_parameters = list(zip(*data_dict.values()))
+
+        self.cursor.executemany(sql_statement=sql_statement, sql_parameters=sql_parameters)
+        if commit_changes:
+            self.connection.commit()
+
     def upsert(self, *, schema_name: str = None, table_name: str = None, view_table_name: str = None,
                data_dict: dict = None, data_json: dict = None,
                data_dict_compare: dict = None, data_json_compare: dict = None,
                order_by: str = None, compare_with_or: bool = False) -> Optional[int]:
         """Inserts a new row into the table, or updates an existing row if a row with the
           same values as data_dict_compare exists,
           and returns the id of the new row or None if an error occurred."""
@@ -210,18 +239,18 @@
     def update_by_id(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> None:
         if datetime.now() > datetime(2024, 5, 20):
             self.logger.warning("GenericCRUD.update_by_id is deprecated, use update_by_column_and_value instead.")
         return self.update_by_column_and_value(schema_name=schema_name, table_name=table_name,
-                                          column_name=column_name, column_value=column_value,
-                                          id_column_name=id_column_name, id_column_value=id_column_value,
-                                          data_dict=data_dict, data_json=data_json,
-                                          limit=limit, order_by=order_by, commit_changes=commit_changes)
+                                               column_name=column_name, column_value=column_value,
+                                               id_column_name=id_column_name, id_column_value=id_column_value,
+                                               data_dict=data_dict, data_json=data_json,
+                                               limit=limit, order_by=order_by, commit_changes=commit_changes)
 
     def update_by_column_and_value(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> None:
         """Updates data in the table by ID."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
@@ -274,20 +303,20 @@
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
                      column_name: str = None, column_value: Any = None,
                      id_column_name: str = None, id_column_value: Any = None) -> None:
         if datetime.now() > datetime(2024, 5, 20):
             self.logger.warning("GenericCRUD.delete_by_id is deprecated, use delete_by_column_and_value instead.")
         return self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
-                                          column_name=column_name, column_value=column_value,
-                                          id_column_name=id_column_name, id_column_value=id_column_value)
+                                               column_name=column_name, column_value=column_value,
+                                               id_column_name=id_column_name, id_column_value=id_column_value)
 
     def delete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
-                              column_name: str = None, column_value: Any = None,
-                              id_column_name: str = None, id_column_value: Any = None) -> None:
+                                   column_name: str = None, column_value: Any = None,
+                                   id_column_name: str = None, id_column_value: Any = None) -> None:
         """Deletes data from the table by id"""
         # checks are done inside delete_by_where
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
         if column_name:  # column_value can be empty
             where, params = self.__get_where_params(column_name, column_value)
@@ -481,15 +510,14 @@
                 "GenericCRUD.select_multi_value_by_id is deprecated, use select_multi_value_by_column_and_value instead.")
         return self.select_multi_value_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by,
             skip_null_values=skip_null_values)
 
-
     def select_multi_value_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         """Selects multiple values from the table by ID and returns them as a list."""
         column_name = column_name or id_column_name
@@ -850,15 +878,16 @@
             where = f"`{column_name}`=%s"
             params = (column_value,)
         else:
             where = f"`{column_name}` IS NULL"
             params = None
         return where, params
 
-    def __where_skip_null_values(self, where: str or None, select_clause_value: str, skip_null_values: bool = False) -> str:
+    def __where_skip_null_values(self, where: str or None, select_clause_value: str,
+                                 skip_null_values: bool = False) -> str:
         select_clause_value = select_clause_value or self.default_select_clause_value
         if skip_null_values:
             self.__validate_single_clause_value(select_clause_value)
             where_skip = f"`{select_clause_value}` IS NOT NULL"
             if where:
                 where += f" AND {where_skip}"
             else:
```

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.303/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.303/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/point.py` & `database_mysql_local-0.0.303/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.303/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.303/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.303/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.303/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.303/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.303/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.302
+Version: 0.0.303
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.302/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.303/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/pyproject.toml` & `database_mysql_local-0.0.303/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.302/setup.py` & `database_mysql_local-0.0.303/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
-# TODO: we are migrating from circles_local_database_python to database_mysql_local
+# TODO: we are migrating from database_mysql_local to database_mysql_local
 #  but in the meantime we want to keep both names
-old_name = "circles_local_database_python"
+old_name = "database_mysql_local"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.302',
+    version='0.0.303',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

