# Comparing `tmp/rubberduckie-2023.7.1-py3-none-any.whl.zip` & `tmp/rubberduckie-2024.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 7085 bytes, number of entries: 16
--rw-r--r--  2.0 unx      346 b- defN 23-Jul-11 05:21 rubberduckie/__init__.py
+Zip file size: 8726 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      415 b- defN 24-May-15 08:34 rubberduckie/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 09:48 rubberduckie/cdsw/__init__.py
--rw-r--r--  2.0 unx     2956 b- defN 23-May-22 10:19 rubberduckie/cdsw/hadoop.py
--rw-r--r--  2.0 unx     3400 b- defN 23-Jul-11 05:19 rubberduckie/cdsw/import_fix.py
+-rw-r--r--  2.0 unx     6384 b- defN 24-May-15 07:46 rubberduckie/cdsw/hadoop.py
+-rw-r--r--  2.0 unx     3414 b- defN 24-May-15 08:33 rubberduckie/cdsw/import_fix.py
+-rw-r--r--  2.0 unx      745 b- defN 24-May-15 08:33 rubberduckie/cdsw/misc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:14 rubberduckie/da/__init__.py
--rw-r--r--  2.0 unx     2439 b- defN 23-Jul-11 05:20 rubberduckie/da/pilot.py
+-rw-r--r--  2.0 unx     2441 b- defN 24-May-15 07:47 rubberduckie/da/pilot.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 11:00 rubberduckie/dl/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/ml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/plot/__init__.py
--rw-r--r--  2.0 unx     1835 b- defN 23-May-22 10:38 rubberduckie/plot/evaluation.py
+-rw-r--r--  2.0 unx     1849 b- defN 24-May-15 07:46 rubberduckie/plot/evaluation.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/xai/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      420 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1338 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/RECORD
-16 files, 12839 bytes uncompressed, 4833 bytes compressed:  62.4%
+-rw-r--r--  2.0 unx        0 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      929 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1419 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/RECORD
+17 files, 17701 bytes uncompressed, 6348 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: rubberduckie/cdsw/hadoop.py
 Comment: 
 
 Filename: rubberduckie/cdsw/import_fix.py
 Comment: 
 
+Filename: rubberduckie/cdsw/misc.py
+Comment: 
+
 Filename: rubberduckie/da/__init__.py
 Comment: 
 
 Filename: rubberduckie/da/pilot.py
 Comment: 
 
 Filename: rubberduckie/dl/__init__.py
@@ -27,23 +30,23 @@
 
 Filename: rubberduckie/plot/evaluation.py
 Comment: 
 
 Filename: rubberduckie/xai/__init__.py
 Comment: 
 
-Filename: rubberduckie-2023.7.1.dist-info/LICENSE.txt
+Filename: rubberduckie-2024.5.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: rubberduckie-2023.7.1.dist-info/METADATA
+Filename: rubberduckie-2024.5.1.dist-info/METADATA
 Comment: 
 
-Filename: rubberduckie-2023.7.1.dist-info/WHEEL
+Filename: rubberduckie-2024.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: rubberduckie-2023.7.1.dist-info/top_level.txt
+Filename: rubberduckie-2024.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rubberduckie-2023.7.1.dist-info/RECORD
+Filename: rubberduckie-2024.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rubberduckie/__init__.py

```diff
@@ -3,14 +3,17 @@
     execute_db_query,
     extract_db_data,
 )
 
 from rubberduckie.cdsw.import_fix import (
     fix_cdsw_import_error,
 )
+from rubberduckie.cdsw.misc import (
+    clean_cdsw_project_trash,
+)
 
 from rubberduckie.plot.evaluation import (
     prepare_confusion_matrix,
 )
 
 from rubberduckie.da.pilot import (
     calc_weeks_between,
```

## rubberduckie/cdsw/hadoop.py

```diff
@@ -1,99 +1,218 @@
 import os
+import math
 import warnings
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
 from impala.dbapi import connect
 from impala.util import as_pandas
 
-DEBUG = True
+DEBUG = False
 if DEBUG:
-    print('DB tools are loaded!')
+    print("DB tools are loaded!")
 
 
 def prepare_connection(host: str):
     """Prepare connection to IDP (Hadoop) in CDSW
-    Colin Li @ 2023-05
+
+    Author:
+        Colin Li @ 2023-05
+
     Args:
         host (str): "impala" or "hive"
 
     Returns:
         impala.dbapi.connect: connection to IDP
     """
     CONN = None
     try:
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore")
-            if host == 'impala':
+            if host == "impala":
                 CONN = connect(
-                    host=os.getenv('IMPALA_HOST'),
-                    port=os.getenv('IMPALA_PORT'),
-                    database='default',
+                    host=os.getenv("IMPALA_HOST"),
+                    port=os.getenv("IMPALA_PORT"),
+                    database="default",
                     use_ssl=True,
                     ca_cert=None,
-                    auth_mechanism='GSSAPI',
-                    user='impala',
-                    password='',
-                    kerberos_service_name='impala')
-            elif host == 'hive':
+                    auth_mechanism="GSSAPI",
+                    user="impala",
+                    password="",
+                    kerberos_service_name="impala",
+                )
+            elif host == "hive":
                 CONN = connect(
-                    host=os.getenv('HIVE_HOST'),
-                    port=os.getenv('HIVE_PORT'),
-                    database='default',
+                    host=os.getenv("HIVE_HOST"),
+                    port=os.getenv("HIVE_PORT"),
+                    database="default",
                     use_ssl=True,
                     ca_cert=None,
-                    auth_mechanism='GSSAPI',
-                    user='hive',
-                    password='',
-                    kerberos_service_name='hive')
+                    auth_mechanism="GSSAPI",
+                    user="hive",
+                    password="",
+                    kerberos_service_name="hive",
+                )
     except TypeError:
         warnings.warn("Update password for Hadoop Authentication in CDSW!")
         warnings.warn("Run this in CDSW ONLY!")
         return None
     return CONN
 
 
 def execute_db_query(conn, query: str):
     """Execute databass query
-    Colin Li @ 2023-05
+
+    Author:
+        Colin Li @ 2023-05
+
     Args:
         conn (impala.dbapi.connect): connection
         query (str): can be either a string (query) or file path of a sql file
     """
-    if os.path.isfile(query) and query[-4:] == '.sql':
+    if os.path.isfile(query) and query[-4:] == ".sql":
         query_path = query
-        with open(query_path, 'r') as f:
+        with open(query_path, "r") as f:
             query = f.read()
-        print(f'Executing task {query_path}')
-    tasks = query.split(';')
+        print(f"Executing task {query_path}")
+    tasks = query.split(";")
     for i, t in enumerate(tasks):
-        if t.replace(' ', '').replace('\n', '') == '':
+        if t.replace(" ", "").replace("\n", "") == "":
             continue
         else:
-            print(f'Executing subtask {i+1}')
+            print(f"Executing subtask {i+1}")
             cursor = conn.cursor()
             cursor.execute(t)
-    print(f'Task is completed!')
+    print(f"Task is completed!")
 
 
 def extract_db_data(conn, query: str):
     """Extract data from database as pandas dataframe
-    Colin Li @ 2023-05
+
+    Author:
+        Colin Li @ 2023-05
 
     Args:
         conn (impala.dbapi.connect): connection
         query (str): can be either a string (query) or file path of a sql file
 
     Returns:
         pandas.DataFrame: Pandas dataframe containing database data
     """
-    if os.path.isfile(query) and query[-4:] == '.sql':
+    if os.path.isfile(query) and query[-4:] == ".sql":
         query_path = query
-        with open(query_path, 'r') as f:
+        with open(query_path, "r") as f:
             query = f.read()
-        print(f'Executing task {query_path}')
+        print(f"Executing task {query_path}")
     cursor = conn.cursor()
     cursor.execute(query)
     df = as_pandas(cursor)
     return df
 
 
+def generate_sql_row(row):
+    """Generate one sql row used in sql insert statement
+    Author:
+        Colin Li @ 2023-02
+    Args:
+        row (pd.Series): pandas data series
+    Returns:
+        str: one sql row used in sql insert statement
+    """
+    tb_row_s0 = row.tolist()
+    for i, c in enumerate(tb_row_s0):
+        if isinstance(c, str):
+            tb_row_s0[i] = '"' + str(c) + '"'
+        elif isinstance(c, (int, np.integer)):
+            tb_row_s0[i] = str(c)
+        elif isinstance(c, (float, np.float32)):
+            if math.isnan(c):
+                tb_row_s0[i] = "NULL"
+            else:
+                tb_row_s0[i] = str(c)[:10]
+        elif pd.isnull(c) or c is None:
+            tb_row_s0[i] = "NULL"
+        else:
+            tb_row_s0[i] = '"' + str(c) + '"'
+    tb_row_s1 = "(" + ",".join(tb_row_s0) + ")"
+    return tb_row_s1
+
+
+def insert_one_row(row, conn, db_table_name):
+    """Insert one row into hadoop table
+    Author:
+        Colin Li @ 2023-02
+    Args:
+        row (_type_): _description_
+        conn (_type_): _description_
+        db_table_name (_type_): _description_
+    """
+    with conn.cursor() as cursor:
+        t = (
+            f"""
+        INSERT INTO {db_table_name}
+        VALUES
+        """
+            + row
+        )
+        cursor.execute(t)
+
+
+def insert_rows_to_table(tasks_insert: list, conn, db_table_name, nrow_per_insert=20):
+    """Insert rows to hadoop table
+
+    Author:
+        Colin Li @ 2023-02
+
+    Args:
+        tasks_insert (list): list of strings which is the output from
+            function generate_sql_row
+        conn (impala.hiveserver2.HiveServer2Connection):
+            connetion to hive/impala
+        db_table_name (str): database and tablename joined by dot '.'
+        nrow_per_insert (int, optional): Number of rows per insert.
+            Defaults to 20.
+    """
+    tasks_size = len(tasks_insert)
+    print(f"Rows to insert: {tasks_size}")
+    n, rem = divmod(tasks_size, nrow_per_insert)
+    st = 0
+    tqdm._instances.clear()
+    if n > 0:
+        for i in tqdm(range(n)):
+            rows = tasks_insert[st : st + nrow_per_insert]
+            if len(rows) > 1:
+                insert_one_row(",".join(rows), conn, db_table_name)
+            else:
+                insert_one_row(rows[0], conn, db_table_name)
+            st += nrow_per_insert
+    if rem != 0:
+        rows = tasks_insert[st:tasks_size]
+        if len(rows) > 1:
+            insert_one_row(",".join(rows), conn, db_table_name)
+        else:
+            insert_one_row(rows[0], conn, db_table_name)
+
+
+def insert_df_to_table(df, conn, db_table_name, nrow_per_insert=20):
+    """Insert pandas dataframe rows into hadoop table
+    Author:
+        Colin Li @ 2024-05
+    Args:
+        df (pandas.DataFrame): pandas dataframe
+        conn (impala.hiveserver2.HiveServer2Connection):
+            connetion to hive/impala
+        db_table_name (str): database and tablename joined by dot '.'
+        nrow_per_insert (int, optional): Number of rows per insert.
+            Defaults to 20.
+    """
+    tasks_insert = df.apply(generate_sql_row, axis=1).tolist()
+    insert_rows_to_table(
+        tasks_insert,
+        conn=conn,
+        db_table_name=db_table_name,
+        nrow_per_insert=nrow_per_insert,
+    )
+
+
 if __name__ == "__main__":
     pass
```

## rubberduckie/cdsw/import_fix.py

```diff
@@ -1,85 +1,93 @@
 import re
 import sys
 import subprocess
+
 # Colin Li @ 202305
 # Constant Setup for Optuna
 PH = "<**>"
-ERROR_CODE_FILE_OPTUNA = "/home/cdsw/.local/lib/python<**>/site-packages/sqlalchemy/util/typing.py"
+ERROR_CODE_FILE_OPTUNA = (
+    "/home/cdsw/.local/lib/python<**>/site-packages/sqlalchemy/util/typing.py"
+)
 
-ERROR_CODE_TEXT_OPTUNA = \
-    """
+ERROR_CODE_TEXT_OPTUNA = """
 \s*from typing_extensions import \(
 \s*dataclass_transform as dataclass_transform,.*
 \s*\)
 """
-FIXED_CODE_TEXT_OPTUNA = \
-    """
+FIXED_CODE_TEXT_OPTUNA = """
 
     import sys
     import importlib.util
     spec = importlib.util.spec_from_file_location(
         "typing_extensions",
         "/home/cdsw/.local/lib/python<**>/site-packages/typing_extensions.py"
     )
     typing_extensions = importlib.util.module_from_spec(spec)
     sys.modules["typing_extensions"] = typing_extensions
     spec.loader.exec_module(typing_extensions)
     dataclass_transform = typing_extensions.dataclass_transform
     
 """
-M_READ_SUCC_OPTUNA = 'Source of error was found successfully!'
-M_READ_FAIL_OPTUNA = 'Source of error was not found.'
-M_FIND_SUCC_OPTUNA = 'Error code was found successfully!'
-M_FIND_FAIL_OPTUNA = 'Error code was not found.'
-M_FIX_SUCC_OPTUNA = 'Optuna import error was fixed successfully!'
-M_FIX_FAIL_OPTUNA = 'Optuna import error was not fixed.'
+M_READ_SUCC_OPTUNA = "Source of error was found successfully!"
+M_READ_FAIL_OPTUNA = "Source of error was not found."
+M_FIND_SUCC_OPTUNA = "Error code was found successfully!"
+M_FIND_FAIL_OPTUNA = "Error code was not found."
+M_FIX_SUCC_OPTUNA = "Optuna import error was fixed successfully!"
+M_FIX_FAIL_OPTUNA = "Optuna import error was not fixed."
 
 
 def fix_cdsw_import_error(package_name, py_version: str):
     """Fix known issues that arise when importing specific packages in CDSW
-    Colin Li @ 2023-06
+
+    Author:
+        Colin Li @ 2023-06
+
     Args:
         package_name (str): Name of the package (current only support optuna)
 
         py_version (str): Python version of environment with issue
     """
     # Check
     if sys.platform != "linux":
-        raise OSError('Please only run this function in CDSW (Linux)')
+        raise OSError("Please only run this function in CDSW (Linux)")
 
     # Setup
-    if package_name == 'optuna':
+    if package_name == "optuna":
         # Dependencies
-        install_1 = subprocess.run(['pip', 'install', '--upgrade', 'typing_extensions'],
-                                   capture_output=True, text=True)
+        install_1 = subprocess.run(
+            ["pip", "install", "--upgrade", "typing_extensions"],
+            capture_output=True,
+            text=True,
+        )
         if install_1.returncode:
-            raise IOError('Installation of typing_extensions is failed.')
+            raise IOError("Installation of typing_extensions is failed.")
         else:
-            print('Installation of typing_extensions is successful!')
+            print("Installation of typing_extensions is successful!")
 
         # Optuna
-        install_2 = subprocess.run(['pip', 'install', 'optuna'],
-                                   capture_output=True, text=True)
+        install_2 = subprocess.run(
+            ["pip", "install", "optuna"], capture_output=True, text=True
+        )
         if install_2.returncode:
-            raise IOError('Installation of optuna is failed.')
+            raise IOError("Installation of optuna is failed.")
         else:
-            print('Installation of optuna is successful!')
+            print("Installation of optuna is successful!")
 
         # Workaround
         fp = ERROR_CODE_FILE_OPTUNA.replace(PH, py_version)
         error = ERROR_CODE_TEXT_OPTUNA.replace(PH, py_version)
         replace = FIXED_CODE_TEXT_OPTUNA.replace(PH, py_version)
 
         try:
-            with open(fp, 'r') as file_in:
+            with open(fp, "r") as file_in:
                 script = file_in.read()
                 print(M_READ_SUCC_OPTUNA)
         except:
-            print(M_READ_FAIL_OPTUNA, '\n', M_FIX_FAIL_OPTUNA)
+            print(M_READ_FAIL_OPTUNA, "\n", M_FIX_FAIL_OPTUNA)
             return None
 
         # Workaround
         if re.search(error, script):
             print(M_FIND_SUCC_OPTUNA)
             try:
                 script_new = re.sub(error, replace, script)
```

## rubberduckie/da/pilot.py

```diff
@@ -11,15 +11,15 @@
 
     Returns:
         int: number of weeks in between
     """
     y_start, w_start = date_start.isocalendar()[:2]
     y_end, w_end = date_end.isocalendar()[:2]
     if y_end == y_start:
-        w = (w_end - w_start + 1)
+        w = w_end - w_start + 1
     elif y_end > y_start:
         w = (52 - w_start + 1) + (52 * (y_end - y_start - 1)) + w_end
     return w
 
 
 def prepare_dev_triangle(df, max_dev_period):
     """Prepare development triangle
@@ -30,47 +30,48 @@
         df (pandas.DataFrame): dataframe contains below colunms:
                                1. uid: unique identifer for each sample
                                2. week_1: week number
                                3. dev_period: development period number
         max_dev_period (int): max number of develop period for triangle
 
     Returns:
-        pandas.DataFrame: dataframe triangle 
+        pandas.DataFrame: dataframe triangle
     """
-    m_cols = len({'uid', 'week_1', 'dev_period'}.intersection(df.columns))
+    m_cols = len({"uid", "week_1", "dev_period"}.intersection(df.columns))
     w_text = "Columns 'uid', 'week_1', 'dev_period' must exist in input dataframe!"
     assert m_cols == 3, w_text
 
     # Generate pivot
-    df['y_pred'] = 1
+    df["y_pred"] = 1
     df_t = pd.pivot_table(
-        data=df, values='y_pred', columns='dev_period',
-        index='week_1', aggfunc='count')
+        data=df, values="y_pred", columns="dev_period", index="week_1", aggfunc="count"
+    )
     df_t.columns.name = None
 
     # Fill missing dev period column(s)
-    week_max = df['week_1'].max()
+    week_max = df["week_1"].max()
     cols_exp = set(range(1, max_dev_period + 1))
     cols_mis = cols_exp - set(df_t.columns)
-    print('Cols created for missing dev period:', cols_mis)
+    print("Cols created for missing dev period:", cols_mis)
     for c in cols_mis:
         df_t[c] = np.nan
     df_t = df_t[cols_exp].copy()
 
     # Fill mising week row(s)
     idx_mis = cols_exp - (set(df_t.index))
-    print('Rows created for missing week number:', idx_mis)
+    print("Rows created for missing week number:", idx_mis)
     for i in idx_mis:
         df_t.loc[i] = np.nan
     df_t = df_t.sort_index().copy()
 
     # Prepare triangle: fill the right cells with 0s
     for w in range(1, max_dev_period + 1):
-        df_t.loc[w, range(1, max_dev_period - w + 2)] = \
-            df_t.loc[w, range(1, max_dev_period - w + 2)].fillna(0)
+        df_t.loc[w, range(1, max_dev_period - w + 2)] = df_t.loc[
+            w, range(1, max_dev_period - w + 2)
+        ].fillna(0)
 
     # Prepare triangle: calculate cumulated sum
     df_t = df_t.cumsum(axis=1)
     df_t.reset_index()
 
     # return df triangle
     return df_t
```

## rubberduckie/plot/evaluation.py

```diff
@@ -1,45 +1,59 @@
 import numpy as np
 from sklearn.metrics import (
-    f1_score, precision_score,
-    recall_score, accuracy_score,
-    confusion_matrix)
+    f1_score,
+    precision_score,
+    recall_score,
+    accuracy_score,
+    confusion_matrix,
+)
 from matplotlib import pyplot as plt
 
-DEBUG = True
+DEBUG = False
 if DEBUG:
-    print('Evalution tools are loaded!')
+    print("Evalution tools are loaded!")
 
 
-def prepare_confusion_matrix(y, y_hat,
-                             model_name='', average='weighted',
-                             save_fig_to=None):
+def prepare_confusion_matrix(
+    y, y_hat, model_name="", average="weighted", save_fig_to=None
+):
     """Prepare confusion matrix for model evaluation
-    Colin Li @ 2023-05
+
+    Author:
+        Colin Li @ 2023-05
 
     Args:
         y (iterable): actual y
         y_hat (iterable): predicted y
         model_name (str, optional): Name of the model. Defaults to ''.
         average (str, optional): average method. Defaults to 'weighted'.
         save_fig_to (str, optional): file path for output. Defaults to None.
     """
     f1 = f1_score(y, y_hat, average=average)
     precision = precision_score(y, y_hat, average=average)
     recall = recall_score(y, y_hat, average=average)
     accuracy = accuracy_score(y, y_hat)
     cm = confusion_matrix(y_true=y, y_pred=y_hat)
-    eval_str = f'Model Evaluation Metrics:\nF1: {f1:.4f}\n' + \
-               f'Precision: {precision:.4f}\n' + \
-               f'Recall: {recall:.4f}\n' + \
-               f'Accuracy: {accuracy:.4f}'
+    eval_str = (
+        f"Model Evaluation Metrics:\nF1: {f1:.4f}\n"
+        + f"Precision: {precision:.4f}\n"
+        + f"Recall: {recall:.4f}\n"
+        + f"Accuracy: {accuracy:.4f}"
+    )
     fig1, axe1 = plt.subplots(figsize=(5, 5), dpi=100, nrows=1, ncols=1)
-    axe1.matshow(cm, aspect=1, cmap='Blues', alpha=0.8)
-    axe1.set_xlabel('Predicted')
-    axe1.set_ylabel('Actual')
-    axe1.set_title(f'Confusion Matrix\n{model_name}', fontsize=10)
+    axe1.matshow(cm, aspect=1, cmap="Blues", alpha=0.8)
+    axe1.set_xlabel("Predicted")
+    axe1.set_ylabel("Actual")
+    axe1.set_title(f"Confusion Matrix\n{model_name}", fontsize=10)
     for (i, j), z in np.ndenumerate(cm):
-        axe1.text(j, i, f'{z:,}', ha='center', va='center', weight='bold')
-    fig1.text(0.5, -0.05, eval_str, ha="center", va='center', fontsize=10,
-              bbox={"facecolor": "lightblue", "alpha": 0.75, "pad": 5})
+        axe1.text(j, i, f"{z:,}", ha="center", va="center", weight="bold")
+    fig1.text(
+        0.5,
+        -0.05,
+        eval_str,
+        ha="center",
+        va="center",
+        fontsize=10,
+        bbox={"facecolor": "lightblue", "alpha": 0.75, "pad": 5},
+    )
     if save_fig_to is not None:
-        fig1.savefig(save_fig_to, bbox_inches='tight')
+        fig1.savefig(save_fig_to, bbox_inches="tight")
```

## Comparing `rubberduckie-2023.7.1.dist-info/RECORD` & `rubberduckie-2024.5.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-rubberduckie/__init__.py,sha256=NOHg64NlglW-sWLjuS_r53NC_lL1F-KbmDMkBziPlxA,346
+rubberduckie/__init__.py,sha256=GzewzdTq6dqhsmCxA8uSjZW_C54yMfrH04NE0T09dxI,415
 rubberduckie/cdsw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie/cdsw/hadoop.py,sha256=upDJewzqbCDwCpB7SoUytxYUe143VQcEyleyha0CUEU,2956
-rubberduckie/cdsw/import_fix.py,sha256=vFb7-KpvfcqOzCJ9wTRm5EZmOgebWwlowZ4IafIaMME,3400
+rubberduckie/cdsw/hadoop.py,sha256=CIDWgXgIL2oeEzgsbpD2GScFctRWvx1D67BIK-yClPY,6384
+rubberduckie/cdsw/import_fix.py,sha256=eD_BqhYnteIoBEIjULA5JDJB0882-JAgKIyUDKfRAoE,3414
+rubberduckie/cdsw/misc.py,sha256=BmmkKa7hqAyDGNMZ5gIUIZuFJUeVYoYA06ifHBjNtYo,745
 rubberduckie/da/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie/da/pilot.py,sha256=Cs5S7_8d-6ZAtLc74NEdFAc49bmxGE_XlYHTqUnu498,2439
+rubberduckie/da/pilot.py,sha256=q7vnGn8kwY4hme0LPMMNdb62Eirb5AB-LdTeWrjzhIU,2441
 rubberduckie/dl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/plot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie/plot/evaluation.py,sha256=tzB_TrCYyMRaC0I-5RLJxPbjbPVtgByFTmZuWDmAma0,1835
+rubberduckie/plot/evaluation.py,sha256=DrjoYTpfuKokaS6dRMHAxKMAZYuqDD0hACYk53Gwwuc,1849
 rubberduckie/xai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie-2023.7.1.dist-info/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie-2023.7.1.dist-info/METADATA,sha256=biXi6-pTpgxgzxqfXgyZzbVrbOH0W7g-FP28k-CdGXs,420
-rubberduckie-2023.7.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rubberduckie-2023.7.1.dist-info/top_level.txt,sha256=10EHDBDRla6FQ9v_RwhUA08sGKU1P499ZlDoj2XQXqc,13
-rubberduckie-2023.7.1.dist-info/RECORD,,
+rubberduckie-2024.5.1.dist-info/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+rubberduckie-2024.5.1.dist-info/METADATA,sha256=xwUqSzlOc_qiPdd2J9G_dQ3LWjhyzYJQwJDLEjBs13s,929
+rubberduckie-2024.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+rubberduckie-2024.5.1.dist-info/top_level.txt,sha256=10EHDBDRla6FQ9v_RwhUA08sGKU1P499ZlDoj2XQXqc,13
+rubberduckie-2024.5.1.dist-info/RECORD,,
```

