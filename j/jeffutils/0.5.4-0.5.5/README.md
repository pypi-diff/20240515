# Comparing `tmp/jeffutils-0.5.4.tar.gz` & `tmp/jeffutils-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.5.4.tar", last modified: Wed May 15 15:17:20 2024, max compression
+gzip compressed data, was "jeffutils-0.5.5.tar", last modified: Wed May 15 16:58:49 2024, max compression
```

## Comparing `jeffutils-0.5.4.tar` & `jeffutils-0.5.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 15:17:20.189269 jeffutils-0.5.4/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.4/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 15:17:20.189269 jeffutils-0.5.4/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.4/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.4/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-15 15:17:20.189269 jeffutils-0.5.4/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-15 15:17:16.000000 jeffutils-0.5.4/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 15:17:20.189269 jeffutils-0.5.4/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 15:17:20.189269 jeffutils-0.5.4/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.4/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    19988 2024-05-15 15:16:36.000000 jeffutils-0.5.4/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 15:17:20.189269 jeffutils-0.5.4/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 15:17:20.000000 jeffutils-0.5.4/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-15 15:17:20.000000 jeffutils-0.5.4/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-15 15:17:20.000000 jeffutils-0.5.4/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-15 15:17:20.000000 jeffutils-0.5.4/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 16:58:49.214716 jeffutils-0.5.5/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.5/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 16:58:49.210716 jeffutils-0.5.5/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.5/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.5/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-15 16:58:49.214716 jeffutils-0.5.5/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-15 16:58:45.000000 jeffutils-0.5.5/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 16:58:49.210716 jeffutils-0.5.5/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 16:58:49.210716 jeffutils-0.5.5/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.5/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    21865 2024-05-15 16:46:43.000000 jeffutils-0.5.5/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 16:58:49.210716 jeffutils-0.5.5/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 16:58:49.000000 jeffutils-0.5.5/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-15 16:58:49.000000 jeffutils-0.5.5/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-15 16:58:49.000000 jeffutils-0.5.5/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-15 16:58:49.000000 jeffutils-0.5.5/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.5.4/LICENSE.txt` & `jeffutils-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.5.4/setup.py` & `jeffutils-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.5.4',
+    version='0.5.5',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.5.4/src/jeffutils/utils.py` & `jeffutils-0.5.5/src/jeffutils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -582,7 +582,62 @@
         conn.close()
         
     if verbose:
         for table_name, col_names in table_info.items():
             print(f'{table_name}:', ", ".join(map(str, col_names)))
             
     return table_info
+
+def get_unique_counts(path_db, table_name, ref_col, cols):
+    """
+    Retrieve the count of unique values for specified columns grouped by a reference column from a SQLite table.
+
+    Args:
+        path_db (str): Path to the SQLite database file.
+        table_name (str): Name of the table in the database.
+        ref_col (str): Name of the reference column to group by.
+        cols (list): List of column names for which to count unique values.
+
+    Returns:
+        pandas.DataFrame: DataFrame containing the count of unique values for each specified column grouped by the reference column.
+
+    Example:
+        Given input data in GameTest table:
+        game_id  A  B
+        0         0  a  a
+        1         0  a  a
+        2         0  a  b
+        3         0  a  b
+        4         0  a  b
+        5         1  b  c
+        6         1  b  c
+        7         1  b  c
+        8         1  b  c
+        9         1  b  d
+        10        1  b  d
+        11        1  b  e
+
+        Calling get_unique_counts('your_database.db', 'GameTest', 'game_id', ['A', 'B']) returns:
+           game_id  unique_A  unique_B
+        0        0         1         2
+        1        1         1         3
+    """
+    if not os.path.exists(path_db):
+        raise FileNotFoundError(f"Database file not found: {path_db}")
+    if not path_db.endswith('.db'):
+        raise ValueError("Database file must have a .db extension")
+    
+    try:
+        with sql.connect(path_db) as conn:
+            cur = conn.cursor()
+            query = (
+                f"SELECT {ref_col}, " + 
+                    ', '.join([f'COUNT(DISTINCT {col}) AS unique_{col}' for col in cols]) + 
+                f" FROM {table_name} \n"
+                f"GROUP BY {ref_col}"
+            )
+            res_df = pd.read_sql_query(query, conn)
+    finally:
+        conn.close()
+        
+    return res_df
+
```

