# Comparing `tmp/lisql-2.1.8.tar.gz` & `tmp/lisql-2.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisql-2.1.8.tar", last modified: Wed May 15 02:57:47 2024, max compression
+gzip compressed data, was "lisql-2.1.86.tar", last modified: Wed May 15 19:34:15 2024, max compression
```

## Comparing `lisql-2.1.8.tar` & `lisql-2.1.86.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 02:57:47.683489 lisql-2.1.8/
--rw-r--r--   0 li         (501) staff       (20)     1068 2024-05-14 14:30:10.000000 lisql-2.1.8/LICENSE
--rw-r--r--   0 li         (501) staff       (20)    18962 2024-05-15 02:57:47.683396 lisql-2.1.8/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)    18180 2024-05-14 14:30:03.000000 lisql-2.1.8/README.md
--rw-r--r--   0 li         (501) staff       (20)      103 2024-05-14 14:30:06.000000 lisql-2.1.8/pyproject.toml
--rw-r--r--   0 li         (501) staff       (20)      644 2024-05-15 02:57:47.683737 lisql-2.1.8/setup.cfg
--rw-r--r--   0 li         (501) staff       (20)      725 2024-05-14 14:29:59.000000 lisql-2.1.8/setup.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 02:57:47.682316 lisql-2.1.8/src/
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 02:57:47.683180 lisql-2.1.8/src/lisql.egg-info/
--rw-r--r--   0 li         (501) staff       (20)    18962 2024-05-15 02:57:47.000000 lisql-2.1.8/src/lisql.egg-info/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)      196 2024-05-15 02:57:47.000000 lisql-2.1.8/src/lisql.egg-info/SOURCES.txt
--rw-r--r--   0 li         (501) staff       (20)        1 2024-05-15 02:57:47.000000 lisql-2.1.8/src/lisql.egg-info/dependency_links.txt
--rw-r--r--   0 li         (501) staff       (20)        6 2024-05-15 02:57:47.000000 lisql-2.1.8/src/lisql.egg-info/top_level.txt
--rw-r--r--   0 li         (501) staff       (20)    28277 2024-05-14 14:29:44.000000 lisql-2.1.8/src/lisql.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:34:15.568587 lisql-2.1.86/
+-rw-r--r--   0 li         (501) staff       (20)     1068 2024-05-15 03:29:18.000000 lisql-2.1.86/LICENSE
+-rw-r--r--   0 li         (501) staff       (20)    18997 2024-05-15 19:34:15.568484 lisql-2.1.86/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)    18214 2024-05-15 03:29:18.000000 lisql-2.1.86/README.md
+-rw-r--r--   0 li         (501) staff       (20)      103 2024-05-14 14:30:06.000000 lisql-2.1.86/pyproject.toml
+-rw-r--r--   0 li         (501) staff       (20)      645 2024-05-15 19:34:15.568831 lisql-2.1.86/setup.cfg
+-rw-r--r--   0 li         (501) staff       (20)      726 2024-05-15 19:34:07.000000 lisql-2.1.86/setup.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:34:15.567598 lisql-2.1.86/src/
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 19:34:15.568238 lisql-2.1.86/src/lisql.egg-info/
+-rw-r--r--   0 li         (501) staff       (20)    18997 2024-05-15 19:34:15.000000 lisql-2.1.86/src/lisql.egg-info/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)      196 2024-05-15 19:34:15.000000 lisql-2.1.86/src/lisql.egg-info/SOURCES.txt
+-rw-r--r--   0 li         (501) staff       (20)        1 2024-05-15 19:34:15.000000 lisql-2.1.86/src/lisql.egg-info/dependency_links.txt
+-rw-r--r--   0 li         (501) staff       (20)        6 2024-05-15 19:34:15.000000 lisql-2.1.86/src/lisql.egg-info/top_level.txt
+-rw-r--r--   0 li         (501) staff       (20)    28248 2024-05-15 19:29:47.000000 lisql-2.1.86/src/lisql.py
```

### Comparing `lisql-2.1.8/LICENSE` & `lisql-2.1.86/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Ali Ahammad
+Copyright (c) 2024 Ali Ahammad
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lisql-2.1.8/PKG-INFO` & `lisql-2.1.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisql
-Version: 2.1.8
+Version: 2.1.86
 Summary: Provides simple funtions to interact with MySQL databases and tables.
 Home-page: https://github.com/li812/lisql
 Author: Ali Ahammad
 Author-email: aliahammad0812@outlook.com
 Project-URL: Bug Tracker, https://github.com/li812/lisql/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -564,11 +564,13 @@
 
 ## License
 
 LiSQL is distributed under the MIT License. See the [LICENSE](https://github.com/li812/lisql/blob/main/LICENSE) file for more details.
 
 ## Contact
 stions, bug reports, or feedback, please feel free to contact the developers via:
-### Email: aliahammad0812@outlook.com 
+### Email: mail@aliahammad.com 
+
+### Website: https://www.aliahammad.com
 
 ### Instagram: https://www.instagram.com/the_raptor_rider_/
```

### Comparing `lisql-2.1.8/README.md` & `lisql-2.1.86/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -544,11 +544,13 @@
 
 ## License
 
 LiSQL is distributed under the MIT License. See the [LICENSE](https://github.com/li812/lisql/blob/main/LICENSE) file for more details.
 
 ## Contact
 stions, bug reports, or feedback, please feel free to contact the developers via:
-### Email: aliahammad0812@outlook.com 
+### Email: mail@aliahammad.com 
+
+### Website: https://www.aliahammad.com
 
 ### Instagram: https://www.instagram.com/the_raptor_rider_/
```

### Comparing `lisql-2.1.8/setup.cfg` & `lisql-2.1.86/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lisql
-version = 2.1.8
+version = 2.1.86
 author = Ali Ahammad
 author_email = aliahammad0812@outlook.com
 description = Provides a simple interface to interact with MySQL databases.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/li812/lisql
 project_urls =
```

### Comparing `lisql-2.1.8/setup.py` & `lisql-2.1.86/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='lisql',
-    version='2.1.8',
+    version='2.1.86',
     py_modules=['lisql'],
     description='Provides simple funtions to interact with MySQL databases and tables.',
     author='Ali Ahammad',
     author_email='aliahammad0812@outlook.com',
     url='https://github.com/li812/lisql',
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

### Comparing `lisql-2.1.8/src/lisql.egg-info/PKG-INFO` & `lisql-2.1.86/src/lisql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisql
-Version: 2.1.8
+Version: 2.1.86
 Summary: Provides simple funtions to interact with MySQL databases and tables.
 Home-page: https://github.com/li812/lisql
 Author: Ali Ahammad
 Author-email: aliahammad0812@outlook.com
 Project-URL: Bug Tracker, https://github.com/li812/lisql/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -564,11 +564,13 @@
 
 ## License
 
 LiSQL is distributed under the MIT License. See the [LICENSE](https://github.com/li812/lisql/blob/main/LICENSE) file for more details.
 
 ## Contact
 stions, bug reports, or feedback, please feel free to contact the developers via:
-### Email: aliahammad0812@outlook.com 
+### Email: mail@aliahammad.com 
+
+### Website: https://www.aliahammad.com
 
 ### Instagram: https://www.instagram.com/the_raptor_rider_/
```

### Comparing `lisql-2.1.8/src/lisql.py` & `lisql-2.1.86/src/lisql.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         else:
             print('MySQL not connected')
         return mydb
     except mysql.connector.Error as e:
         print(f"Error creating remote connection: {e}")
         return None
 
-def create_database(mydb, name, transaction=False):
+def create_database(mydb, name, transaction=True):
     cursor = mydb.cursor()
     create_db_query = f'CREATE DATABASE {name}'
     print(f'Executing command: {create_db_query}')
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
             
@@ -86,15 +86,15 @@
         else:
             print(f'Something else went wrong: {e}')
     except Exception as e:
         print(f'Something else went wrong: {e}')
     return mydb
 
 
-def connect_remote_database(host, username, password, database, transaction=False):
+def connect_remote_database(host, username, password, database, transaction=True):
     try:
         mydb = mysql.connector.connect(
             host=host,
             user=username,
             password=password,
             database=database
         )
@@ -103,15 +103,15 @@
             mydb.autocommit = False  # Disable autocommit to enable transactions
         return mydb
     except mysql.connector.Error as e:
         print(f"Error connecting to {host}: {e}")
         return None
 
 
-def drop_database(mydb, name, transaction=False):
+def drop_database(mydb, name, transaction=True):
     cursor = mydb.cursor()
     drop_db_query = f'DROP DATABASE IF EXISTS {name}'
     print(f'Executing command: {drop_db_query}')
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
             
@@ -126,15 +126,15 @@
             mydb.rollback()  # Roll back the transaction if an error occurs
         if e.errno == mysql.connector.errorcode.ER_BAD_DB_ERROR:
             print(f'Database {name} does not exist')
         else:
             print(f'Something else went wrong: {e}')
 
 
-def connect_database(mydb, name, transaction=False):
+def connect_database(mydb, name, transaction=True):
     try:
         mydb.database = name
         print('Connection established')
 
         if transaction:
             mydb.autocommit = False  # Disable autocommit to enable transactions
         
@@ -156,15 +156,15 @@
         tables = [table[0] for table in cursor]
         print(tables)
         return tables
     except mysql.connector.Error as e:
         print(f"Error while showing tables: {e}")
         return []
     
-def create_table(mydb, table_name, columns, transaction=False):
+def create_table(mydb, table_name, columns, transaction=True):
     cursor = mydb.cursor()
     column_definitions = ", ".join(columns)
     create_table_query = f"CREATE TABLE {table_name} ({column_definitions})"
     print(f'Executing command: {create_table_query}')
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
@@ -177,15 +177,15 @@
         print(f'Table {table_name} created successfully!')
     except mysql.connector.Error as e:
         if transaction:
             mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error creating table: {e}")
 
 
-def drop_table(mydb, table_name, transaction=False):
+def drop_table(mydb, table_name, transaction=True):
     cursor = mydb.cursor()
     drop_table_query = f'DROP TABLE IF EXISTS {table_name}'
     print(f'Executing command: {drop_table_query}')
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
             
@@ -238,15 +238,15 @@
         while row is not None:
             yield row
             row = cursor.fetchone()
     except mysql.connector.Error as e:
         print(f"Error while selecting data: {e}")
         return
 
-def insert_data(mydb, table_name, values, transaction=False):
+def insert_data(mydb, table_name, values, transaction=True):
     try:
         cursor = mydb.cursor()
         value_list = ", ".join(["%s"] * len(values))
         insert_query = f"INSERT INTO {table_name} VALUES ({value_list})"
         
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
@@ -262,15 +262,15 @@
         if transaction:
             mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error inserting data: {e}")
 
 
 
 
-def delete_data(mydb, table_name, condition, transaction=False):
+def delete_data(mydb, table_name, condition, transaction=True):
     try:
         cursor = mydb.cursor()
         delete_query = f"DELETE FROM {table_name} WHERE {condition}"
         
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
             
@@ -283,15 +283,15 @@
         
     except mysql.connector.Error as e:
         if transaction:
             mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error deleting data: {e}")
 
 
-def update_data(mydb, table_name, column_values, condition, transaction=False):
+def update_data(mydb, table_name, column_values, condition, transaction=True):
     try:
         cursor = mydb.cursor()
         column_value_pairs = [f"{col} = %s" for col in column_values.keys()]
         set_clause = ", ".join(column_value_pairs)
         update_query = f"UPDATE {table_name} SET {set_clause} WHERE {condition}"
         
         if transaction:
@@ -306,15 +306,15 @@
         
     except mysql.connector.Error as e:
         if transaction:
             mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error updating data: {e}")
 
 
-def execute_query(mydb, query, fetch=False, transaction=False):
+def execute_query(mydb, query, fetch=False, transaction=True):
     try:
         cursor = mydb.cursor()
         
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
             
         cursor.execute(query)
@@ -366,15 +366,15 @@
                 print(info)
     except mysql.connector.Error as e:
         print(f"Error describing database: {e}")
 
 
 ########################   Start of Aggregate functions     #######################
 
-def select_count(mydb, table, column, transaction=False):
+def select_count(mydb, table, column, transaction=True):
     cursor = mydb.cursor()
     query = f"SELECT COUNT({column}) FROM {table}"
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
         
         cursor.execute(query)
@@ -387,15 +387,15 @@
     except mysql.connector.Error as e:
         if transaction:
             mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
-def select_sum(mydb, table, column, transaction=False):
+def select_sum(mydb, table, column, transaction=True):
     cursor = mydb.cursor()
     query = f"SELECT SUM({column}) FROM {table}"
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
         
         cursor.execute(query)
@@ -408,15 +408,15 @@
     except mysql.connector.Error as e:
         if transaction:
             mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
-def select_avg(mydb, table, column, transaction=False):
+def select_avg(mydb, table, column, transaction=True):
     cursor = mydb.cursor()
     query = f"SELECT AVG({column}) FROM {table}"
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
         
         cursor.execute(query)
@@ -429,15 +429,15 @@
     except mysql.connector.Error as e:
         if transaction:
             mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
-def select_min(mydb, table, column, transaction=False):
+def select_min(mydb, table, column, transaction=True):
     cursor = mydb.cursor()
     query = f"SELECT MIN({column}) FROM {table}"
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
         
         cursor.execute(query)
@@ -450,15 +450,15 @@
     except mysql.connector.Error as e:
         if transaction:
             mydb.rollback()  # Roll back the transaction if an error occurs
         print(f"Error executing query: {e}")
         return None
 
 
-def select_max(mydb, table, column, transaction=False):
+def select_max(mydb, table, column, transaction=True):
     cursor = mydb.cursor()
     query = f"SELECT MAX({column}) FROM {table}"
     try:
         if transaction:
             mydb.start_transaction()  # Start the transaction explicitly
         
         cursor.execute(query)
@@ -513,50 +513,50 @@
         print("  Example: show_databases(mydb)")
         print("  This function shows a list of all databases in the connected local or remote MySQL server.")
         # Group 3: Table Operations
         print("\nTable Operations:")
         print("- show_tables(mydb): Displays a list of tables in the connected database.")
         print("  Example: show_tables(mydb)")
         print("  This function shows a list of tables in the connected local or remote MySQL database.")
-        print("- create_table(mydb, table_name, columns, transaction=False): Creates a table with the specified columns.")
+        print("- create_table(mydb, table_name, columns, transaction=True): Creates a table with the specified columns.")
         print("  Example: columns = ['id INT PRIMARY KEY', 'name VARCHAR(255)', 'age INT']")
         print("           create_table(mydb, 'students', columns, transaction=True)")
         print("  This function creates a new table with the specified name and columns in the connected local or remote MySQL database.")        
-        print("- drop_table(mydb, table_name, transaction=False): Deletes the specified table from the connected database.")
+        print("- drop_table(mydb, table_name, transaction=True): Deletes the specified table from the connected database.")
         print("  Example: drop_table(mydb, 'students', transaction=True)")
         print("  This function drops the specified table from the connected local or remote MySQL database.")
         print("- describe_table(mydb, table_name): Displays information about the specified table in the connected database.")
         print("  Example: describe_table(mydb, 'students')")
         print("  This function describes the specified table in the connected local or remote MySQL database.")
 
         # Group 4: Data Manipulation
         print("\nData Manipulation:")
         print("- select_data(mydb, table_name, columns): Retrieves data from the specified columns in the specified table.")
         print("  Example: columns = ['name', 'age']")
         print("           for data in select_data(mydb, 'students', columns):")
         print("               print(data)")
         print("  This function retrieves data from the specified columns in the specified table in the connected local or remote MySQL database.")
         
-        print("- insert_data(mydb, table_name, values, transaction=False): Inserts data into the specified table.")
+        print("- insert_data(mydb, table_name, values, transaction=True): Inserts data into the specified table.")
         print("  Example: values = (1, 'John Doe', 25)")
         print("           insert_data(mydb, 'students', values, transaction=True)")
         print("  This function inserts data into the specified table in the connected local or remote MySQL database.")
         
-        print("- delete_data(mydb, table_name, condition, transaction=False): Deletes data from the specified table that meets the specified condition.")
+        print("- delete_data(mydb, table_name, condition, transaction=True): Deletes data from the specified table that meets the specified condition.")
         print("  Example: condition = 'age > 30'")
         print("           delete_data(mydb, 'students', condition, transaction=True)")
         print("  This function deletes data from the specified table that meets the specified condition in the connected local or remote MySQL database.")
         
-        print("- update_data(mydb, table_name, column_values, condition, transaction=False): Updates data in the specified table that meets the specified condition.")
+        print("- update_data(mydb, table_name, column_values, condition, transaction=True): Updates data in the specified table that meets the specified condition.")
         print("  Example: column_values = {'name': 'John Smith', 'age': 32}")
         print("           condition = 'id = 1'")
         print("           update_data(mydb, 'students', column_values, condition, transaction=True)")
         print("  This function updates data in the specified table that meets the specified condition in the connected local or remote MySQL database.")
         
-        print("- execute_query(mydb, query, fetch=False, transaction=False): Executes the specified SQL query.")
+        print("- execute_query(mydb, query, fetch=False, transaction=True): Executes the specified SQL query.")
         print("  Example: query = 'SELECT * FROM students'")
         print("           execute_query(mydb, query, fetch=True)")
         print("  This function executes the specified SQL query in the connected local or remote MySQL database.")
         # Group 5: Aggregate Functions
         print("\nAggregate Functions:")
         print("- select_count(connection, table, column): Calculates the COUNT of records in the specified column of the table.")
         print("  Example: count = select_count(mydb, 'students', 'id')")
@@ -572,22 +572,22 @@
         print("  This function retrieves the minimum value in the specified column of the table in the connected local or remote MySQL database.")
         print("- select_max(connection, table, column): Retrieves the maximum value in the specified column of the table.")
         print("  Example: max_age = select_max(mydb, 'students', 'age')")
         print("  This function retrieves the maximum value in the specified column of the table in the connected local or remote MySQL database.")
         # Transaction Support Examples
         print("\nTransaction Support")
         print("Here are the functions in LiSQL that support Transaction Support:")
-        print("- create_database(mydb, name, transaction=False)")
-        print("- drop_database(mydb, name, transaction=False)")
-        print("- create_table(mydb, table_name, columns, transaction=False)")
-        print("- drop_table(mydb, table_name, transaction=False)")
-        print("- insert_data(mydb, table_name, values, transaction=False)")
-        print("- delete_data(mydb, table_name, condition, transaction=False)")
-        print("- update_data(mydb, table_name, column_values, condition, transaction=False)")
-        print("- execute_query(mydb, query, fetch=False, transaction=False)")
+        print("- create_database(mydb, name, transaction=True)")
+        print("- drop_database(mydb, name, transaction=True)")
+        print("- create_table(mydb, table_name, columns, transaction=True)")
+        print("- drop_table(mydb, table_name, transaction=True)")
+        print("- insert_data(mydb, table_name, values, transaction=True)")
+        print("- delete_data(mydb, table_name, condition, transaction=True)")
+        print("- update_data(mydb, table_name, column_values, condition, transaction=True)")
+        print("- execute_query(mydb, query, fetch=False, transaction=True)")
         print("Remember that you need to pass transaction=True as an argument to these functions to enable Transaction Support. This ensures that the operations are executed as part of a single transaction, providing data consistency and rollback capabilities in case of errors.")
         print("- Example 1: Creating a table with transaction support")
         print("  columns = ['id INT PRIMARY KEY', 'name VARCHAR(255)', 'age INT']")
         print("  create_table(mydb, 'students', columns, transaction=True)")
         print("  # This will create a new table 'students' with the specified columns.")
         print("  # The transaction will ensure that the table is created only if all operations succeed. Otherwise, it will be rolled back.")
         print("- Example 2: Inserting data with transaction support")
```

