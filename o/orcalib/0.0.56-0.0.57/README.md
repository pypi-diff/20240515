# Comparing `tmp/orcalib-0.0.56.tar.gz` & `tmp/orcalib-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orcalib-0.0.56.tar", max compression
+gzip compressed data, was "orcalib-0.0.57.tar", max compression
```

## Comparing `orcalib-0.0.56.tar` & `orcalib-0.0.57.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      418 2024-04-02 17:50:15.643609 orcalib-0.0.56/README.md
--rw-r--r--   0        0        0    12670 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/__init__.py
--rw-r--r--   0        0        0    43202 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/batched_scan_result.py
--rw-r--r--   0        0        0    58694 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/client.py
--rw-r--r--   0        0        0     1895 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/client_data_model.py
--rw-r--r--   0        0        0      772 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/data_classes.py
--rw-r--r--   0        0        0    23394 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/database.py
--rw-r--r--   0        0        0     1040 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/exceptions.py
--rw-r--r--   0        0        0    10223 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/file_ingestor.py
--rw-r--r--   0        0        0    11355 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/hf_utils.py
--rw-r--r--   0        0        0     3928 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/index_handle.py
--rw-r--r--   0        0        0     7728 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/index_query.py
--rw-r--r--   0        0        0    11737 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_chat.py
--rw-r--r--   0        0        0     5961 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_expr.py
--rw-r--r--   0        0        0   106921 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_torch.py
--rw-r--r--   0        0        0    24204 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_types.py
--rw-r--r--   0        0        0     3183 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_utils.py
--rw-r--r--   0        0        0    13972 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/table.py
--rw-r--r--   0        0        0    10928 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/table_query.py
--rw-r--r--   0        0        0     4489 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/temp_database.py
--rw-r--r--   0        0        0     1313 2024-04-02 17:50:37.931760 orcalib-0.0.56/pyproject.toml
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 orcalib-0.0.56/PKG-INFO
+-rw-r--r--   0        0        0      571 2024-05-15 16:25:40.042832 orcalib-0.0.57/README.md
+-rw-r--r--   0        0        0    15207 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/__init__.py
+-rw-r--r--   0        0        0    43398 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/batched_scan_result.py
+-rw-r--r--   0        0        0    59349 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/client.py
+-rw-r--r--   0        0        0     1864 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/client_data_model.py
+-rw-r--r--   0        0        0      774 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/data_classes.py
+-rw-r--r--   0        0        0    23442 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/database.py
+-rw-r--r--   0        0        0     1041 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/exceptions.py
+-rw-r--r--   0        0        0    10234 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/file_ingestor.py
+-rw-r--r--   0        0        0    11360 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/hf_utils.py
+-rw-r--r--   0        0        0     3995 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/index_handle.py
+-rw-r--r--   0        0        0     8499 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/index_query.py
+-rw-r--r--   0        0        0    11526 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/orca_chat.py
+-rw-r--r--   0        0        0     6080 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/orca_expr.py
+-rw-r--r--   0        0        0    98758 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/orca_torch.py
+-rw-r--r--   0        0        0    18961 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/orca_torch_mixins.py
+-rw-r--r--   0        0        0    24370 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/orca_types.py
+-rw-r--r--   0        0        0     3183 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/orca_utils.py
+-rw-r--r--   0        0        0    14018 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/table.py
+-rw-r--r--   0        0        0    11075 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/table_query.py
+-rw-r--r--   0        0        0     4532 2024-05-15 16:25:40.042832 orcalib-0.0.57/orcalib/temp_database.py
+-rw-r--r--   0        0        0     1315 2024-05-15 16:26:00.327112 orcalib-0.0.57/pyproject.toml
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 orcalib-0.0.57/PKG-INFO
```

### Comparing `orcalib-0.0.56/orcalib/__init__.py` & `orcalib-0.0.57/orcalib/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+from importlib.metadata import version
 from typing import Any, Optional
 
 from orca_common import TableCreateMode
 from orcalib.database import with_default_database_method
 from pandas import DataFrame
 
 from .batched_scan_result import BatchedScanResult
@@ -15,15 +17,17 @@
     JSONLIngestor,
     ParquetIngestor,
     PickleIngestor,
 )
 from .hf_utils import HFAutoModelWrapper, HFDatasetIngestor
 from .index_handle import IndexHandle
 from .index_query import DefaultIndexQuery, VectorIndexQuery
+from .orca_chat import OrcaChat
 from .orca_expr import ColumnHandle, OrcaExpr
+from .orca_torch_mixins import ClassificationMode, ProjectionMode
 from .orca_types import (
     BFloat16T,
     BoolT,
     DocumentT,
     EnumT,
     Float16T,
     Float32T,
@@ -43,291 +47,347 @@
     UInt32T,
     UInt64T,
     VectorT,
 )
 from .table import TableHandle
 from .temp_database import TemporaryDatabase, TemporaryTable
 
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+
 
 def set_credentials(*, api_key: str, secret_key: str, endpoint: Optional[str] = None) -> None:
     """
     Set the credentials for the Orca client. This must be called before any other Orca functions. This can also be
     called multiple times to change the credentials.
+
     :param api_key: API key
     :param secret_key: Secret key
     :param endpoint: Endpoint (optional)
 
-    example:
-    >>> import orcalib as orca
-    >>> orca.set_credentials(api_key, secret_key)
+    Example:
+
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.set_credentials(api_key, secret_key)
+
     """
     OrcaClient.set_credentials(api_key=api_key, secret_key=secret_key, endpoint=endpoint)
 
 
 @with_default_database_method
 def create_table(
     db: OrcaDatabase,
     table_name: str,
     if_table_exists: TableCreateMode = TableCreateMode.ERROR_IF_TABLE_EXISTS,
     **columns: OrcaTypeHandle,
 ) -> TableHandle:
     """
-    Create a table in the default database. This is a convenience function that calls `create_table` on the default db.
-    :param table_name: Name of the table
-    :param if_table_exists: What to do if the table already exists (default: TableCreateMode.ERROR_IF_TABLE_EXISTS)
-    :param columns: Columns of the table (name -> type mapping)
-    :return: TableHandle
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.create_table("my_table", id=orca.Int64T, name=orca.TextT)
+        Create a table in the default database. This is a convenience function that calls `create_table` on the default db.
+
+        :param table_name: Name of the table
+        :param if_table_exists: What to do if the table already exists (default: TableCreateMode.ERROR_IF_TABLE_EXISTS)
+        :param columns: Columns of the table (name -> type mapping)
+        :return: TableHandle
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.create_table("my_table", id=orca.Int64T, name=orca.TextT)
     """
     return db.create_table(table_name, if_table_exists, **columns)
 
 
 @with_default_database_method
 def get_table(db: OrcaDatabase, table_name: str) -> TableHandle:
     """
-    Get a table from the default database. This is a convenience function that calls `get_table` on the default db.
-    :param table_name: Name of the table
-    :return: TableHandle
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.get_table("my_table")
+        Get a table from the default database. This is a convenience function that calls `get_table` on the default db.
+
+        :param table_name: Name of the table
+        :return: TableHandle
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.get_table("my_table")
     """
     return db.get_table(table_name)
 
 
 @with_default_database_method
 def list_tables(db: OrcaDatabase) -> list[str]:
     """
-    List tables in the default database. This is a convenience function that calls `list_tables` on the default db.
-    :return: List of table names
+        List tables in the default database. This is a convenience function that calls `list_tables` on the default db.
 
-    example:
-    >>> import orcalib as orca
-    >>> orca.list_tables()
+        :return: List of table names
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.list_tables()
     """
     return db.list_tables()
 
 
 @with_default_database_method
 def backup(db: OrcaDatabase) -> tuple[str, str]:
     """
-    Backup the default database. This is a convenience function that calls `backup` on the default db.
-    :return: Backup path and backup name
+        Backup the default database. This is a convenience function that calls `backup` on the default db.
+
+        :return: Backup path and backup name
 
-    example:
-    >>> import orcalib as orca
-    >>> orca.backup()
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.backup()
     """
     return db.backup()
 
 
 @with_default_database_method
 def default_vectorize(db: OrcaDatabase, text: str) -> list[float]:
     """
-    Vectorize text using the default database. This is a convenience function that calls `default_vectorize` on the default db.
-    :param text: Text to vectorize
-    :return: Vector
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.default_vectorize("hello world")
+        Vectorize text using the default database. This is a convenience function that calls `default_vectorize` on the default db.
+
+        :param text: Text to vectorize
+        :return: Vector
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.default_vectorize("hello world")
     """
     return db.default_vectorize(text)
 
 
 @with_default_database_method
 def get_index(db: OrcaDatabase, index_name: str) -> IndexHandle:
     """
-    Get an index from the default database. This is a convenience function that calls `get_index` on the default db.
-    :param index_name: Name of the index
-    :return: IndexHandle
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.get_index("my_index")
+        Get an index from the default database. This is a convenience function that calls `get_index` on the default db.
+
+        :param index_name: Name of the index
+        :return: IndexHandle
+
+        Example:
+
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.get_index("my_index")
     """
     return db.get_index(index_name)
 
 
 @with_default_database_method
 def create_vector_index(
     db: OrcaDatabase,
     index_name: str,
     table_name: str,
     column: str,
     error_if_exists: bool = True,
 ) -> None:
     """
-    Create a vector index for default db. This is a convenience function that calls `create_vector_index` on the default db.
-    :param index_name: Name of the index
-    :param table_name: Name of the table
-    :param column: Name of the column
-    :param error_if_exists: Whether to raise an error if the index already exists (default: True)
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.create_vector_index("my_index", "my_table", "my_column")
+        Create a vector index for default db. This is a convenience function that calls `create_vector_index` on the default db.
+
+        :param index_name: Name of the index
+        :param table_name: Name of the table
+        :param column: Name of the column
+        :param error_if_exists: Whether to raise an error if the index already exists (default: True)
+
+        Example:
+
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.create_vector_index("my_index", "my_table", "my_column")
     """
     db.create_vector_index(index_name, table_name, column, error_if_exists)
 
 
 @with_default_database_method
 def create_document_index(
     db: OrcaDatabase,
     index_name: str,
     table_name: str,
     column: str,
     error_if_exists: bool = True,
 ) -> None:
     """
-    Create a document index for default db. This is a convenience function that calls `create_document_index` on the default db.
-    :param index_name: Name of the index
-    :param table_name: Name of the table
-    :param column: Name of the column
-    :param error_if_exists: Whether to raise an error if the index already exists (default: True)
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.create_document_index("my_index", "my_table", "my_column")
+        Create a document index for default db. This is a convenience function that calls `create_document_index` on the default db.
+
+        :param index_name: Name of the index
+        :param table_name: Name of the table
+        :param column: Name of the column
+        :param error_if_exists: Whether to raise an error if the index already exists (default: True)
+
+        Example:
+
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.create_document_index("my_index", "my_table", "my_column")
     """
     db.create_document_index(index_name, table_name, column, error_if_exists)
 
 
 @with_default_database_method
 def create_text_index(
     db: OrcaDatabase,
     index_name: str,
     table_name: str,
     column: str,
     error_if_exists: bool = True,
 ) -> None:
     """
-    Create a text index for default db. This is a convenience function that calls `create_text_index` on the default db.
-    :param index_name: Name of the index
-    :param table_name: Name of the table
-    :param column: Name of the column
-    :param error_if_exists: Whether to raise an error if the index already exists (default: True)
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.create_text_index("my_index", "my_table", "my_column")
+        Create a text index for default db. This is a convenience function that calls `create_text_index` on the default db.
+
+        :param index_name: Name of the index
+        :param table_name: Name of the table
+        :param column: Name of the column
+        :param error_if_exists: Whether to raise an error if the index already exists (default: True)
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.create_text_index("my_index", "my_table", "my_column")
     """
     db.create_text_index(index_name, table_name, column, error_if_exists)
 
 
 @with_default_database_method
 def create_btree_index(
     db: OrcaDatabase,
     index_name: str,
     table_name: str,
     column: str,
     error_if_exists: bool = True,
 ) -> None:
     """
-    Create a btree index for default db. This is a convenience function that calls `create_btree_index` on the default db.
-    :param index_name: Name of the index
-    :param table_name: Name of the table
-    :param column: Name of the column
-    :param error_if_exists: Whether to raise an error if the index already exists (default: True)
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.create_btree_index("my_index", "my_table", "my_column")
+        Create a btree index for default db. This is a convenience function that calls `create_btree_index` on the default db.
+
+        :param index_name: Name of the index
+        :param table_name: Name of the table
+        :param column: Name of the column
+        :param error_if_exists: Whether to raise an error if the index already exists (default: True)
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.create_btree_index("my_index", "my_table", "my_column")
     """
     db.create_btree_index(index_name, table_name, column, error_if_exists)
 
 
 @with_default_database_method
 def drop_index(db: OrcaDatabase, index_name: str, error_if_not_exists: bool = True) -> None:
     """
-    Drop an index from the default database. This is a convenience function that calls `drop_index` on the default db.
-    :param index_name: Name of the index
-    :param error_if_not_exists: Whether to raise an error if the index does not exist (default: True)
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.drop_index("my_index")
+        Drop an index from the default database. This is a convenience function that calls `drop_index` on the default db.
+
+        :param index_name: Name of the index
+        :param error_if_not_exists: Whether to raise an error if the index does not exist (default: True)
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.drop_index("my_index")
     """
     db.drop_index(index_name, error_if_not_exists)
 
 
 @with_default_database_method
 def drop_table(db: OrcaDatabase, table_name: str, error_if_not_exists: bool = True) -> None:
     """
-    Drop a table from the default database. This is a convenience function that calls `drop_table` on the default db.
-    :param table_name: Name of the table
-    :param error_if_not_exists: Whether to raise an error if the table does not exist (default: True)
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.drop_table("my_table")
+        Drop a table from the default database. This is a convenience function that calls `drop_table` on the default db.
+
+        :param table_name: Name of the table
+        :param error_if_not_exists: Whether to raise an error if the table does not exist (default: True)
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.drop_table("my_table")
     """
     db.drop_table(table_name, error_if_not_exists)
 
 
 @with_default_database_method
 def search_memory(
     db: OrcaDatabase,
     index_name: str,
     query: list[float],
     limit: int,
     columns: Optional[list[str]] = None,
 ) -> Any:
     """
-    Search memory for default db. This is a convenience function that calls `search_memory` on the default db.
-    :param index_name: Name of the index
-    :param query: Query
-    :param limit: Limit
-    :param columns: Columns to return (optional)
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.search_memory("my_index", [1.0, 2.0], 10)
+        Search memory for default db. This is a convenience function that calls `search_memory` on the default db.
+
+        :param index_name: Name of the index
+        :param query: Query
+        :param limit: Limit
+        :param columns: Columns to return (optional)
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.search_memory("my_index", [1.0, 2.0], 10)
     """
     return db.search_memory(index_name, query, limit, columns)
 
 
 @with_default_database_method
 def scan_index(
     db: OrcaDatabase,
     index_name: str,
     query: Any,
 ) -> DefaultIndexQuery:
     """
-    Scan an index for default db. This is a convenience function that calls `scan_index` on the default db.
-    :param index_name: Name of the index
-    :param query: Query
-    :return: DefaultIndexQuery
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.scan_index("my_index", orca.OrcaExpr("$EQ", (orca.ColumnHandle("my_table", "my_column"), 42)))
+        Scan an index for default db. This is a convenience function that calls `scan_index` on the default db.
+
+        :param index_name: Name of the index
+        :param query: Query
+        :return: DefaultIndexQuery
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.scan_index("my_index", orca.OrcaExpr("$EQ", (orca.ColumnHandle("my_table", "my_column"), 42)))
     """
     return db.scan_index(index_name, query)
 
 
 @with_default_database_method
 def vector_scan_index(
     db: OrcaDatabase,
     index_name: str,
     query: Any,
 ) -> VectorIndexQuery:
     """
-    Scan a vector index for default db. This is a convenience function that calls `vector_scan_index` on the default db.
-    :param index_name: Name of the index
-    :param query: Query
-    :return: VectorIndexQuery
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.vector_scan_index("my_index", orca.OrcaExpr("$EQ", (orca.ColumnHandle("my_table", "my_column"), 42)))
+        Scan a vector index for default db. This is a convenience function that calls `vector_scan_index` on the default db.
+
+        :param index_name: Name of the index
+        :param query: Query
+        :return: VectorIndexQuery
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.vector_scan_index("my_index", orca.OrcaExpr("$EQ", (orca.ColumnHandle("my_table", "my_column"), 42)))
     """
     return db.vector_scan_index(index_name, query)
 
 
 @with_default_database_method
 def full_vector_memory_join(
     db: OrcaDatabase,
@@ -336,67 +396,126 @@
     memory_index_name: str,
     num_memories: int,
     query_columns: list[str],
     page_index: int,
     page_size: int,
 ) -> dict[str, list[tuple[list[float], Any]]]:
     """
-    Join a vector index with a memory index for default db. This is a convenience function that calls `full_vector_memory_join` on the default db.
-    :param index_name: Name of the index
-    :param memory_index_name: Name of the memory index
-    :param num_memories: Number of memories
-    :param query_columns: Query columns
-    :param page_index: Page index
-    :param page_size: Page size
-    :return: Results
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.full_vector_memory_join("my_index", "my_memory_index", 10, ["my_column"], 0, 10)
+        Join a vector index with a memory index for default db. This is a convenience function that calls `full_vector_memory_join` on the default db.
+
+        :param index_name: Name of the index
+        :param memory_index_name: Name of the memory index
+        :param num_memories: Number of memories
+        :param query_columns: Query columns
+        :param page_index: Page index
+        :param page_size: Page size
+        :return: Results
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.full_vector_memory_join("my_index", "my_memory_index", 10, ["my_column"], 0, 10)
     """
     return db.full_vector_memory_join(index_name, memory_index_name, num_memories, query_columns, page_index, page_size)
 
 
 @with_default_database_method
 def query(db: OrcaDatabase, query: str, params: list[None | int | float | bytes | str] = []) -> DataFrame:
     """
-    Execute a raw SQL query. This is a convenience function that calls `query` on the default db.
-    :param query: Query
-    :param params: Parameters (optional)
-    :return: DataFrame
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.query("SELECT * FROM my_table")
+        Execute a raw SQL query. This is a convenience function that calls `query` on the default db.
+
+        :param query: Query
+        :param params: Parameters (optional)
+        :return: DataFrame
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.query("SELECT * FROM my_table")
     """
     return db.query(query, params)
 
 
 @with_default_database_method
 def record_model_scores(db: OrcaDatabase, run_ids: list[int] | int, scores: list[float] | float) -> None:
     """
-    Record model scores in the default database. This is a convenience function that calls `record_model_scores` on the default db.
-    :param run_ids: Run IDs
-    :param scores: Scores (list of floats or a single float)
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.record_model_scores(1, 0.5)
+        Record model scores in the default database. This is a convenience function that calls `record_model_scores` on the default db.
+
+        :param run_ids: Run IDs
+        :param scores: Scores (list of floats or a single float)
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.record_model_scores(1, 0.5)
     """
     db.record_model_scores(run_ids, scores)
 
 
 @with_default_database_method
 def record_model_input_output(
     db: OrcaDatabase, run_ids: list[int] | int, inputs: list[Any] | Any, outputs: list[Any] | Any
 ) -> None:
     """
-    Record model inputs and outputs in the default database. This is a convenience function that calls `record_model_input_output` on the default db.
-    :param run_ids: Run IDs
-    :param inputs: Inputs
-    :param outputs: Outputs
-
-    example:
-    >>> import orcalib as orca
-    >>> orca.record_model_input_output(1, "input", "output")
+        Record model inputs and outputs in the default database. This is a convenience function that calls `record_model_input_output` on the default db.
+
+        :param run_ids: Run IDs
+        :param inputs: Inputs
+        :param outputs: Outputs
+
+        Example:
+    .. code-block:: python
+
+        >>> import orcalib as orca
+        >>> orca.record_model_input_output(1, "input", "output")
     """
     db.record_model_input_output(run_ids, inputs, outputs)
+
+
+def get_client_version() -> str:
+    """
+    Get the version of the OrcaLib library.
+
+    :return: Version
+    """
+    return version("orcalib")
+
+
+def get_server_version() -> str:
+    """
+    Get the version of the OrcaDB server.
+
+    :return: Version
+    """
+
+    healthcheck_data = OrcaClient.healthcheck()
+    result = healthcheck_data.get("git_tag", "")
+
+    if result.startswith("v"):
+        result = result[1:]
+    return result
+
+
+def validate_version_compatibility() -> None:
+    """
+    This function ensures that the client and server versions are compatible.
+    If the versions do not match, an exception is raised.
+
+    Example:
+    """
+
+    client_version = get_client_version()
+    server_version = get_server_version()
+
+    if server_version == "0.0.0" or server_version == "":
+        logger.warning(f"Server version is '{server_version}'. Skipping version check.")
+        return
+
+    if client_version == "0.0.0":
+        logger.warning(f"Client version is '{client_version}'. Skipping version check.")
+        return
+
+    if client_version != server_version:
+        raise OrcaException(f"Client version {client_version} does not match server version {server_version}")
```

### Comparing `orcalib-0.0.56/orcalib/batched_scan_result.py` & `orcalib-0.0.57/orcalib/batched_scan_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 from orca_common import ColumnName
 
 from orcalib.orca_types import OrcaTypeHandle
 
 
 def is_single_element_slice(slice_obj: int | slice | str | None, target_length: int) -> bool:
     """Return True if the given slice object selects a single element from a sequence of the given length
+
     :param slice_obj: The slice object (or an index) to check
     :param target_length: The length of the sequence that's being sliced/indexed
-    :returns: True if the slice object selects a single element, False otherwise
+    :return: True if the slice object selects a single element, False otherwise
     """
+
     if slice_obj is None:
         return target_length == 1
     elif isinstance(slice_obj, (str, int)):
         return True
     elif isinstance(slice_obj, list) and len(slice_obj) == 1:
         return True
     elif isinstance(slice_obj, slice):
@@ -26,29 +28,31 @@
         return abs(indices[0] - indices[1]) == 1
     else:
         return False
 
 
 def try_collapse_slice(slice_obj: slice, target_length: int) -> int | slice:
     """Try to collapse the given slice object into a single index, if possible
+
     :param slice_obj: The slice object we're trying to collapse
     :param target_length: The length of the sequence that's being sliced/indexed
-    :returns: The collapsed slice object, or the original slice object if it can't be collapsed
+    :return: The collapsed slice object, or the original slice object if it can't be collapsed
     """
     indices = slice_obj.indices(target_length)
     if indices[0] == indices[1] - 1:
         return indices[0]
     else:
         return slice_obj
 
 
 def index_to_slice(index: int) -> slice:
     """Convert an index to a slice
+
     :param index: The index we want the slice to select
-    :returns: A slice that selects the given index
+    :return: A slice that selects the given index
     """
     if index == -1:
         return slice(index, None)
     return slice(index, index + 1)
 
 
 class BatchedScanResult:
@@ -71,16 +75,15 @@
         data: list[list[list[Any]]],
         batch_slice: slice | int | None = None,
         memory_slice: slice | int | None = None,
         column_slice: Optional[ColumnSlice] = None,
     ):
         """
         :param column_dict: A dictionary of column name to column type. These are the columns that were requested in the query.
-        :param data: The underlying data. This is a list of batches, where each batch is a list of memories,
-        where each memory is a tuple of values.
+        :param data: The underlying data. This is a list of batches, where each batch is a list of memories, where each memory is a tuple of values.
         :param batch_slice: Used internally to maintain a "view" of the data based on a subset of the batches. You shouldn't need to set this manually.
         :param memory_slice: Used internally to maintain a "view" of the data based on a subset of the memories. You shouldn't need to set this manually.
         :param column_slice: Used internally to maintain a "view" of the data based on a subset of the columns. You shouldn't need to set this manually.
         """
         self.data = data
 
         self.batch_size = len(data)
@@ -115,15 +118,17 @@
         overrides["memory_slice"] = overrides.get("memory_slice", self.memory_slice)
         overrides["column_slice"] = overrides.get("column_slice", self.column_slice)
 
         return BatchedScanResult(**overrides)
 
     def _get_column_slice(self, batch_slice, memory_slice, column_slice) -> "BatchedScanResult":
         """Helper function that slices the data based on the given batch, memory, and column slices.
+
         NOTE: When batch_slice and memory_slice are ints, this function doesn't return a BatchedScanResult.
+
         Instead, if one column is selected, it returns a single value. If multiple columns are selected, it returns
         a list of values.
         """
         assert self.column_slice is None, f"BatchedScanResult already fully sliced: {repr(self)}"
 
         return self._clone(batch_slice=batch_slice, memory_slice=memory_slice, column_slice=column_slice)
 
@@ -164,37 +169,48 @@
             raise ValueError(f"item() column_slice must select a single value. You passed: {column_slice}")
         values = self._extract_memory_values(memory, column_slice, force_list=True)
 
         return values[0]
 
     def __getitem__(self, key) -> "BatchedScanResult":
         """Slice the data based on the given batch, memory, and column slices.
+
         :param key: Key for indexing into the current BatchedScanResult.
-            - If we haven't sliced the data at all, then the key must be one of batch_slice,
-              (batch_slice), (batch_slice, memory_slice), or (batch_slice, memory_slice, column_slice)
-            - If batch_slice is already set, then the key must be one of memory_slice,
-              (memory_slice), or (memory_slice, column_slice)
-            - If batch_slice and memory_slice are already set, then the key must be a column_slice.
-        A batch_slice can be a single batch index or a slice of batch indices.
-        A memory_slice can be a single memory index or a slice of memory indices.
-        A column_slice can be a single column name, a list of column names or indices, or a slice of column indices.
-        :returns: A new BatchedScanResult that is a view on the underlying data.
-        NOTE: When batch_slice and memory_slice are ints, this function doesn't return a BatchedScanResult.
+        :return: A new BatchedScanResult that is a view on the underlying data.
+
+        NOTE:
+
+        - If we haven't sliced the data at all, then the key must be one of batch_slice, (batch_slice), (batch_slice, memory_slice), or (batch_slice, memory_slice, column_slice)
+
+        - If batch_slice is already set, then the key must be one of memory_slice, (memory_slice), or (memory_slice, column_slice)
+
+        - If batch_slice and memory_slice are already set, then the key must be a column_slice.
+
+        - A batch_slice can be a single batch index or a slice of batch indices.
+
+        - A memory_slice can be a single memory index or a slice of memory indices.
+
+        - A column_slice can be a single column name, a list of column names or indices, or a slice of column indices.
+
+        When batch_slice and memory_slice are ints, this function doesn't return a BatchedScanResult.
         Instead, if one column is selected, it returns a single value. If multiple columns are selected,
         it returns a list of values.
 
         Examples:
-        >>> # Slice the data by batch, memory, and column
-        >>> first_batch = result[0] # Get the first batch
-        >>> first_batch_last_memory = first_batch[-1:] # Get the last memory of the first batch
-        >>> first_batch_last_memory_vector = first_batch_last_memory["$embedding"] # Get the vector of the last memory of the first batch
-        >>> first_batch[-1:, "$embedding"] # Equivalent to the above
-        >>> result[0, -1:, "$embedding"] # Equivalent to the above
 
-        >>> result[0, -1:, ["$embedding", "col1"]] # Get the vector and col1 of the last memory of the first batch
+        .. code-block:: python
+
+            >>> # Slice the data by batch, memory, and column
+            >>> first_batch = result[0] # Get the first batch
+            >>> first_batch_last_memory = first_batch[-1:] # Get the last memory of the first batch
+            >>> first_batch_last_memory_vector = first_batch_last_memory["$embedding"] # Get the vector of the last memory of the first batch
+            >>> first_batch[-1:, "$embedding"] # Equivalent to the above
+            >>> result[0, -1:, "$embedding"] # Equivalent to the above
+
+            >>> result[0, -1:, ["$embedding", "col1"]] # Get the vector and col1 of the last memory of the first batch
         """
         if self.batch_slice is not None:
             return self._get_memory_slice(self.batch_slice, key)
 
         assert (
             self.memory_slice is None
         ), "Cannot slice a BatchedScanResult with a memory_slice unless batch_slice is slready specified"
@@ -239,32 +255,33 @@
         """
         Convert the selected values from a vector column of the batched scan results into a PyTorch tensor. This method is useful
         for preparing the scan results for machine learning models and other tensor-based computations.
 
         This method assumes that the selected data can be appropriately converted into a tensor. It works best when the data is numeric
         and consistently shaped across batches and memories. Non-numeric data or inconsistent shapes may lead to errors or unexpected results.
 
-        ### Parameters:
         :param column: (Optional[ColumnName | int]): Specifies the column from which to extract the values. If None, the method uses the
                 current column slice. If a column has been singularly selected by previous slicing, this parameter is optional.
         :param dtype: (Optional[torch.dtype]): The desired data type of the resulting tensor. If not provided, the default is inferred based
                 on the data types of the input values.
         :param device: (Optional[torch.device]): The device on which the resulting tensor will be allocated. Use this to specify if the tensor
                 should be on CPU, GPU, or another device. If not provided, the default is the current device setting in PyTorch.
 
-        ### Returns:
-            torch.Tensor: A tensor representation of the selected data. The shape of the tensor is typically (batch_size, mem_count, vector_len),
+        :return: torch.Tensor: A tensor representation of the selected data. The shape of the tensor is typically (batch_size, mem_count, vector_len),
                 but can vary based on the current slicing of the BatchedScanResult object.
 
-        ### Example Usage:
-        >>> result = my_index.vector_scan(...)
-        >>> # Convert the '$embedding' column into a tensor
-        >>> embedding_tensor = result.to_tensor(column='$embedding')
-        >>> # Convert and specify data type and device
-        >>> embedding_tensor = result[0:2, :, 'features'].to_tensor(dtype=torch.float32, device=torch.device('cuda:0'))
+        Examples:
+
+        .. code-block:: python
+
+            >>> result = my_index.vector_scan(...)
+            >>> # Convert the '$embedding' column into a tensor
+            >>> embedding_tensor = result.to_tensor(column='$embedding')
+            >>> # Convert and specify data type and device
+            >>> embedding_tensor = result[0:2, :, 'features'].to_tensor(dtype=torch.float32, device=torch.device('cuda:0'))
         """
         batch_slice, memory_slice, column_slice = self._get_slices()
         column = column if column is not None else column_slice
 
         if isinstance(batch_slice, int):
             batch_slice = index_to_slice(batch_slice)
         if isinstance(memory_slice, int):
@@ -341,17 +358,21 @@
             else:
                 return len(self.data[batch_slice][memory_slice])
         else:
             return len(self.data[batch_slice])
 
     def __iter__(self) -> Iterator:
         """Iterate over the batches of memories
-        :returns: The return type depends on the current slices:
+
+        :return: The return type depends on the current slices:
+
         - When batch_slice is an int (but memory_slice and column_slice are None), this yields each memory from that batch.
+
         - When batch_slice and memory_slice are both ints (but column_slice is None), this yields each value from that memory.
+
         - Otherwise, this yields each batch with the specified subset of selected memories/columns
         """
         batch_slice, memory_slice, column_slice = self._get_slices()
 
         if isinstance(batch_slice, int):
             if isinstance(memory_slice, int):
                 yield from self._extract_memory_values(self.data[batch_slice][memory_slice], column_slice)
@@ -367,20 +388,23 @@
 
     def to_list(
         self,
     ) -> list[list[list[Any] | Any]]:
         """Convert the values of a vector column to a list of lists
 
         Example:
-        >>> bsr[0].to_list() # returns the list of memories in the first batch
-        >>> bsr[0, 0].to_list() # returns a list of the column values in the first memory of the first batch.
-        >>> bsr[0, 0, "col1"].to_list() # returns the value of "col1" for the first memory of the first batch
-        >>> bsr[0, 0, ["col1", "col2"]].to_list() # returns [value of col1, value of col2] for the first memory of the first batch
-        >>> bsr[1:3, -2:, ["col1", "col2"]].to_list() # returns a list of lists of [value of col1, value of col2] for
-        the last two memories of the second and third batches
+
+        .. code-block:: python
+
+            >>> bsr[0].to_list() # returns the list of memories in the first batch
+            >>> bsr[0, 0].to_list() # returns a list of the column values in the first memory of the first batch.
+            >>> bsr[0, 0, "col1"].to_list() # returns the value of "col1" for the first memory of the first batch
+            >>> bsr[0, 0, ["col1", "col2"]].to_list() # returns [value of col1, value of col2] for the first memory of the first batch
+            >>> bsr[1:3, -2:, ["col1", "col2"]].to_list() # returns a list of lists of [value of col1, value of col2] for
+            the last two memories of the second and third batches
         """
         return list(self)
 
     def df(
         self,
         limit: Optional[int] = None,
         explode: bool = False,
@@ -391,34 +415,36 @@
         This method restructures the nested data into a tabular format, while respecting the current slicing of the BatchedScanResult
         object. If the object has been sliced to select certain batches, memories, or columns, only the selected data will be included
         in the DataFrame.
 
         Special columns '_batch' and '_memory' are added to the DataFrame if the batch or memory, respectively, has not been singularly
         selected. These columns track the batch and memory indices of each row in the DataFrame.
 
-        ### Parameters
-        :params limit: (Optional[int]) If provided, limits the number of rows in the resulting DataFrame to the specified value.
-                This can be useful for large datasets where you only need a sample of the data for quick analysis or visualization.
-        :params explode: (bool) If True, any list-like columns in the DataFrame will be 'exploded' into separate rows, each containing
-                one element from the list. This parameter is currently not implemented but can be used in future for handling
-                nested data structures. Currently, its value does not change the behavior of the method.
-
-        ### Returns
-            pandas.DataFrame: A DataFrame representing the selected portions of the batched scan data. The exact shape and content
-                of the DataFrame depend on the current state of the BatchedScanResult object, including any applied batch, memory,
-                and column slices.
-
-        ### Example Usage
-        >>> result = BatchedScanResult(...)
-        >>> # Convert entire data to DataFrame
-        >>> df = result.df()
-        >>> # Convert first 10 rows to DataFrame
-        >>> df_limited = result.df(limit=10)
-        >>> # Convert and 'explode' list-like columns (if implemented)
-        >>> df_exploded = result.df(explode=True)
+        :param limit: (Optional[int]) If provided, limits the number of rows in the resulting DataFrame to the specified value.
+            This can be useful for large datasets where you only need a sample of the data for quick analysis or visualization.
+
+        :param explode: (bool) If True, any list-like columns in the DataFrame will be 'exploded' into separate rows, each containing
+            one element from the list. This parameter is currently not implemented but can be used in future for handling
+            nested data structures. Currently, its value does not change the behavior of the method.
+
+        :return: A DataFrame representing the selected portions of the batched scan data. The exact shape and content
+            of the DataFrame depend on the current state of the BatchedScanResult object, including any applied batch, memory,
+            and column slices.
+
+        Examples
+
+        .. code-block:: python
+
+            >>> result = BatchedScanResult(...)
+            >>> # Convert entire data to DataFrame
+            >>> df = result.df()
+            >>> # Convert first 10 rows to DataFrame
+            >>> df_limited = result.df(limit=10)
+            >>> # Convert and 'explode' list-like columns (if implemented)
+            >>> df_exploded = result.df(explode=True)
         """
         batch_slice, memory_slice, column_slice = self._get_slices()
 
         # First decide which columns to include in the DataFrame
         columns = list(self.column_dict.keys())
         match self.column_slice:
             case None:
@@ -483,16 +509,17 @@
 
 
 class BatchedVectorScanResult_V2:
     """A batched vector scan result, containing batches of memory results. Each
     memory result contains its embedding vector and any additional columns that
     were requested in the query.
 
-    NOTE: This is compatible with OrcaClient._vector_scan_index_v2(...)
-    TODO: Remove this class once the OrcaClient._vector_scan_index_v2(...) is removed
+    NOTE: This is compatible with `OrcaClient._vector_scan_index_v2(...)`
+
+    TODO: Remove this class once the `OrcaClient._vector_scan_index_v2(...)` is removed
 
     This class acts as a view on the underlying data, allowing you to slice it
     by batch, memory, and column. The slicing is lazy, so it doesn't copy any
     of the underlying data.
     """
 
     # The name of the special column that contains the embedding vector
@@ -510,16 +537,15 @@
         data: list[list[tuple[Any, ...]]],
         batch_slice: slice | int | None = None,
         memory_slice: slice | int | None = None,
         column_slice: Optional[ColumnSlice] = None,
     ):
         """
         :param extra_col_names: The names of the extra columns that were requested in the query.
-        :param data: The underlying data. This is a list of batches, where each batch is a list of memories,
-        where each memory is a tuple of values.
+        :param data: The underlying data. This is a list of batches, where each batch is a list of memories, where each memory is a tuple of values.
         :param batch_slice: Used internally to maintain a "view" of the data based on a subset of the batches. You shouldn't need to set this manually.
         :param memory_slice: Used internally to maintain a "view" of the data based on a subset of the memories. You shouldn't need to set this manually.
         :param column_slice: Used internally to maintain a "view" of the data based on a subset of the columns. You shouldn't need to set this manually.
         """
         self.data = data
 
         self.batch_size = len(data)
@@ -544,37 +570,40 @@
 
         self.extra_col_names = extra_col_names
         self.column_names = [self.VECTOR_KEY, *extra_col_names]
         self.column_to_index = {name: i for i, name in enumerate(self.column_names)}
 
     def _clone(self, **overrides) -> "BatchedVectorScanResult_V2":
         """Clone this BatchedVectorScanResult_V2, optionally overriding some parameters
+
         :param overrides: The parameters to override
-        :returns: A new BatchedVectorScanResult_V2
+        :return: A new BatchedVectorScanResult_V2
 
         NOTE: This method should not be called directly. It is used internally."""
 
         overrides["extra_col_names"] = overrides.get("extra_col_names", self.extra_col_names)
         overrides["data"] = overrides.get("data", self.data)
         overrides["batch_slice"] = overrides.get("batch_slice", self.batch_slice)
         overrides["memory_slice"] = overrides.get("memory_slice", self.memory_slice)
         overrides["column_slice"] = overrides.get("column_slice", self.column_slice)
 
         return BatchedVectorScanResult_V2(**overrides)
 
     def _get_column_slice(self, batch_slice, memory_slice, column_slice) -> "BatchedVectorScanResult_V2":
-        """Helper function that slices the data based on the given batch, memory, and column slices.
+        """
+        Helper function that slices the data based on the given batch, memory, and column slices.
+
         NOTE: When batch_slice and memory_slice are ints, this function doesn't return a BatchedVectorScanResult_V2.
         Instead, if one column is selected, it returns a single value. If multiple columns are selected, it returns
         a list of values.
 
         :param batch_slice: The slice of batches to select
         :param memory_slice: The slice of memories to select
         :param column_slice: The slice of columns to select
-        :returns: A new BatchedVectorScanResult_V2 that is a view on the underlying data.
+        :return: A new BatchedVectorScanResult_V2 that is a view on the underlying data.
 
         NOTE: This function is used internally to slice the data based on the given batch, memory, and column slices.
         """
         assert self.column_slice is None, f"BatchedVectorScanResult_V2 already fully sliced: {repr(self)}"
 
         if (
             isinstance(batch_slice, int)
@@ -583,17 +612,18 @@
         ):
             return self._extract_memory_values(self.data[batch_slice][memory_slice], column_slice)
         else:
             return self._clone(batch_slice=batch_slice, memory_slice=memory_slice, column_slice=column_slice)
 
     def _get_memory_slice(self, batch_slice, key: tuple | int) -> "BatchedVectorScanResult_V2":
         """Helper function that slices the data based on the given batch and memory slices.
+
         :param batch_slice: The slice of batches to select
         :param key: The memory slice to select
-        :returns: A new BatchedVectorScanResult_V2 that is a view on the underlying data.
+        :return: A new BatchedVectorScanResult_V2 that is a view on the underlying data.
 
         NOTE: This function is used internally to slice the data based on the given batch and memory slices.
         """
 
         if self.memory_slice is not None:
             return self._get_column_slice(self.batch_slice, self.memory_slice, key)
 
@@ -610,37 +640,48 @@
         else:
             raise ValueError(
                 f"key must be a tuple with (memory_slice) or (memory_slice, column_slice). You passed: {key}"
             )
 
     def __getitem__(self, key) -> "BatchedVectorScanResult_V2":
         """Slice the data based on the given batch, memory, and column slices.
+
         :param key: Key for indexing into the current BatchedVectorScanResult_V2.
-            - If we haven't sliced the data at all, then the key must be one of batch_slice,
-              (batch_slice), (batch_slice, memory_slice), or (batch_slice, memory_slice, column_slice)
-            - If batch_slice is already set, then the key must be one of memory_slice,
-              (memory_slice), or (memory_slice, column_slice)
-            - If batch_slice and memory_slice are already set, then the key must be a column_slice.
-        A batch_slice can be a single batch index or a slice of batch indices.
-        A memory_slice can be a single memory index or a slice of memory indices.
-        A column_slice can be a single column name, a list of column names or indices, or a slice of column indices.
-        :returns: A new BatchedVectorScanResult_V2 that is a view on the underlying data.
-        NOTE: When batch_slice and memory_slice are ints, this function doesn't return a BatchedVectorScanResult_V2.
+        :return: A new BatchedVectorScanResult_V2 that is a view on the underlying data.
+
+        NOTE:
+
+        - If we haven't sliced the data at all, then the key must be one of batch_slice, (batch_slice), (batch_slice, memory_slice), or (batch_slice, memory_slice, column_slice)
+
+        - If batch_slice is already set, then the key must be one of memory_slice, (memory_slice), or (memory_slice, column_slice)
+
+        - If batch_slice and memory_slice are already set, then the key must be a column_slice.
+
+        - A batch_slice can be a single batch index or a slice of batch indices.
+
+        - A memory_slice can be a single memory index or a slice of memory indices.
+
+        - A column_slice can be a single column name, a list of column names or indices, or a slice of column indices.
+
+
+        When batch_slice and memory_slice are ints, this function doesn't return a BatchedVectorScanResult_V2.
         Instead, if one column is selected, it returns a single value. If multiple columns are selected,
         it returns a list of values.
 
         Examples:
-        >>> # Slice the data by batch, memory, and column
-        >>> first_batch = result[0] # Get the first batch
-        >>> first_batch_last_memory = first_batch[-1:] # Get the last memory of the first batch
-        >>> first_batch_last_memory_vector = first_batch_last_memory["__vector__"] # Get the vector of the last memory of the first batch
-        >>> first_batch[-1:, "__vector__"] # Equivalent to the above
-        >>> result[0, -1:, "__vector__"] # Equivalent to the above
 
-        >>> result[0, -1:, ["__vector__", "col1"]] # Get the vector and col1 of the last memory of the first batch
+        .. code-block:: python
+
+            >>> # Slice the data by batch, memory, and column
+            >>> first_batch = result[0] # Get the first batch
+            >>> first_batch_last_memory = first_batch[-1:] # Get the last memory of the first batch
+            >>> first_batch_last_memory_vector = first_batch_last_memory["__vector__"] # Get the vector of the last memory of the first batch
+            >>> first_batch[-1:, "__vector__"] # Equivalent to the above
+            >>> result[0, -1:, "__vector__"] # Equivalent to the above
+            >>> result[0, -1:, ["__vector__", "col1"]] # Get the vector and col1 of the last memory of the first batch
         """
         if self.batch_slice is not None:
             return self._get_memory_slice(self.batch_slice, key)
 
         assert (
             self.memory_slice is None
         ), "Cannot slice a BatchedVectorScanResult_V2 with a memory_slice unless batch_slice is slready specified"
@@ -675,22 +716,26 @@
 
         return f"BatchedVectorScanResult_V2(batch_size={self.batch_size}, mem_count={self.memories_per_batch}, extra_col_names={self.extra_col_names})"
 
     # Need a function to convert the values of a vector column to a tensor with shape (batch_size, mem_count, vector_len)
     def to_tensor(
         self,
     ) -> torch.Tensor:
-        """Convert the values of a vector column to a tensor with shape (batch_size, mem_count, vector_len)
+        """
+        Convert the values of a vector column to a tensor with shape (batch_size, mem_count, vector_len)
 
         NOTE: This function only works when all of the following are true:
-         -- The batch slice is a slice or None (i.e., not an int)
-         -- The memory slice is a slice or None (i.e., not an int)
-         -- The column_slice is None or a single column name or integer.
+
+        * The batch slice is a slice or None (i.e., not an int)
+        * The memory slice is a slice or None (i.e., not an int)
+        * The column_slice is None or a single column name or integer.
+
         NOTE: When column_slice is None, the tensor is built from the embedding vectors (i.e., the __vector__ column)
-        :returns: A tensor with shape (batch_size, mem_count, vector_len)
+
+        :return: A tensor with shape (batch_size, mem_count, vector_len)
         """
         batch_slice, memory_slice, column = self._get_slices()
 
         # NOTE: We don't check for "None" here because None was converted to slice(None) in _get_slices()
         assert isinstance(batch_slice, slice), f"batch_slice must be a slice. You passed: {self.batch_slice}"
         assert isinstance(memory_slice, slice), f"memory_slice must be a slice. You passed: {self.memory_slice}"
 
@@ -708,21 +753,22 @@
             raise ValueError(f"column must be a single column name or integer. You passed: {column}")
         return torch.tensor(
             np.array([[row[col_index] for row in memories[memory_slice]] for memories in self.data[batch_slice]])
         )
 
     def _extract_memory_values(self, memory, column_slice: Optional[ColumnSlice]):
         """Helper function that extracts the values of the given column slice from the given memory
+
         NOTE: When column_slice is a single column, this function doesn't return a list. Instead, it returns
         a single value - might happen to be a list (e.g., if the column was a vector column).
 
         :param memory: The memory to extract values from
         :param column_slice: The slice of columns to extract
         :param force_list: If True, force the return value to be a list
-        :returns: The values of the given column slice from the given memory
+        :return: The values of the given column slice from the given memory
 
         NOTE: This function is used internally to extract the values of a column slice from a memory.
         """
         if column_slice is None:
             return memory[:]
         elif isinstance(column_slice, (int, slice)):
             return memory[column_slice]
@@ -741,47 +787,54 @@
             raise ValueError(
                 f"column_slice must be a slice, int, or list of ints or column names. You passed: {column_slice}"
             )
 
     def _get_slices(self) -> tuple[Any, Any, Any]:
         """
         Helper function that returns the effective batch, memory, and column slices
-        :returns: A tuple of the effective batch, memory, and column slices
+
+        :return: A tuple of the effective batch, memory, and column slices
 
         NOTE: This function is used internally to get the effective slices for the current BatchedVectorScanResult.
         """
         batch_slice = self.batch_slice if self.batch_slice is not None else slice(None)
         memory_slice = self.memory_slice if self.memory_slice is not None else slice(None)
         column_slice = self.column_slice if self.column_slice is not None else slice(None)
 
         return batch_slice, memory_slice, column_slice
 
     def __len__(self) -> int:
         """
         Based on the current slices, return the number of batches, memories, or values in a vector column.
-        :returns: The return type depends on the current slices:
+
+        :return: The return type depends on the current slices:
         """
         batch_slice, memory_slice, column_slice = self._get_slices()
 
         if isinstance(self.batch_slice, int):
             if self.memory_slice is int:
                 return len(self._extract_memory_values(self.data[self.batch_slice][memory_slice], column_slice))
             else:
                 return len(self.data[batch_slice][memory_slice])
         else:
             return len(self.data[batch_slice])
 
     def __iter__(self) -> Iterator:
         """
         Iterate over the batches of memories
-        :returns: The return type depends on the current slices:
+
+        :return: The return type depends on the current slices:
+        :rtype: Iterator
+
         - When batch_slice is an int (but memory_slice and column_slice are None), this yields each memory from that batch.
+
         - When batch_slice and memory_slice are both ints (but column_slice is None), this yields each value from that memory.
+
         - Otherwise, this yields each batch with the specified subset of selected memories/columns
-        :rtype: Iterator
+
         """
         batch_slice, memory_slice, column_slice = self._get_slices()
 
         if isinstance(batch_slice, int):
             if isinstance(memory_slice, int):
                 yield from self._extract_memory_values(self.data[batch_slice][memory_slice], column_slice)
             else:
@@ -796,23 +849,27 @@
 
     def to_list(
         self,
     ) -> list[list[list[Any] | Any]]:
         """
         Convert the values of a vector column to a list of lists
 
+        :return: A list of lists of values
+
         Example:
-        >>> bsr[0].to_list() # returns the list of memories in the first batch
-        >>> bsr[0, 0].to_list() # returns the list of "extra" column values in the first memory of the first batch.
-        NOTE:The "special" keys like __vector__ are not included unless they're specifically requested.
-        >>> bsr[0, 0, "col1"].to_list() # returns [value of col1] for the first memory of the first batch
-        >>> bsr[0, 0, ["col1", "col2"]].to_list() # returns [value of col1, value of col2] for the first memory of the first batch
-        >>> bsr[1:3, -2:, ["col1", "col2"]].to_list() # returns a list of lists of [value of col1, value of col2] for
-        the last two memories of the second and third batches
-        :returns: A list of lists of values
+
+        .. code-block:: python
+
+            >>> bsr[0].to_list() # returns the list of memories in the first batch
+            >>> bsr[0, 0].to_list() # returns the list of "extra" column values in the first memory of the first batch.
+            NOTE:The "special" keys like __vector__ are not included unless they're specifically requested.
+            >>> bsr[0, 0, "col1"].to_list() # returns [value of col1] for the first memory of the first batch
+            >>> bsr[0, 0, ["col1", "col2"]].to_list() # returns [value of col1, value of col2] for the first memory of the first batch
+            >>> bsr[1:3, -2:, ["col1", "col2"]].to_list() # returns a list of lists of [value of col1, value of col2] for
+            the last two memories of the second and third batches
         """
         batch_slice, memory_slice, column_slice = self._get_slices()
 
         if isinstance(batch_slice, int):
             if isinstance(memory_slice, int):
                 value = self._extract_memory_values(self.data[batch_slice][memory_slice], column_slice)
                 return value if isinstance(value, list) else [value]
```

### Comparing `orcalib-0.0.56/orcalib/client.py` & `orcalib-0.0.57/orcalib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,41 +29,45 @@
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 
 def _prepare_file_list(files: list[tuple[str, IO[bytes]]]) -> list[tuple[str, tuple[str, IO[bytes]]]]:
     """
     Prepare the file list for a multipart request
+
     :param files: The list of files to prepare
     :return: The prepared file list
 
     NOTE: This function should not be called directly. It is used internally by the OrcaClient class.
     """
     return [("files", (file_name, file_bytes)) for file_name, file_bytes in files]
 
 
 def default_api_version_key(api_version_key: str) -> Any:
     """
     Automatically sets the `api_version` kwarg to the current api version using the specific api version key
     Essentially, it replaces a None `api_version` parameter with `OrcaClient.current_api_version[api_version_key]`
+
     :param api_version_key: The key to use to get the current api version
     :return: The decorator
     """
 
     def decorator(func: Any) -> Any:
         """
         The decorator
+
         :param func: The function to decorate
         :return: The decorated function
         """
 
         @wraps(func)
         def wrapper(*args, **kwargs) -> Any:
             """
             The wrapper
+
             :param args: The arguments
             :param kwargs: The keyword arguments
             :return: The result of the function
             """
             api_version = kwargs.get("api_version") or OrcaClient.current_api_version[api_version_key]
             kwargs["api_version"] = api_version
             return func(*args, **kwargs)
@@ -96,14 +100,15 @@
         "index.get": "v3",
         "index.create": "v3",
     }
 
     @staticmethod
     def version_string_to_int(api_version: str) -> int:
         """Returns the integer version number from the api version string
+
         :param api_version: The api version string
         :return: The integer version number
 
         Example: "v1" -> 1
         """
         if api_version is None or not api_version.startswith("v") or len(api_version) < 2:
             raise ValueError(f"Invalid api version: {api_version}. Version should be a string like 'v1'")
@@ -112,14 +117,15 @@
             raise ValueError(f"Invalid api version: {api_version}. Version must be >= 1")
         return version
 
     @staticmethod
     def set_credentials(*, api_key: str, secret_key: str, endpoint: Optional[str] = None) -> None:
         """
         Set the api and secret key for the session
+
         :param api_key: The api key
         :param secret_key: The secret key
         :param endpoint: The endpoint to use (optional)
         """
         OrcaClient.API_KEY = api_key
         OrcaClient.SECRET_KEY = secret_key
         if endpoint is not None and endpoint[-1] != "/" and os.name == "nt":  # windows compatibility
@@ -127,14 +133,15 @@
         if endpoint:
             OrcaClient.BASE_URL = endpoint
 
     @staticmethod
     def _format_num_bytes(num: int, suffix: str = "B") -> str:
         """
         Format a number of bytes into a human readable string
+
         :param num: The number of bytes
         :param suffix: The suffix to use (default: "B")
         :return: The formatted string of bytes
 
         NOTE: This function should not be called directly. It is used internally by the OrcaClient class.
         """
         for unit in ("", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"):
@@ -150,14 +157,15 @@
         request_params: Optional[dict[str, Any]] = None,
         retries: int = 3,
         verbose: bool = False,
         file_path: str = None,
     ) -> requests.Response:
         """
         Perform the http request to the web service with auth details
+
         :param method: The http method to use
         :param url: The url to request
         :param request_params: The parameters to send with the request (optional)
         :param retries: The number of times to retry the request if it fails (default: 3)
         :param verbose: If True, print verbose output about the request (default: False)
         :param file_path: The path to a file to upload (optional)
         :return: The response from the web service
@@ -173,16 +181,19 @@
 
         if verbose:
             print(f"Orca request start: {method} {url}")
 
         start_time = time.time()
 
         request_params["headers"] = {
-            "api-key": OrcaClient.API_KEY,
-            "secret-key": OrcaClient.SECRET_KEY,
+            **{
+                "api-key": OrcaClient.API_KEY,
+                "secret-key": OrcaClient.SECRET_KEY,
+            },
+            **request_params.get("headers", {}),
         }
 
         status_force_retry = [500, 502, 504]
 
         retry_config = Retry(
             total=retries,
             read=retries,
@@ -224,51 +235,55 @@
 
         return resp
 
     @staticmethod
     def create_database(db_name: str) -> requests.Response:
         """
         Create a new database
+
         :param db_name: The name of the database
         :return: Creat database response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/create_database")
         request_params = {"params": {"db_name": db_name}}
         res = OrcaClient._orca_request("POST", url, request_params)
         return res
 
     @staticmethod
     def drop_database(db_name: str, ignore_db_not_found: bool = False) -> bool:
         """
         Drop the database
+
         :param db_name: The name of the database
         :param ignore_db_not_found: If True, ignore the error if the database is not found (default: False)
         :return: True if the database was dropped, False if it was not found
         """
         url = os.path.join(OrcaClient.BASE_URL, f"v1/drop/db/{db_name}")
         request_params = {"params": {"ignore_db_not_found": ignore_db_not_found}}
         res = OrcaClient._orca_request("DELETE", url, request_params)
         return res.json()["value"]
 
     @staticmethod
     def database_exists(db_name: str) -> bool:
         """
         Check if the database exists
+
         :param db_name: The name of the database
         :return: True if the database exists, False if it does not
         """
         url = os.path.join(OrcaClient.BASE_URL, f"v1/exists/db/{db_name}")
         request_params = {"params": {}}
         res = OrcaClient._orca_request("GET", url, request_params)
         return res.json()["value"]
 
     @staticmethod
     def restore_backup(target_db_name: str, backup_name: str, checksum: str | None = None) -> requests.Response:
         """
         Restore a database from a backup
+
         :param target_db_name: The name of the target database
         :param backup_name: The name of the backup
         :param checksum: The checksum of the backup file (optional)
         :return: Restore database response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/restore_database")
         request_params = {
@@ -281,26 +296,28 @@
         res = OrcaClient._orca_request("POST", url, request_params)
         return res
 
     @staticmethod
     def create_backup(db_name: str) -> requests.Response:
         """
         Create a backup of the database
+
         :param db_name: The name of the database
         :return: Create backup response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/backup_database")
         request_params = {"params": {"db_name": db_name}}
         res = OrcaClient._orca_request("POST", url, request_params)
         return res.json()
 
     @staticmethod
     def download_backup(backup_file: str, download_path: str = "./data", overwrite: bool = False) -> requests.Response:
         """
         Download a backup from the server
+
         :param backup_file: The name of the backup file
         :param download_path: The path to download the backup file to (default: "./data")
         :param overwrite: If True, overwrite the file if it already exists (default: False)
         :return: Download backup response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/download_backup")
         request_params = {"params": {"backup_file": backup_file}}
@@ -314,77 +331,94 @@
             f.write(res.content)
         return res
 
     @staticmethod
     def upload_backup(file_path: str) -> requests.Response:
         """
         Upload a backup to the server
+
         :param file_path: The path to the backup file
         :return: Upload backup response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/upload_backup")
         res = OrcaClient._orca_request("POST", url, file_path=file_path)
         return res
 
     @staticmethod
     def delete_backup(backup_file_name: str) -> requests.Response:
         """
         Delete a backup from the server
+
         :param backup_file_name: The name of the backup file
         :return: Delete backup response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/delete_backup")
         request_params = {"params": {"backup_file_name": backup_file_name}}
         res = OrcaClient._orca_request("DELETE", url, request_params)
         return res
 
     @staticmethod
     def list_databases() -> list[str]:
         """
         List all the databases on the server
+
         :return: List of database names
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/list_databases")
         res = OrcaClient._orca_request("GET", url)
         return res.json()["databases"]
 
     @staticmethod
     def list_tables(db_name: str) -> list[str]:
         """
         List all the tables in the database
+
         :param db_name: The name of the database
         :return: List of table names
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/get_tables")
         request_params = {"params": {"db_name": db_name}}
         res = OrcaClient._orca_request("GET", url, request_params)
         return res.json()["tables"]
 
     @staticmethod
     def table_info(db_name: str, table_name: str) -> dict[str, Any]:
         """
         Get the information about a table
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :return: Table information
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/table_info")
         request_params = {"params": {"db_name": db_name, "table_name": table_name}}
         res = OrcaClient._orca_request("GET", url, request_params)
         return res.json()
 
     @staticmethod
+    def healthcheck() -> dict[str, Any]:
+        """
+        Perform a healthcheck on the server
+
+        :return: Healthcheck response
+        """
+        url = os.path.join(OrcaClient.BASE_URL, "v1/healthcheck")
+        res = OrcaClient._orca_request("GET", url)
+        return res.json()
+
+    @staticmethod
     def create_table(
         db_name: str,
         table_name: str,
         table_schema: list[dict[str, Any]],
         if_table_exists: TableCreateMode = TableCreateMode.ERROR_IF_TABLE_EXISTS,
     ) -> requests.Response:
         """
         Create a new table in the database
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :param table_schema: The schema of the table
         :param if_table_exists: What to do if the table already exists (default: TableCreateMode.ERROR_IF_TABLE_EXISTS)
         :return: Create table response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/create_table")
@@ -406,14 +440,15 @@
         table_name: str,
         rows: list[RowDict],
         files: list[tuple[str, IO[bytes]]],
         api_version: str | None = None,
     ) -> requests.Response:
         """
         Insert rows into the table
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :param rows: The rows to insert
         :param files: The files to upload
         :param api_version: The api version to use (optional)
         :return: Insert response
         """
@@ -442,14 +477,15 @@
         row: RowDict,
         filter: Any,
         files: list[tuple[str, IO[bytes]]],
         api_version: str | None = None,
     ) -> requests.Response:
         """
         Update a row in the table
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :param row: The row to update
         :param filter: The filter to apply
         :param files: The files to upload
         :param api_version: The api version to use (optional)
         :return: Update response
@@ -479,14 +515,15 @@
         rows: list[RowDict],
         key_columns: list[str],
         files: list[tuple[str, IO[bytes]]],
         api_version: str | None = None,
     ) -> requests.Response:
         """
         Upsert rows into the table
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :param rows: The rows to upsert
         :param key_columns: The key columns to use for the upsert
         :param files: The files to upload
         :param api_version: The api version to use (optional)
         :return: Upsert response
@@ -508,14 +545,15 @@
         res = OrcaClient._orca_request("POST", url, request_params)
         return res
 
     @staticmethod
     def delete(db_name: str, table_name: str, filter: Any) -> requests.Response:
         """
         Delete rows from the table
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :param filter: The filter to apply
         :return: Delete response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/delete")
         request_params = {
@@ -532,14 +570,15 @@
         new_col: list[str],
         dtype: list[str],
         notnull: list[bool],
         unique: list[bool],
     ) -> requests.Response:
         """
         Add a new column to the table
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :param new_col: The name of the new column
         :param dtype: The data type of the new column
         :param notnull: If the new column is not null
         :param unique: If the new column is unique
         :return: Add column response
@@ -561,14 +600,15 @@
     def drop_column(
         db_name: str,
         table_name: str,
         col_names: list[str],
     ) -> requests.Response:
         """
         Drop a column from the table
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :param col_names: The name of the column to drop
         :return: Drop column response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/drop_column")
         request_params = {
@@ -579,14 +619,15 @@
         res = OrcaClient._orca_request("DELETE", url, request_params)
         return res
 
     @staticmethod
     def drop_table(db_name: str, table_name: str, error_if_not_exists: bool = True) -> requests.Response:
         """
         Drop a table from the database
+
         :param db_name: The name of the database
         :param table_name: The name of the table
         :param error_if_not_exists: If True, raise an error if the table does not exist (default: True)
         :return: Drop table response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/drop_table")
         request_params = {
@@ -600,14 +641,15 @@
         res = OrcaClient._orca_request("DELETE", url, request_params)
         return res
 
     @staticmethod
     def drop_index(db_name: str, index_name: str) -> requests.Response:
         """
         Drop an index from the database
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :return: Drop index response
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/drop_index")
         request_params = {
             "params": {"db_name": db_name, "index_name": index_name},
@@ -622,32 +664,38 @@
         table: "TableHandle",  # noqa: F821
         columns: Optional[list[ColumnName]] = None,
         limit: Optional[int] = None,
         filter: Optional[ApiFilter] = None,
         order_by_columns: Optional[OrderByColumns] = None,
         default_order: Order = Order.ASCENDING,
         api_version: str | None = None,
+        use_msgpack: bool = True,
     ) -> TableSelectResponse:
         """
         Perform a select query on the table
+
         :param table: The TableHandle for the table we're querying
         :param columns: The columns to select. If None, all columns are selected (default: None)
         :param limit: The maximum number of rows to return (default: None)
         :param filter: The filter to apply to the query (default: None)
         :param order_by_columns: The columns to order by. If None, no order is applied. (default: None)
         :param default_order: The default order to use if no order is specified. Defaults to ascending. (default: Order.ASCENDING)
         :param api_version: The api version to use (default: None)
         :return: The response from the select query
 
         Example:
-        >>> OrcaClient.select(OrcaTableHandle("my_db", "my_table"),
-                               columns=["col1", "col2"],
-                               limit=100,
-                               filter={"col1": {"$gt": 10}},
-                               order_by_columns=["col1", ("col2", Order.DESCENDING)])
+
+        .. code-block:: python
+
+            >>> OrcaClient.select(OrcaTableHandle("my_db", "my_table"),
+                                    columns=["col1", "col2"],
+                                    limit=100,
+                                    filter={"col1": {"$gt": 10}},
+                                    order_by_columns=["col1", ("col2", Order.DESCENDING)])
+
         """
         url = os.path.join(
             OrcaClient.BASE_URL,
             f"{api_version}/select/db/{table.db_name}/{table.table_name}",
         )
         params = SimpleTableQueryRequest(
             columns=columns,
@@ -656,36 +704,41 @@
             order_by_columns=order_by_columns,
             default_order=default_order,
         )
         request = {
             "params": {},
             "json": params.dict(by_alias=True, exclude_unset=True),
         }
+
+        if not use_msgpack:
+            request["headers"] = {"Accept": "application/json"}
+
         response = OrcaClient._orca_request("POST", url, request)
-        if api_version == "v1":
-            # v1 doesn't support msgpack encoding, so we just return response.json()
+
+        if response.headers["Content-Type"] == "application/json":
             content = response.json()
-        elif api_version == "v2":
+        elif response.headers["Content-Type"] == "application/msgpack":
             content = msgpack.unpackb(response.content, object_hook=decode_ndarray, raw=False)
         else:
-            raise ValueError(f"Unsupported api version: {api_version}")
+            raise ValueError(f"Unsupported content type: {response.headers['Content-Type']}")
 
         col_name_to_type = {
             col_name: OrcaTypeHandle.from_string(table.columns[col_name].dtype) for col_name in table.columns
         }
 
         for row in content["rows"]:
             OrcaClient._deserialize_column_value_dict(col_name_to_type, row["column_values"])
 
         return content
 
     @staticmethod
     def _deserialize_column_value(col_type: OrcaTypeHandle, value: Any) -> Any:
         """
         Deserialize a single column value using the column's data type
+
         :param col_type: The column's data type
         :param value: The value to deserialize
         :return: The deserialized value
 
         NOTE: This function should not be called directly. It is used internally by the OrcaClient class.
         """
         if not isinstance(col_type, CustomSerializable):
@@ -693,30 +746,35 @@
         assert isinstance(value, dict)
         return col_type.msgpack_deserialize(value)
 
     @staticmethod
     def _deserialize_column_value_dict(col_name_to_type: dict[ColumnName, OrcaTypeHandle], row_values: RowDict) -> None:
         """
         Deserialize a dictionary of column values using the given type dictionary
+
         NOTE: This updates the dictionary in place!!
+
         This is used to deserialize the results of select
+
         :param col_name_to_type: A dictionary of column names to their data types
         :param row_values: The dictionary of column values to deserialize
 
         NOTE: This function should not be called directly. It is used internally by the OrcaClient class.
         """
         for col_name, col_type in col_name_to_type.items():
             if col_name in row_values:
                 row_values[col_name] = OrcaClient._deserialize_column_value(col_type, row_values[col_name])
 
     @staticmethod
     def _deserialize_column_value_list(ordered_type_list: list[OrcaTypeHandle], value_list: list[Any]) -> list[Any]:
         """
         Deserialize a list of column values using the given type list
+
         This is used to deserialize the results of scan_index and vector_scan_index
+
         :param ordered_type_list: A list of column data types
         :param value_list: The list of column values to deserialize
         :return: The deserialized list of column values
 
         NOTE: This function should not be called directly. It is used internally by the OrcaClient class.
         """
         assert len(ordered_type_list) == len(value_list)
@@ -724,14 +782,15 @@
 
     @staticmethod
     def _create_index_v1(
         db_name: str, index_name: str, table_name: str, column: str, index_type: str
     ) -> requests.Response:
         """
         Create a new index (v1)
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :param table_name: The name of the table
         :param column: The name of the column to index
         :param index_type: The type of the index
         :return: Create index response (requests.Response)
 
@@ -751,14 +810,15 @@
 
         return OrcaClient._orca_request("POST", url, request_params, verbose=False)
 
     @staticmethod
     def _create_index_v2(db_name: str, index_name: str, table_name: str, column: str, index_type: str) -> IndexHandle:
         """
         Create a new index (v2)
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :param table_name: The name of the table
         :param column: The name of the column to index
         :param index_type: The type of the index
         :return: Create index response (IndexHandle)
 
@@ -789,14 +849,15 @@
         table_name: str,
         column: str,
         index_type: str,
         embedding_model: EmbeddingModel | None = None,
     ) -> IndexHandle:
         """
         Create a new index (v3)
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :param table_name: The name of the table
         :param column: The name of the column to index
         :param index_type: The type of the index
         :param embedding_model: The name of the embedding model (optional) (roberta, sentence_transformer)
         :return: Create index response (IndexHandle)
@@ -837,14 +898,15 @@
         column: str,
         index_type: str,
         api_version: str | None = None,
         embedding_model: EmbeddingModel | None = None,
     ) -> IndexHandle:
         """
         Create a new index
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :param table_name: The name of the table
         :param column: The name of the column to index
         :param index_type: The type of the index
         :param api_version: The api version to use (optional)
         :param embedding_model: The name of the embedding model (optional) (roberta, sentence_transformer)
@@ -859,27 +921,29 @@
             return call_correct_version(db_name, index_name, table_name, column, index_type, embedding_model)
         return call_correct_version(db_name, index_name, table_name, column, index_type)
 
     @staticmethod
     def get_index_status(db_name: str, index_name: str) -> dict[str, Any]:
         """
         Get the status of an index
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :return: Get index status response
         """
         url = os.path.join(OrcaClient.BASE_URL, f"v1/get_index_status/{db_name}/{index_name}")
         request_params = {"params": {}}
         res = OrcaClient._orca_request("GET", url, request_params)
         return res.json()
 
     @staticmethod
     def _get_index_v1(db_name: str, index_name: str):
         """
         Get the details of an index (v1)
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :return: The index details (v1) (IndexHandle)
 
         NOTE: This function should not be called directly. It is used internally by the OrcaClient class.
         """
         url = os.path.join(OrcaClient.BASE_URL, f"v1/db/index_info/{db_name}/{index_name}")
@@ -889,14 +953,15 @@
         json["embedding_type"] = OrcaTypeHandle.from_string(embed_type) if embed_type else None
         return IndexHandle(**json, artifact_columns={})
 
     @staticmethod
     def _get_index_v2(db_name: str, index_name: str):
         """
         Get the details of an index (v2)
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :return: The index details (v2) (IndexHandle)
 
         NOTE: This function should not be called directly. It is used internally by the OrcaClient class.
         """
         url = os.path.join(OrcaClient.BASE_URL, f"v2/db/index_info/{db_name}/{index_name}")
@@ -906,14 +971,15 @@
         json["embedding_type"] = OrcaTypeHandle.from_string(embed_type) if embed_type else None
         return IndexHandle(**json)
 
     @staticmethod
     def _get_index_v3(db_name: str, index_name: str):
         """
         Get the details of an index (v3)
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :return: The index details (v3) (IndexHandle)
 
         NOTE: This function should not be called directly. It is used internally by the OrcaClient class.
         """
         url = os.path.join(OrcaClient.BASE_URL, f"v2/db/index_info/{db_name}/{index_name}")
@@ -929,15 +995,16 @@
         "v3": _get_index_v3,
     }
 
     @staticmethod
     @default_api_version_key("index.get")
     def get_index(db_name: str, index_name: str, api_version: str | None = None) -> IndexHandle:
         """
-         Get the details of an index
+        Get the details of an index
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :return: The index details
 
         """
         call_correct_version = OrcaClient.get_index_strategy.get(api_version, None)
         if call_correct_version is None:
@@ -951,14 +1018,15 @@
         query: Any,
         limit: int,
         columns: Optional[list[str]] = None,
         filter: Optional[str] = None,
     ) -> dict[str, Any]:
         """
         Scan an index
+
         :param db: The OrcaDatabase object
         :param index_name: The name of the index
         :param query: The query to apply
         :param limit: The maximum number of rows to return
         :param columns: The columns to return (optional)
         :param filter: The filter to apply (optional)
         :return: The response from the scan index query
@@ -988,14 +1056,15 @@
         query: Any,
         limit: int,
         columns: Optional[list[str]] = None,
         filter: Optional[str] = None,
     ) -> list[RowDict]:
         """
         Scan an index
+
         :param db: The OrcaDatabase object
         :param index_name: The name of the index
         :param query: The query to apply
         :param limit: The maximum number of rows to return
         :param columns: The columns to return (optional)
         :param filter: The filter to apply (optional)
         :return: The response from the scan index query
@@ -1037,14 +1106,15 @@
         limit: int,
         columns: Optional[list[str]] = None,
         filter: Optional[str] = None,
         api_version: str | None = None,
     ) -> Any:
         """
         Scan an index
+
         :param db: The OrcaDatabase object
         :param index_name: The name of the index
         :param query: The query to apply
         :param limit: The maximum number of rows to return
         :param columns: The columns to return (optional)
         :param filter: The filter to apply (optional)
         :param api_version: The api version to use (optional)
@@ -1071,14 +1141,15 @@
         columns: Optional[list[str]] = None,
         filter: Optional[str] = None,
         curate_run_ids: Optional[list[int]] = None,
         curate_layer_name: Optional[str] = None,
     ) -> dict[str, Any]:
         """
         Scan a vector index
+
         :param table: The TableHandle for the table we're querying
         :param index_name: The name of the index
         :param query: The query to apply
         :param limit: The maximum number of rows to return
         :param columns: The columns to return (optional)
         :param filter: The filter to apply (optional)
         :param curate_run_ids: The curate run ids to apply (optional)
@@ -1113,14 +1184,15 @@
         columns: Optional[list[str]] = None,
         filter: Optional[str] = None,
         curate_run_ids: Optional[list[int]] = None,
         curate_layer_name: Optional[str] = None,
     ) -> "BatchedVectorScanResult_V2":  # noqa: F821
         """
         Scan a vector index
+
         :param table: The TableHandle for the table we're querying
         :param index_name: The name of the index
         :param query: The query to apply
         :param limit: The maximum number of rows to return
         :param columns: The columns to return (optional)
         :param filter: The filter to apply (optional)
         :param curate_run_ids: The curate run ids to apply (optional)
@@ -1171,14 +1243,15 @@
         limit: int,
         columns: Optional[list[str]] = None,
         filter: Optional[str] = None,
         curate_run_ids: Optional[list[int]] = None,
         curate_layer_name: Optional[str] = None,
     ) -> "BatchedScanResult":  # noqa: F821
         """Performs a vector scan index query using the v3 api version.
+
         NOTE: This version-specific method is used to handle the differences in the response format between api versions,
         and is not called directly by FastAPI.
         """
         from orcalib.batched_scan_result import BatchedScanResult
 
         url = os.path.join(OrcaClient.BASE_URL, f"v3/db/vector_scan_index/{table.db_name}/{index_name}")
         request_params = {
@@ -1222,14 +1295,15 @@
         filter: Optional[str] = None,
         curate_run_ids: Optional[list[int]] = None,
         curate_layer_name: Optional[str] = None,
         api_version: str | None = None,
     ) -> "BatchedScanResult":  # noqa: F821
         """
         Scan a vector index
+
         :param table: The TableHandle for the table we're querying
         :param index_name: The name of the index
         :param query: The query to apply
         :param limit: The maximum number of rows to return
         :param columns: The columns to return (optional)
         :param filter: The filter to apply (optional)
         :param curate_run_ids: The curate run ids to apply (optional)
@@ -1261,14 +1335,15 @@
         num_memories: int,
         query_columns: list[str] | str,
         page_size: int = 100,
         page_index: int = 0,
     ) -> requests.Response:
         """
         Perform a full vector memory join
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :param memory_index_name: The name of the memory index
         :param num_memories: The number of memory indexes
         :param query_columns: The columns to query (or a single column)
         :param page_size: The size of the page to return (default: 100)
         :param page_index: The index of the page to return (default: 0)
@@ -1292,14 +1367,15 @@
 
         return OrcaClient._orca_request("POST", url, request_params)
 
     @staticmethod
     def get_index_values(db_name: str, index_name: str) -> requests.Response:
         """
         Get the values of an index
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :return: The response from the get index values query
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/dump_index")
         request_params = {
             "params": {"db_name": db_name, "index_name": index_name},
@@ -1312,14 +1388,15 @@
         db_name: str,
         index_name: str,
         page_index: int = 0,
         page_size: int = 100,
     ) -> requests.Response:
         """
         Get the values of an index paginated
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :param page_index: The index of the page to return (default: 0)
         :param page_size: The size of the page to return (default: 100)
         :return: The response from the get index values paginated query
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/dump_index_paginated")
@@ -1334,14 +1411,15 @@
 
         return OrcaClient._orca_request("GET", url, request_params)
 
     @staticmethod
     def get_index_table(db_name: str, index_name: str) -> requests.Response:
         """
         Get the table of an index
+
         :param db_name: The name of the database
         :param index_name: The name of the index
         :return: The response from the get index table query
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/get_index_table")
         request_params = {
             "params": {"db_name": db_name, "index_name": index_name},
@@ -1349,14 +1427,15 @@
 
         return OrcaClient._orca_request("GET", url, request_params)
 
     @staticmethod
     def run_sql(db_name: str, query: str, params: list[None | int | float | bytes | str] = []) -> list[dict[str, Any]]:
         """
         Run a SQL query
+
         :param db_name: The name of the database
         :param query: The SQL query
         :param params: The parameters for the query
         :return: The response from the SQL query
         """
         url = os.path.join(OrcaClient.BASE_URL, "experimental/sql")
         request_params = {
@@ -1366,28 +1445,30 @@
 
         return OrcaClient._orca_request("POST", url, request_params).json()["rows"]
 
     @staticmethod
     def encode_roberta(strings: list[str]) -> list[dict[str, Any]]:
         """
         Encode a list of strings using the Roberta model
+
         :param strings: The list of strings to encode
         :return: The response from the encode query
         """
         url = os.path.join(OrcaClient.BASE_URL, "experimental/encode/roberta")
         request_params = {
             "json": {"strings": strings},
         }
 
         return OrcaClient._orca_request("POST", url, request_params).json()
 
     @staticmethod
     def encode_sentence_transformer(strings: list[str]) -> list[dict[str, Any]]:
         """
         Encode a list of strings using the Sentence Transformer model
+
         :param strings: The list of strings to encode
         :return: The response from the encode query
         """
         url = os.path.join(OrcaClient.BASE_URL, "experimental/encode/sentence_transformer")
         request_params = {
             "json": {"strings": strings},
         }
@@ -1397,19 +1478,20 @@
     @staticmethod
     def init_forward_pass(
         db_name: str,
         model_id: str,
         batch_size: int,
         model_version: Optional[str] = None,
         seq_id: Optional[UUID] = None,
-        tags: Optional[list[str]] = None,
+        tags: Optional[set[str]] = None,
         metadata: Optional[dict[str, Any]] = None,
     ) -> list[int]:
         """
         Initialize a forward pass
+
         :param db_name: The name of the database
         :param model_id: The id of the model
         :param batch_size: The batch size
         :param model_version: The version of the model (optional)
         :param seq_id: The sequence id for the forward pass (optional)
         :param tags: The tags for the forward pass (optional)
         :param metadata: The metadata for the forward pass (optional)
@@ -1429,14 +1511,15 @@
         }
         return OrcaClient._orca_request("POST", url, request_params).json()
 
     @staticmethod
     def prune_data(db_name: str, model_id: str, filters: list[Any]) -> list[int]:
         """
         Prune data
+
         :param db_name: The name of the database
         :param model_id: The id of the model
         :param filters: The filters
         :return: The response from the prune data query
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/curate/init_forward_pass")
         request_params = {
@@ -1449,14 +1532,15 @@
     def record_model_scores(
         db_name: str,
         run_ids: list[int],
         scores: list[float],
     ) -> dict[str, Any]:
         """
         Record model scores
+
         :param db_name: The name of the database
         :param run_ids: The run ids
         :param scores: The scores
         :return: The response from the record model scores query
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/curate/record_scores")
         request_params = {
@@ -1473,14 +1557,15 @@
         db_name: str,
         run_ids: list[int],
         inputs: list[Any],
         outputs: list[Any],
     ) -> dict[str, Any]:
         """
         Record model input output
+
         :param db_name: The name of the database
         :param run_ids: The run ids
         :param inputs: The inputs
         :param outputs: The outputs
         :return: The response from the record model input output query
         """
         url = os.path.join(OrcaClient.BASE_URL, "v1/curate/record_model_in_out")
```

### Comparing `orcalib-0.0.56/orcalib/client_data_model.py` & `orcalib-0.0.57/orcalib/client_data_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Any, Optional, TypedDict, Union
+from typing import Any, Optional, TypedDict
 
 import numpy as np
 import pandas
 from orca_common import ColumnName, Order, OrderByColumns, RowDict
+from orca_common.api_types import OperationEnum
 from pydantic import BaseModel
 
 
 class ApiFilter(BaseModel):
-    """Client-side model of a filter that's used with calls to `select(...)`
-    NOTE: It doesn't look like we're actually using filters on the client-side anywhere.
-    """
+    """Client-side model of a filter that's used with calls to `select(...)`"""
 
-    op: str
-    args: list[Union[str, int, float, bool, "ApiFilter"]]
+    op: OperationEnum
+    args: tuple[str, str | int | float | bool] | list["ApiFilter"]
 
 
 # Type alias for various types of row data that can be passed to the insert/update/upsert function.
 RowData = RowDict | pandas.DataFrame | list[RowDict]
 OrderByColumn = ColumnName | tuple[ColumnName, Order]
 
 
 class SimpleTableQueryRequest(BaseModel):
     """Client-side model of the request to the `simple_table_query` endpoint.
+
     NOTE: This is currently a duplicate of the server's model, but we want them to
     remain separate for now, since the client's model may change in the future.
     """
 
     columns: Optional[list[str]] = None
     limit: Optional[int] = None
     filter: Optional[ApiFilter] = None
@@ -45,14 +45,16 @@
 
     status_code: int
     rows: list[TableRowResponse]
 
 
 def decode_ndarray(obj: Any) -> Any:
     """Decode a JSON object that was encoded with `encode_ndarray`.
+
     TODO: This needs to be generalized to use the type handles to decode column types.
+
     :param obj: The object to decode
     :return: The decoded object
     """
     if "__ndarray__" in obj:
         return np.array(obj["__ndarray__"])
     return obj
```

### Comparing `orcalib-0.0.56/orcalib/data_classes.py` & `orcalib-0.0.57/orcalib/data_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 
     vec: np.ndarray
     extra: list[Any]
 
     def __str__(self) -> str:
         """
         Return a string representation of this vector scan result.
+
         :return: String representation
         """
         return f"VectorScanResult({','.join([str(item) for item in self.extra])})"
 
     def __repr__(self) -> str:
         """
         Return a string representation of this vector scan result.
+
         :return: String representation
         """
         return self.__str__()
```

### Comparing `orcalib-0.0.56/orcalib/database.py` & `orcalib-0.0.57/orcalib/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Optional
 
 import orjson
 import pandas
 import requests
 import torch
-import tqdm
+from tqdm.auto import trange
 from orca_common import EmbeddingModel, TableCreateMode
 from transformers import AutoModel, AutoTokenizer
 
 from orcalib.client import OrcaClient
 from orcalib.exceptions import OrcaException
 from orcalib.index_handle import IndexHandle
 from orcalib.index_query import DefaultIndexQuery, VectorIndexQuery
@@ -19,103 +19,113 @@
 class OrcaDatabase:
     name: str
     _default_instance = None
 
     def __init__(self, name: str):
         """
         Create a new OrcaDatabase object
+
         :param name: name of the database
         """
         self.name = name
         OrcaClient.create_database(name)
         self.tables = OrcaClient.list_tables(name)
         self.tokenizer = None
         self.model = None
 
     def _load_model_and_tokenizer(self) -> tuple[AutoTokenizer, AutoModel]:
         """
         Load the default model and tokenizer
+
         :return: tokenizer, model
 
         NOTE: This method should not be called directly. It is used internally by the library to load the default model and tokenizer.
         """
         if self.tokenizer is None or self.model is None:
             self.tokenizer = AutoTokenizer.from_pretrained("sentence-transformers/multi-qa-mpnet-base-dot-v1")
             self.model = AutoModel.from_pretrained("sentence-transformers/multi-qa-mpnet-base-dot-v1")  # .to("cuda")
         return self.tokenizer, self.model
 
     def __contains__(self, table_name: str) -> bool:
         """
         Check if a table exists in the database
+
         :param table_name: name of the table
         """
         return table_name in self.tables
 
     def __getitem__(self, table_name: str) -> TableHandle:
         """
         Get a handle to a table by name
+
         :param table_name: name of the table
         :return: TableHandle object
         """
         if table_name not in self.tables:
             raise ValueError(f"Table {table_name} not found in database {self.name}")
         return TableHandle(self.name, table_name)
 
     def get_table(self, table_name: str) -> TableHandle:
         """
         Get a handle to a table by name
+
         :param table_name: name of the table
         :return: TableHandle object
         """
         return self.__getitem__(table_name)
 
     @classmethod
     def get_default_instance(cls) -> "OrcaDatabase":
         """
         Get the default instance of OrcaDatabase
+
         :return: OrcaDatabase object
         """
         if cls._default_instance is None:
             cls._default_instance = cls("default")
         return cls._default_instance
 
     @staticmethod
     def list_databases() -> list[str]:
         """
         List all databases on the server
+
         :return: list of database names
         """
         return OrcaClient.list_databases()
 
     @classmethod
     def is_server_up(cls) -> bool:
         """
         Check if the server is up and running
+
         :return: True if server is up, False otherwise
         """
         try:
             cls.list_databases()
             return True
         except Exception:
             return False
 
     @classmethod
     def drop_database(cls, db: "str | OrcaDatabase", ignore_db_not_found: bool = False) -> None:
         """
         Drops a database by name or using the OrcaDatabase object
+
         :param db: name of the database or OrcaDatabase object to drop
         :param ignore_db_not_found: if True, ignore error if database doesn't exist and continue with the operation anyway (default: False)
         """
         db_name = db.name if isinstance(db, OrcaDatabase) else db
         OrcaClient.drop_database(db_name, ignore_db_not_found)
 
     @classmethod
     def exists(cls, db: "str | OrcaDatabase") -> bool:
         """
         Checks if a database exists by name or using the OrcaDatabase object
+
         :param db: name of the database or OrcaDatabase object
         :return: True if database exists, False otherwise
         """
         db_name = db.name if isinstance(db, OrcaDatabase) else db
         return OrcaClient.database_exists(db_name)
 
     @staticmethod
@@ -131,14 +141,15 @@
         """
         OrcaClient.restore_backup(target_db_name, backup_name, checksum=checksum)
         return OrcaDatabase(target_db_name)
 
     def list_tables(self) -> list[str]:
         """
         List all tables in the database
+
         :return: list of table names
         """
         return OrcaClient.list_tables(self.name)
 
     def backup(self) -> tuple[str, str]:
         """Create a backup of the database
 
@@ -146,39 +157,43 @@
         """
         res = OrcaClient.create_backup(self.name)
         return res["backup_name"], res["checksum"]
 
     @staticmethod
     def download_backup(backup_file_name: str) -> requests.Response:
         """Downloads the backup of the database
+
         :param backup_file_name: name of the backup file
         :return: backed up file
         """
         return OrcaClient.download_backup(backup_file_name)
 
     @staticmethod
     def upload_backup(file_path: str) -> requests.Response:
         """Uploads tar file of the database
+
         :param file_path: path to the tar file
         :return: Upload response
         """
         return OrcaClient.upload_backup(file_path)
 
     @staticmethod
     def delete_backup(backup_file_name: str) -> requests.Response:
         """
         Delete backup file
+
         :param backup_file_name: name of the backup file
         :return: delete response
         """
         return OrcaClient.delete_backup(backup_file_name)
 
     def default_vectorize(self, text: str) -> list[float]:
         """
         Vectorize text using the default model
+
         :param text: text to vectorize
         :return: list of floats
         """
         tokenizer, model = self._load_model_and_tokenizer()
         encoded_input = tokenizer(text, return_tensors="pt", padding="max_length", truncation=True)  # .to("cuda")
         output = model(**encoded_input)
         return output.pooler_output.tolist()[0]
@@ -187,14 +202,15 @@
         self,
         table_name: str,
         if_table_exists: TableCreateMode = TableCreateMode.ERROR_IF_TABLE_EXISTS,
         **columns: OrcaTypeHandle,
     ) -> TableHandle:
         """
         Create a table in the database
+
         :param table_name: name of the table
         :param if_table_exists: what to do if the table already exists
         :param columns: column names and types
         :return: TableHandle object
         """
         # We will deal with the case where the table already exists in server.
         self._create_table(table_name, if_table_exists, **columns)
@@ -204,14 +220,15 @@
         self,
         table_name: str,
         if_table_exists: TableCreateMode,
         **columns: OrcaTypeHandle,
     ) -> TableHandle:
         """
         Create a table in the database
+
         :param table_name: name of the table
         :param if_table_exists: what to do if the table already exists
         :param columns: column names and types
         :return: TableHandle object
 
         NOTE: This method should not be called directly. It is used internally by the library to create a table in the database.
         """
@@ -237,14 +254,15 @@
         index_type: str,
         error_if_exists: bool = True,
         api_version: str | None = None,
         embedding_model: EmbeddingModel | None = None,
     ) -> IndexHandle:
         """
         Create an index on a table
+
         :param index_name: name of the index
         :param table_name: name of the table
         :param column: name of the column
         :param index_type: type of the index
         :param error_if_exists: if True, raise an error if the index already exists (default: True)
         :param api_version: API version to use (default: None)
         :param embedding_model: embedding model to use (default: None) (roberta, sentence_transformer) (only for text and document indexes)
@@ -267,25 +285,27 @@
         except OrcaException as e:
             if error_if_exists:
                 raise e
 
     def get_index_status(self, index_name: str) -> dict[str, Any]:
         """
         Get the status of an index
+
         :param index_name: name of the index
         :return: status of the index
         """
         try:
             return OrcaClient.get_index_status(db_name=self.name, index_name=index_name)
         except OrcaException as e:
             raise e
 
     def get_index(self, index_name: str) -> IndexHandle:
         """
         Get a handle to an index by name
+
         :param index_name: name of the index
         :return: IndexHandle object
         """
         response = OrcaClient.get_index(self.name, index_name)
         return response
 
     def create_vector_index(
@@ -294,14 +314,15 @@
         table_name: str,
         column: str,
         error_if_exists: bool = True,
         api_version: str | None = None,
     ) -> IndexHandle:
         """
         Create a vector index on a table
+
         :param index_name: name of the index
         :param table_name: name of the table
         :param column: name of the column
         :param error_if_exists: if True, raise an error if the index already exists (default: True)
         :param api_version: API version to use (default: None)
         """
         return self._create_index(index_name, table_name, column, "vector", error_if_exists, api_version=api_version)
@@ -313,14 +334,15 @@
         column: str,
         error_if_exists: bool = True,
         embedding_model: EmbeddingModel | None = None,
         api_version: str | None = None,
     ) -> IndexHandle:
         """
         Create a document index on a table
+
         :param index_name: name of the index
         :param table_name: name of the table
         :param column: name of the column
         :param error_if_exists: if True, raise an error if the index already exists (default: True)
         :param embedding_model: embedding model to use (default: None) (roberta, sentence_transformer)
         :param api_version: API version to use (default: None)
 
@@ -343,14 +365,15 @@
         column: str,
         error_if_exists: bool = True,
         embedding_model: EmbeddingModel | None = None,
         api_version: str | None = None,
     ) -> IndexHandle:
         """
         Create a text index on a table
+
         :param index_name: name of the index
         :param table_name: name of the table
         :param column: name of the column
         :param error_if_exists: if True, raise an error if the index already exists (default: True)
         :param embedding_model: embedding model to use (default: None) (roberta, sentence_transformer)
         :param api_version: API version to use (default: None)
 
@@ -372,37 +395,40 @@
         table_name: str,
         column: str,
         error_if_exists: bool = True,
         api_version: str | None = None,
     ) -> IndexHandle:
         """
         Create a btree index on a table
+
         :param index_name: name of the index
         :param table_name: name of the table
         :param column: name of the column
         :param error_if_exists: if True, raise an error if the index already exists (default: True)
         :param api_version: API version to use (default: None)
         """
         return self._create_index(index_name, table_name, column, "btree", error_if_exists, api_version=api_version)
 
     def drop_index(self, index_name: str, error_if_not_exists: bool = True) -> None:
         """
         Drop an index from the database
+
         :param index_name: name of the index
         :param error_if_not_exists: if True, raise an error if the index doesn't exist (default: True)
         """
         try:
             OrcaClient.drop_index(self.name, index_name)
         except OrcaException as e:
             if error_if_not_exists:
                 raise e
 
     def drop_table(self, table_name: str, error_if_not_exists: bool = True) -> None:
         """
         Drop a table from the database
+
         :param table_name: name of the table
         :param error_if_not_exists: if True, raise an error if the table doesn't exist (default: True)
         """
         OrcaClient.drop_table(self.name, table_name, error_if_not_exists)
         if table_name in self.tables:
             self.tables.remove(table_name)
 
@@ -411,14 +437,15 @@
         index_name: str,
         query: list[float],
         limit: int,
         columns: Optional[list[str]] = None,
     ) -> list[tuple[list[float], Any]]:
         """
         Search the memory for a given query
+
         :param index_name: name of the index
         :param query: query vector
         :param limit: maximum number of results to return
         :param columns: optional list of columns to return in the result (default: None)
         :return: list of tuples containing (vector, extra)
         """
         res = OrcaClient.scan_index(
@@ -433,14 +460,15 @@
     def scan_index(
         self,
         index_name: str,
         query: Any,
     ) -> DefaultIndexQuery:
         """
         Scan an index for a given query
+
         :param index_name: name of the index
         :param query: query
         :return: DefaultIndexQuery object
         """
         return DefaultIndexQuery(
             db_name=self.name,
             primary_table=self._get_index_table(index_name),
@@ -451,14 +479,15 @@
     def vector_scan_index(
         self,
         index_name: str,
         query: Any,
     ) -> VectorIndexQuery:
         """
         Scan an index for a given query
+
         :param index_name: name of the index
         :param query: query
         :return: VectorIndexQuery object
         """
         return VectorIndexQuery(
             db_name=self.name,
             primary_table=self._get_index_table(index_name),
@@ -474,14 +503,15 @@
         num_memories: int,
         query_columns: list[str],
         page_index: int,
         page_size: int,
     ) -> dict[str, list[tuple[list[float], Any]]]:
         """
         Join a vector index with a memory index
+
         :param index_name: name of the index
         :param memory_index_name: name of the memory index
         :param num_memories: number of memories to join
         :param query_columns: list of columns to return
         :param page_index: page index
         :param page_size: page size
         :return: dictionary containing the joined vectors and extra columns
@@ -497,14 +527,15 @@
         )
 
         return orjson.loads(res.text)
 
     def _get_index_values(self, index_name: str) -> dict[int, list[float]]:
         """
         Get all values for an index
+
         :param index_name: name of the index
         :return: dictionary containing the index values
 
         NOTE: This method should not be called directly. It is used internally by the library to get all values for an index.
         """
         res = OrcaClient.get_index_values(self.name, index_name).json()
         return {int(k): v for k, v in res.items()}
@@ -512,14 +543,15 @@
     def _get_index_values_paginated(
         self,
         index_name: str,
         page_size: int = 1000,
     ) -> dict[int, list[float]]:
         """
         Get all values for an index, paginated
+
         :param index_name: name of the index
         :param page_size: page size (default: 1000)
         :return: dictionary containing the index values
 
         NOTE: This method should not be called directly. It is used internally by the library to get all values for an index.
         """
         page_index = 0
@@ -534,39 +566,41 @@
 
         for v in res["items"]:
             result[int(v[0])] = v[1]
 
         if num_pages > 1:
             print(f"Fetching vectors for index {index_name} ({num_pages} pages)")
 
-            for page_index in tqdm.tqdm(range(1, num_pages)):
+            for page_index in trange(1, num_pages):
                 res = OrcaClient.get_index_values_paginated(
                     self.name, index_name, page_index=page_index, page_size=page_size
                 ).json()
 
                 for v in res["items"]:
                     result[int(v[0])] = v[1]
 
         print(f"Finished fetching vectors for index {index_name} ({num_pages} pages)")
 
         return result
 
     def _get_index_table(self, index_name: str) -> TableHandle:
         """
         Get the table associated with an index
+
         :param index_name: name of the index
         :return: TableHandle object
 
         NOTE: This method should not be called directly. It is used internally by the library to get the table associated with an index.
         """
         return TableHandle(self.name, OrcaClient.get_index_table(self.name, index_name).json())
 
     def memory_layer(self, index_name: str) -> torch.nn.Module:
         """
         Create a memory layer for the index
+
         :param index_name: name of the index
         :return: torch.nn.Module object
         """
         return torch.nn.Sequential(
             torch.nn.Linear(768, 768),
             torch.nn.ReLU(),
             torch.nn.Linear(768, 768),
@@ -579,24 +613,26 @@
     def wrap_hf_model(self, index_name: str, model_name: str):
         pass
 
     def query(self, query: str, params: list[None | int | float | bytes | str] = []) -> pandas.DataFrame:
         """Send a read query to the database
 
         This cannot be used for inserting, updating, or deleting data.
+
         :param query: SQL query to run
         :param params: optional values to pass to a parametrized query (default: [])
         :return: pandas DataFrame containing the results
         """
         df = pandas.DataFrame(OrcaClient.run_sql(self.name, query, params))
         return df
 
     def record_model_scores(self, run_ids: list[int] | int, scores: list[float] | float) -> None:
         """
         Record model scores in the database
+
         :param run_ids: list of run IDs
         :param scores: list of scores
         """
         if isinstance(run_ids, int):
             run_ids = [run_ids]
             assert isinstance(scores, float), "Only a single score is allowed if a single run_id is provided"
             scores = [scores]
@@ -604,14 +640,15 @@
         OrcaClient.record_model_scores(self.name, run_ids, scores)
 
     def record_model_input_output(
         self, run_ids: list[int] | int, inputs: list[Any] | Any, outputs: list[Any] | Any
     ) -> None:
         """
         Record model input/output in the database
+
         :param run_ids: list of run IDs
         :param inputs: list of inputs
         :param outputs: list of outputs
         """
         if isinstance(run_ids, int):
             run_ids = [run_ids]
             assert not isinstance(inputs, list) and not isinstance(
@@ -621,36 +658,40 @@
             outputs = [outputs]
         assert isinstance(inputs, list) and isinstance(outputs, list)
         OrcaClient.record_model_input_output(self.name, run_ids, inputs, outputs)
 
     def __str__(self) -> str:
         """
         String representation of the database
+
         :return: String representation
         """
         return f"OrcaDatabase({self.name}) - Tables: {', '.join(self.tables)}"
 
     def __repr__(self) -> str:
         """
         String representation of the database
+
         :return: String representation
         """
         return self.__str__()
 
 
 def with_default_database_method(method: Any) -> Any:
     """
     Decorator to add the default database as the first argument to a method.
+
     :param method: method to decorate
     :return: decorated method
     """
 
     def wrapper(*args, **kwargs):
         """
         Wrapper function
+
         :param args: arguments
         :param kwargs: keyword arguments
         """
         default_database = OrcaDatabase.get_default_instance()
         return method(default_database, *args, **kwargs)
 
     return wrapper
```

### Comparing `orcalib-0.0.56/orcalib/exceptions.py` & `orcalib-0.0.57/orcalib/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 class OrcaException(Exception):
     """
     Base exception type of Orca
+
     :param message: The error message
     :param content: The http content of the request if available
     """
 
     def __init__(self, message, content=None):
         """
         :param message: The error message
```

### Comparing `orcalib-0.0.56/orcalib/file_ingestor.py` & `orcalib-0.0.57/orcalib/file_ingestor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from collections import Counter
 from typing import Any, cast
 from urllib.request import urlopen
 
 import numpy as np
 import pandas
 import pyarrow
-import tqdm
+from tqdm.auto import trange
 from orca_common import ColumnName, RowDict
 
 from orcalib.database import OrcaDatabase
 from orcalib.orca_types import (
     BoolT,
     DocumentT,
     DocumentTypeHandle,
@@ -52,14 +52,15 @@
         self._dataset = dataset
         self._auto_table = auto_table
         self._replace = replace
 
     def _schema_from_dataset(self, sample: RowDict) -> dict[ColumnName, OrcaTypeHandle]:
         """
         Infer schema from the dataset
+
         :param sample: Sample row
         :return: Schema
         """
         schema = {}
 
         for col in sample.keys():
             if isinstance(sample[col], str):
@@ -78,33 +79,35 @@
             else:
                 raise ValueError(f"Can't infer type for column {col}")
         return schema
 
     def _create_table(self) -> Any:
         """
         Create table
+
         :return: Table
 
         NOTE: This method should not be called directly. It is used internally.
         """
         if self._replace and self._auto_table and self._table_name in self._db.tables:
             self._db.drop_table(self._table_name)
         schema = self._schema_from_dataset(self._dataset[0])
         print(f"Creating table {self._table_name} with schema {schema}")
         return self._db.create_table(self._table_name, **schema)
 
     def dataframe_to_list(self, df: pandas.DataFrame) -> list[dict]:
         """
         Convert dataframe to list of dictionaries
+
         :param df: Dataframe
         :return: List of dictionaries
         """
         dataset = []
         columns = df.columns.values.tolist()
-        for i in tqdm.tqdm(range(len(df))):
+        for i in trange(len(df)):
             curr_row = df.iloc[i].tolist()
             for j in range(len(curr_row)):
                 # Process vectors and numpy integers
                 if isinstance(curr_row[j], str) and curr_row[j][0] == "[":
                     if curr_row[j][-1] != "]":
                         raise Exception("Incorrectly formatted list in CSV file")
                     curr_row[j] = [float(x.strip()) for x in curr_row[j][1 : len(curr_row[j]) - 1].split(",")]
@@ -114,14 +117,15 @@
                     curr_row[j] = list(curr_row[j])
             dataset.append(dict(zip(columns, curr_row)))
         return dataset
 
     def run(self, only_create_table: bool = False, skip_create_table: bool = False) -> Any:
         """
         Run ingestor
+
         :param only_create_table: Only create table and don't insert data (default: False)
         :param skip_create_table: Skip creating table if it doesn't exist (default: False)
         :return: Table
         """
         if self._auto_table and not skip_create_table:
             table = self._create_table()
         else:
```

### Comparing `orcalib-0.0.56/orcalib/hf_utils.py` & `orcalib-0.0.57/orcalib/hf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         candidates: list[list[int]],
         semantic_scores: list[float],
     ) -> tuple[
         dict[int, float], list[tuple[list[int], float]]
     ]:  # suffix max dict (token -> score), bag_of_words list (token list, score)
         """
         Get the weighted next tokens from memory
+
         :param q_tokens: Query tokens
         :param candidates: Candidates
         :param semantic_scores: Semantic scores
         :return: Weighted next tokens from memory
 
         NOTE: This method should not be called directly. It is used internally.
         """
@@ -92,14 +93,15 @@
     def __call__(
         self,
         input_ids: torch.Tensor,
         scores: torch.Tensor,
     ) -> torch.Tensor:
         """
         Call the processor
+
         :param input_ids: Input ids
         :param scores: Scores
         :return: Adjusted scores
         """
         bs = input_ids.shape[0]
         vocab_size = scores.shape[1]
 
@@ -180,25 +182,27 @@
             self._dataset = dataset
         self._auto_table = auto_table
         self._replace = replace
 
     def _create_table(self) -> TableHandle:
         """
         Create table
+
         :return: Table
 
         NOTE: This method should not be called directly. It is used internally.
         """
         if self._replace and self._auto_table and self._table_name in self._db.tables:
             self._db.drop_table(self._table_name)
         return self._db.create_table(self._table_name, **self._schema_from_dataset(self._dataset.select([0])[0]))  # type: ignore
 
     def run(self) -> TableHandle:
         """
         Run
+
         :return: Table
         """
         if self._auto_table:
             table = self._create_table()
         else:
             table = self._db[self._table_name]
         temp = cast(
@@ -209,16 +213,16 @@
         return table
 
 
 def getHFModelAndTokenizer(
     model_name: str, cache_dir: Optional[str] = None, hf_access_token: Optional[str] = None
 ) -> tuple[Any, Any]:
     """
-    HuggingFace AutoModel does not currently support Llama-2,
-    hence this function.
+    HuggingFace AutoModel does not currently support Llama-2, hence this function.
+
     :param model_name: Model name
     :param cache_dir: Cache directory (default: None)
     :param hf_access_token: HuggingFace access token (default: None)
     :return: Model and tokenizer
     """
     try:
         from transformers import AutoModelForPreTraining
@@ -276,14 +280,15 @@
         self._index_name = index_name
         self.override_memories: Optional[pandas.DataFrame] = None
         self.model, self.tokenizer = getHFModelAndTokenizer(model_name=model_name, hf_access_token=hf_access_token)
 
     def _search_index(self, query: str) -> tuple[str, pandas.DataFrame]:
         """
         Search index
+
         :param query: Query
         :return: Search index
 
         NOTE: This method should not be called directly. It is used internally.
         """
         if self.override_memories is None:
             self.latest_memories = (
@@ -298,37 +303,40 @@
                 "\n".join([r["__segment"] for r in self.override_memories.to_dict(orient="records")]) + "\n",
                 self.override_memories,
             )
 
     def __call__(self, query: str) -> str:
         """
         Call
+
         :param query: Query
         :return: Response
         """
         context, _ = self._search_index(query)
 
         input_text = context + "\n\n =================== \n" + query
         input_ids = self.tokenizer(input_text, return_tensors="pt").input_ids.to(self.model.device)  # type: ignore
 
         outputs = self.model.generate(input_ids, max_new_tokens=50)  # type: ignore
         return self.tokenizer.decode(outputs[0], skip_special_tokens=True)
 
     def _memory_update(self, df: pandas.DataFrame) -> None:
         """
         Memory update
+
         :param df: Dataframe
 
         NOTE: This method should not be called directly. It is used internally.
         """
         self.override_memories = df
 
     def inspect_latest_memories(self, *columns: str) -> None:
         """
         Inspect latest memories
+
         :param columns: Columns
         """
         with gr.Blocks() as demo:
             with gr.Row():
                 gr.Markdown("# Accessed Memories")
                 gr.Markdown("![](file/demo/logo-small.jpg)")
             selected_df = self.latest_memories[list(columns) + ["__segment"]]
```

### Comparing `orcalib-0.0.56/orcalib/index_handle.py` & `orcalib-0.0.57/orcalib/index_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Optional
 
 from orca_common import ColumnName
 from orca_common.embedding_models import EmbeddingModel
+
 from orcalib.orca_types import NumericTypeHandle, OrcaTypeHandle
 
 
 class IndexHandle:
     """A handle to an index in an Orca database."""
 
     def __init__(
@@ -41,24 +42,28 @@
             column: (OrcaTypeHandle.from_string(column_type) if isinstance(column_type, str) else column_type)
             for column, column_type in artifact_columns.items()
         }
         self.embedding_model = embedding_model
 
     @property
     def embedding_dim(self) -> Optional[int]:
-        """Return the embedding dimension of this index (if any)."""
+        """Return the embedding dimension of this index (if any).
+
+        :return: embedding dimension
+        :rtype: Optional[int]
+        """
         if self.embedding_type is None or not isinstance(self.embedding_type, NumericTypeHandle):
             return None
 
         return self.embedding_type.length
 
     def scan(self, query: Any) -> "DefaultIndexQuery":  # noqa: F821
         """
-        Scan the index for a given query.
-        This is the default index query method.
+        Scan the index for a given query. This is the default index query method.
+
         :param query: Query to scan the index with
         :return: DefaultIndexQuery
         """
         from orcalib.database import OrcaDatabase
         from orcalib.index_query import DefaultIndexQuery
 
         return DefaultIndexQuery(
@@ -66,16 +71,16 @@
             primary_table=OrcaDatabase(self.db_name).get_table(self.table_name),
             index=self.name,
             index_query=query,
         )
 
     def vector_scan(self, query: Any) -> "VectorIndexQuery":  # noqa: F821
         """
-        Scan the index for a given query.
-        This is the vector index query method.
+        Scan the index for a given query. This is the vector index query method.
+
         :param query: Query to scan the index with
         :return: VectorIndexQuery
         """
         from orcalib.database import OrcaDatabase
         from orcalib.index_query import VectorIndexQuery
 
         return VectorIndexQuery(
@@ -84,26 +89,29 @@
             index=self.name,
             index_query=query,
         )
 
     def get_status(self) -> dict[str, Any]:
         """
         Get the status of this index.
+
         :return: Index status
         """
         from orcalib.client import OrcaClient
 
         return OrcaClient.get_index_status(self.db_name, self.name)
 
     def __str__(self) -> str:
         """
         Return a string representation of this index.
+
         :return: String representation
         """
         return f"{self.index_type} index: {self.name} on {self.db_name}.{self.table_name}.{self.column_name} ({self.column_type})"
 
     def __repr__(self) -> str:
         """
         Return a string representation of this index.
+
         :return: String representation
         """
         return str(self)
```

### Comparing `orcalib-0.0.56/orcalib/index_query.py` & `orcalib-0.0.57/orcalib/index_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,31 +47,53 @@
         self.index = index
         self.index_query = index_query
         self.index_value = index_value
 
     def _clone(self, **kwargs) -> "DefaultIndexQuery":
         """
         Clone this query, optionally overriding some parameters
+
         :param kwargs: The parameters to override
-        :returns: A new DefaultIndexQuery
+        :return: A new DefaultIndexQuery
 
         NOTE: This method should not be called directly. It is used internally.
         """
         kwargs["index"] = kwargs.get("index", self.index)
         kwargs["index_query"] = kwargs.get("index_query", self.index_query)
         kwargs["index_value"] = kwargs.get("index_value", self.index_value)
         return super()._clone(**kwargs)
 
+    def _parse_params_columns(self, *columns: str | ColumnHandle) -> list[ColumnName]:
+        """Parse the columns parameter into a dict mapping table names to column names
+
+        Unlike the base class, we allow you to request column names that aren't in the primary
+        table, so that you can request things like $embedding and $distance from the index.
+
+        :param columns: The columns we're parsing. These can be strings or ColumnHandles.
+        """
+        result = []
+
+        for c in columns:
+            if isinstance(c, str):
+                result.append(c)
+            elif isinstance(c, ColumnHandle):
+                result.append(c.column_name)
+            else:
+                raise ValueError(f"Invalid column: {c}")
+
+        return result
+
     @default_api_version_key("index.scan")
     def fetch(self, limit: int, api_version: Optional[str]) -> list[RowDict]:
         """
         Fetch the results of this query
+
         :param limit: The maximum number of rows to return
         :param api_version: The API version to use
-        :returns: The results of this query
+        :return: The results of this query
         """
         from orcalib.database import OrcaDatabase
 
         data = OrcaClient.scan_index(
             OrcaDatabase(self.db_name),
             self.index,
             self.index_query,
@@ -85,17 +107,18 @@
                 row[self.index_value] = row["__index_value"]
                 del row["__index_value"]
         return data
 
     def df(self, limit: Optional[int], explode: bool = False) -> pandas.DataFrame:
         """
         Fetch the results of this query as a pandas DataFrame
+
         :param limit: The maximum number of rows to return
         :param explode: Whether to explode the index_value column (if it exists) into multiple rows (default: False)
-        :returns: The results of this query as a pandas DataFrame
+        :return: The results of this query as a pandas DataFrame
         """
         ret = super().df(limit=limit)
         if explode and self.index_value is not None:
             ret = ret.explode(self.index_value, ignore_index=True)
         return ret
 
 
@@ -109,14 +132,15 @@
         index: IndexName,
         index_query: OrcaExpr,
         curate_run_ids: Optional[list[int]] = None,
         curate_layer_name: Optional[str] = None,
         **kwargs,
     ):
         """A query on a (for now) single table. This is used to build up a query and then execute it with .fetch()
+
         :param db_name: The name of the database to query.
         :param primary_table: The primary table to query.
         :param columns: The columns to select
         :param filter: The filter to apply to the query.
         :param order_by_columns: The columns to order by.
         :param limit: The maximum number of rows to return.
         :param default_order: The default order to use with "order_by" if no order is specified.
@@ -131,16 +155,17 @@
         self.index_query = index_query
         self.curate_run_ids = curate_run_ids
         self.curate_layer_name = curate_layer_name
 
     def _clone(self, **kwargs) -> "VectorIndexQuery":
         """
         Clone this query, optionally overriding some parameters
+
         :param kwargs: The parameters to override
-        :returns: A new VectorIndexQuery
+        :return: A new VectorIndexQuery
 
         NOTE: This method should not be called directly. It is used internally.
         """
         kwargs["index"] = kwargs.get("index", self.index_name)
         kwargs["index_query"] = kwargs.get("index_query", self.index_query)
         kwargs["curate_run_ids"] = kwargs.get("curate_run_ids", self.curate_run_ids)
         kwargs["curate_layer_name"] = kwargs.get("curate_layer_name", self.curate_layer_name)
@@ -161,17 +186,18 @@
 
         return result
 
     @default_api_version_key("index.vector_scan")
     def fetch(self, limit: int, api_version: Optional[str]) -> BatchedScanResult:
         """
         Fetch the results of this query
+
         :param limit: The maximum number of rows to return
         :param api_version: The API version to use
-        :returns: The results of this query
+        :return: The results of this query
         """
 
         data = OrcaClient.vector_scan_index(
             self.primary_table,
             self.index_name,
             self.index_query,
             limit=limit,
@@ -181,12 +207,13 @@
             api_version=api_version,
         )
         return data
 
     def track_with_curate(self, run_ids: list[int], layer_name: str) -> "VectorIndexQuery":
         """
         Track this query with curate
+
         :param run_ids: The run ids to use for curate
         :param layer_name: The layer name to use for curate
-        :returns: A new VectorIndexQuery
+        :return: A new VectorIndexQuery
         """
         return self._clone(curate_run_ids=run_ids, curate_layer_name=layer_name)
```

### Comparing `orcalib-0.0.56/orcalib/orca_chat.py` & `orcalib-0.0.57/orcalib/orca_chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,108 +1,102 @@
 """
 Here are a few examples of building with Orca.
 """
 
+from dataclasses import dataclass
 from threading import Thread
 from typing import Any, Optional
 
 import torch
+import torch.nn as nn
 from transformers import (
     AutoModelForCausalLM,
     AutoTokenizer,
     LogitsProcessorList,
     PreTrainedModel,
     PreTrainedTokenizerBase,
     TextIteratorStreamer,
 )
 
 from orcalib.database import OrcaDatabase
 from orcalib.hf_utils import OrcaGroundingProcessor
-from orcalib.orca_torch import (
-    OrcaGenericLookupLayer,
-    OrcaLookupConfig,
-    OrcaLookupType,
-    OrcaModel,
-    OrcaModule,
-)
+from orcalib.orca_torch import OrcaLookupLayer, OrcaModel, OrcaModule
 from orcalib.orca_types import TextT
 
 orca_llama_system_prompt = """You are a helpful and direct assistant.
 You should try to be as direct and succinct as possible.
 You will be provided with context to help answer user queries.
 Some of the context may or may not be useful.
 If it is, be as true to the context as possible, with priority in order of the context.
 If it is not, say you cannot answer or do not know.
 DO NOT MENTION THE CONTEXT OR TALK ABOUT UNRELATED ENTITIES IN THE CONTEXT.
 Potentially useful context:"""
 
 
-class OrcaChat(OrcaModule):
+class OrcaChat(OrcaModel):
     """
     A basic wrapper for a chatbot model that uses Orca for memory retrieval,
     and a base model with a generate method for response generation.
     """
 
     def __init__(
         self,
-        orca_lookup_config: OrcaLookupConfig,
+        num_memories: int = 20,
         model: str | PreTrainedModel | torch.nn.Module = "facebook/opt-350m",
         model_id: str = "orca_public_chatbot_v0",
         mode: str = "chat",
         use_rag: bool = False,
         use_ground: bool = False,
         max_context_length: int = 4096,
         tokenizer=None,
         **kwargs,
     ):
         """
-        :param orca_lookup_config: OrcaLookupConfig
+        :param orca_db_name: Orca database name
+        :param index_name: Index name
+        :param lookup_column_names: Lookup column names
+        :param num_memories: Number of memories to retrieve
         :param model: Model to use for response generation (default: "facebook/opt-350m")
         :param model_id: Model ID (default: "orca_public_chatbot_v0")
         :param mode: Mode (default: "chat")
         :param use_rag: Whether to use RAG (default: False)
         :param use_ground: Whether to use grounding (default: False)
         :param max_context_length: Maximum context length for response generation (default: 4096)
         :param tokenizer: Tokenizer to use for response generation (if model is a string) or if model is a PreTrainedModel or torch.nn.Module instance (default: None)
         :param kwargs: Additional keyword arguments
         """
-        super().__init__()
+        super().__init__(
+            model_id=model_id,
+            num_memories=num_memories,
+            propagate_lookup_settings=True,
+        )
 
         self.use_rag = use_rag
         self.use_ground = use_ground
 
+        if use_rag:
+            # Lookup settings will be automatically propagated to this layer
+            self.lookup = OrcaLookupLayer()
+        else:
+            self.lookup = None
+
         if isinstance(model, str):
             self.model = AutoModelForCausalLM.from_pretrained(model, **kwargs)
             self.tokenizer = AutoTokenizer.from_pretrained(
                 model,
                 use_default_system_prompt=True if not use_rag else False,
                 **kwargs,
             )
 
         elif isinstance(model, PreTrainedModel) or isinstance(model, torch.nn.Module):
             assert hasattr(model, "generate")
             assert isinstance(tokenizer, PreTrainedTokenizerBase)
             self.tokenizer = tokenizer
             self.model = model
 
-        self.lookup_type = OrcaLookupType(
-            index_type=TextT,
-            return_column_types=(TextT, TextT),
-        )
-        self.orca_lookup_config = orca_lookup_config
-
-        if use_rag:
-            self._orca_db_instance = OrcaDatabase(orca_lookup_config.orca_db_name)
-            self.lookup = OrcaModel(self._orca_db_instance)(OrcaGenericLookupLayer)(  # type: ignore
-                orca_lookup_type=self.lookup_type,
-                orca_lookup_config=orca_lookup_config,
-            )
-        else:
-            self.lookup = None
-
         self.streamer = TextIteratorStreamer(
             tokenizer=self.tokenizer,  # type: ignore
             skip_special_tokens=True,
             skip_prompt=True,
             timeout=15.0,
         )
 
@@ -124,42 +118,32 @@
         self.last_retrieval_query = None
         self.last_model_input = None
         self.last_accessed_memories: Optional[list[list[Any]]] = None
         self.text_memories: list[list[str]] = []
         self.sim_weight = 0.0
         self.bag_weight = 0.0
 
-    def enable_curate(self) -> None:
-        """
-        This is temporary until the workflow for attaching orca and curate to models is changed here.
-        This will likely change based on how we decide the interface for swapping/attaching databases,
-        indices, and columns looks.
-        """
-        if self.lookup is not None:
-            self.lookup.init_curate(
-                model_id=self.model_id, model_version="0.0.1", extra_tags=["from_chatbot_demo"], batch_size=1
-            )
-            self.lookup.enable_curate()
-
     def determine_retrieval_query(self) -> str:
         """
         Determine the retrieval query based on the last user input
         and other context.
 
         Currently, this just combines all user inputs into a single query.
+
         :return: str
         """
         if self.mode == "StatelessQA":
             return " ".join([msgs["content"] if msgs["role"] == "user" else "" for msgs in [self.chat_history[-1]]])
         else:
             return " ".join([obj["content"] if obj["role"] == "user" else "" for obj in self.chat_history])
 
     def prep_next_gen(self, last_user_input: str) -> tuple[str, list[list[str]], Optional[list[list[Any]]]]:
         """
         Prepares the next generation by updating the chat history and last user input.
+
         :param last_user_input: Last user input
         :return: tuple[str, list[list[str]], Optional[list[list[Any]]]]
         """
         if self.mode == "StatelessQA":
             self.clear_chat()
 
         self.last_user_input = last_user_input
@@ -179,24 +163,25 @@
         self.last_retrieval_query = retrieval_query
 
         return "", self.ui_history, self.last_accessed_memories
 
     def retrieve(self, query: str) -> list[str]:
         """
         Do the retrieval of memories from the orca database.
+
         :param query: Query
         :return: list[str]
         """
 
         if self.lookup is None:
             return []
 
         # HACK-y, TODO Fix this
         self._batch_size = 1
-        self.lookup._batch_size = 1
+        self.lookup.curate_batch_size = 1
 
         payload = self.lookup([query])[0]
         memory_texts = []
         for doc in payload:
             # the first element is the vector, the second is the meta
             memory_texts.append(doc[1])
 
@@ -205,14 +190,15 @@
         self.lookup_history.append(memory_texts)
 
         return memory_texts
 
     def gen_response(self, ui_history) -> Any:
         """
         Generate a response based on the last user input and the current context.
+
         :param ui_history: UI history
         :return: Any
         """
         if self.mode == "chat" or self.mode == "StatelessQA":
             formatted_query = self.tokenizer.apply_chat_template(self.chat_history, tokenize=False)
             # Ensure formatted_query is a string to satisfy the type checker and for runtime safety.
             if not isinstance(formatted_query, str):
@@ -262,15 +248,15 @@
             {
                 "role": "assistant",
                 "content": gen_text_stream,
             }
         )
 
         if self.lookup is not None:
-            self.lookup.record_model_input_output(*self.ui_history[-1])
+            self.record_model_input_output(*self.ui_history[-1])
 
     def clear_chat(self) -> None:
         """
         This clears all histories.
         """
         self.lookup_history = []
         if self.use_rag:
@@ -283,41 +269,57 @@
         else:
             self.chat_history = []
         self.ui_history = []
 
     def format_context(self, memories: list[str]) -> str:
         """
         String format memories for prompt injection to model
+
         :param memories: Memories
         :return: str
         """
         context = ""
         for i, memory in enumerate(memories):
             context += f"\n\n{i + 1}. {memory}"
 
         return context
 
     def update_grounding_params(self, sim_weight: float, bag_weight: float) -> None:
         """
         Update the grounding parameters for the OrcaGroundingProcessor.
+
         :param sim_weight: Similarity weight
         :param bag_weight: Bag weight
         """
         self.sim_weight = sim_weight
         self.bag_weight = bag_weight
 
-    def switch_config(self, new_config: OrcaLookupConfig) -> None:
+    def switch_config(
+        self,
+        database_name: Optional[str],
+        index_name: Optional[str],
+        lookup_column_names: Optional[list[str]],
+        num_memories: Optional[int],
+    ) -> None:
         """
-        Switch the OrcaLookupConfig for the OrcaChat instance,
-        clearing the chat history.
+        Switch the OrcaLookupConfig for the OrcaChat instance, clearing the chat history.
+        NOTE: The settings will be propagated to the OrcaLookupLayer, if it exists.
+
         :param new_config: New config
         """
-        self.orca_lookup_config = new_config
-        if self.lookup is not None:
-            self.lookup.set_lookup_config(new_config)
+
+        if database_name is not None:
+            self.lookup_database = database_name
+        if index_name is not None:
+            self.memory_index_name = index_name
+        if lookup_column_names is not None:
+            self.lookup_column_names = lookup_column_names
+        if num_memories is not None:
+            self.num_memories = num_memories
+
         self.clear_chat()
 
     def print_chat_log(self) -> None:
         """
         Print the chat log to whatever/wherever the stdout is.
         """
         print("*" * 80)
```

### Comparing `orcalib-0.0.56/orcalib/orca_expr.py` & `orcalib-0.0.57/orcalib/orca_expr.py`

 * *Files 8% similar despite different names*

```diff
@@ -129,26 +129,27 @@
         """
         self.op = op
         self.args = args
 
     def _serialize_arg(self, arg: OperableType) -> Union[str, dict[str, Union[str, list]]]:
         """
         Serialize the argument to a format that can be sent to the server
+
         :param arg: The argument to serialize
 
         NOTE: This method should not be called directly. It is used internally.
         """
         if isinstance(arg, OrcaExpr):
             return arg.as_serializable()
         elif isinstance(arg, ColumnHandle):
             return arg.as_serializable()
-        elif isinstance(arg, str):
-            return f"'{arg}'"
+        elif isinstance(arg, str) or isinstance(arg, float) or isinstance(arg, int) or isinstance(arg, bool):
+            return f"{arg}"
         else:
-            return arg
+            raise ValueError(f"{arg} is not a valid value for arg")
 
     def as_serializable(self) -> dict[str, Union[str, list]]:
         """
         Serialize the expression to a format that can be sent to the server
         """
         return {
             "op": self.op,
```

### Comparing `orcalib-0.0.56/orcalib/orca_torch.py` & `orcalib-0.0.57/orcalib/orca_torch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,862 +1,597 @@
 import logging
 import time
-from abc import ABC
-from collections import defaultdict
-from dataclasses import dataclass
-from enum import Enum
-from functools import lru_cache
-from typing import Any, Callable, NamedTuple, Optional, cast
+from collections import defaultdict, deque
+from typing import Any, Callable, Iterator, Optional, TypeVar, cast, final
 from uuid import UUID
 
-import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from orca_common import ColumnName
 from torch import Tensor
 from torch.utils.data import DataLoader, Dataset
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from orcalib.batched_scan_result import BatchedScanResult
 from orcalib.client import OrcaClient
-from orcalib.data_classes import VectorScanResult
 from orcalib.database import OrcaDatabase
-from orcalib.index_handle import IndexHandle
 from orcalib.orca_expr import ColumnHandle
-from orcalib.orca_types import OrcaTypeHandle
+from orcalib.orca_torch_mixins import (
+    ClassificationMode,
+    CurateSettingsMixin,
+    LabelColumnNameMixin,
+    LookupSettingsMixin,
+    PostInitMixin,
+    PreForwardMixin,
+    ProjectionMode,
+)
 from orcalib.table import TableHandle
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
-@dataclass
-class CurateRunInfo:
-    run_ids: list[int]
-    model_id: str
-    model_version: Optional[str]
-    batch_size: int
-    tags: list[str]
-    metadata: dict[str, Any]
-    seq_id: Optional[UUID]
-
-
-# TODO: Consider making this a metaclass instead
-def OrcaModel(  # noqa: C901
-    db: OrcaDatabase,
-    model_id: Optional[str] = None,
-    model_version: Optional[str] = None,
-    tags: Optional[list[str]] = None,
-    metadata: Optional[dict[str, Any]] = None,
-    **module_settings_override: Any,
-) -> Callable[[nn.Module], nn.Module]:
-    """A decorator that enables Orca on a PyTorch model.
-
-    Primary purpose is attaching a database to the model, but it also supports applying various settings, notably: enabling curate tracking.
-
-    :param db: (OrcaDatabase) The OrcaDatabase instance to be used for this model.
-    :param model_id: (Optional[str]) The ID (aka name) of the model to be curated. (default: None)
-    :param model_version: (Optional[str]) A version string of the model being run. (e.g., "v1.0.0") (default: None)
-    :param tags: (Optional[list[str]]) A list of tags to be added to the model run. (e.g., ["production", "v1"]) (default: None)
-    :param metadata: (Optional[dict[str, Any]]) A dictionary of metadata to be added to the model run. (default: None)
-    :param module_settings_override: (Any) Any additional settings to be applied to the model.
+########################
+### Orca PyTorch Layers
+########################
+
+MODULE_TYPE = TypeVar("MODULE_TYPE", bound="OrcaModule")
 
-    Example usage:
-    .. code-block:: python
 
-            import torch
-            from orcalib import OrcaModel
+class OrcaModule(nn.Module, CurateSettingsMixin):
+    """OrcaModule is for PyTorch modules that support Curate tracking. It is the base class for all Orca PyTorch layers.
 
-            @OrcaModel(db, model_id="my_model", model_version="v1", tags=["production"])
-            class MyModel(torch.nn.Module):
-                def __init__(self):
-                    super().__init__()
-                    self.linear = torch.nn.Linear(10, 10)
-
-                def forward(self, x):
-                    return self.linear(x)
-
-            model = MyModel()
-            model.init_curate(batch_size=32)
-            model.enable_curate()
-            model.disable_curate()
-            model.disable_memory()
-            model.enable_memory()
-            model.last_curate_run_info()
+    NOTE: Curate setting propagation is handled by the OrcaModel (model, not module) class, which recursively sets the
+    curate settings for all children of the model to use the same instance of the curate settings object.
     """
-    _batch_size: Optional[int] = None
-    _seq_id: Optional[UUID] = None
 
-    _model_id: Optional[str] = model_id
-    _model_version: Optional[str] = model_version
-    _tags: list[str] = tags or []
-    _metadata: dict[str, Any] = metadata or {}
-    _latest_run_ids: Optional[list[int]] = None
+    def __init__(
+        self,
+        curate_database: OrcaDatabase | str | None = None,
+        model_id: Optional[str] = None,
+        model_version: Optional[str] = None,
+        metadata: Optional[dict[str, Any]] = None,
+        curate_enabled: bool = False,
+        tags: Optional[set[str]] = None,
+    ):
+        """Initializes the module with the specified Curate settings.
+        :param curate_database: The OrcaDatabase instance to use for Curate tracking. (default: None)
+        :param model_id: The ID of the model. (default: None)
+        :param model_version: The version of the model. (default: None)
+        :param metadata: The metadata to be stored with Curate runs. (default: None)
+        :param curate_enabled: Whether Curate tracking is enabled. (default: False)
+        :param tags: The tags to be included in Curate runs. (default: None)
+        """
+        nn.Module.__init__(self)
+        CurateSettingsMixin.__init__(
+            self,
+            curate_database=curate_database,
+            model_id=model_id,
+            model_version=model_version,
+            metadata=metadata,
+            curate_enabled=curate_enabled,
+            tags=tags,
+        )
+
+    def __hash__(self):
+        return id(self)
+
+    def get_orca_modules_recursively(
+        self,
+        max_depth: Optional[int] = None,
+        include_self: bool = True,
+        filter_type: type[MODULE_TYPE] = None,
+    ) -> Iterator[MODULE_TYPE]:
+        """
+        Get all OrcaModule in the model recursively. NOTE: This will search through all children - even
+        those that aren't OrcaModule - but it will only return OrcaModule. This allows for a more general
+        search of the model.
+
+        :param max_depth: The maximum depth to search. Setting this to 0 will only include this module, setting it
+         to 1 will include only this module and its children (default: None). Passing through modules that don't
+         match the filter_type will not increment the depth.
+        :param skip_self: Whether to include the current OrcaModule in the results. (default: True)
+        :param filter_type: The type of module to filter by. (default: OrcaModule)
+        :return: An iterator of OrcaModule.
+        NOTE: All parent nodes will be processed before their children
+        """
+        unvisited = deque([self])
+        node_depth = dict({self: 0})
+
+        filter_type = filter_type or OrcaModule
+
+        while unvisited:
+            parent = unvisited.popleft()
+            if isinstance(parent, filter_type) and (include_self or parent != self):
+                yield parent
+
+            # We only want to increment the depth if there is no parent or it's an instance of the filter type
+            if parent is None or isinstance(parent, filter_type):
+                next_depth = node_depth[parent] + 1
+            else:
+                next_depth = node_depth[parent]
+
+            if max_depth is not None and next_depth > max_depth:
+                continue
+            for child in parent.children():
+                node_depth[child] = next_depth
+                unvisited.append(child)  # type: ignore
 
-    def memory_setting_passthrough(inst: nn.Module, enable: bool) -> None:
+    def enable_curate(self, recursive: bool = True):
         """
-        A passthrough function to enable/disable memory access for the model and all its children.
-        :param inst: A PyTorch model instance.
-        :param enable: Whether to enable or disable memory access.
+        Enable Curate tracking for the model and (if recursive is True) for all its descendants.
+        :param recursive: Whether to enable Curate tracking recursively. (default: True)
         """
-        for child in inst.children():
-            child._orca_memory_toggle(enable)  # type: ignore
+        if not recursive:
+            self.curate_enabled = True
+            return
+        for child in self.get_orca_modules_recursively():
+            child.curate_enabled = True
 
-    # TODO: this will break in weird ways if someone is monkey patching a model after instantiation (an edge case we can live with for now)
-    def build_layer_names(inst: nn.Module, root_name: Optional[str] = None) -> None:
+    def disable_curate(self, recursive: bool = True):
         """
-        Builds layer names for the model and all its children.
-        :param inst: A PyTorch model instance.
-        :param root_name: The name of the root layer. (default: None)
+        Disable Curate tracking for this module and (if recursive is True) for all its descendants.
+        :param recursive: Whether to disable Curate tracking recursively. (default: True)
         """
-        if isinstance(inst, OrcaModule):
-            inst.set_curate_layer_name(root_name)
-        for name, child in inst.named_children():
-            build_layer_names(
-                child,
-                f"{root_name + '.' if root_name is not None else ''}{name}",
-            )
+        if not recursive:
+            self.curate_enabled = False
+            return
+        for child in self.get_orca_modules_recursively():
+            child.curate_enabled = False
 
-    def apply_global_settings(inst: nn.Module, module_settings_override: dict[str, Any]) -> None:
-        """
-        Applies global settings to the model and all its children.
-        :param inst: A PyTorch model instance.
-        :param module_settings_override: The settings to be applied to the model.
+
+class OrcaLookupModule(OrcaModule, LookupSettingsMixin, PostInitMixin):
+    """
+    OrcaLookupModule is for PyTorch modules that support both Curate tracking AND memory lookups, and is the
+    base class for all Orca PyTorch layers that support lookups—either directly or through their children.
+
+    NOTE: Lookup settings are propagated to all children of OrcaLookupModule, which recursively sets the lookup
+    settings for all OrcaLookupModule its descendents to use the same instance of the lookup settings object.
+    """
+
+    def __init__(
+        self,
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        model_id: Optional[str] = None,
+        model_version: Optional[str] = None,
+        metadata: Optional[dict[str, Any]] = None,
+        curate_enabled: bool = False,
+        tags: Optional[set[str]] = None,
+        # Memory Lookup Settings
+        memory_index_name: Optional[str] = None,
+        lookup_column_names: Optional[list[str]] = None,
+        num_memories: Optional[int] = None,
+        freeze_num_memories: bool = False,
+        propagate_lookup_settings: bool = True,
+    ):
+        """Initializes the module with the specified Curate and memory lookup settings.
+        :param database: The OrcaDatabase instance to use for Curate and memory lookups. (default: None)
+        :param model_id: The ID of the model. (default: None)
+        :param model_version: The version of the model. (default: None)
+        :param metadata: The metadata to be stored with Curate runs. (default: None)
+        :param curate_enabled: Whether Curate tracking is enabled. (default: False)
+        :param tags: The tags to be included in Curate runs. (default: None)
+        :param memory_index_name: The name of the index to use for lookups. (default: None)
+        :param lookup_column_names: The names of the columns to return from the index during a lookup. (default: None)
+        :param num_memories: The number of memories to return from the index during a lookup. (default: None)
+        :param freeze_num_memories: Whether the number of memories should be frozen. (default: False) When
+        set to True, an error will be raised if an attempt is made to change the number of memories.
+        :param propagate_lookup_settings: Whether to propagate lookup settings to all children. (default: False)
         """
-        if isinstance(inst, OrcaModule):
-            inst.apply_orca_settings(**module_settings_override)
-        for child in inst.children():
-            apply_global_settings(child, module_settings_override)
+        OrcaModule.__init__(
+            self,
+            model_id=model_id,
+            model_version=model_version,
+            metadata=metadata,
+            curate_enabled=curate_enabled,
+            tags=tags,
+            curate_database=database,
+        )
+        LookupSettingsMixin.__init__(
+            self,
+            lookup_database=database,
+            memory_index_name=memory_index_name,
+            lookup_column_names=lookup_column_names,
+            num_memories=num_memories,
+            freeze_num_memories=freeze_num_memories,
+            propagate_lookup_settings=propagate_lookup_settings,
+        )
+
+    def post_init(self):
+        super().post_init()
 
-    def post_init(inst: nn.Module) -> None:
+        self._propagate_lookup_settings()
+
+
+class OrcaModel(OrcaLookupModule, PostInitMixin, PreForwardMixin):
+    """OrcaModel should be the base class for all PyTorch models that include custom Orca layers.
+
+    This class is responsible for:
+      * Propagating Curate and memory lookup settings to all children of the model.
+      * Getting curate run ids and preparing tracking before the forward pass.
+      * Building layer names for all children of the model.
+
+    This class provides functions to let you:
+      * Enable and disable Curate tracking for the model and all its children.
+      * Record Curate scores for the last run.
+      * Record model input and output for the last run.
+      * Enable and disable memory access for the model and all its children.
+      * Update Curate tracking settings for the model and all its children.
+
+    When using OrcaModel, you can set global settings for Curate tracking and memory lookups that will be propagated
+    to all children of the model. This allows you to set these settings once for the entire model and have them
+    automatically applied to all layers.
+    """
+
+    def __init__(
+        self,
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        model_id: Optional[str] = None,
+        model_version: Optional[str] = None,
+        metadata: Optional[dict[str, Any]] = None,
+        curate_enabled: bool = False,
+        tags: Optional[set[str]] = None,
+        # Memory Lookup Settings
+        memory_index_name: Optional[str] = None,
+        lookup_column_names: Optional[list[str]] = None,
+        num_memories: Optional[int] = None,
+        freeze_num_memories: bool = False,
+        propagate_lookup_settings: bool = True,
+    ):
         """
-        Post-initialization function to attach the database to the model and all its children.
-        :param inst: A PyTorch model instance.
+        Initializes the model with global settings.
+        :param database: The OrcaDatabase instance to use for Curate and memory lookups. (default: None)
+        :param model_id: model_id will be included in Curate runs. (default: None)
+        :param model_version: model_version will be included in Curate runs. (default: None)
+        :param metadata: metadata is a dictionary of additional information to be stored with Curate runs. (default: None)
+        :param curate_enabled: Whether Curate tracking is enabled. (default: False)
+        :param tags: tags is a set of strings to be included in Curate runs. (default: None)
+        :param memory_index_name: The name of the index to use for lookups. (default: None)
+        :param lookup_column_names: The names of the columns to return from the index during a lookup. (default: None)
+        :param num_memories: The number of memories to return from the index during a lookup. (default: None)
+        :param freeze_num_memories: Whether the number of memories should be frozen after initialization. (default: False) When
+        set to True, an error will be raised if an attempt is made to change the number of memories.
+        :param propagate_lookup_settings: Whether to propagate lookup settings to all children. (default: False)
         """
-        if isinstance(inst, OrcaModule):
-            inst._orca_db_instance = db
-        if not hasattr(inst, "_orca_memory_toggle"):
-            inst._orca_memory_toggle = memory_setting_passthrough  # type: ignore
-        for child in inst.children():
-            post_init(child)
+        super().__init__(
+            database=database,
+            model_id=model_id,
+            model_version=model_version,
+            metadata=metadata,
+            curate_enabled=curate_enabled,
+            tags=tags,
+            memory_index_name=memory_index_name,
+            lookup_column_names=lookup_column_names,
+            num_memories=num_memories,
+            freeze_num_memories=freeze_num_memories,
+            propagate_lookup_settings=propagate_lookup_settings,
+        )
 
-    def enable_memory(inst: nn.Module) -> None:
-        """
-        Enables memory access for the model and all its children.
-        :param inst: A PyTorch model instance.
+    def pre_forward(self, *args, **kwargs):
+        """Called before the forward pass, this is where we setup curate tracking."""
+        self.setup_curate(*args, **kwargs)
+
+    def post_init(self) -> None:
+        """
+        Function that runs after the __init__ method. This is used to apply global settings to the model and build
+        the curate layer names. You can override this function to add new post-init behavior in derived classes.
+
+        This will override the curate settings for all children to use the parent's settings.
+        NOTE: This means that changing the child's settings will change the parent's settings and vice versa.
+        """
+        super().post_init()
+        OrcaModel._build_layer_names(self)
+
+        for child in self.get_orca_modules_recursively(include_self=False):
+            child._curate_settings = self._curate_settings
+            child.curate_enabled = self.curate_enabled
+
+    def init_curate(
+        self,
+        model_id: Optional[str] = None,
+        model_version: Optional[str] = None,
+        tags: Optional[set[str]] = None,
+        extra_tags: Optional[set[str]] = None,
+        metadata: Optional[dict[str, Any]] = None,
+        extra_metadata: Optional[dict[str, Any]] = None,
+        batch_size: Optional[int] = None,
+        seq_id: Optional[UUID] = None,
+    ) -> None:
         """
-        inst._orca_memory_toggle(inst, True)  # type: ignore
+        Initializes curate tracking for the module and all its children.
+        :param model_id: The ID of the model.
+        :param model_version: The version of the model.
+        :param new_tags: The new tags to be added to the model.
+        :param extra_tags: The extra tags to be added to the model.
+        :param new_metadata: The new metadata to be added to the model.
+        :param extra_metadata: The extra metadata to be added to the model.
+        :param batch_size: The batch size to be used for the model.
+        :param seq_id: The sequence ID to be used for the model.
+        """
+
+        self.curate_model_id = model_id or self.curate_model_id
+        self.curate_model_version = model_version or self.curate_model_version
+        self.curate_tags = tags or self.curate_tags or []
+        if extra_tags:
+            self.curate_tags += extra_tags
+        self.curate_metadata = metadata or self.curate_metadata or {}
+        if extra_metadata:
+            self.curate_metadata.update(extra_metadata)
+        self.curate_batch_size = batch_size or self.curate_batch_size
+        self.curate_seq_id = seq_id or self.curate_seq_id
 
-    def disable_memory(inst: nn.Module) -> None:
+    @staticmethod
+    def _build_layer_names(inst: nn.Module, root_name: Optional[str] = None) -> None:
         """
-        Disables memory access for the model and all its children.
+        Builds layer names for the model and all its children.
         :param inst: A PyTorch model instance.
+        :param root_name: The name of the root layer. (default: None)
         """
-        inst._orca_memory_toggle(inst, False)  # type: ignore
+        if isinstance(inst, OrcaModule):
+            inst.curate_layer_name = root_name
+        for name, child in inst.named_children():
+            OrcaModel._build_layer_names(
+                child,
+                f"{root_name + '.' if root_name is not None else ''}{name}",
+            )
 
-    def is_curate_enabled_anywhere(inst: nn.Module) -> bool:
+    def _is_curate_enabled_anywhere(self) -> bool:
         """
         Checks if curate tracking is enabled anywhere in the model or its children.
-        :param inst: A PyTorch model instance.
         :return: Whether curate tracking is enabled anywhere in the model or its children.
         """
-        if isinstance(inst, OrcaModule) and inst._curate_enabled:
-            return True
-        for child in inst.children():
-            if is_curate_enabled_anywhere(child):
-                return True
-        return False
 
-    def set_run_ids(inst: nn.Module, run_ids: list[int]) -> None:
-        """
-        Sets the run IDs for the model and all its children.
-        :param inst: A PyTorch model instance.
-        :param run_ids: The run IDs to be set.
-        """
-        if isinstance(inst, OrcaModule):
-            inst.set_curate_run_ids(run_ids)
-        for child in inst.children():
-            set_run_ids(child, run_ids)
+        return any(child.curate_enabled for child in self.get_orca_modules_recursively())
 
-    def try_infer_batch_size(*args: Any, **kwargs: Any) -> Optional[int]:
+    def _try_infer_batch_size(*args: Any, **kwargs: Any) -> Optional[int]:
         """
         Attempts to infer the batch size from the model's input arguments.
         :param args: The positional arguments.
         :param kwargs: The keyword arguments.
         :return: The inferred batch size.
         """
+
         for arg in args:
             if isinstance(arg, torch.Tensor) and len(arg.shape) > 1:
                 return arg.shape[0]
         for kwarg in kwargs.values():
             if isinstance(kwarg, torch.Tensor) and len(kwarg.shape) > 1:
                 return kwarg.shape[0]
-        return None
-
-    def decorator(cls) -> nn.Module:
-        """
-        The decorator function that wraps the model class.
-        :param cls: The model class to be wrapped.
-        :return: The wrapped model class.
-        """
-        old_init = cls.__init__
-        old_forward = cls.forward
-
-        def wrapped_init(self, *args, **kwargs) -> None:
-            """
-            The wrapped init function that initializes the model and applies global settings.
-            :param args: The positional arguments.
-            :param kwargs: The keyword arguments.
-            """
-            old_init(self, *args, **kwargs)
-            post_init(self)
-            build_layer_names(self)
-            apply_global_settings(self, module_settings_override)
-
-        def init_curate(
-            self,
-            model_id: Optional[str] = None,
-            model_version: Optional[str] = None,
-            new_tags: Optional[list[str]] = None,
-            extra_tags: Optional[list[str]] = None,
-            new_metadata: Optional[dict[str, Any]] = None,
-            extra_metadata: Optional[dict[str, Any]] = None,
-            batch_size: Optional[int] = None,
-            seq_id: Optional[UUID] = None,
-        ) -> None:
-            """
-            Initializes the curation process for a model.
-
-            :param model_id: (Optional[str]) The ID (aka name) of the model to be curated. (default: None)
-            :param model_version: (Optional[str]) The version of the model being run. (e.g., "v1.0.0") (default: None)
-            :param new_tags: (Optional[list[str]]) A list of new tags to be added to the model run (replacing existing tags). (default: None)
-            :param extra_tags: (Optional[list[str]]) A list of additional tags to be added to the model run. (default: None)
-            :param new_metadata: (Optional[dict[str, Any]]) A dictionary of new metadata to be added to the model. (default: None)
-            :param extra_metadata: (Optional[dict[str, Any]]) A dictionary of additional metadata to be added to the model run. (default: None)
-            :param batch_size: (Optional[int]) The batch size to be used for the model forward pass. (default: None)
-            :param seq_id: (Optional[UUID]) The sequence ID to be used for the model (for sequence models). (default: None)
-            """
-            nonlocal _model_id
-            nonlocal _model_version
-            nonlocal _tags
-            nonlocal _metadata
-            nonlocal _batch_size
-            nonlocal _seq_id
-            if model_id is not None:
-                _model_id = model_id
-            if model_version is not None:
-                _model_version = model_version
-            if new_tags is not None:
-                _tags = new_tags
-            if extra_tags is not None:
-                if _tags is None:
-                    _tags = []
-                _tags.extend(extra_tags)
-            if new_metadata is not None:
-                _metadata = new_metadata
-            if extra_metadata is not None:
-                _metadata.update(extra_metadata)
-            if batch_size is not None:
-                _batch_size = batch_size
-            if seq_id is not None:
-                _seq_id = seq_id
-
-        def last_curate_run_info(self) -> CurateRunInfo:
-            """
-            Returns the information of the last curate run on the model.
-            """
-            assert (
-                _model_id is not None and _batch_size is not None and _latest_run_ids is not None
-            ), "It seems there is no last curate run on this model"
-            return CurateRunInfo(
-                run_ids=_latest_run_ids,
-                model_id=_model_id,
-                model_version=_model_version,
-                batch_size=_batch_size,
-                tags=_tags,
-                metadata=_metadata,
-                seq_id=_seq_id,
-            )
-
-        def record_curate_scores(self, scores: list[float] | float) -> None:
-            """
-            Records the scores of the last curate run on the model.
-            :param scores: The scores to be recorded.
-            """
-            assert _latest_run_ids is not None, "It seems there is no last curate run on this model"
-            if isinstance(scores, float):
-                scores = [scores]
-            assert isinstance(scores, list)
-            assert len(scores) == len(_latest_run_ids), "Number of scores must match number of run IDs"
-            db.record_model_scores(_latest_run_ids, scores)
-
-        def record_model_input_output(self, inputs: list[Any] | Any, outputs: list[Any] | Any) -> None:
-            """
-            Records the inputs and outputs of the last curate run on the model.
-            :param inputs: The inputs to be recorded.
-            :param outputs: The outputs to be recorded.
-            """
-            assert _latest_run_ids is not None, "It seems there is no last curate run on this model"
-            if not isinstance(inputs, list):
-                inputs = [inputs]
-            if not isinstance(outputs, list):
-                outputs = [outputs]
-            assert (
-                len(inputs) == len(outputs) == len(_latest_run_ids)
-            ), f"Inputs/Outputs not of the correct size (got {len(inputs)}, {len(outputs)}, expected {len(_latest_run_ids)})"
-            db.record_model_input_output(_latest_run_ids, inputs, outputs)
-
-        def wrapped_forward(self: nn.Module, *args, **kwargs) -> Any:
-            """
-            The wrapped forward function that enables Curate tracking.
-            :param self: A PyTorch model instance.
-            :param args: The positional arguments.
-            :param kwargs: The keyword arguments.
-            :return: The output of the model's forward pass.
-            """
-            if is_curate_enabled_anywhere(self):
-                nonlocal _batch_size
-                if _batch_size is None:
-                    _batch_size = try_infer_batch_size(*args, **kwargs)
-                    if _batch_size is None:
-                        raise ValueError(
-                            "Batch size could not be inferred. Please set batch size manually via init_curate."
-                        )
-                assert (
-                    _model_id is not None
-                ), "Model ID must be set when Curate tracking is enabled. Please set in decorator or via init_curate."
-                run_ids = OrcaClient.init_forward_pass(
-                    db_name=db.name,
-                    model_id=_model_id,
-                    model_version=_model_version,
-                    batch_size=_batch_size,
-                    tags=_tags,
-                    metadata=_metadata,
-                    seq_id=_seq_id,
-                )
-                nonlocal _latest_run_ids
-                _latest_run_ids = run_ids
-                set_run_ids(self, run_ids)
-            return old_forward(self, *args, **kwargs)
-
-        cls.__init__ = wrapped_init
-        cls.forward = wrapped_forward
-        cls.enable_memory = enable_memory
-        cls.disable_memory = disable_memory
-        cls.init_curate = init_curate
-        cls.last_curate_run_info = last_curate_run_info
-        cls.record_curate_scores = record_curate_scores
-        cls.record_model_input_output = record_model_input_output
-
-        return cls
-
-    return decorator
-
-
-########################
-### Orca PyTorch Layers
-########################
-class OrcaModule(nn.Module, ABC):
-    """Parent Class for all Orca Modules to handle all global settings (e.g. enable/disable curate tracking)
-
-    This currently only operates with the Curate database; it does not handle memory access with a memory database (attached via a separate decorator).
-
-    Example usage:
-    .. code-block:: python
 
-            import torch
-            from orcalib import OrcaModule
+        raise ValueError("Curate batch size could not be inferred. Please set batch size manually via init_curate.")
 
-            class MyModule(OrcaModule):
-                def __init__(self):
-                    super().__init__()
-                    self.linear = torch.nn.Linear(10, 10)
-
-                def forward(self, x):
-                    return self.linear(x)
-
-            model = MyModel()
-            model.init_curate(batch_size=32)
-            model.enable_curate()
-            model.disable_curate()
-            model.disable_memory()
-            model.enable_memory()
-            model.last_curate_run_info()
-    """
-
-    # TODO: enable/disable memory access should move here from the decorator
-
-    def __init__(self, **settings):
-        """
-        :param settings: Additional settings to be applied to the module.
+    def setup_curate(self, *args, **kwargs) -> None:
         """
-        super().__init__()
-        self._orca_db_instance: Optional[OrcaDatabase] = None
-        self.apply_orca_settings(**settings)
-
-    def apply_orca_settings(
-        self,
-        curate_enabled: bool = False,
-        orca_db_instance: Optional[OrcaDatabase] = None,
-        curate_layer_name: Optional[str] = None,
-    ) -> None:
+        Sets up curate tracking for the model and all its children.
+        :param args: The positional arguments.
+        :param kwargs: The keyword arguments.
         """
-        Applies global settings to the module.
-        :param curate_enabled: Whether curate tracking is enabled. (default: False)
-        :param orca_db_instance: The OrcaDatabase instance to be used for this module. (default: None)
-        :param curate_layer_name: The name of the layer to be used for curate tracking. (default: None)
-        """
-        self._curate_enabled = curate_enabled
-        if orca_db_instance is not None:
-            self._orca_db_instance = orca_db_instance
-        if curate_layer_name is not None:
-            self._layer_name = curate_layer_name
+        if not self._is_curate_enabled_anywhere():
+            return
 
-    def _set_curate_enabled(self, enabled: bool) -> None:
-        """
-        Sets the curate tracking status for the module and all its children.
-        :param enabled: Whether curate tracking is enabled.
+        self.curate_batch_size = self.curate_batch_size or self._try_infer_batch_size(*args, **kwargs)
 
-        NOTE: This method should not be called directly. It is used internally.
-        """
-        self._curate_enabled = enabled
+        assert (
+            self.curate_model_id is not None
+        ), "Model ID must be set when Curate tracking is enabled. Please set in decorator or via init_curate."
 
-        def set_curate_enable_for_children(root: nn.Module) -> None:
-            """
-            Sets the curate tracking status for the module and all its children.
-            :param root: The root module.
-            """
-            for child in root.children():
-                if isinstance(child, OrcaModule):
-                    child._set_curate_enabled(enabled)
-                else:
-                    set_curate_enable_for_children(child)
+        assert self.curate_database_instance is not None, "Database must be set before Curate tracking is enabled."
 
-        set_curate_enable_for_children(self)
+        self._last_curate_run_ids = self.curate_run_ids
 
-    def enable_curate(self) -> None:
-        """
-        Enables curate tracking for the module and all its children.
-        """
-        self._set_curate_enabled(True)
+        self.curate_run_ids = OrcaClient.init_forward_pass(
+            db_name=self.curate_database_instance.name,
+            model_id=self.curate_model_id,
+            model_version=self.curate_model_version,
+            batch_size=self.curate_batch_size,
+            tags=self.curate_tags,
+            metadata=self.curate_metadata,
+            seq_id=self.curate_seq_id,
+        )
 
-    def disable_curate(self) -> None:
+    def record_curate_scores(self, scores: list[float] | float) -> None:
         """
-        Disables curate tracking for the module and all its children.
+        Records the scores of the last curate run on the model.
+        :param scores: The scores to be recorded.
         """
-        self._set_curate_enabled(False)
+        assert self.curate_run_ids is not None, "It seems there is no last curate run on this model"
+        if isinstance(scores, float):
+            scores = [scores]
+        assert isinstance(scores, list)
+        assert len(scores) == len(self.curate_run_ids), "Number of scores must match number of run IDs"
+        assert self.curate_database_instance is not None, "Database must be set before Curate tracking is enabled."
+        self.curate_database_instance.record_model_scores(self.curate_run_ids, scores)
+
+    def record_model_input_output(self, inputs: list[Any] | Any, outputs: list[Any] | Any) -> None:
+        """
+        Records the inputs and outputs of the last curate run on the model.
+        :param inputs: The inputs to be recorded.
+        :param outputs: The outputs to be recorded.
+        """
+        assert self.curate_run_ids is not None, "It seems there is no last curate run on this model"
+        if not isinstance(inputs, list):
+            inputs = [inputs]
+        if not isinstance(outputs, list):
+            outputs = [outputs]
+        assert (
+            len(inputs) == len(outputs) == len(self.curate_run_ids)
+        ), f"Inputs/Outputs not of the correct size (got {len(inputs)}, {len(outputs)}, expected {len(self.curate_run_ids)})"
+        assert self.curate_database_instance is not None, "Database must be set before Curate tracking is enabled."
+        self.curate_database_instance.record_model_input_output(self.curate_run_ids, inputs, outputs)
 
-    def set_curate_layer_name(self, name: Optional[str]) -> None:
+    def enable_memory(self) -> None:
         """
-        Sets the name of the layer for curate tracking.
-        :param name: The name of the layer.
+        Enables memory access for the model and all its children.
         """
-        self._layer_name = name
+        for child in self.get_orca_modules_recursively():
+            if hasattr(child, "_memory_enabled"):
+                child._memory_enabled = True
 
-    def set_curate_run_ids(self, run_ids: list[int]) -> None:
+    def disable_memory(self) -> None:
         """
-        Sets the run IDs for the module and all its children.
-        :param run_ids: The run IDs to be set.
+        Disables memory access for the model and all its children.
         """
-        self._run_ids = run_ids
+        for child in self.get_orca_modules_recursively():
+            if hasattr(child, "_memory_enabled"):
+                child._memory_enabled = False
 
 
+@final
 class _LinearClassificationHead(OrcaModule):
     """A 2-Layer linear classification head generally used for a transformer model.
     Example usage:
-        .. code-block:: python
 
-                import torch
-                from orcalib import OrcaModule, _LinearClassificationHead
+    .. code-block:: python
 
-                class MyModule(OrcaModule):
-                    def __init__(self):
-                        super().__init__()
-                        self.linear = torch.nn.Linear(10, 10)
-                        self.classifier = _LinearClassificationHead(10, 5)
-
-                    def forward(self, x):
-                        x = self.linear(x)
-                        x = self.classifier(x)
-                        return x
+        import torch
+        from orcalib import OrcaModule, _LinearClassificationHead
 
-                model = MyModel()
+        class MyModule(OrcaModule):
+            def __init__(self):
+                super().__init__()
+                self.linear = torch.nn.Linear(10, 10)
+                self.classifier = _LinearClassificationHead(10, 5)
+
+            def forward(self, x):
+                x = self.linear(x)
+                x = self.classifier(x)
+                return x
+
+        model = MyModel()
     """
 
     def __init__(
         self,
         model_dim: int,
         num_labels: int,
         activation: Callable[[Tensor], Tensor] = F.relu,
         dropout: float = 0.1,
     ):
         """
-        :param model_dim: (int) The dimension of the input vector and hidden layers.
-        :param num_labels: (int) The size of the output vector.
-        :param activation: (Callable[[Tensor], Tensor]) The activation function to be used between the two linear layers. (default: F.relu)
-        :param dropout: (float) The dropout rate to be used between the two linear layers. (default: 0.1)
+        :param model_dim: The dimension of the input tensor.
+        :param num_labels: The number of labels.
+        :param activation: The activation function. (default: F.relu)
+        :param dropout: The dropout rate. (default: 0.1)
         """
         super().__init__()
 
+        self.model_dim = model_dim
+        self.num_labels = num_labels
         self.activation = activation
+        self.dropout = dropout
 
         self.linear1 = nn.Linear(model_dim, model_dim)
-        self.dropout = nn.Dropout(dropout)
+        self.dropout_layer = nn.Dropout(self.dropout)
         self.linear2 = nn.Linear(model_dim, num_labels)
 
     def forward(self, x) -> torch.Tensor:
         """
         Performs a forward pass through the linear classification head.
+
         :param x: The input tensor.
         :return: The output tensor.
         """
         x = self.linear1(x)
         x = self.activation(x)
-        x = self.dropout(x)
+        x = self.dropout_layer(x)
         x = self.linear2(x)
         return x
 
 
-class OrcaLookupType(NamedTuple):
-    """
-    A dataclass that represents the type of lookup to be performed in an OrcaDatabase index.
-    """
-
-    index_type: OrcaTypeHandle
-    return_column_types: tuple[OrcaTypeHandle, ...]
-
-
-@dataclass(slots=True)
-class OrcaLookupConfig:
-    """
-    A dataclass that represents the configuration for looking up in an OrcaDatabase index.
-    """
-
-    orca_db_name: str
-    index_name: str
-    lookup_column_names: tuple[ColumnName, ...]
-    num_memories: int
-
-    def __eq__(self, other):
-        if not isinstance(other, OrcaLookupConfig):
-            return False
-        my_db_name = self.orca_db_name
-        other_db_name = other.orca_db_name
-        return (
-            my_db_name == other_db_name
-            and self.index_name == other.index_name
-            and self.lookup_column_names == other.lookup_column_names
-            and self.num_memories == other.num_memories
-        )
-
-    def __hash__(self):
-        return hash((self.orca_db_name, self.index_name, self.lookup_column_names, self.num_memories))
-
-
-class OrcaGenericLookupLayer(OrcaModule):
-    """
-    A generic layer that instantiates a OrcaLookupType, and allows
-    for swapping of a OrcaLookupConfig for looking up in an OrcaDatabase index and returning the top k results,
-    based on the OrcaLookupType.
-
-    Currently this is only being used by the ChatBot Demo. A larger refactor is needed to change all interfaces
-    here and in all demos currently using OrcaLookupLayer. The merge should be fairly clean, with the only
-    larger issue being that the interface in user-land will change to use OrcaLookupType and OrcaLookupConfig
-    rather than passing db names, index names, column names, num memories, separately.
-    """
-
-    _cache: dict[tuple, Any] = {}
-
-    def __init__(
-        self,
-        orca_lookup_type: OrcaLookupType,
-        orca_lookup_config: Optional[OrcaLookupConfig] = None,
-        cache_ttl: Optional[float] = None,
-        **orca_module_settings,
-    ):
-        """
-        :param orca_lookup_type: The OrcaLookupType to use.
-        :param orca_lookup_config: The OrcaLookupConfig to use. If None, needs to be specified later. (default: None)
-        :param cache_ttl: The time to live (in seconds) for the lookup cache. If None, the cache is disabled. (default: None)
-        :param **orca_module_settings: Additional settings to pass to the parent OrcaModule constructor.
-        """
-
-        self._orca_lookup_type: OrcaLookupType = orca_lookup_type
-        self._orca_lookup_config: Optional[OrcaLookupConfig] = None
-        self._orca_db_instance: Optional[OrcaDatabase] = None
-
-        if orca_lookup_config:
-            self._orca_lookup_config = self._verify_compatible_lookup_config(orca_lookup_config)
-            self._orca_db_instance = OrcaDatabase(self._orca_lookup_config.orca_db_name)
-            super().__init__(orca_db_instance=self._orca_db_instance, **orca_module_settings)
-        else:
-            super().__init__(**orca_module_settings)
-
-        self.use_lookup_cache = cache_ttl is not None
-        assert (
-            not self.use_lookup_cache or not self._curate_enabled
-        ), "Curate tracking is not supported when using the lookup cache"
-        assert cache_ttl is None or isinstance(cache_ttl, (int, float))
-        self.cache_ttl = cache_ttl
-
-    @property
-    def orca_lookup_type(self) -> OrcaLookupType:
-        """
-        Returns the OrcaLookupType for this layer.
-        :return: The OrcaLookupType for this layer.
-        """
-        return self._orca_lookup_type
-
-    @property
-    def orca_lookup_config(self) -> OrcaLookupConfig | None:
-        """
-        Returns the OrcaLookupConfig for this layer.
-        :return: The OrcaLookupConfig for this layer.
-        """
-        return self._orca_lookup_config
-
-    @property
-    def orca_db_instance(self) -> OrcaDatabase | None:
-        """
-        Returns the OrcaDatabase instance for this layer.
-        :return: The OrcaDatabase instance for this layer.
-        """
-        return self._orca_db_instance
-
-    @lru_cache(maxsize=16)
-    def _verify_compatible_lookup_config(self, lookup_config: OrcaLookupConfig) -> OrcaLookupConfig:
-        """
-        Verifies that the lookup config is compatible with the lookup type.
-
-        The verification results are cached to avoid redundant checks.
-
-        :param lookup_config: The OrcaLookupConfig to be verified.
-        :return: The verified OrcaLookupConfig.
-
-        NOTE: This method should not be called directly. It is used internally.
-        """
-
-        db = OrcaDatabase(lookup_config.orca_db_name)
-
-        new_index = db.get_index(lookup_config.index_name)
-        assert (
-            new_index.column_type == self.orca_lookup_type.index_type
-        ), f"Index type mismatch. Expected: {self.orca_lookup_type.index_type}, got: {new_index.index_type}"
-
-        assert len(lookup_config.lookup_column_names) == len(
-            self.orca_lookup_type.return_column_types
-        ), f"Column count mismatch. Expected: {len(self.orca_lookup_type.return_column_types)}, got: {len(lookup_config.lookup_column_names)}"
-
-        # get the table info for this index and verify the column types
-        table_info = db._get_index_table(lookup_config.index_name)
-
-        assert len(lookup_config.lookup_column_names) == len(
-            self.orca_lookup_type.return_column_types
-        ), f"Column count mismatch. Expected: {len(self.orca_lookup_type.return_column_types)}, got: {len(lookup_config.lookup_column_names)}"
-
-        for column_name, column_type in zip(
-            lookup_config.lookup_column_names, self.orca_lookup_type.return_column_types
-        ):
-            if column_name in table_info:
-                assert (
-                    table_info[column_name] == column_type
-                ), f"Column type mismatch for {column_name}. Expected: {column_type}, got: {table_info[column_name]}"
-            elif column_name[0] == "$" and column_name[1:] in new_index.artifact_columns:
-                computed_column_name = column_name[1:]
-                assert (
-                    new_index.artifact_columns[computed_column_name] == column_type
-                ), f"Column type mismatch for {column_name}. Expected: {column_type}, got: {new_index.artifact_columns[computed_column_name]}"
-            else:
-                raise ValueError(f"Column {column_name} not found in table or index {lookup_config.index_name}")
-
-        return lookup_config
-
-    def set_lookup_config(self, lookup_config: OrcaLookupConfig) -> None:
-        """Overrides the OrcaLookupConfig for this layer with a new one if it matches the OrcaLookupType.
-
-        :param lookup_config: The new OrcaLookupConfig to use.
-        """
-        self._orca_lookup_config = self._verify_compatible_lookup_config(lookup_config)
-        self._orca_db_instance = OrcaDatabase(name=self._orca_lookup_config.orca_db_name)
-
-    def _db_lookup(
-        self,
-        query: Any,
-        db: OrcaDatabase,
-        orca_lookup_config: OrcaLookupConfig,
-    ) -> BatchedScanResult:
-        """
-        Performs the lookup in the OrcaDatabase index.
-        :param query: The query to be used for the lookup.
-        :param orca_lookup_config: The OrcaLookupConfig to be used for the lookup.
-        :return: The result of the lookup.
-
-        NOTE: This method should not be called directly. It is used internally.
-        """
-
-        cache_key = None
-        if self.use_lookup_cache:
-            cache_key = (
-                query,
-                orca_lookup_config,
-            )
-            mem = OrcaGenericLookupLayer._cache.get(cache_key, None)
-            if mem is not None:
-                result, timestamp = mem
-                if timestamp + self.cache_ttl > time.time():
-                    return result
-
-        # TODO same hack as in OrcaTextLookupLayer, will change with index refactor
-        if isinstance(query, torch.Tensor):
-            query = query.detach().cpu().to(torch.float32).numpy().tolist()
-        req = db.vector_scan_index(orca_lookup_config.index_name, query)
-
-        # track this particular lookup using Curate
-        if self._curate_enabled:
-            if isinstance(query, torch.Tensor):
-                assert query.shape[0] == len(
-                    self._run_ids
-                ), f"Batch size inference appears incorrect. Please set batch size manually. Inferred: {query.shape[0]}, expected: {len(self._run_ids)}"
-                req = req.track_with_curate(self._run_ids, self._layer_name or "NA")
-
-            elif isinstance(query, list):
-                assert len(query) == len(
-                    self._run_ids
-                ), f"Batch size inference appears incorrect. Please set batch size manually. Inferred: {len(query)}, expected: {len(self._run_ids)}"
-                req = req.track_with_curate(self._run_ids, self._layer_name or "NA")
-
-        res = req.select(*orca_lookup_config.lookup_column_names).fetch(orca_lookup_config.num_memories)  # type: ignore
-
-        if self.use_lookup_cache:
-            OrcaGenericLookupLayer._cache[cache_key] = (res, time.time())  # type: ignore
-
-        return res
-
-    def forward(
-        self,
-        x: Any,
-        orca_lookup_config: Optional[OrcaLookupConfig] = None,
-    ) -> BatchedScanResult:
-        """Performs a "forward pass" or call/retrieval to the lookup layer.
-        :param x: The input list of length batch_size or tensor of shape (batch_size, vector_dim)
-        :param orca_lookup_config: Optional override for the OrcaLookupConfig to use. (default: None)
-        :return: dependent on the orca_lookup_config (return column types)
-        """
-        if orca_lookup_config is not None:
-            orca_lookup_config = self._verify_compatible_lookup_config(orca_lookup_config)
-            db = OrcaDatabase(name=orca_lookup_config.orca_db_name)
-        else:
-            orca_lookup_config = self._orca_lookup_config
-            db = self._orca_db_instance
-            assert orca_lookup_config is not None, "OrcaLookupConfig must be set before lookup, or passed to forward()"
-            assert db is not None, "No OrcaDatabase instance, set_lookup_config or pass OrcaLookupConfig to forward()"
-
-        if orca_lookup_config.num_memories is not None and orca_lookup_config.num_memories <= 0:
-            raise ValueError(f"num_memories must be > 0, but is {orca_lookup_config.num_memories}")
-
-        res = self._db_lookup(x, db, orca_lookup_config)
-
-        return res
-
-
-class OrcaLookupLayer(OrcaModule):
+class OrcaLookupLayer(OrcaLookupModule):
     """A layer that looks up a vector in an OrcaDatabase index and returns the top k results.
     This requires a database to be attached to the model, with the index already created.
 
     Example usage:
+
     .. code-block:: python
 
-            import torch
-            from orcalib import OrcaModule, OrcaLookupLayer
+        import torch
+        from orcalib import OrcaModule, OrcaLookupLayer
 
-            class MyModule(OrcaModule):
-                def __init__(self):
-                    super().__init__()
-                    self.linear = torch.nn.Linear(10, 10)
-                    self.lookup = OrcaLookupLayer("my_index", ["my_label, my_extra_columns"], 10)
-
-                def forward(self, x):
-                    x = self.linear(x)
-                    x, meta = self.lookup(x)
-                    return x, meta
+        class MyModule(OrcaModule):
+            def __init__(self):
+                super().__init__()
+                self.linear = torch.nn.Linear(10, 10)
+                self.lookup = OrcaLookupLayer("my_index", ["my_label, my_extra_columns"], 10)
 
-            model = MyModel()
+            def forward(self, x):
+                x = self.linear(x)
+                x, meta = self.lookup(x)
+                return x, meta
+
+        model = MyModel()
 
     """
 
-    _orca_db_instance: OrcaDatabase
     _cache: dict[tuple, Any] = {}
 
     def __init__(
         self,
-        index_name: Optional[str] = None,
-        lookup_column_names: Optional[list[ColumnName]] = None,
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Memory Lookup Settings
+        memory_index_name: Optional[str] = None,
+        lookup_column_names: Optional[list[str]] = None,
         num_memories: Optional[int] = None,
-        cache_ttl: Optional[float] = None,
-        orca_db_instance: Optional[OrcaDatabase] = None,
-        **settings,
+        freeze_num_memories: bool = False,
+        cache_ttl: Optional[int] = None,
     ):
         """
-        :param index_name: The name of the index to use. (default: None)
-        :param lookup_column_names: The names of the columns to return from the index. (default: None)
-        :param num_memories: The number of memories to return from the index. (default: None)
-        :param cache_ttl: The time to live (in seconds) for the lookup cache. If None, the cache is disabled. (default: None)
-        :param orca_db_instance: The OrcaDatabase instance to use. If None, the default OrcaDatabase instance is used. (default: None)
-        :param **settings: Additional settings to pass to the parent constructor.
-        """
-        super().__init__(orca_db_instance=orca_db_instance, **settings)
-        self.index_name = index_name
-        self.lookup_column_names = lookup_column_names
-        self.num_memories = num_memories
-        self.use_lookup_cache = cache_ttl is not None
-        assert (
-            not self.use_lookup_cache or not self._curate_enabled
-        ), "Curate tracking is not supported when using the lookup cache"
-        assert cache_ttl is None or isinstance(cache_ttl, (int, float))
-        self.cache_ttl = cache_ttl
-
-    @property
-    def orca_db_instance(self) -> OrcaDatabase:
-        """
-        Returns the OrcaDatabase instance for this layer.
-        :return: The OrcaDatabase instance for this layer.
+        :param database: The OrcaDatabase instance to use for lookups and curate tracking. (default: None)
+        :param curate_enabled: Whether Curate tracking is enabled. (default: False)
+        :param memory_index_name: The name of the index to use for lookups. (default: None)
+        :param lookup_column_names: The names of the columns to return from the index during a lookup. (default: None)
+        :param num_memories: The number of memories to return from the index during a lookup. (default: None)
+        :param freeze_num_memories: Whether the number of memories should be frozen. (default: False)
+        :param cache_ttl: The time-to-live for the lookup cache. (default: None)
         """
-        return self._orca_db_instance
 
-    @orca_db_instance.setter
-    def orca_db_instance(self, value: OrcaDatabase) -> None:
-        """
-        Sets the OrcaDatabase instance for this layer.
-        :param value: The OrcaDatabase instance to be set.
-        """
-        self._orca_db_instance = value
+        super().__init__(
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            lookup_column_names=lookup_column_names,
+            num_memories=num_memories,
+            freeze_num_memories=freeze_num_memories,
+            propagate_lookup_settings=False,
+        )
+        self.cache_ttl = cache_ttl
+        self.use_lookup_cache = self.cache_ttl is not None
+        assert (
+            not self.use_lookup_cache or not self.curate_enabled
+        ), "Curate tracking is not supported when using the lookup cache"
 
     def _get_index_info_with_overrides(
         self,
         orca_db_instance: Optional[OrcaDatabase] = None,
         index_name: Optional[str] = None,
         lookup_column_names: Optional[list[str]] = None,
         num_memories: Optional[int] = None,
     ) -> tuple[OrcaDatabase, str, list[str], int]:
         """
         Returns the index-lookup info, with overrides applied where provided
+
         :param orca_db_instance: The OrcaDatabase instance to use. (default: None)
         :param index_name: The name of the index to use. (default: None)
         :param lookup_column_names: The names of the columns to return from the index. (default: None)
         :param num_memories: The number of memories to return from the index. (default: None)
         :return: A tuple of (OrcaDatabase, index_name, lookup_column_names, num_memories)
 
         NOTE: This method should not be called directly. It is used internally.
         """
-        orca_db_instance = orca_db_instance or self.orca_db_instance
+        orca_db_instance = orca_db_instance or self.lookup_database_instance  # type: ignore
         if orca_db_instance is None:
             raise ValueError("OrcaDatabase instance must be set before lookup or passed to forward()")
 
-        index_name = index_name or self.index_name
+        index_name = index_name or self.memory_index_name
         if index_name is None:
             raise ValueError("Index name must be set before lookup or passed to forward()")
 
         lookup_column_names = lookup_column_names or self.lookup_column_names
         if lookup_column_names is None:
             raise ValueError("Lookup column names must be set before lookup or passed to forward()")
 
@@ -872,14 +607,15 @@
         orca_db_instance: OrcaDatabase,
         index_name: str,
         lookup_column_names: list[str],
         num_memories: int,
     ) -> BatchedScanResult:
         """
         Performs the lookup in the OrcaDatabase index.
+
         :param x: The input tensor of shape (batch_size, vector_dim)
         :param orca_db_instance: The OrcaDatabase instance to use.
         :param index_name: The name of the index to use.
         :param lookup_column_names: The names of the columns to return from the index.
         :param num_memories: The number of memories to return from the index.
         :return: The result of the lookup.
 
@@ -900,19 +636,20 @@
                 if timestamp + self.cache_ttl > time.time():
                     return result
 
         query = x.detach().cpu().to(torch.float32).numpy().tolist()
         req = orca_db_instance.vector_scan_index(index_name, query)
 
         # track this particular lookup using Curate
-        if self._curate_enabled:
+        if self.curate_enabled:
+            assert self.curate_run_ids is not None, "Run IDs must be set when using lookup layers with Curate enabled"
             assert x.shape[0] == len(
-                self._run_ids
-            ), f"Batch size inference appears incorrect. Please set batch size manually. Inferred: {x.shape[0]}, expected: {len(self._run_ids)}"
-            req = req.track_with_curate(self._run_ids, self._layer_name or "NA")
+                self.curate_run_ids
+            ), f"Batch size inference appears incorrect. Please set batch size manually. Inferred: {x.shape[0]}, expected: {len(self.curate_run_ids)}"
+            req = req.track_with_curate(self.curate_run_ids, self.curate_layer_name or "NA")
 
         # execute the lookup (fetch), where meta is a list of additional columns to be returned
         # aside from the index vector matches
         res = req.select(*lookup_column_names).fetch(num_memories)  # type: ignore
 
         if self.use_lookup_cache:
             OrcaLookupLayer._cache[cache_key] = (res, time.time())  # type: ignore
@@ -924,22 +661,22 @@
         x: torch.Tensor,
         orca_db_instance: Optional[OrcaDatabase] = None,
         index_name: Optional[str] = None,
         lookup_column_names: Optional[list[str]] = None,
         num_memories: Optional[int] = None,
     ) -> BatchedScanResult:
         """Performs a forward pass
+
         :param x: The input tensor of shape (batch_size, vector_dim)
         :param orca_db_instance: Optional override for the OrcaDatabase instance to use. (default: None)
         :param index_name: Optional override for the name of the index to use. (default: None)
         :param lookup_column_names: Optional override for the names of the columns to return from the index. (default: None)
         :param num_memories: Optional override for the number of memories to return from the index. (default: None)
-        :return: A tuple of (memories, extra) where
-        memories is a tensor of shape (batch_size, num_memories, vector_dim) and
-        extra is a list of lists of metadata values of shape (batch_size, num_memories, num_meta_columns)
+        :return: A tuple of (memories, extra) where memories is a tensor of shape (batch_size, num_memories, vector_dim) and
+            extra is a list of lists of metadata values of shape (batch_size, num_memories, num_meta_columns)
         """
         if num_memories is not None and num_memories <= 0:
             raise ValueError(f"num_memories must be > 0, but is {num_memories}")
 
         index_settings = self._get_index_info_with_overrides(
             orca_db_instance, index_name, lookup_column_names, num_memories
         )
@@ -950,23 +687,24 @@
         # res "shape" is (batch_size, num_memories, num_meta_columns)
         # res[i][j] is a VectorScanResult object, which includes a vector and extra metadata
 
         assert isinstance(res, BatchedScanResult)
         return res
 
 
-class OrcaLabelLookupLayer(OrcaLookupLayer):
+class OrcaLabelLookupLayer(OrcaLookupLayer, LabelColumnNameMixin):
     """A layer that looks up the embedding and label in an OrcaDatabase index and returns the top k results.
 
     A layer that looks up a vector in an OrcaDatabase index and returns a tuple of two tensors that contain
     the embedding and label for the top k results.
 
     This requires a database to be attached to the model, with the index already created.
 
     Example usage:
+
     .. code-block:: python
 
         import torch
         from orcalib import OrcaModule, OrcaLabelLookupLayer
 
         class MyModule(OrcaModule):
             def __init__(self):
@@ -984,101 +722,124 @@
                 return embeddings,labels
 
         model = MyModel()
     """
 
     def __init__(
         self,
-        index_name: str,
-        label_column_name: ColumnName,
-        num_memories: int,
-        cache_ttl: Optional[float] = None,
-        orca_db_instance: Optional[OrcaDatabase] = None,
-        **settings,
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Lookup Settings
+        memory_index_name: Optional[str] = None,
+        label_column_name: Optional[ColumnName] = None,
+        num_memories: Optional[int] = None,
+        freeze_num_memories: bool = False,
     ):
         """Initializes the OrcaLabelLookupLayer.
-        :param index_name: The name of the index to use.
-        :param label_column_name: The name of the label column to return from the index.
-        :param num_memories: The number of memories to return from the index.
-        :param cache_ttl: The time to live (in seconds) for the lookup cache. If None, the cache is disabled. (default: None)
-        :param orca_db_instance: The OrcaDatabase instance to use. If None, the default OrcaDatabase instance is used. (default: None)
-        :param **settings: Additional settings to pass to the parent constructor.
+        :param database: The OrcaDatabase instance to use for lookups and curate tracking. (default: None)
+        :param curate_enabled: Whether Curate tracking is enabled. (default: False)
+        :param memory_index_name: The name of the index to use for lookups. (default: None)
+        :param label_column_name: The name of the label column to return from the index. (default: None)
+        :param num_memories: The number of memories to return from the index during a lookup. (default: None)
+        :param freeze_num_memories: Whether the number of memories should be frozen. (default: False) When
+        set to True, an error will be raised if an attempt is made to change the number of memories.
         """
         super().__init__(
-            index_name, ["$embedding", label_column_name], num_memories, cache_ttl, orca_db_instance, **settings
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            lookup_column_names=None,
+            num_memories=num_memories,
+            freeze_num_memories=freeze_num_memories,
+            cache_ttl=None,
         )
-
-        self._label_column_name = label_column_name
+        self.label_column_name = label_column_name
 
     def forward(
         self,
         x: torch.Tensor,
         orca_db_instance: Optional[OrcaDatabase] = None,
         index_name: Optional[str] = None,
         label_column_name: Optional[ColumnName] = None,
         num_memories: Optional[int] = None,
     ) -> tuple[Tensor, Tensor]:
         """
         Performs a forward pass
+
         :param x: The input tensor of shape (batch_size, vector_dim)
         :param orca_db_instance: Optional override for the OrcaDatabase instance to use. (default: None)
         :param index_name: Optional override for the name of the index to use. (default: None)
         :param label_column_name: Optional override for the name of the label column to return from the index. (default: None)
         :param num_memories: Optional override for the number of memories to return from the index. (default: None)
-        :return: A tuple of (embeddings, labels) where
-        embeddings is a tensor of shape (batch_size, num_memories, vector_dim) and
-        labels is an int64 tensor of shape (batch_size, num_memories)
+        :return: A tuple of (embeddings, labels) where embeddings is a tensor of shape (batch_size, num_memories, vector_dim) and
+            labels is an int64 tensor of shape (batch_size, num_memories)
         """
         label_override = None
         if label_column_name:
             label_override = ["$embedding", label_column_name]
         else:
-            label_column_name = self._label_column_name
+            label_column_name = self.label_column_name
 
-        label_column_name = label_column_name or self._label_column_name
+        label_column_name = label_column_name or self.label_column_name
         result = super().forward(x, orca_db_instance, index_name, label_override, num_memories)
         memories = result.to_tensor("$embedding", dtype=x.dtype, device=x.device)
         labels = result.to_tensor(label_column_name, dtype=torch.int64, device=x.device).squeeze(-1)
         return memories, labels
 
 
-class OrcaClassificationMemoryGuideLayer(OrcaModule):
+class OrcaClassificationMemoryGuideLayer(OrcaLookupModule, LabelColumnNameMixin):
     """
     A PyTorch module that implements a memory-guided classification layer.
 
     This layer biases the output of a classification model towards a set of memories
     The bias is controlled by a weight parameter, which determines how strongly the model should be biased towards the memories.
     """
 
     def __init__(
         self,
         num_classes: int,
-        memory_index: str,
-        memory_label: str,
         num_memories: int,
-        guide_weight: float,
         enable_in_training: bool = False,
-        **settings,
+        guide_weight: float = 0.1,
+        # Shared settings
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Lookup Settings
+        memory_index_name: Optional[str] = None,
+        label_column_name: Optional[ColumnName] = None,
     ):
         """
         :param num_classes: The number of classes in the classification task.
-        :param memory_index: The name of the memory index to use.
-        :param memory_label: The column name of the label for the classification task in the table underpinning memory_index.
         :param num_memories: The number of memories the layer should use.
-        :param guide_weight: The weight of the memory guide (i.e. how strongly to bias towards the memory distribution)
-        :param enable_in_training: Whether to enable the module in training mode. (default: False)
-        :param **settings: Additional settings to pass to the parent constructor.
+        :param enable_in_training: Whether to enable the layer during training. (default: False)
+        :param guide_weight: The weight of the memory guide. (default: 0.1)
+        :param database: The OrcaDatabase instance to use for lookups and curate tracking. (default: None)
+        :param curate_enabled: Whether Curate tracking is enabled. (default: False)
+        :param memory_index_name: The name of the index to use for lookups. (default: None)
+        :param label_column_name: The name of the label column to return from the index. (default: None)
         """
-        super().__init__(**settings)
+        super().__init__(
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            lookup_column_names=None,
+            num_memories=num_memories,
+            freeze_num_memories=True,
+            propagate_lookup_settings=True,
+        )
 
         self.num_classes = num_classes
-        self.guide_weight = guide_weight
         self.enable_in_training = enable_in_training
-        self.memory_label = memory_label
-        self.lookup = OrcaLabelLookupLayer(memory_index, memory_label, num_memories)
+        self.guide_weight = guide_weight
+        self.label_column_name = label_column_name
+
+        # Lookup settings will be propagated to the lookup layer
+        self.lookup = OrcaLabelLookupLayer(database=database)
 
     def forward(
         self,
         logits: torch.Tensor,
         memory_key: torch.Tensor,
         ctx: Optional[torch.Tensor] = None,
         labels: Optional[torch.Tensor] = None,
@@ -1107,100 +868,111 @@
         bias = torch.sum(bias, dim=1)
         bias = torch.nn.functional.softmax(bias, dim=1)
         logits = probs + self.guide_weight * bias
 
         return logits
 
 
-class ProjectionMode(Enum):
-    """
-    Determines how the values from the memory should be "projected" into the models embedding space (i.e. what's the V in the attention mechanism QKV).
-
-    Attributes:
-        LABEL: Project the memory's label into the model embedding space.
-        POSITIONAL: Project the memory's position (0...num_memories-1) into the model embedding space.
-    """
-
-    LABEL = 0
-    POSITIONAL = 1
-
-
-class OrcaClassificationCrossAttentionLayer(OrcaModule):
+class OrcaClassificationCrossAttentionLayer(OrcaLookupModule, LabelColumnNameMixin):
     """A transformer decoder layer block that does cross attention
 
     Note that this is Classification-specific, and the labels returned by the lookup layer are used as the value-weights for the cross attention.
 
     The block contains the typical transformer components: multi-head attention, feed forward, and layer norm.
     The block also contains a lookup layer that looks up a vector in an OrcaDatabase index and returns the top k results.
     These results are used as the memory context for the cross attention.
     """
 
     def __init__(
         self,
         model_dim: int,
         num_heads: int,
         num_classes: int,
-        memory_index: str,
-        memory_label: str,
         num_memories: int,
-        activation: Callable[[Tensor], Tensor] = F.relu,
         dropout: float = 0.1,
-        split_retrieval_path: bool = False,
+        activation: Callable[[Tensor], Tensor] = F.relu,
         projection_mode: ProjectionMode = ProjectionMode.LABEL,
-        **settings,
+        split_retrieval_path: bool = False,
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Lookup Settings
+        memory_index_name: Optional[str] = None,
+        label_column_name: Optional[ColumnName] = None,
     ):
         """
         :param model_dim: (int) The dimension of the input vector and hidden layers.
         :param num_heads: (int) The number of heads to be used in the multi-head attention layer.
         :param num_classes: (int) The number of classes for the output classification and weights for cross attention.
-        :param memory_index: (str) The name of the OrcaDatabase index to be used for the memory lookup.
-        :param memory_label: (str) The name of the column in the OrcaDatabase index to be used as the memory label for value weighting. (e.g., "label")
         :param num_memories: (int) The number of memory vectors to be returned from the lookup.
-        :param activation: (Callable[[Tensor], Tensor]) The activation function to be used between the two linear layers. (default: F.relu)
-        :param dropout: (float) The dropout rate to be used between the two linear layers. (default: 0.1)
-        :param split_retrieval_path: (bool) Whether to split the retrieval path from the forward pass. If True, the memory key must be passed in to the forward pass. (default: False)
-        :param projection_mode: (ProjectionMode) The mode to be used for projecting the memory into the model embedding space. (default: ProjectionMode.LABEL)
-        This is used when the memory key is different from the input vector
+        :param dropout: (float) The dropout rate. (default: 0.1)
+        :param activation: (Callable[[Tensor], Tensor]) The activation function. (default: F.relu)
+        :param projection_mode: (ProjectionMode) The projection mode to use for the memory labels. (default: ProjectionMode.LABEL)
+        :param split_retrieval_path: (bool) Whether to split the retrieval path. (default: False)
+        :param database: (OrcaDatabase | str | None) The OrcaDatabase instance to use for lookups and curate tracking. (default: None)
+        :param curate_enabled: (bool) Whether Curate tracking is enabled. (default: False)
+        :param memory_index_name: (Optional[str]) The name of the index to use for lookups. (default: None)
+        :param label_column_name: (Optional[ColumnName]) The name of the label column to return from the index. (default: None)
         """
-        super().__init__(**settings)
 
+        super().__init__(
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            lookup_column_names=None,
+            num_memories=num_memories,
+            freeze_num_memories=True,
+            propagate_lookup_settings=True,
+        )
+
+        self.model_dim = model_dim
+        self.num_heads = num_heads
         self.num_classes = num_classes
-        self.memory_index = memory_index
-        self.memory_label = memory_label
+        self.dropout = dropout
         self.activation = activation
-        self.split_retrieval_path = split_retrieval_path
         self.projection_mode = projection_mode
-        self.num_memories = num_memories
+        self.split_retrieval_path = split_retrieval_path
+        self.label_column_name = label_column_name
 
-        self.lookup = OrcaLabelLookupLayer(memory_index, memory_label, num_memories)
+        # Lookup settings will be automatically propagated to the lookup layer
+        self.lookup = OrcaLabelLookupLayer(database=database, num_memories=num_memories)
 
         self.cross_attention = nn.MultiheadAttention(
-            model_dim, num_heads, dropout=dropout, batch_first=True, vdim=num_classes
+            self.model_dim,
+            self.num_heads,
+            dropout=self.dropout,
+            batch_first=True,
+            vdim=self.num_classes,
         )
-        self.attn_norm = nn.LayerNorm(model_dim)
+        self.attn_norm = nn.LayerNorm(self.model_dim)
 
-        self.linear1 = nn.Linear(model_dim, model_dim * 4)
-        self.dropout1 = nn.Dropout(dropout)
-        self.linear2 = nn.Linear(model_dim * 4, model_dim)
-        self.dropout2 = nn.Dropout(dropout)
-        self.ff_norm = nn.LayerNorm(model_dim)
+        self.linear1 = nn.Linear(self.model_dim, self.model_dim * 4)
+        self.dropout1 = nn.Dropout(self.dropout)
+        self.linear2 = nn.Linear(self.model_dim * 4, self.model_dim)
+        self.dropout2 = nn.Dropout(self.dropout)
+        self.ff_norm = nn.LayerNorm(self.model_dim)
 
     def forward(
         self,
         x: torch.Tensor,  # Shape (batch_size, vector_dim)
         ctx: Optional[torch.Tensor] = None,  # Shape (batch_size, num_memories, vector_dim)
         labels: Optional[torch.Tensor] = None,  # Shape (batch_size, num_memories, meta_column_count)
         memory_key: Optional[torch.Tensor] = None,  # Shape (batch_size, vector_dim)
     ) -> torch.Tensor:  # x is the input vector N x D, ctx is the memory context N x K x D
-        """x, ctx, labels act as Q, K, V for the cross attention layer.
+        """
+        x, ctx, labels act as Q, K, V for the cross attention layer.
+
         When ctx is None:
-            If split_retrieval_path is False, x is used as both Q and K.
-            If split_retrieval_path is True, memory_key is used as K (instead of x)
+
+        * If split_retrieval_path is False, x is used as both Q and K.
+        * If split_retrieval_path is True, memory_key is used as K (instead of x)
+
         When ctx is not None:
-            values
+
+        * values
 
         :param x: The input tensor of shape (N, D), where N is the batch size and D is the model embedding dimension.
         :param ctx: The memory context tensor of shape (N, K, D), where N is the batch size, K is the number of memories, and D is the model embedding dimension. (default: None)
         :param labels: The memory label tensor of shape (N, K), where N is the batch size and K is the number of memories. (default: None)
         :param memory_key: The memory key tensor of shape (N, D), where N is the batch size and D is the model embedding dimension. (default: None)
         :return: The output tensor of shape (N, D), where N is the batch size and D is the model embedding dimension.
         """
@@ -1232,30 +1004,55 @@
         y = self.linear2(y)  # N x D
         y = self.dropout2(y)
         x = self.ff_norm(y + x)  # N x D
 
         return x
 
 
-class OrcaMemoryBindingLayer(OrcaModule):
+class OrcaMemoryBindingLayer(OrcaLookupModule, LabelColumnNameMixin):
     """
     A PyTorch module that implements a memory binding layer.
     """
 
-    def __init__(self, num_classes: int, memory_index: str, memory_label: str, num_memories: int):
+    def __init__(
+        self,
+        num_memories: int,
+        num_classes: int,
+        # Shared Settings
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Lookup Settings
+        memory_index_name: Optional[str] = None,
+        label_column_name: Optional[ColumnName] = None,
+    ):
         """
-        :param num_classes: The number of classes in the classification task.
-        :param memory_index: The name of the OrcaDatabase index to be used for the memory lookup.
-        :param memory_label: The name of the column in the OrcaDatabase index to be used as the memory label for value weighting. (e.g., "label")
         :param num_memories: The number of memory vectors to be returned from the lookup.
+        :param num_classes: The number of classes for the output classification and weights for cross attention.
+        :param settings: The settings for the OrcaMemoryBindingLayer.
         """
-        super().__init__()
+        super().__init__(
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            lookup_column_names=None,
+            num_memories=num_memories,
+            freeze_num_memories=True,
+            propagate_lookup_settings=True,
+        )
 
-        self.lookup = OrcaLabelLookupLayer(memory_index, memory_label, num_memories)
         self.num_classes = num_classes
+        self.label_column_name = label_column_name
+
+        # Lookup settings will be automatically propagated to the lookup layer
+        self.lookup = OrcaLabelLookupLayer(
+            database=database,
+            num_memories=num_memories,
+            freeze_num_memories=True,
+        )
 
     def forward(
         self,
         logits: torch.Tensor,
         memory_key: Optional[torch.Tensor] = None,
         ctx: Optional[torch.Tensor] = None,
         labels: Optional[torch.Tensor] = None,
@@ -1273,129 +1070,151 @@
 
         mem_labels = (
             torch.nn.functional.one_hot(labels, num_classes=self.num_classes).to(logits.dtype).to(logits.device)  # type: ignore
         )
         return torch.bmm(logits.unsqueeze(1), mem_labels).squeeze()
 
 
-class ClassificationMode(Enum):
-    """
-    Determined how the final classification is performed.
-
-    Attributes:
-        DIRECT: Predicts directly into `num_classes` like a conventional classification model.
-        MEMORY_BOUND: which uses memory binding to make the prediction (i.e. pick from the classes in the memories).
-    """
-
-    DIRECT = 0
-    MEMORY_BOUND = 1
-
-
 class OrcaClassificationHead(
-    OrcaModule
+    OrcaLookupModule, LabelColumnNameMixin
 ):  # Input: single vector of size hidden_size, optional memory context (otherwise looked up), Output: single vector of size num_labels
-    """A transformer decoder layer block that does cross attention with memory lookup
+    """
+    A transformer decoder layer block that does cross attention with memory lookup
 
     Example usage:
+
     .. code-block:: python
+
         import torch
         from orcalib.orca_torch import OrcaModule, OrcaClassificationHead
 
         class MyModule(OrcaModule):
             def __init__(self):
                 super().__init__()
-                self.linear = torch.nn.Linear(10, 10)
+                self.trunk = torch.nn.Linear(10, 10)
                 self.classifier = OrcaClassificationHead(model_dim=10, num_classes=5, "my_index", "my_label", num_memories=10)
 
             def forward(self, x):
-                x = self.linear(x) # N x 10
+                x = self.trunk(x) # N x 10
                 x = self.classifier(x)
                 return x # N x 5, e.g., where each row may become logits for a softmax
     """
 
     def __init__(
         self,
-        model_dim,
-        num_classes,
-        memory_index: str,
-        memory_label: str,
+        model_dim: int,
+        num_classes: int,
         num_memories: int,
         num_layers: int = 1,
         num_heads: int = 8,
+        classification_mode: ClassificationMode = ClassificationMode.DIRECT,
         activation: Callable[[Tensor], Tensor] = F.relu,
         dropout: float = 0.1,
-        deep_residuals: bool = False,
+        deep_residuals: bool = True,
         split_retrieval_path: bool = False,
         memory_guide_weight: float = 0.0,
-        classification_mode: ClassificationMode = ClassificationMode.DIRECT,  # DIRECT implies ProjectionMode.LABEL, MEMORY_BOUND implies ProjectionMode.POSITIONAL
         single_lookup: bool = True,
-        **settings,
+        # Shared Settings
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Lookup Settings
+        memory_index_name: Optional[str] = None,
+        label_column_name: Optional[ColumnName] = None,
     ):
         """
         :param model_dim: (int) The dimension of the input vector and hidden layers.
         :param num_classes: (int) The size of the output vector.
-        :param memory_index: (str) The name of the OrcaDatabase index to be used for the memory lookup.
-        :param memory_label: (str) The name of the column in the OrcaDatabase index to be used as the memory label. (e.g., "label")
         :param num_memories: (int) The number of memory vectors to be returned from the lookup.
         :param num_layers: (int) The number of attention blocks to be used, copies of OrcaClassificationCrossAttentionLayer. (default: 1)
         :param num_heads: (int) The number of heads to be used in the multi-head attention layer. (default: 8)
-        :param activation: (Callable[[Tensor], Tensor]) The activation function used throughout the attention blocks. (default: F.relu)
-        :param dropout: (float) The dropout rate to be used between the two linear layers. (default: 0.1)
-        :param deep_residuals: (bool) Whether to use the residual (skip) connections. (default: False)
-        :param split_retrieval_path: (bool) Whether to split the retrieval path from the forward pass. If True, the memory key must be passed in to the forward pass. (default: False)
-        :param memory_guide_weight: (float) The weight of the memory guide (i.e. how strongly to bias towards the memory distribution). (default: 0.0)
         :param classification_mode: (ClassificationMode) The mode of classification to be used. (default: ClassificationMode.DIRECT)
-        :param single_lookup: (bool) Whether to use a single lookup for the memory context. (default: True)
-        :param settings: (Any) Any additional settings to be applied to the model.
+        :param activation: (Callable[[Tensor], Tensor]) The activation function. (default: F.relu)
+        :param dropout: (float) The dropout rate. (default: 0.1)
+        :param deep_residuals: (bool) Whether to use deep residuals. (default: True)
+        :param split_retrieval_path: (bool) Whether to split the retrieval path. (default: False)
+        :param memory_guide_weight: (float) The weight of the memory guide. (default: 0.0)
+        :param single_lookup: (bool) Whether to use a single lookup. (default: True)
+        :param database: (OrcaDatabase | str | None) The OrcaDatabase instance to use for lookups and curate tracking. (default: None)
+        :param curate_enabled: (bool) Whether Curate tracking is enabled. (default: False)
+        :param memory_index_name: (Optional[str]) The name of the index to use for lookups. (default: None)
+        :param label_column_name: (Optional[ColumnName]) The name of the label column to return from the index. (default: None)
         """
-        super().__init__(**settings)
+        super().__init__(
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            lookup_column_names=None,
+            num_memories=num_memories,
+            freeze_num_memories=True,
+            propagate_lookup_settings=True,
+        )
+
         self.classification_mode = classification_mode
+        self.model_dim = model_dim
+        self.num_classes = num_classes
+        self.activation = activation
+
+        self.dropout = dropout
+        self.deep_residuals = deep_residuals
+        self.split_retrieval_path = split_retrieval_path
+        self.memory_guide_weight = memory_guide_weight
+        self.single_lookup = single_lookup
+        self.label_column_name = label_column_name
+
         if classification_mode == ClassificationMode.MEMORY_BOUND:
-            projection_mode = ProjectionMode.POSITIONAL
-            self.memory_binding = OrcaMemoryBindingLayer(num_classes, memory_index, memory_label, num_memories)
-            inner_classes = num_memories
+            self.projection_mode = ProjectionMode.POSITIONAL
+            # Lookup settings will be automatically propagated to the lookup layer
+            self.memory_binding = OrcaMemoryBindingLayer(
+                num_memories=num_memories,
+                num_classes=num_classes,
+            )
+            self.inner_classes = self.num_memories
         elif classification_mode == ClassificationMode.DIRECT:
-            projection_mode = ProjectionMode.LABEL
+            self.projection_mode = ProjectionMode.LABEL
             self.memory_binding = torch.nn.Identity()
-            inner_classes = num_classes
+            self.inner_classes = self.num_classes
         else:
-            raise ValueError(f"Unknown classification mode {classification_mode}")
+            raise ValueError(f"Unrecognized classification mode: {self.classification_mode}")
 
-        self.single_lookup = single_lookup
-        # The name of the column containing the memory's label
-        self.memory_label = memory_label
-        self.lookup = OrcaLabelLookupLayer(memory_index, memory_label, num_memories)
+        # Lookup settings will be automatically propagated to the lookup layer
+        self.lookup = OrcaLabelLookupLayer()
+
+        self.classification_mode = classification_mode
 
         self.memory_layers = nn.ModuleList(
-            [
+            (
+                # Lookup settings will be automatically propagated this layer
                 OrcaClassificationCrossAttentionLayer(
-                    model_dim,
+                    model_dim=model_dim,
                     num_heads=num_heads,
-                    num_classes=inner_classes,
-                    memory_index=memory_index,
-                    memory_label=memory_label,
+                    num_classes=self.inner_classes,
                     num_memories=num_memories,
-                    activation=activation,
                     dropout=dropout,
+                    activation=activation,
+                    projection_mode=self.projection_mode,
                     split_retrieval_path=split_retrieval_path,
-                    projection_mode=projection_mode,
+                    database=database,
                 )
-                for i in range(num_layers)
-            ]
+                for _ in range(num_layers)
+            )
+        )
+
+        self.num_layers = num_layers
+        self.classifier = _LinearClassificationHead(
+            model_dim=model_dim, num_labels=self.inner_classes, activation=activation, dropout=dropout
         )
-        self.classifier = _LinearClassificationHead(model_dim, inner_classes, dropout=dropout, activation=activation)
+
         self._memory_enabled = True
-        self.deep_residuals = deep_residuals
-        self.memory_guide_weight = memory_guide_weight
+        # Lookup settings will be automatically propagated to the lookup layer
         self.guide = OrcaClassificationMemoryGuideLayer(
             num_classes=num_classes,
-            memory_index=memory_index,
-            memory_label=memory_label,
             num_memories=num_memories,
             guide_weight=memory_guide_weight,
+            database=database,
         )
 
     def forward(
         self,
         x: torch.Tensor,
         ctx: Optional[torch.Tensor] = None,
         labels: Optional[torch.Tensor] = None,
@@ -1427,70 +1246,77 @@
         if self.memory_guide_weight > 0.0:
             x = self.guide(x, memory_key or inpt, ctx, labels)
         return x
 
     def _orca_memory_toggle(self, enable: bool) -> None:
         """
         Toggles the memory guide layer on or off.
+
         :param enable: Whether to enable the memory guide layer.
 
         NOTE: This method should not be called directly. It is used internally.
         """
         self._memory_enabled = enable
 
 
-class OrcaLLMMemoryGuideLayer(OrcaModule):
+class OrcaLLMMemoryGuideLayer(OrcaLookupModule, LabelColumnNameMixin):
     """
     A PyTorch module that implements a memory-guided generation layer for Language Models.
 
     This layer biases the output distribution of the model towards a set of memories.
     """
 
     def __init__(
         self,
+        num_memories: int,
         alpha: float,
         beta: float,
-        memory_index: str,
-        memory_col: str,
-        num_memories: int,
-        tokenizer: Callable[[str | list[str]], list[int] | list[list[int]]],
         vocab_size: int,
+        tokenizer: Callable[[str | list[str]], list[int] | list[list[int]]],
         S_min: int = 3,
         S_max: int = 10,
         enable_in_training: bool = False,
-        **settings,
+        # Shared Settings
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Lookup Settings
+        memory_index_name: Optional[str] = None,
+        label_column_name: Optional[list[str]] = None,
     ):
         """
-        :param alpha: How strongly to bias the model output distribution towards similar stirng continuations in the memories. Needs hyperparameter tuning.
-        :param beta: How strongly to bias the model output distribution towards tokens that appear in the memories. Needs hyperparameter tuning.
-        :param memory_index: The memory index.
-        :param memory_col: The memory column.
         :param num_memories: The number of memories.
-        :param tokenizer: The tokenizer function for the underlying language model model.
-        :param vocab_size: The vocabulary size for the underlying language model.
-        :param S_min: The minimum matching length for the string contunuation bias (overall weight controlled by alpha). Should not need hyperparameter tuning. (default: 3)
-        :param S_max: The maximum matching length for the string contunuation bias (overall weight controlled by alpha). Should not need hyperparameter tuning. (default: 10)
-        :param enable_in_training: Flag to enable in training. (Not recommended) (default: False)
-        :param **settings: Additional settings to pass to the parent constructor.
+        :param settings: The settings for the OrcaLLMMemoryGuideLayer.
         """
-        super().__init__(**settings)
+
+        super().__init__(
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            num_memories=num_memories,
+            freeze_num_memories=True,
+            propagate_lookup_settings=True,
+        )
+
         self.alpha = alpha
         self.beta = beta
+        self.vocab_size = vocab_size
+        self.tokenizer = tokenizer
         self.S_min = S_min
         self.S_max = S_max
-        self.tokenizer = tokenizer
         self.enable_in_training = enable_in_training
-        self.vocab_size = vocab_size
-        self.memory_col = memory_col
+        self.label_column_name = label_column_name
 
-        self.lookup = OrcaLookupLayer(memory_index, ["$embedding", memory_col], num_memories)
+        # Lookup settings will be automatically propagated to the lookup layer
+        self.lookup = OrcaLookupLayer()
 
     def _compute_lps_array(self, pattern) -> list[int]:
         """
         Compute the longest prefix that is also a suffix (lps) array used in KMP algorithm.
+
         :param pattern: The pattern to compute the lps array for.
         :return: The lps array.
 
         NOTE: This method should not be called directly. It is used internally.
         """
         lps = [0] * len(pattern)
         length = 0  # length of the previous longest prefix suffix
@@ -1510,16 +1336,16 @@
                     lps[i] = 0
                     i += 1
 
         return lps
 
     def _find_suffixes_in_sequence(self, S, M, S_min, S_max) -> list[tuple[int, int, str]]:
         """
-        Find the starting indexes where the suffixes of S of lengths between S_min and S_max
-        are contained in M.
+        Find the starting indexes where the suffixes of S of lengths between S_min and S_max are contained in M.
+
         :param S: The sequence to search for suffixes in M.
         :param M: The sequence to search for suffixes of S.
         :param S_min: The minimum length of the suffixes to search for.
         :param S_max: The maximum length of the suffixes to search for.
         :return: A list of tuples containing the starting index of the suffix in M, the length of the suffix, and the next token in M after the suffix.
 
         NOTE: This method should not be called directly. It is used internally.
@@ -1558,14 +1384,15 @@
                         i += 1
 
         return occurrences
 
     def _extract_occurance_ranks(self, occurrences, ref_length) -> dict[int, float]:
         """
         Extract the occurance ranks from the occurrences.
+
         :param occurrences: The occurrences to extract the ranks from.
         :param ref_length: The length of the reference sequence.
         :return: A dictionary of token to occurance rank.
 
         NOTE: This method should not be called directly. It is used internally.
         """
         scores = defaultdict(int)
@@ -1575,14 +1402,15 @@
             if length > scores[next_token]:
                 scores[next_token] = length / ref_length
         return dict(scores)
 
     def _bag_of_words_probs(self, bag_of_words: list[tuple[list[int], float]]) -> torch.Tensor:
         """
         Compute the bag of words probabilities.
+
         :param bag_of_words: The bag of words to compute the probabilities for.
         :return: The bag of words probabilities.
 
         NOTE: This method should not be called directly. It is used internally.
         """
         res = torch.zeros(self.vocab_size)
         for bag, score in bag_of_words:
@@ -1593,23 +1421,24 @@
     def _weighted_next_tokens_from_memory(
         self, memory_key: torch.Tensor, q_tokens: list[int]
     ) -> tuple[
         dict[int, float], list[tuple[list[int], float]]
     ]:  # suffix max dict (token -> score), bag_of_words list (token list, score)
         """
         Compute the weighted next tokens from memory.
+
         :param memory_key: The memory key to use for memory lookup.
         :param q_tokens: The input tokens.
         :return: A tuple containing the weighted next tokens from the memory and the bag of words.
 
         NOTE: This method should not be called directly. It is used internally.
         """
         result = self.lookup(memory_key)
         ctx = result.to_tensor("$embedding", dtype=memory_key.dtype, device=memory_key.device)
-        candidates: list[str] = result[0, :, self.memory_col].to_list()
+        candidates: list[str] = result[0, :, self.label_column_name].to_list()
         semantic_scores: list[float] = (ctx.squeeze() @ memory_key.squeeze()).tolist()
         tokens_and_weights: dict[int, float] = {}
         for candidate, semantic_score in zip(candidates, semantic_scores):
             tokens = self.tokenizer(candidate)
             suffixes = self._find_suffixes_in_sequence(q_tokens[0], tokens, self.S_min, self.S_max)
             scores = self._extract_occurance_ranks(suffixes, len(tokens))
             for token, score in scores.items():
@@ -1623,14 +1452,15 @@
                 strict=True,
             )
         )
 
     def forward(self, memory_key: torch.Tensor, logits: torch.Tensor, inpt_tokens: list[int]) -> torch.Tensor:
         """
         Forward pass.
+
         :param memory_key: The memory key to use for memory lookup.
         :param logits: The original model logits.
         :param inpt_tokens: The input tokens.
         :return: The updated logits.
         """
         if self.training and not self.enable_in_training:
             return logits
@@ -1643,88 +1473,103 @@
                 probs[0][token] += self.alpha * score
 
         if self.beta > 0.0:
             probs[0] += self.beta * self._bag_of_words_probs(bag_of_words).to(probs.device)
         return probs
 
 
-class OrcaRankingCrossAttentionLayer(OrcaModule):
+class OrcaRankingCrossAttentionLayer(OrcaLookupModule, LabelColumnNameMixin):
     """A transformer decoder layer block that does cross attention for rankings.
 
     Note that this is Ranking-specific, and the rankings returned by the lookup layer are used as the value-weights for the cross attention.
 
     The block contains the typical transformer components: multi-head attention, feed forward, and layer norm.
     The block also contains a lookup layer that looks up a vector in an OrcaDatabase index and returns the top k results.
     These results are used as the memory context for the cross attention.
     """
 
     def __init__(
         self,
         model_dim: int,
         num_heads: int,
-        num_ranks: int,
-        memory_index: str,
-        memory_col: str,
         num_memories: int,
+        num_ranks: int,
         activation: Callable[[Tensor], Tensor] = F.relu,
         dropout: float = 0.1,
         split_retrieval_path: bool = False,
         projection_mode: ProjectionMode = ProjectionMode.LABEL,
-        **settings,
+        # Shared Settings
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Lookup Settings
+        memory_index_name: Optional[str] = None,
+        label_column_name: Optional[list[str]] = None,
     ):
         """
         :param model_dim: (int) The dimension of the input vector and hidden layers.
         :param num_heads: (int) The number of heads to be used in the multi-head attention layer.
-        :param num_ranks: (int) The number of ranks for the output classification and weights for cross attention.
-        :param orca_lookup_type: (OrcaLookupType) The type of the OrcaLookupLayer to be used for the memory lookup.
-        :param orca_lookup_config: (OrcaLookupConfig) The configuration for the OrcaLookupLayer to be used for the memory lookup.
-        :param activation: (Callable[[Tensor], Tensor]) The activation function to be used between the two linear layers. (default: F.relu)
-        :param dropout: (float) The dropout rate to be used between the two linear layers. (default: 0.1)
-        :param split_retrieval_path: (bool) Whether to split the retrieval path from the forward pass. If True, the memory key must be passed in to the forward pass. (default: False)
-        :param projection_mode: (ProjectionMode) Determines how the values from the memory should be "projected" into the models embedding space (i.e. what's the V in the attention mechanism QKV). (default: ProjectionMode.LABEL)
+        :param num_memories: (int) The number of memory vectors to be returned from the lookup.
         :param settings: (Any) Additional settings to pass to the parent constructor.
+
         This is used when the memory key is different from the input vector
         """
-        super().__init__(**settings)
+        super().__init__(
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            lookup_column_names=None,
+            num_memories=num_memories,
+            freeze_num_memories=True,
+            propagate_lookup_settings=True,
+        )
 
+        self.model_dim = model_dim
+        self.num_heads = num_heads
         self.num_ranks = num_ranks
         self.activation = activation
+        self.dropout = dropout
         self.split_retrieval_path = split_retrieval_path
         self.projection_mode = projection_mode
-        self.memory_col = memory_col
+        self.label_column_name = label_column_name
 
-        self.lookup = OrcaLabelLookupLayer(memory_index, memory_col, num_memories)
+        # Lookup settings will be automatically propagated to the lookup layer
+        self.lookup = OrcaLabelLookupLayer()
 
         self.cross_attention = nn.MultiheadAttention(
-            model_dim,
-            num_heads,
-            dropout=dropout,
+            self.model_dim,
+            self.num_heads,
+            dropout=self.dropout,
             batch_first=True,
         )
-        self.attn_norm = nn.LayerNorm(model_dim)
+        self.attn_norm = nn.LayerNorm(self.model_dim)
 
-        self.linear1 = nn.Linear(model_dim, model_dim * 4)
-        self.dropout1 = nn.Dropout(dropout)
-        self.linear2 = nn.Linear(model_dim * 4, model_dim)
-        self.dropout2 = nn.Dropout(dropout)
-        self.ff_norm = nn.LayerNorm(model_dim)
+        self.linear1 = nn.Linear(self.model_dim, self.model_dim * 4)
+        self.dropout1 = nn.Dropout(self.dropout)
+        self.linear2 = nn.Linear(self.model_dim * 4, self.model_dim)
+        self.dropout2 = nn.Dropout(self.dropout)
+        self.ff_norm = nn.LayerNorm(self.model_dim)
 
     def forward(
         self,
         x: torch.Tensor,  # Shape (batch_size, vector_dim)
         ctx: Optional[torch.Tensor] = None,  # Shape (batch_size, num_memories, vector_dim)
         ranks: Optional[torch.Tensor] = None,  # Shape (batch_size, num_memories, meta_column_count)
         memory_key: Optional[torch.Tensor] = None,  # Shape (batch_size, vector_dim)
     ) -> torch.Tensor:  # x is the input vector N x D, ctx is the memory context N x K x D
         """x, ctx, ranks act as Q, K, V for the cross attention layer.
+
         When ctx is None:
-            If split_retrieval_path is False, x is used as both Q and K.
-            If split_retrieval_path is True, memory_key is used as K (instead of x)
+
+        * If split_retrieval_path is False, x is used as both Q and K.
+        * If split_retrieval_path is True, memory_key is used as K (instead of x)
+
         When ctx is not None:
-            ranks
+
+        * ranks
 
         :param x: The input tensor of shape (N, D), where N is the batch size and D is the model embedding dimension.
         :param ctx: The memory context tensor of shape (N, K, D), where N is the batch size, K is the number of memories, and D is the model embedding dimension. (default: None)
         :param ranks: The memory rank tensor of shape (N, K), where N is the batch size and K is the number of memories. (default: None)
         :param memory_key: The memory key tensor of shape (N, D), where N is the batch size and D is the model embedding dimension. (default: None)
         :return: The output tensor of shape (N, D), where N is the batch size and D is the model embedding dimension.
         """
@@ -1755,87 +1600,106 @@
         y = self.linear2(y)  # N x D
         y = self.dropout2(y)
         x = self.ff_norm(y + x)  # N x D
 
         return x
 
 
-class OrcaRankingHead(
-    OrcaModule
-):  # Input: single vector of size hidden_size, optional memory context (otherwise looked up), Output: single element of size 1
+class OrcaRankingHead(OrcaLookupModule, LabelColumnNameMixin):
+    # Input: single vector of size hidden_size, optional memory context (otherwise looked up), Output: single element of size 1
     """A transformer decoder layer block that does cross attention with memory lookup for ranking problems"""
 
     def __init__(
         self,
-        model_dim,
-        num_ranks,
-        memory_index: str,
-        memory_label: str,
+        model_dim: int,
         num_memories: int,
+        num_ranks: int,
         num_layers: int = 1,
         num_heads: int = 8,
         activation: Callable[[Tensor], Tensor] = F.relu,
         dropout: float = 0.1,
-        deep_residuals: bool = False,
         split_retrieval_path: bool = False,
+        projection_mode: ProjectionMode = ProjectionMode.LABEL,
         memory_guide_weight: float = 0.0,
         single_lookup: bool = True,
-        **settings,
+        deep_residuals: bool = False,
+        # Shared Settings
+        database: OrcaDatabase | str | None = None,
+        # Curate Settings
+        curate_enabled: bool = False,
+        # Lookup Settings
+        memory_index_name: Optional[str] = None,
+        label_column_name: Optional[str] = None,
     ):
         """
         :param model_dim: (int) The dimension of the input vector and hidden layers.
-        :param num_ranks: (int) The number of ranks for the output classification and weights for cross attention.
-        :param memory_index: (str) The name of the OrcaDatabase index to be used for the memory lookup.
-        :param memory_label: (str) The name of the column in the OrcaDatabase index to be used as the memory label. (e.g., "label")
         :param num_memories: (int) The number of memory vectors to be returned from the lookup.
         :param num_layers: (int) The number of attention blocks to be used, copies of OrcaClassificationCrossAttentionLayer. (default: 1)
         :param num_heads: (int) The number of heads to be used in the multi-head attention layer. (default: 8)
-        :param activation: (Callable[[Tensor], Tensor]) The activation function used throughout the attention blocks. (default: F.relu)
-        :param dropout: (float) The dropout rate to be used between the two linear layers. (default: 0.1)
-        :param deep_residuals: (bool) Whether to use the residual (skip) connections. (default: False)
-        :param split_retrieval_path: (bool) Whether to split the retrieval path from the forward pass. If True, the memory key must be passed in to the forward pass. (default: False)
-        :param memory_guide_weight: (float) The weight to be applied to the memory guide layer. (default: 0.0)
-        :param single_lookup: (bool) Whether to use a single lookup for the memory context. (default: True)
-        :param settings: (Any) Any additional settings to be applied to the model. (e.g., "device")
+        :param settings: (Any) Additional settings to pass to the parent constructor.
         """
-        super().__init__(**settings)
+        super().__init__(
+            database=database,
+            curate_enabled=curate_enabled,
+            memory_index_name=memory_index_name,
+            lookup_column_names=None,
+            num_memories=num_memories,
+            freeze_num_memories=True,
+            propagate_lookup_settings=True,
+        )
 
+        self.model_dim = model_dim
+        self.num_heads = num_heads
+        self.activation = activation
+        self.dropout = dropout
+        self.split_retrieval_path = split_retrieval_path
+        self.projection_mode = projection_mode
+        self.num_layers = num_layers
+        self.memory_guide_weight = memory_guide_weight
         self.single_lookup = single_lookup
-        self.memory_label = memory_label
-        self.lookup = OrcaLabelLookupLayer(memory_index, memory_label, num_memories)
+        self.deep_residuals = deep_residuals
+        self.label_column_name = label_column_name
+
+        self._memory_enabled = True
+
+        # Lookup settings will be automatically propagated to the lookup layer
+        self.lookup = OrcaLabelLookupLayer()
 
         self.memory_layers = nn.ModuleList(
             [
+                # Lookup settings will be automatically propagated to this layer
                 OrcaRankingCrossAttentionLayer(
-                    model_dim,
+                    model_dim=model_dim,
                     num_heads=num_heads,
-                    num_ranks=num_ranks,
-                    memory_index=memory_index,
-                    memory_col=memory_label,
                     num_memories=num_memories,
+                    num_ranks=num_ranks,
                     activation=activation,
                     dropout=dropout,
                     split_retrieval_path=split_retrieval_path,
+                    projection_mode=projection_mode,
+                    database=database,
                 )
-                for i in range(num_layers)
+                for _ in range(self.num_layers)
             ]
         )
-        self.classifier = _LinearClassificationHead(model_dim, 1, dropout=dropout, activation=activation)
-        self._memory_enabled = True
-        self.deep_residuals = deep_residuals
+
+        self.classifier = _LinearClassificationHead(
+            model_dim=model_dim, num_labels=1, activation=activation, dropout=dropout
+        )
 
     def forward(
         self,
         x: torch.Tensor,
         ctx: Optional[torch.Tensor] = None,
         ranks: Optional[torch.Tensor] = None,
         memory_key: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:  # x is the input vector N x D, ctx is the memory context N x K x D
         """
-        forward pass
+        Forward pass
+
         :param x: The input tensor of shape (N, D), where N is the batch size and D is the model embedding dimension.
         :param ctx: The memory context tensor of shape (N, K, D), where N is the batch size, K is the number of memories, and D is the model embedding dimension. (default: None)
         :param ranks: The memory rank tensor of shape (N, K), where N is the batch size and K is the number of memories. (default: None)
         :param memory_key: The memory key tensor of shape (N, D), where N is the batch size and D is the model embedding dimension. (default: None)
         :return: The output tensor of shape (N, 1), where N is the batch size. The output is the rank of the input vector.
         """
         if ctx is None and self.single_lookup:
@@ -1852,14 +1716,15 @@
                     x = y
         x = self.classifier(x)
         return x
 
     def _orca_memory_toggle(self, enable: bool) -> None:
         """
         Toggles the memory layer on or off.
+
         :param enable: (bool) Whether to enable the memory layer.
 
         NOTE: This method should not be called directly. It is used internally.
         """
         self._memory_enabled = enable
 
 
@@ -1948,26 +1813,28 @@
         self.mem_id_map = list(self.mem_vecs_dict.keys())
 
         print(f"Finished preparing OrcaMemoryDataset for index {index} with memory index {memory_index}")
 
     def __get_mems(self, row_id: int) -> tuple[Tensor, list[Any] | Any]:
         """
         Get the memory vectors and metadata for a given row id.
+
         :param row_id: The row id to get the memory vectors and metadata for.
         :return: A tuple containing the memory vectors and metadata.
         """
         mem_idxs = self.top_k_dict[row_id]
         mems = self.mem_vecs[mem_idxs]
         mem_data_ids = [int(self.mem_id_map[mem_idx]) for mem_idx in mem_idxs]
 
         mem_column_dicts = [self.mem_data[mem_data_id] for mem_data_id in mem_data_ids]
 
         def _get_one_mem(mem_column_dict: dict[str, Any]) -> list[Any] | Any:
             """
             Get one memory vector and metadata.
+
             :param mem_column_dict: The memory column dictionary to get the memory vector and metadata from.
             :return: A tuple containing the memory vector and metadata.
 
             NOTE: This method should not be called directly. It is used internally.
             """
             if not isinstance(self.mem_columns, list):
                 col_name = (
@@ -1984,14 +1851,15 @@
         mem_columns = [_get_one_mem(mem_column_dict) for mem_column_dict in mem_column_dicts]
 
         return mems, mem_columns
 
     def __getitem__(self, index: int) -> tuple[Tensor, list[Any] | Any, Tensor, list[Any] | Any]:
         """
         Get an item from the dataset.
+
         :param index: The index of the item to get.
         :return: A tuple containing the item vector, item metadata, topk memory vectors, and topk memory metadata.
         """
         itemid, columns_dicts = self.data[index]
 
         if len(columns_dicts) == 1:
             columns = list(columns_dicts.values())[0]
@@ -2009,33 +1877,30 @@
         return Tensor(vec), columns, Tensor(mems), mem_columns
 
     def __len__(self) -> int:
         return len(self.data)
 
 
 class OrcaMemoryDatasetV2(Dataset):
-    """A PyTorch dataset that pulls the entire index on demand from an OrcaDatabase to be used locally
-
+    """
     A PyTorch dataset that pulls the entire index on demand from an OrcaDatabase to be used locally
     for training Orca-based layers and models. This is useful for small datasets that can
     fit in memory, or for debugging purposes.
 
     The dataset consists of a list of tuples, where each tuple contains:
-    - The item vector
-    - The item metadata
-    - The topk memory vectors
-    - The topk memory metadata
-
-    The item vector is a Tensor of shape (vector_dim,)
-    The item metadata is a list of arbitrary metadata values
-    The topk memory vectors is a Tensor of shape (num_memories, vector_dim)
-    The topk memory metadata is a list of lists of arbitrary metadata values
+
+    * The item vector: a Tensor of shape (vector_dim,)
+    * The item metadata: a list of arbitrary metadata values
+    * The topk memory vectors: a Tensor of shape (num_memories, vector_dim)
+    * The topk memory metadata: a list of lists of arbitrary metadata values
 
     Example usage:
+
     .. code-block:: python
+
         import torch
         from orcalib.orca_torch import OrcaMemoryDataset
 
         dataset = OrcaMemoryDataset(db, index="my_index",
                                         columns="my_label",
                                         memory_index="my_index",
                                         mem_columns="my_label",
@@ -2102,25 +1967,26 @@
         self.mem_data = dict(
             cast(
                 list[tuple[int, dict[str, Any]]],
                 mem_table.select(*self.__ensure_list(mem_columns)).fetch(include_ids=True),
             )
         )
 
-        self.length = first_page["total_size"]
+        self.length: int = int(first_page["total_size"])
         self.num_pages = first_page["num_pages"]
         self.page_size = first_page["page_size"]
 
         assert first_page["page_index"] == 0
 
         self.pages = {0: first_page}
 
     def __get_page_for_index(self, index: int) -> dict[str, Any]:
         """
         Get the page for the given index.
+
         :param index: The index to get the page for.
         :return: The page for the given index.
         """
         page_index = index // self.page_size  # type: ignore
 
         if page_index in self.pages:
             return self.pages[page_index]
@@ -2140,38 +2006,41 @@
         )
         self.pages[page_index] = page
         return page
 
     def __ensure_list(self, x: Any) -> list[Any]:
         """
         Ensure that the given value is a list.
+
         :param x: The value to ensure is a list.
         :return: The value as a list.
         """
         if isinstance(x, list):
             return x
         return [x]
 
     def __get_column_name(self, column: str | ColumnHandle) -> str:
         """
         Get the column name from the given column handle.
+
         :param column: The column handle to get the column name from.
         :return: The column name.
         """
         if isinstance(column, ColumnHandle):
             return column.column_name
         return column
 
     def __get_dict_values(
         self,
         d: dict[str, Any],
         keys: list[str | ColumnHandle] | str | ColumnHandle,
     ) -> list[Any]:
         """
         Get the values from the given dictionary for the given keys.
+
         :param d: The dictionary to get the values from.
         :param keys: The keys to get the values for.
         :return: The values from the dictionary for the given keys.
         """
         if isinstance(keys, list):
             col_names = [self.__get_column_name(column) for column in keys]
             return [d[col_name] for col_name in col_names]
@@ -2208,25 +2077,27 @@
     def __len__(self) -> int:
         """Returns the length of the dataset"""
         return self.length
 
     def get_dict(self, index: int) -> dict:
         """
         Returns the dictionary for the item at the given index
+
         :param index: The index of the item to get the dictionary for.
         :return: The dictionary for the item at the given index.
         """
         page = self.__get_page_for_index(index)
         sub_index = index % self.page_size  # type: ignore
         return page["items"][sub_index]
 
     def get_score(self) -> float:
-        """Classification score for the dataset, which is the product of the hit rate and the correct rate
+        """Classification score for the dataset, which is the product of the hit rate and the correct rate.
 
         This is a measure of how well the memory vectors are able to classify the items in the dataset.
+
         :return: The classification score for the dataset.
         """
         total = 0
         contains_correct = 0
         count_correct = 0
         count_wrong = 0
         total_mems = 0
@@ -2309,26 +2180,28 @@
         if param_groups is None:
             param_groups = model.parameters()
         self.optimizer = torch.optim.Adam(param_groups, lr=0.001)  # type: ignore
 
     def _get_accuracy(self, logits, labels) -> float:
         """
         Computes and returns the accuracy of the model.
+
         :param logits: The logits from the model.
         :param labels: The labels for the data.
         :return: The accuracy of the model.
 
         NOTE: This method should not be called directly. It is used internally.
         """
         _, preds = torch.max(logits, 1)
         return (preds == labels).float().mean().item()
 
     def get_test_accuracy(self, testloader_override: DataLoader | None = None) -> float:
         """
-        Computes and returns the average accuray of the model either on the main testset (from the constructor) or on the provided testloader_override
+        Computes and returns the average accuray of the model either on the main testset (from the constructor) or on the provided testloader_override.
+
         :param testloader_override: (Optional) The DataLoader to use for the testset. If None, the main testset will be used. (default: None)
         :return: The average accuracy of the model on the testset.
         """
         self.model.eval()
         if testloader_override is not None:
             testloader = testloader_override
         else:
@@ -2364,14 +2237,15 @@
             avg_test_acc = test_acc / test_steps
         self.model.train()
         return avg_test_acc
 
     def train_one_epoch(self, epoch=None, num_epochs=None) -> None:
         """
         Trains the model for one epoch.
+
         :param epoch: (Optional) The current epoch number. (default: None)
         :param num_epochs: (Optional) The total number of epochs. (default: None)
         """
         self.model.train()
         running_loss = 0.0
         running_acc = 0.0
         steps = 0
@@ -2417,11 +2291,12 @@
         print(
             f"Epoch [{epoch}/{num_epochs}], Loss: {avg_loss:.4f}, Accuracy: {avg_acc:.4f}, Test Accuracy: {self.get_test_accuracy():.4f}"
         )
 
     def train(self, num_epochs=10) -> None:
         """
         Trains the model for the given number of epochs.
+
         :param num_epochs: (Optional) The number of epochs to train for. (default: 10)
         """
         for epoch in range(num_epochs):
             self.train_one_epoch(epoch + 1, num_epochs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `orcalib-0.0.56/orcalib/orca_types.py` & `orcalib-0.0.57/orcalib/orca_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,50 +20,59 @@
 import numpy as np
 import torch
 from orca_common import ImageFormat, NumericType, NumericTypeAlternative
 from PIL import Image as PILImage
 
 
 class OrcaTypeHandle(ABC):
-    """Base class for all Orca types. Derived classes represent the types of columns in a table.
+    """
+    Base class for all Orca types. Derived classes represent the types of columns in a table.
+
+    --- How to declare new types ---
 
-    ---- How to declare new types ----
     1. Create a new class that inherits from OrcaTypeHandle
     2. Decorate the class with the `@register_column_type` decorator
     3. Implement the `parameters` property to return the type parameters as a list
     4. Make sure that the constructor takes the type parameters as arguments in the same order as they are returned by the `parameters` property
-    4. Make sure the constructor can accept type parameters as `ActualType | str | None` (where `ActualType` is the type of the parameter)
-    5. Implement the `__getitem__` method to allow type parameters to be specified using the `[]` operator
+    5. Make sure the constructor can accept type parameters as `ActualType | str | None` (where `ActualType` is the type of the parameter)
+    6. Implement the `__getitem__` method to allow type parameters to be specified using the `[]` operator
+
+    --- How to use the derived classes ---
 
-    ---- How to use the derived classes ----
-    >>> column.type = VectorT[768]
-    >>> column.type = VectorT[768].notnull
-    >>> column.type = VectorT[768].unique
-    >>> column.type = VectorT[768].notnull.unique
+    .. code-block:: python
+
+        >>> column.type = VectorT[768]
+        >>> column.type = VectorT[768].notnull
+        >>> column.type = VectorT[768].unique
+        >>> column.type = VectorT[768].notnull.unique
 
     """
 
     # NOTE: This is updated by the @register_column_type decorator and manually for numeric types
     _name_to_type: dict[str, Type] = {}  # Maps type names to their corresponding classes
 
     def __init__(self, t_name: str, notnull: bool = False, unique: bool = False):
         """Initializes the type with the type name and constraints.
+
         :param t_name: The name of the type, e.g., "vector" or "image"
         :param notnull: Whether the column must have a value
         :param unique: Whether the column must have a unique value
         """
         self.t_name = t_name
         self._notnull = notnull
         self._unique = unique
 
     @classmethod
     def from_string(cls, type_str: str) -> "OrcaTypeHandle":
         """Parses a type string into an OrcaTypeHandle.
+
         Examples: `float`, `vector[128] NOT NULL UNIQUE`, or `image[PNG] UNIQUE`.
+
         NOTE: Essentially, you can reconstruct a type after using str(), repr(), or the type's `full_name` property.
+
         :param type_str: The type string to parse
         :return: An OrcaTypeHandle instance
         """
 
         # This regex has 4 capture groups that match the following for "vector[128] NOT NULL UNIQUE":
         # 1. The type name (e.g., "vector") - required
         # 2. The type parameters (e.g., "128" for a vector) - optional
@@ -80,14 +89,15 @@
             raise ValueError(f"Unknown type: {t_name}")
 
         return cls._name_to_type[t_name](*params, notnull=notnull, unique=unique)
 
     def __eq__(self, other: Any) -> bool:
         """
         Returns True if the two types are equal, False otherwise.
+
         :param other: The other type to compare with
         """
         if not isinstance(other, OrcaTypeHandle):
             return False
         return (
             self.t_name == other.t_name
             and self._unique == other._unique
@@ -97,23 +107,25 @@
 
     def __hash__(self) -> int:
         """Returns a hash of the type."""
         return hash((self.t_name, self._unique, self._notnull, *self.parameters))
 
     def __str__(self) -> str:
         """Returns the type name, including type parameters and constraints.
+
         Example: `vector[128] NOT NULL UNIQUE` or `image[PNG] UNIQUE`."""
         return f"{self.full_name}" + (" NOT NULL" if self._notnull else "") + (" UNIQUE" if self._unique else "")
 
     def __repr__(self) -> str:
         """Returns a string representation of the type."""
         return self.__str__()
 
     def _clone_with_overrides(self, **kwargs):
         """Returns a copy of this type with the specified overrides.
+
         :param kwargs: The overrides to apply
 
         NOTE: This method should not be called directly. It is used internally.
         """
         cls = type(self)
         args = inspect.signature(cls.__init__).parameters
 
@@ -181,14 +193,15 @@
             else:
                 yield str(param)
 
     @property
     def full_name(self):
         """
         Returns the full name of the type, including type parameters.
+
         For example, `vector[128]` or `image[PNG]`.
         """
         param_strings = list(self._get_param_strings())
         if len(param_strings) > 0:
             return f"{self.t_name}[{','.join(param_strings)}]"
         else:
             return self.t_name
@@ -227,14 +240,15 @@
 
         self.dtype = dtype
         self.length = length
 
     def __getitem__(self, length: int) -> "NumericTypeHandle":
         """
         Returns a copy of this type with the specified vector length.
+
         :param length: The length of the vector
         """
         return self._clone_with_overrides(length=length)
 
     @property
     def is_vector(self) -> bool:
         """Returns True if this is a vector type, False otherwise."""
@@ -284,15 +298,17 @@
 )
 
 OrcaTypeHandle._name_to_type.update(numeric_type_dict)
 
 
 def register_column_type(type_name: str):
     """Decorator for registering a new OrcaTypeHandle
+
     NOTE: This is required to be able to instantiate the type using OrcaHandle.from_string(...)
+
     :param type_name: The name of the type, e.g., "vector" or "image"
     """
 
     def wrapper(cls: Type[OrcaTypeHandle]) -> Type[OrcaTypeHandle]:
         OrcaTypeHandle._name_to_type[type_name] = cls
         return cls
 
@@ -327,16 +343,17 @@
         :param unique: Whether the column must have a unique value
         """
         super().__init__("text", notnull, unique)
 
     @property
     def numpy_dtype(self) -> Optional[np.dtype]:
         """
-        Returns the corresponding numpy type: np.str_
-        :return: The numpy type for this column type (np.str_) or None if it doesn't exist
+        Returns the corresponding numpy type: `np.str_`
+
+        :return: The numpy type for this column type (`np.str_`) or None if it doesn't exist
         """
         return np.str_
 
 
 class EnumTypeHandle(OrcaTypeHandle):
     """Represents an enum column type, such as `enum` or `enum NOT NULL UNIQUE`."""
 
@@ -356,14 +373,15 @@
         `__getitem__` method to specify the values. This is primarily used when cloning the type.
         """
         super().__init__("enum_as_str" if store_as_string else "enum_as_int", notnull, unique)
 
         def extract_arg(arg_string: str) -> tuple[str, int]:
             """
             Extracts the name and value from the argument string. Example: "foo=1"
+
             :param arg_string: The argument string, of the format "name=value"
             :return: A tuple with the name and value
             """
             name, value = arg_string.split("=")
             return name, int(value)
 
         assert not (args and name_to_value), "Cannot pass the key values as both *args and name_to_value!"
@@ -376,27 +394,30 @@
                 raise ValueError("All arguments must be strings of the format 'name=value', e.g., 'foo=1'")
             self.name_to_value = dict(extract_arg(arg) for arg in args)
         else:
             self.name_to_value: dict[str, int] = name_to_value or {}
 
     def __getitem__(self, *args) -> "EnumTypeHandle":
         """
-        Returns a copy of this type with the specified enum values. It accepts a variety of input formats,
-        which are described in the examples below.
+                Returns a copy of this type with the specified enum values. It accepts a variety of input formats,
+                which are described in the examples below.
+
+                Examples:
 
-        Examples:
-        >>> EnumT = EnumTypeHandle()
-        >>> EnumT["foo", "bar"] # A sequence of names, the values are the indices
-        >>> EnumT["foo=2", "bar=3"] # A series of "name=value" strings
-        >>> EnumT["foo=2", "bar"] # Using a mix of "name=value" and "name" strings
-        >>> EnumT[["foo", "bar"]] # A list/tuple containing a sequence of names, the values are the indices
-        >>> EnumT[[("foo", 1), ("bar", 2)]] # A sequence of name-value pairs
-        >>> EnumT[("foo", 1), ("bar", 2)] # Passing name-value pairs as separate arguments
-        >>> EnumT[{"foo": 1, "bar": 2}] # A dictionary of name-value pairs
-        >>> EnumT[MyEnum] # A reference to another enum
+        .. code-block:: python
+
+            >>> EnumT = EnumTypeHandle()
+            >>> EnumT["foo", "bar"] # A sequence of names, the values are the indices
+            >>> EnumT["foo=2", "bar=3"] # A series of "name=value" strings
+            >>> EnumT["foo=2", "bar"] # Using a mix of "name=value" and "name" strings
+            >>> EnumT[["foo", "bar"]] # A list/tuple containing a sequence of names, the values are the indices
+            >>> EnumT[[("foo", 1), ("bar", 2)]] # A sequence of name-value pairs
+            >>> EnumT[("foo", 1), ("bar", 2)] # Passing name-value pairs as separate arguments
+            >>> EnumT[{"foo": 1, "bar": 2}] # A dictionary of name-value pairs
+            >>> EnumT[MyEnum] # A reference to another enum
         """
 
         def is_str_int_tuple(value: Any) -> bool:
             return (
                 isinstance(value, tuple) and len(value) == 2 and isinstance(value[0], str) and isinstance(value[1], int)
             )
 
@@ -466,16 +487,17 @@
     def as_integer(self) -> "EnumTypeHandle":
         """Returns a copy of this type that will store its values as integers in the DB"""
         return self._clone_with_overrides(store_as_string=False)
 
     @property
     def numpy_dtype(self) -> Optional[np.dtype]:
         """
-        Returns the corresponding numpy type: np.str_
-        :return: The numpy type for this column type (np.str_) or None if it doesn't exist
+        Returns the corresponding numpy type: `np.str_`
+
+        :return: The numpy type for this column type (`np.str_`) or None if it doesn't exist
         """
         return np.str_ if self.store_as_string else np.int64
 
 
 # We need to add the enum types to the type dictionary, because we can't use a decorator
 # to register a single class with multiple names
 enum_type_dict = {
@@ -495,15 +517,15 @@
         :param notnull: Whether the column must have a value (default: False)
         :param unique: Whether the column must have a unique value (default: False)
         """
         super().__init__("bool", notnull, unique)
 
     @property
     def numpy_dtype(self) -> Optional[np.dtype]:
-        """Returns the corresponding numpy type: np.bool_"""
+        """Returns the corresponding numpy type `np.bool_`"""
         return np.bool_
 
 
 @register_column_type("document")
 class DocumentTypeHandle(OrcaTypeHandle):
     """Represents a document column type, such as `document` or `document NOT NULL UNIQUE`."""
 
@@ -548,35 +570,38 @@
     def parameters(self) -> list[Any]:
         """Returns the type parameters as a tuple."""
         return [self.format]
 
     def __getitem__(self, format: ImageFormat | str) -> "ImageTypeHandle":
         """
         Returns a copy of this type with the specified image format.
+
         :param format: The image format
         """
         return self._clone_with_overrides(format=format)
 
     ##### CustomSerializable methods #####
 
     def binary_serialize(self, value: PILImage.Image) -> io.BytesIO:
         """
         Serializes the image as a binary stream, so we can send it to the server.
+
         :param value: The image to serialize
         :return: The serialized image
         """
         # We're not using a context manager clarify that the stream is open after this function returns
         byte_stream = io.BytesIO()
         value.save(byte_stream, format=self.format.name)
         byte_stream.seek(0)  # Reset the pointer to the beginning of the stream
         return byte_stream
 
     def msgpack_deserialize(self, value: dict[str, Any]) -> PILImage.Image:
         """
         Deserializes the image from a msgpack-compatible dictionary.
+
         :param value: The dictionary to deserialize
         :return: The deserialized image
         """
         image_data = value.get(f"__{self.full_name}__", None)
         assert image_data is not None, f"Expected image data for type {self.full_name}, got {value} instead"
         byte_stream = io.BytesIO(image_data)
         image = PILImage.open(byte_stream, formats=[self.format.name])
```

### Comparing `orcalib-0.0.56/orcalib/orca_utils.py` & `orcalib-0.0.57/orcalib/orca_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import torch
 
 
 def compute_lps_array(pattern) -> list[int]:
     """
     Compute the longest prefix that is also a suffix (lps) array used in KMP algorithm.
+
     :param pattern: Pattern
     :return: lps array
     """
     lps = [0] * len(pattern)
     length = 0  # length of the previous longest prefix suffix
 
     # Loop calculates lps[i] for i = 1 to M-1
@@ -28,16 +29,16 @@
                 i += 1
 
     return lps
 
 
 def find_suffixes_in_sequence(S, M, S_min, S_max) -> list[tuple[int, int, str]]:
     """
-    Find the starting indexes where the suffixes of S of lengths between S_min and S_max
-    are contained in M.
+    Find the starting indexes where the suffixes of S of lengths between S_min and S_max are contained in M.
+
     :param S: Sequence
     :param M: Subsequence
     :param S_min: Minimum length of suffix
     """
     occurrences = []
 
     # Iterate through the range of lengths for suffixes of S
@@ -73,14 +74,15 @@
 
     return occurrences
 
 
 def extract_occurance_ranks(occurrences, ref_length) -> dict:
     """
     Extract the scores of the occurrences of the suffixes in the reference sequence.
+
     :param occurrences: Occurrences
     :param ref_length: Length of reference sequence
     :return: Scores
     """
     scores = defaultdict(int)
     for _, length, next_token in occurrences:
         if next_token is None:
@@ -89,14 +91,15 @@
             scores[next_token] = length / ref_length
     return dict(scores)
 
 
 def bag_of_words_scores(bag_of_words: list[tuple[list[int], float]], vocab_size: int) -> torch.Tensor:
     """
     Compute the scores of the bag of words.
+
     :param bag_of_words: Bag of words
     :param vocab_size: Vocabulary size
     :return: Scores
     """
     res = torch.zeros(vocab_size)
     for bag, score in bag_of_words:
         for token in bag:
```

### Comparing `orcalib-0.0.56/orcalib/table.py` & `orcalib-0.0.57/orcalib/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from itertools import chain
 from typing import IO, Any, Optional, cast
 
 import pandas
-import tqdm
+from tqdm.auto import tqdm
 from orca_common import ColumnName, RowDict, TableName
 
 from orcalib.client import OrcaClient, default_api_version_key
 from orcalib.client_data_model import RowData
 from orcalib.data_classes import ColumnSpec
 from orcalib.orca_expr import ColumnHandle, OrcaExpr
 from orcalib.orca_types import CustomSerializable, OrcaTypeHandle
@@ -24,14 +24,15 @@
         self,
         db_name: str,
         table_name: str,
         # This parameter is used when cloning a table handle to prevent unnecessary calls to the server
         _columns: Optional[dict[ColumnName, ColumnSpec]] = None,
     ):
         """Create a handle to a table in the database.
+
         :param db_name: The database name
         :param table_name: The table name
         """
 
         #
         if _columns is None:
             table_info = OrcaClient.table_info(db_name, table_name)
@@ -41,119 +42,132 @@
 
         self.db_name = db_name
         self.table_name = table_name
 
     def get_column_type_dict(self) -> dict[ColumnName, OrcaTypeHandle]:
         """
         Get a dictionary of column names and orca types for this table
+
         :return: A dictionary of column names and orca types
         """
         return {name: OrcaTypeHandle.from_string(spec.dtype) for name, spec in self.columns.items()}
 
     def copy(self) -> "TableHandle":
         """
         Create a copy of this table handle
+
         :return: A copy of this table handle
         """
         return TableHandle(
             self.db_name,
             self.table_name,
             _columns=self.columns.copy(),
         )
 
     def copy_with_overrides(self, **kwargs) -> "TableHandle":
         """
         Create a copy of this table handle with the specified attributes changed
+
         :param kwargs: the attributes to change
         :return: A copy of this table handle with the specified attributes changed
         """
         result = self.copy()
 
         for key, value in kwargs.items():
             setattr(result, key, value)
 
         return result
 
     def __getattr__(self, column_name: str | ColumnHandle) -> ColumnHandle:
         """
         Get a column handle by name
+
         :param column_name: The name of the column
         :return: A column handle
         """
         if isinstance(column_name, ColumnHandle):
             if column_name.table_name != self.table_name:
                 raise ValueError(f"Column {column_name.column_name} not found in table {self.table_name}")
             return column_name
         if column_name not in self.columns:
             raise Exception(f"Column {column_name} not found in table {self.table_name}")
         return ColumnHandle(self.db_name, self.table_name, column_name)
 
     def __getitem__(self, column_name: str | ColumnHandle) -> ColumnHandle:
         """
         Get a column handle by name
+
         :param column_name: The name of the column
         :return: A column handle
         """
         return self.__getattr__(column_name)
 
     def __contains__(self, column_name: str) -> bool:
         return column_name in self.columns
 
     def get_column(self, column_name: str | ColumnHandle) -> ColumnHandle:
         """
         Get a column handle by name
+
         :param column_name: The name of the column
         :return: A column handle
         """
         return self.__getattr__(column_name)
 
     def select(self, *args) -> TableQuery:
         """
         Start a new query on this table
+
         :param args: The columns to select
         :return: A new table query
         """
         return TableQuery(self.db_name, self).select(*args)
 
     def where(self, *args) -> TableQuery:
         """
         Start a new query on this table
+
         :param args: The columns to select
         :return: A new table query
         """
         return TableQuery(self.db_name, self).where(*args)
 
     def order_by(self, *args, **kwargs) -> TableQuery:
         """
         Start a new query on this table
+
         :param args: The columns to select
         :return: A new table query
         """
         return TableQuery(self.db_name, self).order_by(*args, **kwargs)
 
     def fetch(self, *args, **kwargs) -> list[RowDict] | list[tuple[int, RowDict]]:
         """
         Fetch rows from the table
+
         :param args: The columns to fetch
         :return: A list of rows
         """
         return TableQuery(self.db_name, self).fetch(*args, **kwargs)
 
     def df(self, limit: Optional[int] = None) -> pandas.DataFrame:
         """
         Fetch rows from the table and return as a pandas DataFrame
+
         :param limit: The maximum number of rows to fetch (default: None)
         :return: A pandas DataFrame
         """
         return pandas.DataFrame(self.fetch(limit))
 
     def _extract_rowdicts(self, row_data: RowData) -> list[RowDict]:
         """
         Builds a list of RowDict objects from various sources of row data.
+
         TODO: Add constraint validation based on column type parameters
+
         TODO: Collect file-like object dict for binary uploads
 
         :param row_data: The row data to insert. This can be a RowDict, a pandas DataFrame, or a list of RowDicts.
         :return: A list of RowDict objects
 
         NOTE: This method should not be called directly. It is used internally.
         """
@@ -172,15 +186,17 @@
                 return row_data
             case _:
                 raise TypeError(f"Invalid argument for insert: {row_data} type {type(row_data)}")
 
     def _parse_row_data(self, positional_data: tuple[RowData, ...], kw_data: Any = None) -> list[RowDict]:
         """
         Converts the positional and keyword arguments to a list of RowDict objects
+
         TODO: Add collecting constraint violations based on column type parameters
+
         TODO: Add collecting file-like objects for binary uploads
 
         :param positional_data: The positional row data to insert. This can be a RowDict, a pandas DataFrame, or a list of RowDicts.
         :param kw_data: The keyword row data to insert. This should be a dict[str, Any] where the keys are column names. (default: None)
         :return: A list of RowDict objects
 
         NOTE: This method should not be called directly. It is used internally.
@@ -194,16 +210,18 @@
         if positional_data:
             return list(chain.from_iterable(self._extract_rowdicts(data) for data in positional_data))
         return [kw_data]
 
     def _extract_binary_values(self, row_dicts: list[RowDict]) -> list[tuple[str, IO[bytes]]]:
         """
         Extracts binary values from row dicts and adds them to the file dict
+
         NOTE: DO NOT read/log/inspect the file contents before sending them with the request!
         Otherwise, the file pointer will be at the end of the file and the server will receive an empty file.
+
         :param row_dicts: The row data to insert. This can be a RowDict, a pandas DataFrame, or a list of RowDicts.
         :return: A list of tuples of (filename, file-like object) that is required for the multipart upload
 
         NOTE: This method should not be called directly. It is used internally.
         """
         # This is a list of tuples of (filename, file-like object) that is required for the multipart upload
         named_file_list: list[tuple[str, IO[bytes]]] = []
@@ -223,30 +241,32 @@
         self,
         *positions_args: RowData,
         api_version: str | None = None,
         **column_values: Any,
     ) -> None:
         """
         Insert rows into the table
+
         NOTE: You may not specify both positional and keyword arguments
+
         :param positions_args: The row data to insert. This can be a RowDict, a pandas DataFrame, or a list of RowDicts.
         :param column_values: Specifies the keys and values to insert. This can be used to insert a single row.
         :param api_version: The version of the API to use (default: None)
         """
         api_version_num = OrcaClient.version_string_to_int(api_version)
         MAX_BATCH_SIZE = 100
 
         rows = self._parse_row_data(positions_args, column_values)
         if len(rows) <= MAX_BATCH_SIZE:
             file_list = self._extract_binary_values(rows) if api_version_num >= 2 else []
             OrcaClient.insert(self.db_name, self.table_name, rows, file_list, api_version=api_version)
         else:
             # large batch mode
             batches = (rows[i : i + MAX_BATCH_SIZE] for i in range(0, len(rows), MAX_BATCH_SIZE))
-            with tqdm.tqdm(total=len(rows)) as progress_bar:
+            with tqdm(total=len(rows)) as progress_bar:
                 for batch in batches:
                     file_list = self._extract_binary_values(batch) if api_version_num >= 2 else []
                     OrcaClient.insert(
                         self.db_name,
                         self.table_name,
                         batch,
                         file_list,
@@ -254,14 +274,15 @@
                     )
                     progress_bar.update(len(batch))
 
     @default_api_version_key("table.update")
     def update(self, data: RowDict, filter: OrcaExpr, api_version: str | None = None) -> None:
         """
         Update rows in the table
+
         :param data: The row data to update. This should be a dict[str, Any] where the keys are column names.
         :param filter: The filter to apply to the rows to update
         :param api_version: The version of the API to use (default: None)
         """
         api_version_num = OrcaClient.version_string_to_int(api_version)
 
         file_list = self._extract_binary_values([data]) if api_version_num >= 2 else []
@@ -277,15 +298,17 @@
     @default_api_version_key("table.upsert")
     def upsert(
         self,
         data: RowData,
         key_columns: list[ColumnName],
         api_version: str | None = None,
     ) -> None:
-        """Upsert rows into the table
+        """
+        Upsert rows into the table
+
         :param data: The row data to insert. This can be a RowDict, a pandas DataFrame, or a list of RowDicts.
         :param key_columns: The columns to use as the primary key
         :param api_version: The version of the API to use (default: None)
         """
         api_version_num = OrcaClient.version_string_to_int(api_version)
 
         rows = self._parse_row_data((data,))
@@ -298,48 +321,53 @@
             file_list,
             api_version=api_version,
         )
 
     def delete(self, filter: OrcaExpr) -> None:
         """
         Delete rows from the table
+
         :param filter: The filter to apply to the rows to delete
         """
         OrcaClient.delete(self.db_name, self.table_name, filter.as_serializable())
 
     def add_column(self, **columns: OrcaTypeHandle) -> None:
         """
         Add columns to the table
+
         :param columns: The columns to add
         """
         names, dtypes, notnulls, uniques = [], [], [], []
         for column_name, column_type in columns.items():
             names.append(column_name)
             dtypes.append(column_type.full_name)
             notnulls.append(column_type._notnull)
             uniques.append(column_type._unique)
         OrcaClient.add_column(self.db_name, self.table_name, names, dtypes, notnulls, uniques)
 
     def drop_column(self, column_names: list[str]) -> None:
         """
         Drop columns from the table
+
         :param column_names: The columns to drop
         """
         OrcaClient.drop_column(self.db_name, self.table_name, column_names)
 
     def __str__(self) -> str:
         """
         Get a string representation of this table handle
+
         :return: A string representation of this table handle
         """
         ret = f"{self.db_name}.{self.table_name}(\n"
         for column in self.columns.values():
             ret += f"\t{column.name} {column.dtype}{' NOT NULL' if column.notnull else ''}{' UNIQUE' if column.unique else ''},\n"
         ret += ")"
         return ret
 
     def __repr__(self) -> str:
         """
         Get a string representation of this table handle
+
         :return: A string representation of this table handle
         """
         return self.__str__()
```

### Comparing `orcalib-0.0.56/orcalib/table_query.py` & `orcalib-0.0.57/orcalib/table_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         columns: Optional[list[ColumnName]] = None,
         filter: Optional[OrcaExpr] = None,
         order_by_columns: Optional[OrderByColumns] = None,
         limit: Optional[int] = None,
         default_order: Order = Order.ASCENDING,
     ):
         """Create a new query on the given table
+
         :param db_name: The name of the database to query
         :param primary_table: The primary table to query
         :param columns: The columns we're selecting to return (if any) (default: None)
         :param filter: The filter to apply to the query (if any) (default: None)
         :param order_by_columns: The columns to order by (if any) (default: None)
         :param limit: The maximum number of rows to return (default: None)
         :param default_order: The default order to use with "order_by" if no order is specified (default: Order.ASCENDING)
@@ -63,15 +64,17 @@
         self.filter = filter
         self.order_by_columns = order_by_columns
         self.default_order = default_order
         self.limit = limit
 
     def _clone(self, **kwargs) -> T:
         """Clone the query, optionally overriding some of the parameters
+
         NOTE: This is primarily intended for internal use, but may have limited external use (without parameters).
+
         :param kwargs: The parameters to override
         :return: A new TableQuery with the given parameters overridden
         """
         kwargs["db_name"] = kwargs.get("db_name", self.db_name)
         kwargs["primary_table"] = kwargs.get("primary_table", self.primary_table)
         kwargs["columns"] = kwargs.get("columns", self.columns.copy() if self.columns is not None else None)
         kwargs["filter"] = kwargs.get("filter", self.filter)
@@ -83,14 +86,15 @@
         kwargs["limit"] = kwargs.get("limit", self.limit)
 
         return self.__class__(**kwargs)
 
     def _parse_column_name(self, column: ColumnName | ColumnHandle) -> ColumnName:
         """
         Convert a string or ColumnHandle to a column name, and verify the column exists
+
         :param column: The column to parse
         :return: The column name
 
         NOTE: This method should not be called directly. It is used internally.
         """
         if isinstance(column, ColumnHandle):
             col_name = column.column_name
@@ -101,14 +105,15 @@
         if col_name not in self.primary_table.columns:
             raise ValueError(f"Column '{col_name}' not found in table {self.primary_table.table_name}")
         return col_name
 
     def _parse_params_columns(self, *columns: str | ColumnHandle) -> list[ColumnName]:
         """
         Parse the columns parameter into a dict mapping table names to column names
+
         :param columns: The columns to parse
         :return: The parsed columns
 
         NOTE: This method should not be called directly. It is used internally.
         """
         result = []
 
@@ -124,39 +129,45 @@
             raise ValueError(f"Invalid columns: {invalid_columns} for table {self.primary_table.table_name}")
         return result
 
     def select(
         self,
         *columns: ColumnName | ColumnHandle | tuple[ColumnName | ColumnHandle, Order],
     ) -> T:
-        """Selects the given columns from the table. If no columns are specified, all columns are selected.
-
-        select("col1", "col2", "col3") # string "ColumnName"
-        select("table1.col1", "table2.col2") # string "TableName.ColumnName"
-        select(table.column1, table.column2) # Using ColumnHandle
+        """
+        Selects the given columns from the table. If no columns are specified, all columns are selected.
 
         :param columns: The columns to select
         :return: A new TableQuery with the given columns selected
+
+        .. code-block:: python
+
+            select("col1", "col2", "col3") # string "ColumnName"
+            select("table1.col1", "table2.col2") # string "TableName.ColumnName"
+            select(table.column1, table.column2) # Using ColumnHandle
+
         """
         return self._clone(columns=self._parse_params_columns(*columns))
 
     def where(self, filter: OrcaExpr) -> T:
         """
         Filters the table by the given filter expression.
+
         :param filter: The filter expression
         :return: A new TableQuery with the given filter applied
         """
         return self._clone(filter=filter)
 
     def _parse_param_orderby(
         self,
         *params: ColumnHandle | ColumnName | tuple[ColumnName | ColumnHandle, Order],
     ) -> OrderByColumns:
         """
         Parse any column handles into column names to be compatible with the backend
+
         :param params: The parameters to parse
         :return: The parsed parameters
 
         NOTE: This method should not be called directly. It is used internally.
         """
         ret: OrderByColumns = []
         for p in params:
@@ -170,34 +181,37 @@
     def order_by(
         self,
         *columns: ColumnName | ColumnHandle | tuple[ColumnName | ColumnHandle, Order],
         default_order: Order = Order.ASCENDING,
     ) -> T:
         """
         Orders the table by the given columns. If no columns are specified, the table is ordered by the primary key.
+
         :param columns: The columns to order by
         :param default_order: The default order to use with "order_by" if no order is specified (default: Order.ASCENDING)
         :return: A new TableQuery with the given order applied
         """
         if default_order == Order.DEFAULT:
             default_order = Order.ASCENDING
         columns = self._parse_param_orderby(*columns) if columns else None
         return self._clone(order_by_columns=columns, default_order=default_order)
 
     def limit(self, limit: int) -> T:
         """
         Limits the number of rows returned by the query.
+
         :param limit: The maximum number of rows to return
         :return: A new TableQuery with the given limit applied
         """
         return self._clone(limit=limit)
 
     def _apply_default_order(self, t: OrderByColumn) -> tuple[ColumnName, Order]:
         """
         Apply the default order to the given column if no order is specified
+
         :param t: The column to apply the default order to
         :return: The column with the default order applied
 
         NOTE: This method should not be called directly. It is used internally.
         """
         if isinstance(t, tuple):
             if t[1] == Order.DEFAULT:
@@ -207,14 +221,15 @@
         if isinstance(t, str):
             return (t, self.default_order)
         raise ValueError(f"Invalid order by column: {t}")
 
     def _prepare_orderby_columns(self) -> OrderByColumns | None:
         """
         Prepare the order by columns for for the client call in fetch()
+
         :return: The prepared order by columns
 
         NOTE: This method should not be called directly. It is used internally.
         """
         orderby_columns = self.order_by_columns
         if orderby_columns is not None:
             if not isinstance(orderby_columns, list):
@@ -224,41 +239,46 @@
 
     @default_api_version_key("table.fetch")
     def fetch(
         self,
         limit: int | None = None,
         include_ids: bool = False,
         api_version: Optional[str] = None,
+        use_msgpack: bool = True,
     ) -> list[RowDict]:
         """Fetch rows from the table
+
         :param limit: The maximum number of rows to return (default: None)
         :param include_ids: Whether to include the row ids in the result (default: False)
         :param api_version: The API version to use for this request (default: None)
-        :return: A list of row data"""
+        :return: A list of row data
+        """
         passed_filter = self.filter.as_serializable() if self.filter is not None else None
         columns = self.columns or list(self.primary_table.columns.keys())
         orderby_columns = self._prepare_orderby_columns()
         limit = self.limit or limit or None
         res = OrcaClient.select(
             self.primary_table,
             limit=limit,
             columns=columns,
             filter=passed_filter,
             order_by_columns=orderby_columns,
             default_order=self.default_order,
             api_version=api_version,
+            use_msgpack=use_msgpack,
         )
         if res["status_code"] != 200:
             raise Exception(f"Error fetching data from {self.table_name}: {res}")
 
         if include_ids:
             return [(row["row_id"], row["column_values"]) for row in res["rows"]]
         return [row["column_values"] for row in res["rows"]]
 
     def df(self, limit: int | None) -> pandas.DataFrame:
         """
         Fetch rows from the table and return as a DataFrame
+
         :param limit: The maximum number of rows to return (default: None)
         :return: A DataFrame of row data
         """
         limit = limit or self.limit
         return pandas.DataFrame(self.fetch(limit=limit))
```

### Comparing `orcalib-0.0.56/orcalib/temp_database.py` & `orcalib-0.0.57/orcalib/temp_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         db_name (Optional[str]): The name of the temporary database. If not provided, a random name will be generated.
         verbose (bool): Whether to log verbose information about the creation and dropping of the temporary database.
 
     Returns:
         OrcaDatabase: The temporary database object.
 
     Example:
+
+    .. code-block:: python
+
         with TemporaryDatabase(db_name="my_temp_db", verbose=True) as temp_db:
             # Use the temporary database
             ...
     """
 
     def __init__(self, db_name: Optional[str] = None, verbose: bool = False) -> None:
         """
@@ -46,14 +49,15 @@
 
         self.db = OrcaDatabase(self.db_name)
         return self.db
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         """
         Drop the temporary database.
+
         :param exc_type: The type of the exception
         :param exc_value: The exception value
         :param traceback: The traceback
         """
         if self.verbose:
             logger.info(f"Dropping temporary database: {self.db_name}")
 
@@ -70,14 +74,17 @@
         verbose (bool, optional): Whether to log information about creating and dropping the temporary table.
         **kwargs: Additional keyword arguments to be passed to the `create_table` method of the database.
 
     Returns:
         TableHandle: The handle to the created temporary table.
 
     Example:
+
+    .. code-block:: python
+
         with TemporaryTable(db, table_name="my_temp_table", verbose=True, columns=["id INT", "name TEXT"]) as table:
             # Use the temporary table within this block
             ...
     """
 
     def __init__(self, db: OrcaDatabase, table_name: Optional[str] = None, verbose: bool = False, **kwargs):
         """
@@ -93,27 +100,27 @@
             self.table_name = "temp_table_" + str(uuid.uuid4()).replace("-", "_")
         else:
             self.table_name = table_name
 
         self.kwargs = kwargs
 
     def __enter__(self) -> TableHandle:
-        """
-        Create the temporary table and return the table handle.
+        """Create the temporary table and return the table handle.
+
         :return: TableHandle
         """
         if self.verbose:
             logger.info(f"Creating temporary table: {self.table_name} in database {self.db.name}")
 
         self.table = self.db.create_table(self.table_name, **self.kwargs)
         return self.table
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
-        """
-        Drop the temporary table.
+        """Drop the temporary table.
+
         :param exc_type: The type of the exception
         :param exc_value: The exception value
         :param traceback: The traceback
         """
         if self.verbose:
             logger.info(f"Dropping temporary table: {self.table_name} in database {self.db.name}")
```

### Comparing `orcalib-0.0.56/pyproject.toml` & `orcalib-0.0.57/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "orcalib"
-version = "0.0.56"                              # will be set by CI before building the wheel from the git tag
+version = "0.0.57"                              # will be set by CI before building the wheel from the git tag
 description = "client library for Orca DB"
 license = "Apache-2.0"
 authors = ["Orca DB Inc. <dev-rel@orcadb.ai>"]
 readme = "README.md"
 packages = [{ include = "orcalib" }]
 
 [tool.poetry.dependencies]
 orjson = "^3.8.5"
 requests = "^2.28.2"
 pyarrow = "^14.0.1"
 # the following are peer dependencies and should thus not require a too specific version:
 python = "^3.10,<3.12"
 numpy = "^1.24"
-transformers = "^4.26"
+transformers = "^4.38"
 pandas = ">=1.5, <3.0"
 torch = "^2.1.1"
 pydantic = ">=1.10, <3.0"
 # TODO: make the following optional dependencies to reduce the size of the package:
-gradio = "^3.24"
+gradio = "^4.14.0"
 datasets = "^2.9"
-python-multipart = "^0.0.5"
+python-multipart = "^0.0.7"
 msgpack = "^1.0.7"
 pdoc = "^14.1.0"
-orca-common = "0.1.2"
+orca-common = "0.1.3"
 huggingface-hub = "^0.20.3"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest-env = "^1.0.1"
```

