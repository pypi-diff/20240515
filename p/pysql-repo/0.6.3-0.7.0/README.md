# Comparing `tmp/pysql-repo-0.6.3.tar.gz` & `tmp/pysql-repo-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysql-repo-0.6.3.tar", last modified: Mon May 13 09:43:10 2024, max compression
+gzip compressed data, was "pysql-repo-0.7.0.tar", last modified: Wed May 15 12:47:05 2024, max compression
```

## Comparing `pysql-repo-0.6.3.tar` & `pysql-repo-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo/_constants/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_constants/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_database_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    18596 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22801 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/async_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/async_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/async_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/async_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/libs/file_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-13 09:43:09.000000 pysql-repo-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:47:05.657525 pysql-repo-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-15 12:47:05.657525 pysql-repo-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:47:05.657525 pysql-repo-0.7.0/pysql_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:47:05.657525 pysql-repo-0.7.0/pysql_repo/_constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/_constants/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/_database_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23747 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:47:05.657525 pysql-repo-0.7.0/pysql_repo/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/asyncio/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/asyncio/async_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/asyncio/async_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/asyncio/async_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:47:05.657525 pysql-repo-0.7.0/pysql_repo/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-15 12:47:03.000000 pysql-repo-0.7.0/pysql_repo/libs/file_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:47:05.657525 pysql-repo-0.7.0/pysql_repo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-15 12:47:05.000000 pysql-repo-0.7.0/pysql_repo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 12:47:05.000000 pysql-repo-0.7.0/pysql_repo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:47:05.000000 pysql-repo-0.7.0/pysql_repo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 12:47:05.000000 pysql-repo-0.7.0/pysql_repo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 12:47:05.000000 pysql-repo-0.7.0/pysql_repo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:47:05.657525 pysql-repo-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-15 12:47:05.000000 pysql-repo-0.7.0/setup.py
```

### Comparing `pysql-repo-0.6.3/PKG-INFO` & `pysql-repo-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.6.3
+Version: 0.7.0
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.3.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.6.3/README.md` & `pysql-repo-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.3/pysql_repo/__init__.py` & `pysql-repo-0.7.0/pysql_repo/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,54 @@
 # MODULES
 import logging
 import time
+from typing import Any, Tuple
 
 # SQLALCHEMY
 from sqlalchemy import Engine, event
+from sqlalchemy.engine import Connection, ExecutionContext
+from sqlalchemy.engine.interfaces import DBAPICursor
 
 # PYSQL_REPO
-from pysql_repo._database import DataBase
-from pysql_repo._decorators import with_session
-from pysql_repo._repository import Repository
-from pysql_repo._service import Service
-from pysql_repo._utils import RelationshipOption, FilterType
-from pysql_repo._constants.enum import Operators, LoadingTechnique
+from pysql_repo._database import DataBase as DataBase
+from pysql_repo._decorators import with_session as with_session
+from pysql_repo._repository import Repository as Repository
+from pysql_repo._service import Service as Service
+from pysql_repo._utils import (
+    RelationshipOption as RelationshipOption,
+    FilterType as FilterType,
+)
+from pysql_repo._constants.enum import (
+    Operators as Operators,
+    LoadingTechnique as LoadingTechnique,
+)
 
 
 logging.basicConfig()
 _logger = logging.getLogger("pysql_repo.cursor")
 _logger.setLevel(logging.INFO)
 
 
 @event.listens_for(Engine, "before_cursor_execute")
-def before_cursor_execute(conn, cursor, statement, parameters, context, executemany):
+def before_cursor_execute(
+    conn: Connection,
+    cursor: DBAPICursor,
+    statement: str,
+    parameters: Tuple[Any],
+    context: ExecutionContext,
+    executemany: bool,
+) -> None:
     conn.info.setdefault("query_start_time", []).append(time.perf_counter())
     _logger.debug("Start Query: %s, {%s}", statement, parameters)
 
 
 @event.listens_for(Engine, "after_cursor_execute")
-def after_cursor_execute(conn, cursor, statement, parameters, context, executemany):
+def after_cursor_execute(
+    conn: Connection,
+    cursor: DBAPICursor,
+    statement: str,
+    parameters: Tuple[Any],
+    context: ExecutionContext,
+    executemany: bool,
+) -> None:
     total = time.perf_counter() - conn.info["query_start_time"].pop(-1)
     _logger.debug("Query completed in %fs", total)
```

### Comparing `pysql-repo-0.6.3/pysql_repo/_constants/enum.py` & `pysql-repo-0.7.0/pysql_repo/_constants/enum.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.3/pysql_repo/_database.py` & `pysql-repo-0.7.0/pysql_repo/_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # MODULES
 import logging
-from typing import Any, Generator, List, Optional
+from typing import Any, Generator, List, Optional, Type
 from pathlib import Path
 
 # SQLALCHEMY
 from sqlalchemy import text, MetaData, create_engine, Table
-from sqlalchemy.orm import DeclarativeMeta, Session, sessionmaker
+from sqlalchemy.orm import DeclarativeBase, Session, sessionmaker
 from sqlalchemy.inspection import inspect
 
 # CONTEXTLIB
 from contextlib import contextmanager
 
 # UTILS
 from pysql_repo._database_base import (
@@ -24,15 +24,15 @@
     """
     Represents a database connection and provides methods for database operations.
 
     Args:
         _database_config (DataBaseConfigTypedDict): The configuration for the databases.
         _engine: (Engine): The engine used for database operations.
         _logger (Logger): An instance of the logger to use for logging.
-        _base (DeclarativeMeta): The base class for the database models.
+        _base (DeclarativeBase): The base class for the database models.
         _metadata_views (Optional[List[MetaData]]): Optional list of metadata views.
         _session_factory (sessionmaker[Session]): The factory for creating sessions.
         _views (List[Table]): The list of metadata views.
 
     Methods:
         views: Get the list of views in the database.
         ini: Get the 'ini' property from the database configuration.
@@ -44,15 +44,15 @@
         session_factory: Context manager for creating a session.
         init_tables_from_json_files: Initializes tables from JSON files.
     """
 
     def __init__(
         self,
         databases_config: _DataBaseConfigTypedDict,
-        base: DeclarativeMeta,
+        base: Type[DeclarativeBase],
         metadata_views: Optional[List[MetaData]] = None,
         autoflush: bool = False,
         expire_on_commit: bool = False,
         echo: bool = False,
     ) -> None:
         """
         Initialize a new instance of the _Database class.
@@ -61,18 +61,20 @@
             databases_config (_DataBaseConfigTypedDict): A dictionary containing the configuration for the databases.
             logger (Logger): The logger object to be used for logging.
             base (DeclarativeMeta): The base class for the declarative models.
             metadata_views (List[MetaData] | None, optional): A list of metadata views. Defaults to None.
         """
         super().__init__(databases_config, _logger, base, metadata_views)
 
+        assert self._connection_string is not None, "Connection string is required."
+
         self._engine = create_engine(
-            self._database_config.get("connection_string"),
+            self._connection_string,
             echo=echo,
-            connect_args=self._database_config.get("connect_args") or {},
+            connect_args=self._connect_args,
         )
 
         self._session_factory = sessionmaker(
             bind=self._engine,
             autoflush=autoflush,
             expire_on_commit=expire_on_commit,
         )
@@ -118,15 +120,15 @@
         finally:
             session.close()
 
     def init_tables_from_json_files(
         self,
         directory: Path,
         table_names: List[str],
-        timezone="CET",
+        timezone: str = "CET",
     ) -> List[Table]:
         """
         Initializes tables in the database by inserting data from JSON files.
 
         Args:
             directory (Path): The directory containing the JSON files.
             table_names (List[str]): A list of table names to initialize.
```

### Comparing `pysql-repo-0.6.3/pysql_repo/_database_base.py` & `pysql-repo-0.7.0/pysql_repo/_database_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # MODULES
 import pytz
 import re
-from typing import Any, Dict, List, Optional, TypedDict
+from typing import Any, Dict, List, Optional, Type, TypedDict, Union
 from pathlib import Path
 from datetime import datetime
 from logging import Logger
 
 # SQLALCHEMY
 from sqlalchemy import Table, MetaData
-from sqlalchemy.orm import DeclarativeMeta
+from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy.schema import sort_tables
 
 # LIBS
 from pysql_repo.libs.file_lib import open_json_file
 
 
-class DataBaseConfigTypedDict(TypedDict):
+class DataBaseConfigTypedDict(TypedDict, total=False):
     """
     Represents the configuration options for a database connection.
 
     Attributes:
         connection_string (str): The connection string for the database.
         ini (bool): Indicates whether an INI file is used for configuration.
         init_database_dir_json (Optional[str]): The directory path for initializing the database from a JSON file.
         connect_args (Optional[Dict]): Additional connection arguments for the database.
     """
 
     connection_string: str
     ini: bool
     init_database_dir_json: Optional[str]
-    connect_args: Optional[Dict]
+    connect_args: Optional[Dict[str, Any]]
 
 
 class DataBase:
     """
     Represents a database object.
 
     Attributes:
         _database_config (DataBaseConfigTypedDict): The configuration for the databases.
         _logger (Logger): The logger object for logging.
-        _base (DeclarativeMeta): The base class for the database models.
+        _base (DeclarativeBase): The base class for the database models.
         _metadata_views (Optional[List[MetaData]]): The list of metadata views.
 
     Methods:
         views: Get the list of views in the database.
         ini: Get the 'ini' property from the database configuration.
         init_database_dir_json: Get the 'init_database_dir_json' property from the database configuration.
         _pre_process_data_for_initialization: Pre-processes the data for initialization.
@@ -51,27 +51,30 @@
         _get_ordered_tables: Gets the ordered tables based on the given table names.
     """
 
     def __init__(
         self,
         databases_config: DataBaseConfigTypedDict,
         logger: Logger,
-        base: DeclarativeMeta,
+        base: Type[DeclarativeBase],
         metadata_views: Optional[List[MetaData]] = None,
     ) -> None:
         """
         Initializes a Database object.
 
         Args:
             databases_config (DataBaseConfigTypedDict): The configuration for the databases.
             logger (Logger): The logger object for logging.
             base (DeclarativeMeta): The base class for the database models.
             metadata_views (Optional[List[MetaData]], optional): The list of metadata views. Defaults to None.
         """
         self._database_config = databases_config
+        self._connection_string = self._database_config.get("connection_string")
+        self._connect_args = self._database_config.get("connect_args") or {}
+
         self._logger = logger
         self._base = base
         self._metadata_views = metadata_views
 
         self._views = [
             table
             for metadata in self._metadata_views or []
@@ -92,28 +95,30 @@
     def ini(self) -> bool:
         """
         Get the 'ini' property from the database configuration.
 
         Returns:
             bool: The 'ini' property value.
         """
-        return self._database_config.get("ini")
+        return self._database_config.get("ini", False)
 
     @property
     def init_database_dir_json(self) -> Optional[str]:
         """
         Get the 'init_database_dir_json' property from the database configuration.
 
         Returns:
             Optional[str]: The 'init_database_dir_json' property value.
         """
         return self._database_config.get("init_database_dir_json")
 
     @classmethod
-    def _pre_process_data_for_initialization(cls, data: Dict[str, Any], timezone: str):
+    def _pre_process_data_for_initialization(
+        cls, data: Dict[str, Any], timezone: str
+    ) -> Dict[str, Any]:
         """
         Pre-processes the data for initialization.
 
         Args:
             data (Dict[str, Any]): The data to be pre-processed.
             timezone (str): The timezone to be used for conversion.
 
@@ -135,15 +140,15 @@
 
         return data
 
     def _get_pre_process_data_for_initialization(
         self,
         path: Path,
         timezone: str,
-    ) -> Optional[List[Dict[str, Any]]]:
+    ) -> Optional[Union[List[Dict[str, Any]], Dict[str, Any]]]:
         """
         Gets the pre-processed data for initialization.
 
         Args:
             path (Path): The path to the JSON file.
             timezone (str): The timezone to be used for conversion.
 
@@ -153,23 +158,30 @@
         try:
             raw_data = open_json_file(path=path)
         except FileNotFoundError:
             self._logger.warning(
                 f"Failed to initialize table due to the absence of the file at [{path}]."
             )
 
-            return
+            return None
 
-        return [
-            self._pre_process_data_for_initialization(
-                data,
+        return (
+            [
+                self._pre_process_data_for_initialization(
+                    data,
+                    timezone=timezone,
+                )
+                for data in raw_data
+            ]
+            if isinstance(raw_data, list)
+            else self._pre_process_data_for_initialization(
+                raw_data,
                 timezone=timezone,
             )
-            for data in raw_data
-        ]
+        )
 
     def _get_ordered_tables(self, table_names: List[str]) -> List[Table]:
         """
         Gets the ordered tables based on the given table names.
 
         Args:
             table_names (List[str]): The list of table names.
@@ -181,13 +193,14 @@
             ValueError: If 'ini' property is not available in the database configuration.
         """
         if not (init := self.ini):
             raise ValueError(
                 f"Unable to init database tables because {init=} in config"
             )
 
-        table_names = table_names or set()
         tables = {
-            k: v for k, v in self._base.metadata.tables.items() if k in table_names
+            k: v
+            for k, v in self._base.metadata.tables.items()
+            if k in table_names or []
         }
 
         return sort_tables(tables.values())
```

### Comparing `pysql-repo-0.6.3/pysql_repo/_decorators.py` & `pysql-repo-0.7.0/pysql_repo/_decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # MODULES
-from typing import Any, Dict, List, Union
+import functools
+from typing import Callable, TypeVar, ParamSpec
 
 # SQLALCHEMY
 from sqlalchemy.orm import Session
 
+_P = ParamSpec("_P")
+_T = TypeVar("_T")
 
-def check_values(as_list: bool = False):
+
+def check_values(
+    as_list: bool = False,
+) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]:
     """
     Decorator that checks the validity of the 'values' argument passed to a function.
 
     Args:
         as_list (bool, optional): Specifies whether the 'values' argument should be a list of dictionaries or a single dictionary. Defaults to False.
 
     Raises:
         TypeError: If the 'values' argument is not of the expected type or format.
 
     Returns:
         function: The decorated function.
     """
 
-    def decorator(func):
-        def wrapper(self, *args, **kwargs):
-            values_attr: Union[Dict[str, Any], List[Dict[str, Any]]] = kwargs.get(
-                "values", None
-            )
+    def decorator(func: Callable[_P, _T]) -> Callable[_P, _T]:
+
+        @functools.wraps(func)
+        def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> _T:
+            values_attr = kwargs.get("values", None)
 
             if as_list:
                 if (
                     values_attr is None
                     or not isinstance(values_attr, list)
                     or len(values_attr) == 0
                     or not all(
@@ -46,57 +52,61 @@
                     or len(values_attr) == 0
                     or not all(isinstance(key, str) for key in values_attr.keys())
                 ):
                     raise TypeError(
                         "values expected to be a non-empty dictionary with string keys"
                     )
 
-            return func(self, *args, **kwargs)
+            return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
 def with_session(
     param_session: str = "session",
-):
+) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]:
     """
     Decorator that provides a session to the decorated method.
 
     Args:
         param_session (str, optional): The name of the session parameter. Defaults to "session".
 
     Raises:
         TypeError: If the decorated object is not an instance of Repository or Service.
         TypeError: If the session is not an instance of Session.
 
     Returns:
         Callable: The decorated method.
     """
 
-    def decorator(func):
-        def wrapper(self, *args, **kwargs):
+    def decorator(func: Callable[_P, _T]) -> Callable[_P, _T]:
+
+        @functools.wraps(func)
+        def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> _T:
+            self = kwargs.get("self")
+
             if not isinstance(self, (Repository, Service)):
                 raise TypeError(
                     f"{self.__class__.__name__} must be instance of {Repository.__name__} or {Service.__name__}"
                 )
 
             session = kwargs.get(param_session)
 
             if session is None:
                 with self.session_manager() as session:
                     kwargs[param_session] = session
-                    return func(self, *args, **kwargs)
+                    return func(*args, **kwargs)
             elif not isinstance(session, Session):
                 raise TypeError(
                     f"{param_session} must be instance of {Session.__name__}"
                 )
 
-            return func(self, *args, **kwargs)
+            return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
 from pysql_repo._repository import Repository
```

### Comparing `pysql-repo-0.6.3/pysql_repo/_repository.py` & `pysql-repo-0.7.0/pysql_repo/asyncio/async_repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,42 +9,43 @@
     Type,
     TypeVar,
     Union,
     Sequence,
 )
 
 # CONTEXTLIB
-from contextlib import AbstractContextManager
+from contextlib import AbstractAsyncContextManager
 
 # SQLALCHEMY
 from sqlalchemy import ColumnExpressionArgument, Select
-from sqlalchemy.orm import Session, InstrumentedAttribute, declarative_base
+from sqlalchemy.ext.asyncio import AsyncSession
+from sqlalchemy.orm import DeclarativeBase, InstrumentedAttribute
 
 # DECORATORS
-from pysql_repo._decorators import check_values as _check_values, with_session
+from pysql_repo._decorators import check_values as _check_values
 
 # UTILS
 from pysql_repo._utils import (
     FilterType,
     RelationshipOption,
+    async_apply_pagination as _async_apply_pagination,
     build_delete_stmt as _build_delete_stmt,
     build_insert_stmt as _build_insert_stmt,
     build_select_stmt as _build_select_stmt,
     build_update_stmt as _build_update_stmt,
     select_distinct as _select_distinct,
-    apply_pagination as _apply_pagination,
 )
 
 
-_T = TypeVar("_T", bound=declarative_base())
+_T = TypeVar("_T", bound=DeclarativeBase)
 
 
-class Repository:
+class AsyncRepository:
     """
-    Represents a repository for database operations.
+    Represents an asynchronous repository for database operations.
 
     Attributes:
         _session_factory: The session factory used for creating sessions.
 
     Methods:
         session_manager: Returns the session factory.
         _select: Selects a single row from the database.
@@ -53,554 +54,581 @@
         _select_all_stmt: Selects all rows from the database using a custom statement.
         _select_paginate: Selects a paginated set of rows from the database.
         _select_paginate_stmt: Selects a paginated set of rows from the database using a custom statement.
     """
 
     def __init__(
         self,
-        session_factory: Callable[..., AbstractContextManager[Session]],
+        session_factory: Callable[..., AbstractAsyncContextManager[AsyncSession]],
     ) -> None:
         """
-        Initializes the Repository.
+        Initializes the AsyncRepository.
 
         Args:
-            session_factory: A callable that returns a context manager
+            session_factory: A callable that returns an asynchronous context manager
                              for creating and managing database sessions.
 
         Returns:
             None
         """
         self._session_factory = session_factory
 
-    def session_manager(self) -> AbstractContextManager[Session]:
+    def session_manager(self) -> AbstractAsyncContextManager[AsyncSession]:
         """
         Get a session manager.
 
         Returns:
-            AbstractContextManager[Session]: An context manager for managing database sessions.
+            AbstractAsyncContextManager[AsyncSession]: An asynchronous context manager for managing database sessions.
         """
         return self._session_factory()
 
-    @with_session()
-    def _select(
+    async def _select(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
-        distinct: Optional[ColumnExpressionArgument] = None,
+        distinct: Optional[ColumnExpressionArgument[Any]] = None,
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
-        session: Optional[Session] = None,
     ) -> Optional[_T]:
         """
         Selects a single object from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             distinct: The distinct column expression.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
-            session: The session to use.
 
         Returns:
-            The selected object or None if not found.
+            The selected row.
+
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return self._select_stmt(
+        return await self._select_stmt(
+            __session__,
             stmt=stmt,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
-            session=session,
         )
 
-    @with_session()
-    def _select_stmt(
+    async def _select_stmt(
         self,
+        __session__: AsyncSession,
+        /,
         stmt: Select[Tuple[_T]],
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
-        group_by: Optional[ColumnExpressionArgument] = None,
-        session: Optional[Session] = None,
+        group_by: Optional[ColumnExpressionArgument[Any]] = None,
     ) -> Optional[_T]:
         """
         Selects a single object from the database using a custom statement.
 
         Args:
+            __session__: The session to use.
             stmt: The custom select statement.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             group_by: The column expression to group by.
-            session: The session to use.
 
         Returns:
             The selected object or None if not found.
+
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
         )
 
-        return session.execute(stmt).unique().scalar_one_or_none()
+        result = await __session__.execute(stmt)
 
-    @with_session()
-    def _select_all(
+        return result.unique().scalar_one_or_none()
+
+    async def _select_all(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
-        distinct: Optional[List[ColumnExpressionArgument]] = None,
+        distinct: Optional[ColumnExpressionArgument[Any]] = None,
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
-        limit: int = None,
-        session: Optional[Session] = None,
+        limit: Optional[int] = None,
     ) -> Sequence[_T]:
         """
         Selects all objects from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             distinct: The distinct column expressions.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of objects to return.
-            session: The session to use.
 
         Returns:
             A sequence of selected objects.
+
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return self._select_all_stmt(
+        return await self._select_all_stmt(
+            __session__,
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             order_by=order_by,
             direction=direction,
             limit=limit,
-            session=session,
         )
 
-    @with_session()
-    def _select_all_stmt(
+    async def _select_all_stmt(
         self,
+        __session__: AsyncSession,
+        /,
         stmt: Select[Tuple[_T]],
         model: Type[_T],
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
-        group_by: Optional[ColumnExpressionArgument] = None,
+        group_by: Optional[ColumnExpressionArgument[Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
-        limit: int = None,
-        session: Optional[Session] = None,
+        limit: Optional[int] = None,
     ) -> Sequence[_T]:
         """
         Selects all objects from the database using a custom statement.
 
         Args:
+            __session__: The session to use.
             stmt: The custom select statement.
             model: The model class representing the table.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             group_by: The column expression to group by.
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of rows to return.
-            session: The session to use.
 
         Returns:
             A sequence of selected objects.
+
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
             order_by=order_by,
             direction=direction,
             limit=limit,
         )
 
-        return session.execute(stmt).unique().scalars().all()
+        result = await __session__.execute(stmt)
+
+        return result.unique().scalars().all()
 
-    @with_session()
-    def _select_paginate(
+    async def _select_paginate(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
         page: int,
         per_page: int,
-        distinct: Optional[ColumnExpressionArgument] = None,
+        distinct: Optional[ColumnExpressionArgument[Any]] = None,
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
-        limit: int = None,
-        session: Optional[Session] = None,
+        limit: Optional[int] = None,
     ) -> Tuple[Sequence[_T], str]:
         """
         Selects a paginated set of objects from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             page: The page number.
             per_page: The number of items per page.
             distinct: The distinct column expression.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of objects to return.
-            session: The session to use.
 
         Returns:
             A tuple containing the selected objects and pagination information.
+
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return self._select_paginate_stmt(
+        return await self._select_paginate_stmt(
+            __session__,
             stmt=stmt,
             model=model,
             page=page,
             per_page=per_page,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             order_by=order_by,
             direction=direction,
             limit=limit,
-            session=session,
         )
 
-    @with_session()
-    def _select_paginate_stmt(
+    async def _select_paginate_stmt(
         self,
+        __session__: AsyncSession,
+        /,
         stmt: Select[Tuple[_T]],
         model: Type[_T],
         page: int,
         per_page: int,
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
-        group_by: Optional[ColumnExpressionArgument] = None,
+        group_by: Optional[ColumnExpressionArgument[Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
-        limit: int = None,
-        session: Optional[Session] = None,
+        limit: Optional[int] = None,
     ) -> Tuple[Sequence[_T], str]:
         """
         Selects a paginated set of rows from the database using a custom statement.
 
         Args:
+            __session__: The session to use.
             stmt: The custom select statement.
             model: The model class representing the table.
             page: The page number.
             per_page: The number of items per page.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             group_by: The column expression to group by.
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of rows to return.
-            session: The session to use.
 
         Returns:
             A tuple containing the selected objects and pagination information.
+
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
             order_by=order_by,
             direction=direction,
             limit=limit,
         )
 
-        stmt, pagination = _apply_pagination(
-            session=session,
+        stmt, pagination = await _async_apply_pagination(
+            __session__,
             stmt=stmt,
             page=page,
             per_page=per_page,
         )
 
-        return session.execute(stmt).unique().scalars().all(), pagination
+        result = await __session__.execute(stmt)
+
+        return result.unique().scalars().all(), pagination
 
     @_check_values(as_list=False)
-    @with_session()
-    def _update_all(
+    async def _update_all(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
         values: Dict[str, Any],
         filters: Optional[FilterType] = None,
         flush: bool = False,
         commit: bool = False,
-        session: Optional[Session] = None,
     ) -> Sequence[_T]:
         """
         Updates multiple objects in the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             values: A dictionary of column-value pairs to update.
             filters: The filters to apply.
             flush: Whether to flush the session after the update.
             commit: Whether to commit the session after the update.
-            session: The session to use.
 
         Returns:
             A sequence of updated objects.
         """
         stmt = _build_update_stmt(
             model=model,
             values=values,
             filters=filters,
         )
 
-        sequence = session.execute(stmt).unique().scalars().all()
+        result = await __session__.execute(stmt)
+
+        sequence = result.unique().scalars().all()
 
         if flush:
-            session.flush()
+            await __session__.flush()
         if commit:
-            session.commit()
+            await __session__.commit()
 
-        [session.refresh(item) for item in sequence]
+        for item in sequence:
+            await __session__.refresh(item)
 
         return sequence
 
     @_check_values(as_list=False)
-    @with_session()
-    def _update(
+    async def _update(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
         values: Dict[str, Any],
         filters: Optional[FilterType] = None,
         flush: bool = False,
         commit: bool = False,
-        session: Optional[Session] = None,
     ) -> Optional[_T]:
         """
         Updates a single object in the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             values: A dictionary of column-value pairs to update.
             filters: The filters to apply.
             flush: Whether to flush the session after the update.
             commit: Whether to commit the session after the update.
-            session: The session to use.
 
         Returns:
             The updated object or None if not found.
         """
         stmt = _build_update_stmt(
             model=model,
             values=values,
             filters=filters,
         )
 
-        item = session.execute(stmt).unique().scalar_one_or_none()
+        result = await __session__.execute(stmt)
+
+        item = result.unique().scalar_one_or_none()
 
         if item is None:
             return None
 
         if flush:
-            session.flush()
+            await __session__.flush()
         if commit:
-            session.commit()
+            await __session__.commit()
 
-        session.refresh(item)
+        await __session__.refresh(item)
 
         return item
 
     @_check_values(as_list=True)
-    @with_session()
-    def _add_all(
+    async def _add_all(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
         values: List[Dict[str, Any]],
         flush: bool = False,
         commit: bool = False,
-        session: Optional[Session] = None,
     ) -> Sequence[_T]:
         """
         Adds multiple objects to the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             values: A list of dictionaries containing column-value pairs for each object.
             flush: Whether to flush the session after adding the objects.
             commit: Whether to commit the session after adding the objects.
-            session: The session to use.
 
         Returns:
             A sequence of added objects.
         """
         stmt = _build_insert_stmt(model=model)
 
-        sequence = session.execute(stmt, values).unique().scalars().all()
+        result = await __session__.execute(stmt, values)
+
+        sequence = result.unique().scalars().all()
 
         if flush:
-            session.flush()
+            await __session__.flush()
         if commit:
-            session.commit()
+            await __session__.commit()
 
         if flush or commit:
-            [session.refresh(item) for item in sequence]
+            for item in sequence:
+                await __session__.refresh(item)
 
         return sequence
 
     @_check_values(as_list=False)
-    @with_session()
-    def _add(
+    async def _add(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
         values: Dict[str, Any],
         flush: bool = False,
         commit: bool = False,
-        session: Optional[Session] = None,
     ) -> _T:
         """
         Adds a single object to the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             values: A dictionary of column-value pairs for the object.
             flush: Whether to flush the session after adding the object.
             commit: Whether to commit the session after adding the object.
-            session: The session to use.
 
         Returns:
             The added object.
+
         """
         stmt = _build_insert_stmt(model=model)
 
-        item = session.execute(stmt, values).unique().scalar_one()
+        result = await __session__.execute(stmt, values)
+
+        item = result.unique().scalar_one()
 
         if flush:
-            session.flush()
+            await __session__.flush()
         if commit:
-            session.commit()
+            await __session__.commit()
 
         if flush or commit:
-            session.refresh(item)
+            await __session__.refresh(item)
 
         return item
 
-    @with_session()
-    def _delete_all(
+    async def _delete_all(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
-        filters: Optional[FilterType] = None,
+        filters: FilterType,
         flush: bool = True,
         commit: bool = False,
-        session: Optional[Session] = None,
     ) -> bool:
         """
         Deletes multiple objects from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             filters: The filters to apply.
             flush: Whether to flush the session after the deletion.
             commit: Whether to commit the session after the deletion.
-            session: The session to use.
 
         Returns:
             True if any objects were deleted, False otherwise.
         """
         stmt = _build_delete_stmt(
             model=model,
             filters=filters,
         )
 
-        sequence = session.execute(stmt).unique().scalars().all()
+        result = await __session__.execute(stmt)
+
+        sequence = result.unique().scalars().all()
 
         if len(sequence) == 0:
             return False
 
         if flush:
-            session.flush()
+            await __session__.flush()
         if commit:
-            session.commit()
+            await __session__.commit()
 
         return True
 
-    @with_session()
-    def _delete(
+    async def _delete(
         self,
+        __session__: AsyncSession,
+        /,
         model: Type[_T],
-        filters: Optional[FilterType] = None,
+        filters: FilterType,
         flush: bool = True,
         commit: bool = False,
-        session: Optional[Session] = None,
     ) -> bool:
         """
         Deletes a single object from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             filters: The filters to apply.
             flush: Whether to flush the session after the deletion.
             commit: Whether to commit the session after the deletion.
-            session: The session to use.
 
         Returns:
             True if the object was deleted, False otherwise.
         """
         stmt = _build_delete_stmt(
             model=model,
             filters=filters,
         )
 
-        item = session.execute(stmt).unique().scalar_one_or_none()
+        result = await __session__.execute(stmt)
+
+        item = result.unique().scalar_one_or_none()
 
         if item is None:
             return False
 
         if flush:
-            session.flush()
+            await __session__.flush()
         if commit:
-            session.commit()
+            await __session__.commit()
 
         return True
```

### Comparing `pysql-repo-0.6.3/pysql_repo/_service.py` & `pysql-repo-0.7.0/pysql_repo/_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.3/pysql_repo/_utils.py` & `pysql-repo-0.7.0/pysql_repo/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # MODULES
-from ast import Delete
 from dataclasses import dataclass, field
 import json
 from typing import (
+    cast,
     Any,
     Dict,
     Iterable,
     List,
     Optional,
     Tuple,
     Type,
@@ -14,81 +14,89 @@
     TypeAlias,
     Union,
 )
 
 # SQLALCHEMY
 from sqlalchemy import (
     ColumnExpressionArgument,
+    Delete,
     Select,
+    UnaryExpression,
     Update,
     and_,
     asc,
     delete,
     desc,
     insert,
     select,
     distinct,
     tuple_,
     func,
     update,
 )
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import (
+    DeclarativeBase,
     Session,
     noload,
     lazyload,
     joinedload,
     subqueryload,
     selectinload,
     raiseload,
     contains_eager,
-    declarative_base,
 )
 from sqlalchemy.orm.attributes import InstrumentedAttribute
+from sqlalchemy.orm.strategy_options import _AbstractLoad
 from sqlalchemy.sql.dml import ReturningDelete, ReturningInsert, ReturningUpdate
 from sqlalchemy.sql.elements import Null, BinaryExpression
 
 # Enum
 from pysql_repo._constants.enum import LoadingTechnique, Operators
 
 FilterType: TypeAlias = Dict[
-    Union[InstrumentedAttribute, Tuple[InstrumentedAttribute]], Any
+    Union[InstrumentedAttribute[Any], Tuple[InstrumentedAttribute[Any]]], Any
 ]
 
-_Base = declarative_base()
+_T = TypeVar("_T", bound=DeclarativeBase)
 
+_T_SELECT_UPDATE = TypeVar("_T_SELECT_UPDATE", bound=Union[Select[Any], Update])
 
-_T = TypeVar("_T", bound=_Base)
+_T_SELECT_UPDATE_DELETE = TypeVar(
+    "_T_SELECT_UPDATE_DELETE", bound=Union[Select[Any], Update, Delete]
+)
 
 
 @dataclass
 class RelationshipOption:
     """
     Represents options for a relationship between two entities.
 
     Attributes:
         lazy (LoadingTechnique): The loading technique for the relationship.
         added_criteria (Optional[BinaryExpression]): Additional criteria for the relationship.
         children (Dict[InstrumentedAttribute, "RelationshipOption"]): Child relationships.
     """
 
     lazy: LoadingTechnique
-    added_criteria: Optional[BinaryExpression] = field(default=None)
-    children: Dict[InstrumentedAttribute, "RelationshipOption"] = field(default=None)
+    added_criteria: Optional[BinaryExpression[Any]] = field(default=None)
+    children: Optional[Dict[InstrumentedAttribute[Any], "RelationshipOption"]] = field(
+        default=None
+    )
 
 
 def build_select_stmt(
-    stmt: Select[Tuple[_T]],
+    stmt: Select[Any],
     model: Optional[Type[_T]] = None,
     filters: Optional[FilterType] = None,
     optional_filters: Optional[FilterType] = None,
     relationship_options: Optional[
-        Dict[InstrumentedAttribute, RelationshipOption]
+        Dict[InstrumentedAttribute[Any], RelationshipOption]
     ] = None,
-    group_by: Optional[ColumnExpressionArgument] = None,
+    group_by: Optional[ColumnExpressionArgument[Any]] = None,
     order_by: Optional[Union[List[str], str]] = None,
     direction: Optional[Union[List[str], str]] = None,
     limit: Optional[int] = None,
 ) -> Select[Tuple[_T]]:
     """
     Builds and returns a select statement with optional filters, group by, order by, and limit clauses.
 
@@ -122,30 +130,31 @@
     )
 
     stmt = apply_group_by(
         stmt=stmt,
         group_by=group_by,
     )
 
-    stmt = apply_order_by(
-        stmt=stmt,
-        model=model,
-        order_by=order_by,
-        direction=direction,
-    )
+    if model is not None:
+        stmt = apply_order_by(
+            stmt=stmt,
+            model=model,
+            order_by=order_by,
+            direction=direction,
+        )
 
     return apply_limit(
         stmt=stmt,
         limit=limit,
     )
 
 
 def build_update_stmt(
     model: Type[_T],
-    values: Dict,
+    values: Dict[Any, Any],
     filters: Optional[FilterType] = None,
 ) -> ReturningUpdate[Tuple[_T]]:
     """
     Build and delete an update statement for the given model, values, and filters.
 
     Args:
         model (Type[_T]): The model class to update.
@@ -198,15 +207,15 @@
         stmt=delete(model),
         filter_dict=filters,
     ).returning(model)
 
 
 def select_distinct(
     model: Type[_T],
-    expr: ColumnExpressionArgument,
+    expr: Optional[ColumnExpressionArgument[Any]] = None,
 ) -> Select[Tuple[_T]]:
     """
     Selects distinct values from a column expression.
 
     Args:
         model: The model type to select from.
         expr: The column expression to select distinct values from.
@@ -216,15 +225,15 @@
         If the column expression is None, it selects all columns from the model.
     """
     return select(distinct(expr)) if expr is not None else select(model)
 
 
 def apply_group_by(
     stmt: Select[Tuple[_T]],
-    group_by: ColumnExpressionArgument,
+    group_by: Optional[ColumnExpressionArgument[Any]] = None,
 ) -> Select[Tuple[_T]]:
     """
     Apply the GROUP BY clause to the given SQL statement.
 
     Args:
         stmt (Select[Tuple[_T]]): The SQL statement to apply the GROUP BY clause to.
         group_by (ColumnExpressionArgument): The column or expression to group by.
@@ -232,58 +241,59 @@
     Returns:
         Select[Tuple[_T]]: The modified SQL statement with the GROUP BY clause applied.
     """
     return stmt.group_by(group_by) if group_by is not None else stmt
 
 
 def apply_relationship_options(
-    stmt: Union[Select[Tuple[_T]], Update],
-    relationship_options: Dict[InstrumentedAttribute, RelationshipOption],
-    parents: Optional[List[InstrumentedAttribute]] = None,
-) -> Union[Select[Tuple[_T]], Update]:
+    stmt: _T_SELECT_UPDATE,
+    relationship_options: Optional[
+        Dict[InstrumentedAttribute[Any], RelationshipOption]
+    ] = None,
+    parents: Optional[List[InstrumentedAttribute[Any]]] = None,
+) -> _T_SELECT_UPDATE:
     """
     Apply relationship options to a SQLAlchemy statement.
 
     Args:
-        stmt (Union[Select[Tuple[_T]], Update]): The SQLAlchemy statement to apply the relationship options to.
+        stmt (_T_SELECT_UPDATE): The SQLAlchemy statement to apply the relationship options to.
         relationship_options (Dict[InstrumentedAttribute, RelationshipOption]): A dictionary of relationship options.
         parents (List[InstrumentedAttribute], optional): The list of parent relationships. Defaults to None.
 
     Returns:
-        Union[Select[Tuple[_T]], Update]: The modified SQLAlchemy statement with the applied relationship options.
+        _T_SELECT_UPDATE: The modified SQLAlchemy statement with the applied relationship options.
     """
 
     def get_load(
         loading_technique: LoadingTechnique,
-        items: List[InstrumentedAttribute],
-        extra_conditions: Optional[BinaryExpression] = None,
-    ):
+        items: List[InstrumentedAttribute[Any]],
+        extra_conditions: Optional[BinaryExpression[Any]] = None,
+    ) -> _AbstractLoad:
         items_post = []
         for item in items:
             if extra_conditions is not None:
                 items_post.append(item.and_(*extra_conditions))
             else:
                 items_post.append(item)
 
-        if loading_technique == LoadingTechnique.CONTAINS_EAGER:
-            return contains_eager(*items_post)
-        elif loading_technique == LoadingTechnique.LAZY:
-            return lazyload(*items_post)
-        elif loading_technique == LoadingTechnique.JOINED:
-            return joinedload(*items_post)
-        elif loading_technique == LoadingTechnique.SUBQUERY:
-            return subqueryload(*items_post)
-        elif loading_technique == LoadingTechnique.SELECTIN:
-            return selectinload(*items_post)
-        elif loading_technique == LoadingTechnique.RAISE:
-            return raiseload(*items_post)
-        elif loading_technique == LoadingTechnique.NOLOAD:
-            return noload(*items_post)
-
-        return None
+        match loading_technique:
+            case LoadingTechnique.CONTAINS_EAGER:
+                return contains_eager(*items_post)
+            case LoadingTechnique.LAZY:
+                return lazyload(*items_post)
+            case LoadingTechnique.JOINED:
+                return joinedload(*items_post)
+            case LoadingTechnique.SUBQUERY:
+                return subqueryload(*items_post)
+            case LoadingTechnique.SELECTIN:
+                return selectinload(*items_post)
+            case LoadingTechnique.RAISE:
+                return raiseload(*items_post)
+            case LoadingTechnique.NOLOAD:
+                return noload(*items_post)
 
     if relationship_options is None:
         return stmt
 
     for relationship, sub_relationships in relationship_options.items():
         if any(
             [
@@ -300,55 +310,59 @@
         load = get_load(
             loading_technique=sub_relationships.lazy,
             items=sub_items,
             extra_conditions=sub_relationships.added_criteria,
         )
 
         if load is not None:
-            stmt = stmt.options(load)
+            stmt = cast(_T_SELECT_UPDATE, stmt.options(load))
 
         if (children := sub_relationships.children) is not None:
             stmt = apply_relationship_options(
                 stmt,
                 relationship_options=children,
                 parents=sub_items,
             )
 
     return stmt
 
 
 def apply_filters(
-    stmt: Union[Select[Tuple[_T]], Update],
-    filter_dict: FilterType,
+    stmt: _T_SELECT_UPDATE_DELETE,
+    filter_dict: Optional[FilterType] = None,
     with_optional: bool = False,
-) -> Union[Select[Tuple[_T]], Update, Delete]:
+) -> _T_SELECT_UPDATE_DELETE:
     """
     Apply filters to the given statement.
 
     Args:
-        stmt (Union[Select[Tuple[_T]], Update]): The statement to apply filters to.
+        stmt (_T_SELECT_UPDATE_DELETE): The statement to apply filters to.
         filter_dict (_FilterType): The dictionary containing the filters.
         with_optional (bool, optional): Whether to include optional filters. Defaults to False.
 
     Returns:
-        Union[Select[Tuple[_T]], Update, Delete]: The statement with applied filters.
+        _T_SELECT_UPDATE_DELETE: The statement with applied filters.
     """
     filters = get_filters(
         filters=filter_dict,
         with_optional=with_optional,
     )
 
-    return stmt if len(filters) == 0 else stmt.filter(and_(*filters))
+    return (
+        stmt
+        if len(filters) == 0
+        else cast(_T_SELECT_UPDATE_DELETE, stmt.filter(and_(*filters)))
+    )
 
 
 def apply_order_by(
     stmt: Select[Tuple[_T]],
     model: Type[_T],
-    order_by: Union[List[str], str],
-    direction: Union[List[str], str],
+    order_by: Optional[Union[List[str], str]] = None,
+    direction: Optional[Union[List[str], str]] = None,
 ) -> Select[Tuple[_T]]:
     """
     Apply order by clause to the given SQLAlchemy select statement.
 
     Args:
         stmt (Select[Tuple[_T]]): The SQLAlchemy select statement.
         model (Type[_T]): The model class.
@@ -366,105 +380,111 @@
 
     if isinstance(direction, str):
         direction = [direction]
 
     if len(order_by) != len(direction):
         raise ValueError("order_by length must be equals to direction length")
 
-    order_by_list = []
+    order_by_list: List[UnaryExpression[Any]] = []
     for column, dir in zip(order_by, direction):
         if dir == "desc":
             order_by_list.append(desc(getattr(model, column)))
         elif dir == "asc":
             order_by_list.append(asc(getattr(model, column)))
 
     return stmt.order_by(*order_by_list)
 
 
 def apply_pagination(
-    session: Session,
-    stmt: Select[Tuple[_T]],
+    __session__: Session,
+    /,
+    stmt: Select[Any],
     page: int,
     per_page: int,
-) -> Tuple[Select[Tuple[_T]], str]:
+) -> Tuple[Select[Any], str]:
     """
     Apply pagination to a SQLAlchemy select statement.
 
     Args:
-        session (Session): The SQLAlchemy session object.
+        __session__ (Session): The SQLAlchemy session object.
         stmt (Select[Tuple[_T]]): The select statement to apply pagination to.
         page (int): The page number.
         per_page (int): The number of results per page.
 
     Returns:
         Tuple[Select[Tuple[_T]], str]: A tuple containing the modified select statement
         with pagination applied, and a JSON string representing the pagination information.
     """
-    if page is None or per_page is None:
-        return stmt, None
-
-    total_results = session.scalar(select(func.count()).select_from(stmt))
-    total_pages = (total_results + per_page - 1) // per_page
-
-    pagination = {
-        "total": total_results,
-        "page": page,
-        "per_page": per_page,
-        "total_pages": total_pages,
-    }
-
-    pagination = json.dumps(pagination)
-
-    stmt = stmt.offset((page - 1) * per_page).limit(per_page)
+    total_results = __session__.scalar(
+        select(func.count()).select_from(stmt.subquery())
+    )
 
-    return stmt, pagination
+    return _apply_pagination(
+        stmt=stmt,
+        total_results=total_results or 0,
+        page=page,
+        per_page=per_page,
+    )
 
 
 async def async_apply_pagination(
-    session: AsyncSession,
+    __session__: AsyncSession,
+    /,
     stmt: Select[Tuple[_T]],
     page: int,
     per_page: int,
 ) -> Tuple[Select[Tuple[_T]], str]:
     """
     Apply pagination to a SQLAlchemy select statement asynchronously.
 
     Args:
-        session (AsyncSession): The SQLAlchemy async session.
+        __session__ (AsyncSession): The SQLAlchemy async session.
         stmt (Select[Tuple[_T]]): The select statement to apply pagination to.
         page (int): The page number.
         per_page (int): The number of results per page.
 
     Returns:
         Tuple[Select[Tuple[_T]], str]: A tuple containing the modified select statement
         with pagination applied, and a JSON string representing the pagination details.
     """
-    if page is None or per_page is None:
-        return stmt, None
+    total_results = await __session__.scalar(
+        select(func.count()).select_from(stmt.subquery())
+    )
+
+    return _apply_pagination(
+        stmt=stmt,
+        total_results=total_results or 0,
+        page=page,
+        per_page=per_page,
+    )
+
+
+def _apply_pagination(
+    stmt: Select[Tuple[_T]], total_results: int, page: int, per_page: int
+) -> Tuple[Select[Tuple[_T]], str]:
 
-    total_results = await session.scalar(select(func.count()).select_from(stmt))
     total_pages = (total_results + per_page - 1) // per_page
 
-    pagination = {
+    pagination_dict = {
         "total": total_results,
         "page": page,
         "per_page": per_page,
         "total_pages": total_pages,
     }
 
-    pagination = json.dumps(pagination)
+    pagination = json.dumps(pagination_dict)
 
     stmt = stmt.offset((page - 1) * per_page).limit(per_page)
 
     return stmt, pagination
 
 
 def apply_limit(
     stmt: Select[Tuple[_T]],
-    limit: int,
+    limit: Optional[int] = None,
 ) -> Select[Tuple[_T]]:
     """
     Apply a limit to the given SQL statement.
 
     Args:
         stmt (Select[Tuple[_T]]): The SQL statement to apply the limit to.
         limit (int): The maximum number of rows to return.
@@ -474,15 +494,15 @@
     """
     return stmt.limit(limit) if limit is not None else stmt
 
 
 def get_conditions_from_dict(
     values: FilterType,
     with_optional: bool = False,
-) -> List[ColumnExpressionArgument]:
+) -> List[ColumnExpressionArgument[Any]]:
     """
     Convert a dictionary of filter conditions into a list of SQLAlchemy conditions.
 
     Args:
         values (dict): A dictionary containing the filter conditions.
         with_optional (bool, optional): Whether to include optional conditions with a value of None. Defaults to False.
 
@@ -512,30 +532,34 @@
                     case Operators.IDIFFERENT:
                         if not isinstance(v, Null):
                             conditions.append(func.lower(key) != func.lower(v))
                         else:
                             conditions.append(key != v)
                     case Operators.LIKE:
                         if not isinstance(v, Null):
-                            conditions.append(key.like(v))
+                            if isinstance(key, InstrumentedAttribute):
+                                conditions.append(key.like(v))
                         else:
                             conditions.append(key == v)
                     case Operators.NOT_LIKE:
                         if not isinstance(v, Null):
-                            conditions.append(~key.like(v))
+                            if isinstance(key, InstrumentedAttribute):
+                                conditions.append(~key.like(v))
                         else:
                             conditions.append(key != v)
                     case Operators.ILIKE:
                         if not isinstance(v, Null):
-                            conditions.append(key.ilike(v))
+                            if isinstance(key, InstrumentedAttribute):
+                                conditions.append(key.ilike(v))
                         else:
                             conditions.append(key == v)
                     case Operators.NOT_ILIKE:
                         if not isinstance(v, Null):
-                            conditions.append(~key.ilike(v))
+                            if isinstance(key, InstrumentedAttribute):
+                                conditions.append(~key.ilike(v))
                         else:
                             conditions.append(key != v)
                     case Operators.BETWEEN:
                         if len(v) != 2:
                             continue
                         if v[0] is not None:
                             conditions.append(key > v[0])
@@ -562,15 +586,15 @@
                             conditions.append(tuple_(*key).in_(v))
                         else:
                             conditions.append(key.in_(v))
                     case Operators.IIN:
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
                             conditions.append(
-                                tuple_([func.lower(key_) for key_ in key]).in_(
+                                tuple_(*(func.lower(key_) for key_ in key)).in_(
                                     [
                                         (
                                             func.lower(v_)
                                             if not isinstance(v_, Null)
                                             else v_
                                         )
                                         for v_ in v
@@ -597,15 +621,15 @@
                         else:
                             conditions.append(key.notin_(v))
 
                     case Operators.NOT_IIN:
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
                             conditions.append(
-                                tuple_([func.lower(key_) for key_ in key]).notin_(
+                                tuple_(*(func.lower(key_) for key_ in key)).notin_(
                                     [
                                         (
                                             func.lower(v_)
                                             if not isinstance(v_, Null)
                                             else v_
                                         )
                                         for v_ in v
@@ -627,33 +651,35 @@
                             )
                     case Operators.HAS:
                         v = get_filters(
                             v,
                             with_optional=with_optional,
                         )
                         for condition in v:
-                            conditions.append(key.has(condition))
+                            if isinstance(key, InstrumentedAttribute):
+                                conditions.append(key.has(condition))
                     case Operators.ANY:
                         v = get_filters(
                             v,
                             with_optional=with_optional,
                         )
 
                         if len(v) == 0:
                             continue
 
-                        conditions.append(key.any(and_(*v)))
+                        if isinstance(key, InstrumentedAttribute):
+                            conditions.append(key.any(and_(*v)))
 
     return conditions
 
 
 def get_filters(
-    filters: FilterType,
+    filters: Optional[FilterType] = None,
     with_optional: bool = False,
-) -> List[ColumnExpressionArgument]:
+) -> List[ColumnExpressionArgument[Any]]:
     """
     Get the conditions for filtering data based on the given filters.
 
     Args:
         filters (dict): The filters to apply on the data.
         with_optional (bool, optional): Whether to include optional filters. Defaults to False.
 
@@ -661,18 +687,16 @@
         List[ColumnExpressionArgument]: The conditions for filtering the data.
     """
     if filters is None:
         return []
     if not isinstance(filters, dict):
         raise TypeError("<filters> must be type of <dict>")
 
-    filters = [{x: y} for x, y in filters.items()]
-
     conditions = []
-    for filter_c in filters:
+    for filter_c in [{x: y} for x, y in filters.items()]:
         if type(filter_c) is not dict:
             continue
 
         conditions_from_dict = get_conditions_from_dict(
             filter_c,
             with_optional=with_optional,
         )
```

### Comparing `pysql-repo-0.6.3/pysql_repo/asyncio/async_database.py` & `pysql-repo-0.7.0/pysql_repo/asyncio/async_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # MODULES
 import logging
-from typing import Any, AsyncGenerator, List, Optional
+from typing import Any, AsyncGenerator, List, Optional, Type
 from pathlib import Path
 
 # SQLALCHEMY
 from sqlalchemy import text, MetaData, Connection, Table
-from sqlalchemy.orm import DeclarativeMeta
+from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy.inspection import inspect
 from sqlalchemy.ext.asyncio import (
     create_async_engine,
     async_sessionmaker,
     AsyncSession,
 )
 
@@ -49,15 +49,15 @@
         session_factory: Context manager for creating an async session.
         init_tables_from_json_files: Initializes tables from JSON files.
     """
 
     def __init__(
         self,
         databases_config: _DataBaseConfigTypedDict,
-        base: DeclarativeMeta,
+        base: Type[DeclarativeBase],
         metadata_views: Optional[List[MetaData]] = None,
         autoflush: bool = False,
         expire_on_commit: bool = False,
         echo: bool = False,
     ) -> None:
         """
         Initializes an instance of AsyncDatabase.
@@ -69,18 +69,20 @@
             metadata_views: Optional list of metadata views.
 
         Returns:
             None
         """
         super().__init__(databases_config, _logger, base, metadata_views)
 
+        assert self._connection_string is not None, "Connection string is required."
+
         self._engine = create_async_engine(
-            self._database_config.get("connection_string"),
+            self._connection_string,
             echo=echo,
-            connect_args=self._database_config.get("connect_args") or {},
+            connect_args=self._connect_args,
         )
 
         self._session_factory = async_sessionmaker(
             bind=self._engine,
             autoflush=autoflush,
             expire_on_commit=expire_on_commit,
         )
@@ -92,15 +94,15 @@
         Returns:
             None
 
         Raises:
             Exception: If an error occurs during the database creation process.
         """
 
-        def inspect_view_names(conn: Connection):
+        def inspect_view_names(conn: Connection) -> List[str]:
             inspector = inspect(conn)
 
             return [item.lower() for item in inspector.get_view_names()]
 
         async with self._engine.connect() as conn:
             current_view_names = await conn.run_sync(inspect_view_names)
 
@@ -161,15 +163,17 @@
                     timezone=timezone,
                 )
 
                 if raw_data is None:
                     continue
 
                 await session.execute(table.delete())
-                await session.execute(table.insert().values(raw_data))
+
+                if len(raw_data) > 0:
+                    await session.execute(table.insert().values(raw_data))
 
                 self._logger.info(
                     f"Successfully initialized {table_name=} from the file at {str(path)}."
                 )
 
             await session.commit()
```

### Comparing `pysql-repo-0.6.3/pysql_repo/asyncio/async_decorator.py` & `pysql-repo-0.7.0/pysql_repo/asyncio/async_decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+# MODULES
+import functools
+from typing import Any, Callable, Coroutine, ParamSpec, TypeVar
+
 # SQLALCHEMY
 from sqlalchemy.ext.asyncio import AsyncSession
 
+_P = ParamSpec("_P")
+_T = TypeVar("_T")
+
 
 def with_async_session(
     param_session: str = "session",
-):
+) -> Callable[
+    [Callable[_P, Coroutine[Any, Any, _T]]], Callable[_P, Coroutine[Any, Any, _T]]
+]:
     """
     Decorator that provides an async session to the decorated method.
     If the session is not provided as a keyword argument, it creates a new session using the session manager.
     The session is then passed as a keyword argument to the decorated method.
 
     Args:
         param_session (str, optional): The name of the session parameter. Defaults to "session".
@@ -17,33 +26,38 @@
         TypeError: If the decorated object is not an instance of AsyncRepository or AsyncService.
         TypeError: If the session is not an instance of AsyncSession.
 
     Returns:
         Callable: The decorated method.
     """
 
-    def decorator(func):
-        async def wrapper(self, *args, **kwargs):
+    def decorator(
+        func: Callable[_P, Coroutine[Any, Any, _T]]
+    ) -> Callable[_P, Coroutine[Any, Any, _T]]:
+
+        @functools.wraps(func)
+        async def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> _T:
+            self = kwargs.get("self")
             if not isinstance(self, (AsyncRepository, AsyncService)):
                 raise TypeError(
                     f"{self.__class__.__name__} must be instance of {AsyncRepository.__name__} or {AsyncService.__name__}"
                 )
 
             session = kwargs.get(param_session)
 
             if session is None:
                 async with self.session_manager() as session:
                     kwargs[param_session] = session
-                    return await func(self, *args, **kwargs)
+                    return await func(*args, **kwargs)
             elif not isinstance(session, AsyncSession):
                 raise TypeError(
                     f"{param_session} must be instance of {AsyncSession.__name__}"
                 )
 
-            return await func(self, *args, **kwargs)
+            return await func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
 from pysql_repo.asyncio.async_repository import AsyncRepository
```

### Comparing `pysql-repo-0.6.3/pysql_repo/asyncio/async_repository.py` & `pysql-repo-0.7.0/pysql_repo/_repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,45 +9,42 @@
     Type,
     TypeVar,
     Union,
     Sequence,
 )
 
 # CONTEXTLIB
-from contextlib import AbstractAsyncContextManager
+from contextlib import AbstractContextManager
 
 # SQLALCHEMY
 from sqlalchemy import ColumnExpressionArgument, Select
-from sqlalchemy.ext.asyncio import AsyncSession
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import InstrumentedAttribute
+from sqlalchemy.orm import DeclarativeBase, Session, InstrumentedAttribute, Session
 
 # DECORATORS
 from pysql_repo._decorators import check_values as _check_values
-from pysql_repo.asyncio.async_decorator import with_async_session
 
 # UTILS
 from pysql_repo._utils import (
     FilterType,
     RelationshipOption,
-    async_apply_pagination as _async_apply_pagination,
     build_delete_stmt as _build_delete_stmt,
     build_insert_stmt as _build_insert_stmt,
     build_select_stmt as _build_select_stmt,
     build_update_stmt as _build_update_stmt,
     select_distinct as _select_distinct,
+    apply_pagination as _apply_pagination,
 )
 
 
-_T = TypeVar("_T", bound=declarative_base())
+_T = TypeVar("_T", bound=DeclarativeBase)
 
 
-class AsyncRepository:
+class Repository:
     """
-    Represents an asynchronous repository for database operations.
+    Represents a repository for database operations.
 
     Attributes:
         _session_factory: The session factory used for creating sessions.
 
     Methods:
         session_manager: Returns the session factory.
         _select: Selects a single row from the database.
@@ -56,579 +53,556 @@
         _select_all_stmt: Selects all rows from the database using a custom statement.
         _select_paginate: Selects a paginated set of rows from the database.
         _select_paginate_stmt: Selects a paginated set of rows from the database using a custom statement.
     """
 
     def __init__(
         self,
-        session_factory: Callable[..., AbstractAsyncContextManager[AsyncSession]],
+        session_factory: Callable[..., AbstractContextManager[Session]],
     ) -> None:
         """
-        Initializes the AsyncRepository.
+        Initializes the Repository.
 
         Args:
-            session_factory: A callable that returns an asynchronous context manager
+            session_factory: A callable that returns a context manager
                              for creating and managing database sessions.
 
         Returns:
             None
         """
         self._session_factory = session_factory
 
-    def session_manager(self) -> AbstractAsyncContextManager[AsyncSession]:
+    def session_manager(self) -> AbstractContextManager[Session]:
         """
         Get a session manager.
 
         Returns:
-            AbstractAsyncContextManager[AsyncSession]: An asynchronous context manager for managing database sessions.
+            AbstractContextManager[Session]: An context manager for managing database sessions.
         """
         return self._session_factory()
 
-    @with_async_session()
-    async def _select(
+    def _select(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
-        distinct: Optional[ColumnExpressionArgument] = None,
+        distinct: Optional[ColumnExpressionArgument[Any]] = None,
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
-        session: Optional[AsyncSession] = None,
     ) -> Optional[_T]:
         """
         Selects a single object from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             distinct: The distinct column expression.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
-            The selected object or None if not found.
 
         Returns:
-            The selected row.
-
+            The selected object or None if not found.
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return await self._select_stmt(
+        return self._select_stmt(
+            __session__,
             stmt=stmt,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
-            session=session,
         )
 
-    @with_async_session()
-    async def _select_stmt(
+    def _select_stmt(
         self,
+        __session__: Session,
+        /,
         stmt: Select[Tuple[_T]],
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
-        group_by: Optional[ColumnExpressionArgument] = None,
-        session: Optional[AsyncSession] = None,
+        group_by: Optional[ColumnExpressionArgument[Any]] = None,
     ) -> Optional[_T]:
         """
         Selects a single object from the database using a custom statement.
 
         Args:
+            __session__: The session to use.
             stmt: The custom select statement.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             group_by: The column expression to group by.
-            session: The session to use.
 
         Returns:
             The selected object or None if not found.
-
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
         )
 
-        result = await session.execute(stmt)
-
-        return result.unique().scalar_one_or_none()
+        return __session__.execute(stmt).unique().scalar_one_or_none()
 
-    @with_async_session()
-    async def _select_all(
+    def _select_all(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
-        distinct: Optional[List[ColumnExpressionArgument]] = None,
+        distinct: Optional[ColumnExpressionArgument[Any]] = None,
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
-        limit: int = None,
-        session: Optional[AsyncSession] = None,
+        limit: Optional[int] = None,
     ) -> Sequence[_T]:
         """
         Selects all objects from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             distinct: The distinct column expressions.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of objects to return.
-            session: The session to use.
 
         Returns:
             A sequence of selected objects.
-
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return await self._select_all_stmt(
+        return self._select_all_stmt(
+            __session__,
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             order_by=order_by,
             direction=direction,
             limit=limit,
-            session=session,
         )
 
-    @with_async_session()
-    async def _select_all_stmt(
+    def _select_all_stmt(
         self,
+        __session__: Session,
+        /,
         stmt: Select[Tuple[_T]],
         model: Type[_T],
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
-        group_by: Optional[ColumnExpressionArgument] = None,
+        group_by: Optional[ColumnExpressionArgument[Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
-        limit: int = None,
-        session: Optional[AsyncSession] = None,
+        limit: Optional[int] = None,
     ) -> Sequence[_T]:
         """
         Selects all objects from the database using a custom statement.
 
         Args:
+            __session__: The session to use.
             stmt: The custom select statement.
             model: The model class representing the table.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             group_by: The column expression to group by.
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of rows to return.
-            session: The session to use.
 
         Returns:
             A sequence of selected objects.
-
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
             order_by=order_by,
             direction=direction,
             limit=limit,
         )
 
-        result = await session.execute(stmt)
-
-        return result.unique().scalars().all()
+        return __session__.execute(stmt).unique().scalars().all()
 
-    @with_async_session()
-    async def _select_paginate(
+    def _select_paginate(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
         page: int,
         per_page: int,
-        distinct: Optional[ColumnExpressionArgument] = None,
+        distinct: Optional[ColumnExpressionArgument[Any]] = None,
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
-        limit: int = None,
-        session: Optional[AsyncSession] = None,
+        limit: Optional[int] = None,
     ) -> Tuple[Sequence[_T], str]:
         """
         Selects a paginated set of objects from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             page: The page number.
             per_page: The number of items per page.
             distinct: The distinct column expression.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of objects to return.
-            session: The session to use.
 
         Returns:
             A tuple containing the selected objects and pagination information.
-
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return await self._select_paginate_stmt(
+        return self._select_paginate_stmt(
+            __session__,
             stmt=stmt,
             model=model,
             page=page,
             per_page=per_page,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             order_by=order_by,
             direction=direction,
             limit=limit,
-            session=session,
         )
 
-    @with_async_session()
-    async def _select_paginate_stmt(
+    def _select_paginate_stmt(
         self,
+        __session__: Session,
+        /,
         stmt: Select[Tuple[_T]],
         model: Type[_T],
         page: int,
         per_page: int,
         filters: Optional[FilterType] = None,
         optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
-            Dict[InstrumentedAttribute, RelationshipOption]
+            Dict[InstrumentedAttribute[Any], RelationshipOption]
         ] = None,
-        group_by: Optional[ColumnExpressionArgument] = None,
+        group_by: Optional[ColumnExpressionArgument[Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
-        limit: int = None,
-        session: Optional[AsyncSession] = None,
+        limit: Optional[int] = None,
     ) -> Tuple[Sequence[_T], str]:
         """
         Selects a paginated set of rows from the database using a custom statement.
 
         Args:
+            __session__: The session to use.
             stmt: The custom select statement.
             model: The model class representing the table.
             page: The page number.
             per_page: The number of items per page.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             group_by: The column expression to group by.
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of rows to return.
-            session: The session to use.
 
         Returns:
             A tuple containing the selected objects and pagination information.
-
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
             order_by=order_by,
             direction=direction,
             limit=limit,
         )
 
-        stmt, pagination = await _async_apply_pagination(
-            session=session,
+        stmt, pagination = _apply_pagination(
+            __session__,
             stmt=stmt,
             page=page,
             per_page=per_page,
         )
 
-        result = await session.execute(stmt)
-
-        return result.unique().scalars().all(), pagination
+        return __session__.execute(stmt).unique().scalars().all(), pagination
 
     @_check_values(as_list=False)
-    @with_async_session()
-    async def _update_all(
+    def _update_all(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
         values: Dict[str, Any],
         filters: Optional[FilterType] = None,
         flush: bool = False,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
     ) -> Sequence[_T]:
         """
         Updates multiple objects in the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             values: A dictionary of column-value pairs to update.
             filters: The filters to apply.
             flush: Whether to flush the session after the update.
             commit: Whether to commit the session after the update.
-            session: The session to use.
 
         Returns:
             A sequence of updated objects.
         """
         stmt = _build_update_stmt(
             model=model,
             values=values,
             filters=filters,
         )
 
-        result = await session.execute(stmt)
-
-        sequence = result.unique().scalars().all()
+        sequence = __session__.execute(stmt).unique().scalars().all()
 
         if flush:
-            await session.flush()
+            __session__.flush()
         if commit:
-            await session.commit()
+            __session__.commit()
 
-        [await session.refresh(item) for item in sequence]
+        for item in sequence:
+            __session__.refresh(item)
 
         return sequence
 
     @_check_values(as_list=False)
-    @with_async_session()
-    async def _update(
+    def _update(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
         values: Dict[str, Any],
         filters: Optional[FilterType] = None,
         flush: bool = False,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
     ) -> Optional[_T]:
         """
         Updates a single object in the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             values: A dictionary of column-value pairs to update.
             filters: The filters to apply.
             flush: Whether to flush the session after the update.
             commit: Whether to commit the session after the update.
-            session: The session to use.
 
         Returns:
             The updated object or None if not found.
         """
         stmt = _build_update_stmt(
             model=model,
             values=values,
             filters=filters,
         )
 
-        result = await session.execute(stmt)
-
-        item = result.unique().scalar_one_or_none()
+        item = __session__.execute(stmt).unique().scalar_one_or_none()
 
         if item is None:
             return None
 
         if flush:
-            await session.flush()
+            __session__.flush()
         if commit:
-            await session.commit()
+            __session__.commit()
 
-        await session.refresh(item)
+        __session__.refresh(item)
 
         return item
 
     @_check_values(as_list=True)
-    @with_async_session()
-    async def _add_all(
+    def _add_all(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
         values: List[Dict[str, Any]],
         flush: bool = False,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
     ) -> Sequence[_T]:
         """
         Adds multiple objects to the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             values: A list of dictionaries containing column-value pairs for each object.
             flush: Whether to flush the session after adding the objects.
             commit: Whether to commit the session after adding the objects.
-            session: The session to use.
 
         Returns:
             A sequence of added objects.
         """
         stmt = _build_insert_stmt(model=model)
 
-        result = await session.execute(stmt, values)
-
-        sequence = result.unique().scalars().all()
+        sequence = __session__.execute(stmt, values).unique().scalars().all()
 
         if flush:
-            await session.flush()
+            __session__.flush()
         if commit:
-            await session.commit()
+            __session__.commit()
 
         if flush or commit:
-            [await session.refresh(item) for item in sequence]
+            for item in sequence:
+                __session__.refresh(item)
 
         return sequence
 
     @_check_values(as_list=False)
-    @with_async_session()
-    async def _add(
+    def _add(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
         values: Dict[str, Any],
         flush: bool = False,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
     ) -> _T:
         """
         Adds a single object to the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             values: A dictionary of column-value pairs for the object.
             flush: Whether to flush the session after adding the object.
             commit: Whether to commit the session after adding the object.
-            session: The session to use.
 
         Returns:
             The added object.
-
         """
         stmt = _build_insert_stmt(model=model)
 
-        result = await session.execute(stmt, values)
-
-        item = result.unique().scalar_one()
+        item = __session__.execute(stmt, values).unique().scalar_one()
 
         if flush:
-            await session.flush()
+            __session__.flush()
         if commit:
-            await session.commit()
+            __session__.commit()
 
         if flush or commit:
-            await session.refresh(item)
+            __session__.refresh(item)
 
         return item
 
-    @with_async_session()
-    async def _delete_all(
+    def _delete_all(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
-        filters: Optional[FilterType] = None,
+        filters: FilterType,
         flush: bool = True,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
     ) -> bool:
         """
         Deletes multiple objects from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             filters: The filters to apply.
             flush: Whether to flush the session after the deletion.
             commit: Whether to commit the session after the deletion.
-            session: The session to use.
 
         Returns:
             True if any objects were deleted, False otherwise.
         """
         stmt = _build_delete_stmt(
             model=model,
             filters=filters,
         )
 
-        result = await session.execute(stmt)
-
-        sequence = result.unique().scalars().all()
+        sequence = __session__.execute(stmt).unique().scalars().all()
 
         if len(sequence) == 0:
             return False
 
         if flush:
-            await session.flush()
+            __session__.flush()
         if commit:
-            await session.commit()
+            __session__.commit()
 
         return True
 
-    @with_async_session()
-    async def _delete(
+    def _delete(
         self,
+        __session__: Session,
+        /,
         model: Type[_T],
-        filters: Optional[FilterType] = None,
+        filters: FilterType,
         flush: bool = True,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
     ) -> bool:
         """
         Deletes a single object from the database.
 
         Args:
+            __session__: The session to use.
             model: The model class representing the table.
             filters: The filters to apply.
             flush: Whether to flush the session after the deletion.
             commit: Whether to commit the session after the deletion.
-            session: The session to use.
 
         Returns:
             True if the object was deleted, False otherwise.
         """
         stmt = _build_delete_stmt(
             model=model,
             filters=filters,
         )
 
-        result = await session.execute(stmt)
-
-        item = result.unique().scalar_one_or_none()
+        item = __session__.execute(stmt).unique().scalar_one_or_none()
 
         if item is None:
             return False
 
         if flush:
-            await session.flush()
+            __session__.flush()
         if commit:
-            await session.commit()
+            __session__.commit()
 
         return True
```

### Comparing `pysql-repo-0.6.3/pysql_repo/asyncio/async_service.py` & `pysql-repo-0.7.0/pysql_repo/asyncio/async_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # MODULES
 from typing import TypeVar, Generic
-from logging import Logger
 
 # CONTEXTLIB
 from contextlib import AbstractAsyncContextManager
 
 # SQLALCHEMY
 from sqlalchemy.ext.asyncio import AsyncSession
```

### Comparing `pysql-repo-0.6.3/pysql_repo/libs/file_lib.py` & `pysql-repo-0.7.0/pysql_repo/libs/file_lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 # MODULES
 import json
 from pathlib import Path
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Union, cast
 
 
 from typing import List, Dict, Union
 from pathlib import Path
 import json
 
 
-def open_json_file(path: Path, encoding: str = "utf-8") -> Union[List[Dict], Dict]:
+def open_json_file(
+    path: Path, encoding: str = "utf-8"
+) -> Union[List[Dict[str, Any]], Dict[str, Any]]:
     """
     Opens a JSON file and returns its contents as a Python object.
 
     Args:
         path (Path): The path to the JSON file.
         encoding (str, optional): The encoding of the file. Defaults to "utf-8".
 
     Returns:
-        Union[List[Dict], Dict]: The contents of the JSON file as a Python object.
+        JSONType: The contents of the JSON file as a Python object.
 
     Raises:
         FileNotFoundError: If the specified path does not exist.
         FileExistsError: If the specified path is not a file.
     """
     if not path.exists():
         raise FileNotFoundError(f"Path {path} does not exist")
 
     if not path.is_file():
         raise FileExistsError(f"Path {path} is not a file")
 
     with open(path, encoding=encoding) as json_file:
         raw_data = json.load(json_file)
 
-    return raw_data
+    return cast(Union[List[Dict[str, Any]], Dict[str, Any]], raw_data)
 
 
 def open_file(path: Path, encoding: str = "utf-8") -> bytes:
     """
     Opens a file at the given path and returns its content as bytes.
 
     Args:
@@ -54,25 +56,25 @@
     if not path.exists():
         raise FileNotFoundError(f"Path {path} does not exist")
 
     if not path.is_file():
         raise FileExistsError(f"Path {path} is not a file")
 
     with open(path, encoding=encoding) as file:
-        raw_data = file.read()
-        raw_data = raw_data.encode(encoding)
+        data = file.read()
+        encoded_data = data.encode(encoding)
 
-    return raw_data
+    return encoded_data
 
 
 def save_json_file(
     path: Path,
     data: Any,
     encoding: str = "utf-8",
-):
+) -> None:
     """
     Save data as a JSON file at the specified path.
 
     Args:
         path (Path): The path where the JSON file will be saved.
         data (Any): The data to be saved as JSON.
         encoding (str, optional): The encoding to be used when writing the file. Defaults to "utf-8".
@@ -85,15 +87,15 @@
 
 
 def save_file(
     path: Path,
     data: bytes,
     encoding: str = "utf-8",
     new_line: str = "\n",
-):
+) -> None:
     """
     Save the given data to a file at the specified path.
 
     Args:
         path (Path): The path where the file should be saved.
         data (bytes): The data to be saved.
         encoding (str, optional): The encoding to be used when writing the file. Defaults to "utf-8".
```

### Comparing `pysql-repo-0.6.3/pysql_repo.egg-info/PKG-INFO` & `pysql-repo-0.7.0/pysql_repo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.6.3
+Version: 0.7.0
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.3.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.6.3/pysql_repo.egg-info/SOURCES.txt` & `pysql-repo-0.7.0/pysql_repo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.3/setup.py` & `pysql-repo-0.7.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.6.3"
+version = "0.7.0"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="pysql-repo",
     version=version,
```

