# Comparing `tmp/lisql-2.1.3.tar.gz` & `tmp/lisql-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisql-2.1.3.tar", last modified: Fri Apr  5 12:30:24 2024, max compression
+gzip compressed data, was "lisql-2.1.8.tar", last modified: Wed May 15 02:57:47 2024, max compression
```

## Comparing `lisql-2.1.3.tar` & `lisql-2.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-04-05 12:30:24.346324 lisql-2.1.3/
--rw-r--r--   0 li         (501) staff       (20)     1068 2024-04-05 11:57:55.000000 lisql-2.1.3/LICENSE
--rw-r--r--   0 li         (501) staff       (20)    18962 2024-04-05 12:30:24.346138 lisql-2.1.3/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)    18180 2024-04-05 11:57:55.000000 lisql-2.1.3/README.md
--rw-r--r--   0 li         (501) staff       (20)      103 2024-04-05 11:57:55.000000 lisql-2.1.3/pyproject.toml
--rw-r--r--   0 li         (501) staff       (20)      644 2024-04-05 12:30:24.346704 lisql-2.1.3/setup.cfg
--rw-r--r--   0 li         (501) staff       (20)      725 2024-04-05 12:09:19.000000 lisql-2.1.3/setup.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-04-05 12:30:24.344795 lisql-2.1.3/src/
-drwxr-xr-x   0 li         (501) staff       (20)        0 2024-04-05 12:30:24.345820 lisql-2.1.3/src/lisql.egg-info/
--rw-r--r--   0 li         (501) staff       (20)    18962 2024-04-05 12:30:24.000000 lisql-2.1.3/src/lisql.egg-info/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)      196 2024-04-05 12:30:24.000000 lisql-2.1.3/src/lisql.egg-info/SOURCES.txt
--rw-r--r--   0 li         (501) staff       (20)        1 2024-04-05 12:30:24.000000 lisql-2.1.3/src/lisql.egg-info/dependency_links.txt
--rw-r--r--   0 li         (501) staff       (20)        6 2024-04-05 12:30:24.000000 lisql-2.1.3/src/lisql.egg-info/top_level.txt
--rw-r--r--   0 li         (501) staff       (20)    22742 2024-04-05 11:57:55.000000 lisql-2.1.3/src/lisql.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 02:57:47.683489 lisql-2.1.8/
+-rw-r--r--   0 li         (501) staff       (20)     1068 2024-05-14 14:30:10.000000 lisql-2.1.8/LICENSE
+-rw-r--r--   0 li         (501) staff       (20)    18962 2024-05-15 02:57:47.683396 lisql-2.1.8/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)    18180 2024-05-14 14:30:03.000000 lisql-2.1.8/README.md
+-rw-r--r--   0 li         (501) staff       (20)      103 2024-05-14 14:30:06.000000 lisql-2.1.8/pyproject.toml
+-rw-r--r--   0 li         (501) staff       (20)      644 2024-05-15 02:57:47.683737 lisql-2.1.8/setup.cfg
+-rw-r--r--   0 li         (501) staff       (20)      725 2024-05-14 14:29:59.000000 lisql-2.1.8/setup.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 02:57:47.682316 lisql-2.1.8/src/
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-15 02:57:47.683180 lisql-2.1.8/src/lisql.egg-info/
+-rw-r--r--   0 li         (501) staff       (20)    18962 2024-05-15 02:57:47.000000 lisql-2.1.8/src/lisql.egg-info/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)      196 2024-05-15 02:57:47.000000 lisql-2.1.8/src/lisql.egg-info/SOURCES.txt
+-rw-r--r--   0 li         (501) staff       (20)        1 2024-05-15 02:57:47.000000 lisql-2.1.8/src/lisql.egg-info/dependency_links.txt
+-rw-r--r--   0 li         (501) staff       (20)        6 2024-05-15 02:57:47.000000 lisql-2.1.8/src/lisql.egg-info/top_level.txt
+-rw-r--r--   0 li         (501) staff       (20)    28277 2024-05-14 14:29:44.000000 lisql-2.1.8/src/lisql.py
```

### Comparing `lisql-2.1.3/LICENSE` & `lisql-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lisql-2.1.3/PKG-INFO` & `lisql-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisql
-Version: 2.1.3
+Version: 2.1.8
 Summary: Provides simple funtions to interact with MySQL databases and tables.
 Home-page: https://github.com/li812/lisql
 Author: Ali Ahammad
 Author-email: aliahammad0812@outlook.com
 Project-URL: Bug Tracker, https://github.com/li812/lisql/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lisql-2.1.3/README.md` & `lisql-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `lisql-2.1.3/setup.cfg` & `lisql-2.1.8/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lisql
-version = 2.1.3
+version = 2.1.8
 author = Ali Ahammad
 author_email = aliahammad0812@outlook.com
 description = Provides a simple interface to interact with MySQL databases.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/li812/lisql
 project_urls =
```

### Comparing `lisql-2.1.3/setup.py` & `lisql-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='lisql',
-    version='2.1.3',
+    version='2.1.8',
     py_modules=['lisql'],
     description='Provides simple funtions to interact with MySQL databases and tables.',
     author='Ali Ahammad',
     author_email='aliahammad0812@outlook.com',
     url='https://github.com/li812/lisql',
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

### Comparing `lisql-2.1.3/src/lisql.egg-info/PKG-INFO` & `lisql-2.1.8/src/lisql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisql
-Version: 2.1.3
+Version: 2.1.8
 Summary: Provides simple funtions to interact with MySQL databases and tables.
 Home-page: https://github.com/li812/lisql
 Author: Ali Ahammad
 Author-email: aliahammad0812@outlook.com
 Project-URL: Bug Tracker, https://github.com/li812/lisql/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lisql-2.1.3/src/lisql.py` & `lisql-2.1.8/src/lisql.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+print("""
+                                                                                                   
+888      d8b  .d8888b.   .d88888b.  888           
+888      Y8P d88P  Y88b d88P" "Y88b 888           
+888          Y88b.      888     888 888           
+888      888  "Y888b.   888     888 888           
+888      888     "Y88b. 888     888 888           
+888      888       "888 888 Y8b 888 888           
+888      888 Y88b  d88P Y88b.Y8b88P 888           
+88888888 888  "Y8888P"   "Y888888"  88888888     2.2
+                               Y8b                
+                                                  
+                                                                                                                                                   
+""")
 
 import importlib
 
 def check_and_install_mysql_connector():
     try:
         importlib.import_module('mysql.connector')
     except ImportError:
@@ -195,14 +209,29 @@
         databases = [database[0] for database in cursor]
         print(databases)
         return databases
     except mysql.connector.Error as e:
         print(f"Error while showing databases: {e}")
         return []
 
+def show_table(db, table_name):
+    try:
+        cursor = db.cursor()
+        cursor.execute(f"SELECT * FROM {table_name}")
+        rows = cursor.fetchall()
+        if len(rows) == 0:
+            print(f"No data found in table '{table_name}'")
+        else:
+            print(f"Contents of table '{table_name}':")
+            for row in rows:
+                print(row)
+    except mysql.connector.Error as e:
+        print(f"Error displaying table '{table_name}': {e}")
+
+
 def select_data(mydb, table_name, columns):
     try:
         cursor = mydb.cursor()
         column_list = ", ".join(columns)
         select_query = f"SELECT {column_list} FROM {table_name}"
         cursor.execute(select_query)
         row = cursor.fetchone()
@@ -337,100 +366,168 @@
                 print(info)
     except mysql.connector.Error as e:
         print(f"Error describing database: {e}")
 
 
 ########################   Start of Aggregate functions     #######################
 
-
-def select_count(connection, table, column):
+def select_count(mydb, table, column, transaction=False):
+    cursor = mydb.cursor()
     query = f"SELECT COUNT({column}) FROM {table}"
-    result = connection.execute(query).fetchone()
-    return result[0]
+    try:
+        if transaction:
+            mydb.start_transaction()  # Start the transaction explicitly
+        
+        cursor.execute(query)
+        result = cursor.fetchone()[0]
+        
+        if transaction:
+            mydb.commit()  # Commit the transaction if transaction=True
+        
+        return result
+    except mysql.connector.Error as e:
+        if transaction:
+            mydb.rollback()  # Roll back the transaction if an error occurs
+        print(f"Error executing query: {e}")
+        return None
+
 
-def select_sum(connection, table, column):
+def select_sum(mydb, table, column, transaction=False):
+    cursor = mydb.cursor()
     query = f"SELECT SUM({column}) FROM {table}"
-    result = connection.execute(query).fetchone()
-    return result[0]
+    try:
+        if transaction:
+            mydb.start_transaction()  # Start the transaction explicitly
+        
+        cursor.execute(query)
+        result = cursor.fetchone()[0]
+        
+        if transaction:
+            mydb.commit()  # Commit the transaction if transaction=True
+        
+        return result
+    except mysql.connector.Error as e:
+        if transaction:
+            mydb.rollback()  # Roll back the transaction if an error occurs
+        print(f"Error executing query: {e}")
+        return None
+
 
-def select_avg(connection, table, column):
+def select_avg(mydb, table, column, transaction=False):
+    cursor = mydb.cursor()
     query = f"SELECT AVG({column}) FROM {table}"
-    result = connection.execute(query).fetchone()
-    return result[0]
+    try:
+        if transaction:
+            mydb.start_transaction()  # Start the transaction explicitly
+        
+        cursor.execute(query)
+        result = cursor.fetchone()[0]
+        
+        if transaction:
+            mydb.commit()  # Commit the transaction if transaction=True
+        
+        return result
+    except mysql.connector.Error as e:
+        if transaction:
+            mydb.rollback()  # Roll back the transaction if an error occurs
+        print(f"Error executing query: {e}")
+        return None
+
 
-def select_min(connection, table, column):
+def select_min(mydb, table, column, transaction=False):
+    cursor = mydb.cursor()
     query = f"SELECT MIN({column}) FROM {table}"
-    result = connection.execute(query).fetchone()
-    return result[0]
+    try:
+        if transaction:
+            mydb.start_transaction()  # Start the transaction explicitly
+        
+        cursor.execute(query)
+        result = cursor.fetchone()[0]
+        
+        if transaction:
+            mydb.commit()  # Commit the transaction if transaction=True
+        
+        return result
+    except mysql.connector.Error as e:
+        if transaction:
+            mydb.rollback()  # Roll back the transaction if an error occurs
+        print(f"Error executing query: {e}")
+        return None
 
 
-def select_max(connection, table, column):
+def select_max(mydb, table, column, transaction=False):
+    cursor = mydb.cursor()
     query = f"SELECT MAX({column}) FROM {table}"
-    result = connection.execute(query).fetchone()
-    return result[0]
+    try:
+        if transaction:
+            mydb.start_transaction()  # Start the transaction explicitly
+        
+        cursor.execute(query)
+        result = cursor.fetchone()[0]
+        
+        if transaction:
+            mydb.commit()  # Commit the transaction if transaction=True
+        
+        return result
+    except mysql.connector.Error as e:
+        if transaction:
+            mydb.rollback()  # Roll back the transaction if an error occurs
+        print(f"Error executing query: {e}")
+        return None
 
 
 ########################   End of Aggregate functions     #######################
 
 
 ########################   Start of help    #######################
 def help(func=None):
     if func is None:
         print("LiSQL Package - Python Package for Interacting with MySQL Databases")
         print("Version: 2.1")
         print("Description: LiSQL is a Python package that simplifies working with MySQL databases by providing various functions for connection management, database operations, table operations, and data manipulation.")
         print("\nAvailable functions:")
-
         # Group 1: Connection Management
         print("\nConnection Management:")
         print("- create_connection(): Creates a local connection to a MySQL database.")
         print("  Example: create_connection()")
         print("  This function establishes a connection to a local MySQL database and returns the connection object.")
-        
         print("- create_remote_connection(host, user, password): Creates a remote connection to a MySQL database on a specified host.")
         print("  Example: create_remote_connection('remote_host', 'remote_user', 'remote_password')")
-        print("  This function establishes a remote connection to a MySQL database on the specified host and returns the connection object.")
-        
+        print("  This function establishes a remote connection to a MySQL database on the specified host and returns the connection object.")        
         print("- connect_remote_database(host, username, password, database): Connects to a remote MySQL database on a specified host.")
         print("  Example: connect_remote_database('remote_host', 'remote_user', 'remote_password', 'remote_db')")
-        print("  This function connects to a remote MySQL database on the specified host with the specified username, password, and database name, and returns the connection object.")
-        
+        print("  This function connects to a remote MySQL database on the specified host with the specified username, password, and database name, and returns the connection object.")       
         # Group 2: Database Operations
         print("\nDatabase Operations:")
         print("- create_database(mydb, name): Creates a new database with the specified name in the local or remote connection.")
         print("  Example: create_database(mydb, 'new_database')")
-        print("  This function creates a new database with the specified name in the connected local or remote MySQL connection.")
-        
+        print("  This function creates a new database with the specified name in the connected local or remote MySQL connection.")        
         print("- drop_database(mydb, name): Deletes the database with the specified name from the local or remote connection.")
         print("  Example: drop_database(mydb, 'existing_database')")
         print("  This function drops the database with the specified name from the connected local or remote MySQL connection.")
         
         print("- connect_database(mydb, name): Connects to an existing database with the specified name in the local or remote connection.")
         print("  Example: connect_database(mydb, 'existing_database')")
         print("  This function connects to an existing database with the specified name in the connected local or remote MySQL connection.")
         
         print("- show_databases(mydb): Displays a list of all databases in the connected server.")
         print("  Example: show_databases(mydb)")
         print("  This function shows a list of all databases in the connected local or remote MySQL server.")
-
         # Group 3: Table Operations
         print("\nTable Operations:")
         print("- show_tables(mydb): Displays a list of tables in the connected database.")
         print("  Example: show_tables(mydb)")
         print("  This function shows a list of tables in the connected local or remote MySQL database.")
-        
         print("- create_table(mydb, table_name, columns, transaction=False): Creates a table with the specified columns.")
         print("  Example: columns = ['id INT PRIMARY KEY', 'name VARCHAR(255)', 'age INT']")
         print("           create_table(mydb, 'students', columns, transaction=True)")
-        print("  This function creates a new table with the specified name and columns in the connected local or remote MySQL database.")
-        
+        print("  This function creates a new table with the specified name and columns in the connected local or remote MySQL database.")        
         print("- drop_table(mydb, table_name, transaction=False): Deletes the specified table from the connected database.")
         print("  Example: drop_table(mydb, 'students', transaction=True)")
         print("  This function drops the specified table from the connected local or remote MySQL database.")
-
         print("- describe_table(mydb, table_name): Displays information about the specified table in the connected database.")
         print("  Example: describe_table(mydb, 'students')")
         print("  This function describes the specified table in the connected local or remote MySQL database.")
 
         # Group 4: Data Manipulation
         print("\nData Manipulation:")
         print("- select_data(mydb, table_name, columns): Retrieves data from the specified columns in the specified table.")
@@ -455,37 +552,31 @@
         print("           update_data(mydb, 'students', column_values, condition, transaction=True)")
         print("  This function updates data in the specified table that meets the specified condition in the connected local or remote MySQL database.")
         
         print("- execute_query(mydb, query, fetch=False, transaction=False): Executes the specified SQL query.")
         print("  Example: query = 'SELECT * FROM students'")
         print("           execute_query(mydb, query, fetch=True)")
         print("  This function executes the specified SQL query in the connected local or remote MySQL database.")
-        
         # Group 5: Aggregate Functions
         print("\nAggregate Functions:")
         print("- select_count(connection, table, column): Calculates the COUNT of records in the specified column of the table.")
         print("  Example: count = select_count(mydb, 'students', 'id')")
         print("  This function calculates the COUNT of records in the specified column of the table in the connected local or remote MySQL database.")
-        
         print("- select_sum(connection, table, column): Calculates the SUM of values in the specified column of the table.")
         print("  Example: total_age = select_sum(mydb, 'students', 'age')")
         print("  This function calculates the SUM of values in the specified column of the table in the connected local or remote MySQL database.")
-        
         print("- select_avg(connection, table, column): Calculates the AVG of values in the specified column of the table.")
         print("  Example: avg_age = select_avg(mydb, 'students', 'age')")
         print("  This function calculates the AVG of values in the specified column of the table in the connected local or remote MySQL database.")
-        
         print("- select_min(connection, table, column): Retrieves the minimum value in the specified column of the table.")
         print("  Example: min_age = select_min(mydb, 'students', 'age')")
         print("  This function retrieves the minimum value in the specified column of the table in the connected local or remote MySQL database.")
-        
         print("- select_max(connection, table, column): Retrieves the maximum value in the specified column of the table.")
         print("  Example: max_age = select_max(mydb, 'students', 'age')")
         print("  This function retrieves the maximum value in the specified column of the table in the connected local or remote MySQL database.")
-        
         # Transaction Support Examples
         print("\nTransaction Support")
         print("Here are the functions in LiSQL that support Transaction Support:")
         print("- create_database(mydb, name, transaction=False)")
         print("- drop_database(mydb, name, transaction=False)")
         print("- create_table(mydb, table_name, columns, transaction=False)")
         print("- drop_table(mydb, table_name, transaction=False)")
@@ -494,21 +585,48 @@
         print("- update_data(mydb, table_name, column_values, condition, transaction=False)")
         print("- execute_query(mydb, query, fetch=False, transaction=False)")
         print("Remember that you need to pass transaction=True as an argument to these functions to enable Transaction Support. This ensures that the operations are executed as part of a single transaction, providing data consistency and rollback capabilities in case of errors.")
         print("- Example 1: Creating a table with transaction support")
         print("  columns = ['id INT PRIMARY KEY', 'name VARCHAR(255)', 'age INT']")
         print("  create_table(mydb, 'students', columns, transaction=True)")
         print("  # This will create a new table 'students' with the specified columns.")
-        print("  # The transaction will ensure that the table is created only if the entire operation is successful.")
-        
-        print("\n- Example 2: Dropping a table with transaction support")
-        print("  drop_table(mydb, 'students', transaction=True)")
-        print("  # This will drop the table 'students' from the database.")
-        print("  # The transaction will ensure that the table is dropped only if the entire operation is successful.")
+        print("  # The transaction will ensure that the table is created only if all operations succeed. Otherwise, it will be rolled back.")
+        print("- Example 2: Inserting data with transaction support")
+        print("  values = (1, 'John Doe', 25)")
+        print("  insert_data(mydb, 'students', values, transaction=True)")
+        print("  # This will insert the specified data into the 'students' table.")
+        print("  # The transaction will ensure that the data is inserted only if all operations succeed. Otherwise, it will be rolled back.")
+        print("- Example 3: Executing multiple queries with transaction support")
+        print("  query1 = 'INSERT INTO students (id, name, age) VALUES (2, 'Jane Smith', 30)'")
+        print("  query2 = 'UPDATE students SET age = 31 WHERE id = 2'")
+        print("  execute_query(mydb, query1, transaction=True)")
+        print("  execute_query(mydb, query2, transaction=True)")
+        print("  # This will execute the specified queries as part of a single transaction.")
+        print("  # If any of the queries fail, the entire transaction will be rolled back.")
+        # Help for Aggregate Functions
+        print("\nHelp for Aggregate Functions")
+        print("Here are the functions in LiSQL that provide Aggregate Function Support:")
+        print("- select_count(connection, table, column)")
+        print("- select_sum(connection, table, column)")
+        print("- select_avg(connection, table, column)")
+        print("- select_min(connection, table, column)")
+        print("- select_max(connection, table, column)")
+        print("These functions allow you to perform aggregate calculations on the data in your MySQL database.")
+        print("To use these functions, simply call them with the appropriate arguments, and they will return the result of the aggregate calculation.")
+        print("For example, you can calculate the total number of records, the sum of values, the average value, the minimum value, or the maximum value in a column.")
+        print("Remember to pass the connection object, table name, and column name as arguments to these functions.")
+        print("For more information on each function, you can use the help() function followed by the function name.")
+        print("For example, help(select_count) will display information about the select_count() function.")
+        print("You can also refer to the LiSQL documentation for detailed usage instructions and examples.")
+    elif func.__name__ in globals():
+        print(help(func.__name__))
+    else:
+        print(f"No help available for {func.__name__}.")
+########################   End of help    #######################
+
+
 
-        print("\nNote: When transaction=True is passed as an argument to the functions that support it, the function will start a transaction, execute the query, and then commit the transaction. If an error occurs, it will roll back the transaction.")
 
-########################   End of help    #######################
 
 def __version__():
-    return 2.1
+    return 2.2
```

