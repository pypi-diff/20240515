# Comparing `tmp/sqldatamodel-0.6.1.tar.gz` & `tmp/sqldatamodel-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldatamodel-0.6.1.tar", last modified: Tue May 14 20:30:50 2024, max compression
+gzip compressed data, was "sqldatamodel-0.6.2.tar", last modified: Wed May 15 16:57:57 2024, max compression
```

## Comparing `sqldatamodel-0.6.1.tar` & `sqldatamodel-0.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 20:30:50.383577 sqldatamodel-0.6.1/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.6.1/LICENSE
--rw-rw-rw-   0        0        0    29574 2024-05-14 20:30:50.373577 sqldatamodel-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    27682 2024-05-13 19:59:36.000000 sqldatamodel-0.6.1/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 20:30:50.385251 sqldatamodel-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     2424 2024-05-14 20:13:33.000000 sqldatamodel-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:30:48.845023 sqldatamodel-0.6.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 20:30:50.062310 sqldatamodel-0.6.1/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.6.1/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.6.1/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.6.1/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   627858 2024-05-14 20:28:25.000000 sqldatamodel-0.6.1/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.6.1/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.6.1/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.6.1/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.6.1/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2820 2024-05-14 15:14:12.000000 sqldatamodel-0.6.1/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:30:50.275714 sqldatamodel-0.6.1/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.6.1/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.6.1/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-05-14 20:30:50.365350 sqldatamodel-0.6.1/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    29574 2024-05-14 20:30:48.000000 sqldatamodel-0.6.1/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-05-14 20:30:48.000000 sqldatamodel-0.6.1/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:30:48.000000 sqldatamodel-0.6.1/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-14 20:30:48.000000 sqldatamodel-0.6.1/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 20:30:50.296379 sqldatamodel-0.6.1/tests/
--rw-rw-rw-   0        0        0    69579 2024-05-14 19:12:35.000000 sqldatamodel-0.6.1/tests/test_Future.py
--rw-rw-rw-   0        0        0    69582 2024-05-14 19:12:37.000000 sqldatamodel-0.6.1/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:57:57.489242 sqldatamodel-0.6.2/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0    29574 2024-05-15 16:57:57.480216 sqldatamodel-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0    27682 2024-05-15 14:21:26.000000 sqldatamodel-0.6.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:57:57.490241 sqldatamodel-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     2424 2024-05-15 16:55:55.000000 sqldatamodel-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:57:56.033851 sqldatamodel-0.6.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 16:57:57.228846 sqldatamodel-0.6.2/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.6.2/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.6.2/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.6.2/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   628498 2024-05-15 16:49:40.000000 sqldatamodel-0.6.2/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.6.2/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.6.2/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.6.2/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.6.2/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2820 2024-05-14 15:14:12.000000 sqldatamodel-0.6.2/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:57:57.397839 sqldatamodel-0.6.2/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.6.2/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.6.2/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-05-15 16:57:57.472565 sqldatamodel-0.6.2/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    29574 2024-05-15 16:57:55.000000 sqldatamodel-0.6.2/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-05-15 16:57:56.000000 sqldatamodel-0.6.2/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:57:55.000000 sqldatamodel-0.6.2/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-15 16:57:55.000000 sqldatamodel-0.6.2/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 16:57:57.416083 sqldatamodel-0.6.2/tests/
+-rw-rw-rw-   0        0        0    72895 2024-05-15 15:10:10.000000 sqldatamodel-0.6.2/tests/test_Future.py
+-rw-rw-rw-   0        0        0    72898 2024-05-15 15:10:24.000000 sqldatamodel-0.6.2/tests/test_SQLDataModel.py
```

### Comparing `sqldatamodel-0.6.1/LICENSE` & `sqldatamodel-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/PKG-INFO` & `sqldatamodel-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.6.1
+Version: 0.6.2
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
@@ -339,22 +339,22 @@
 num_epochs = 10
 for epoch in range(num_epochs):
     # Train the model and get the metrics
     train_loss, train_acc = train(model, criterion, optimizer, train_loader, device)
     val_loss, val_acc = validate(model, criterion, val_loader, device)
 
     # Let's store the results first
-    sdm.insert_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
+    sdm.append_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
 
     # Print training results to terminal
     print(f'Epoch [{epoch+1}/{num_epochs}], '
           f'Train Loss: {train_loss:.4f}, Train Acc: {train_acc:.2f}%, '
           f'Val Loss: {val_loss:.4f}, Val Acc: {val_acc:.2f}%')
 ```
-We use the `insert_row()` method to store the results from training, inserting a new row for each epoch. Now that we're storing the data instead of just printing it to the terminal, we can track our results and easily export them into whichever format we need. For this example, let's store them as a `.json` file. All we need is to add one more line at the end of our training loop:
+We use the `append_row()` method to store the results from training, inserting a new row for each epoch. Now that we're storing the data instead of just printing it to the terminal, we can track our results and easily export them into whichever format we need. For this example, let's store them as a `.json` file. All we need is to add one more line at the end of our training loop:
 
 ```python
 # ... Training loop ...
 sdm.to_json('Training-Metrics.json')
 ```
 This will export all the training data stored in our model to a new JSON file `Training-Metrics.json`, trimmed for brevity:
 
@@ -393,15 +393,15 @@
 num_epochs = 10
 for epoch in range(num_epochs):
     # Train the model and get the metrics
     train_loss, train_acc = train(model, criterion, optimizer, train_loader, device)
     val_loss, val_acc = validate(model, criterion, val_loader, device)
 
     # Let's store the results first
-    sdm.insert_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
+    sdm.append_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
 
     # Pretty print last row of training results to terminal
     print(sdm[-1])
 
 # Print all results when training finishes
 print(sdm)
```

### Comparing `sqldatamodel-0.6.1/README.md` & `sqldatamodel-0.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -314,22 +314,22 @@
 num_epochs = 10
 for epoch in range(num_epochs):
     # Train the model and get the metrics
     train_loss, train_acc = train(model, criterion, optimizer, train_loader, device)
     val_loss, val_acc = validate(model, criterion, val_loader, device)
 
     # Let's store the results first
-    sdm.insert_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
+    sdm.append_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
 
     # Print training results to terminal
     print(f'Epoch [{epoch+1}/{num_epochs}], '
           f'Train Loss: {train_loss:.4f}, Train Acc: {train_acc:.2f}%, '
           f'Val Loss: {val_loss:.4f}, Val Acc: {val_acc:.2f}%')
 ```
-We use the `insert_row()` method to store the results from training, inserting a new row for each epoch. Now that we're storing the data instead of just printing it to the terminal, we can track our results and easily export them into whichever format we need. For this example, let's store them as a `.json` file. All we need is to add one more line at the end of our training loop:
+We use the `append_row()` method to store the results from training, inserting a new row for each epoch. Now that we're storing the data instead of just printing it to the terminal, we can track our results and easily export them into whichever format we need. For this example, let's store them as a `.json` file. All we need is to add one more line at the end of our training loop:
 
 ```python
 # ... Training loop ...
 sdm.to_json('Training-Metrics.json')
 ```
 This will export all the training data stored in our model to a new JSON file `Training-Metrics.json`, trimmed for brevity:
 
@@ -368,15 +368,15 @@
 num_epochs = 10
 for epoch in range(num_epochs):
     # Train the model and get the metrics
     train_loss, train_acc = train(model, criterion, optimizer, train_loader, device)
     val_loss, val_acc = validate(model, criterion, val_loader, device)
 
     # Let's store the results first
-    sdm.insert_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
+    sdm.append_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
 
     # Pretty print last row of training results to terminal
     print(sdm[-1])
 
 # Print all results when training finishes
 print(sdm)
```

### Comparing `sqldatamodel-0.6.1/setup.py` & `sqldatamodel-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.6.1',
+     version='0.6.2',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords=['SQL','ETL','dataframe','terminal-tables','pretty-print-tables','sql2sql','data-analysis','data-science','datamodel','extract','transform','load','web-scraping-tables','data-mining','html','html-table-parsing','apache-arrow','pyarrow','pyarrow-conversion','pyarrow-to-table','pyarrow-to-sql','pyarrow-to-csv','parquet-file-parsing','csv','csv-parsing','markdown','markdown-table-parsing','latex','latex-table-parsing','delimited','delimited-data-parsing','file-conversion','format-conversion','terminal-styling','table-styling','from-sqlite','to-sqlite','from-postgresql','to-postgresql','sql-to-sql','excel','xlsx-file','excel-to-sql','DataFrames','polars2pandas','pandas2polars'],
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/ANSIColor.py` & `sqldatamodel-0.6.2/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/HTMLParser.py` & `sqldatamodel-0.6.2/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/JSONEncoder.py` & `sqldatamodel-0.6.2/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/SQLDataModel.py` & `sqldatamodel-0.6.2/src/SQLDataModel/SQLDataModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -10566,45 +10566,54 @@
         Example::
         
             from SQLDataModel import SQLDataModel
 
             # Create the model
             sdm = SQLDataModel.from_csv('example.csv', headers=['Column1', 'Column2'])
 
-            # Create the fetch query to use
+            # Create the SQL query to execute
             query = 'SELECT * FROM sdm WHERE Column1 > 10'
 
             # Fetch and save the result to a new instance
             result_model = sdm.execute_fetch(query)
 
+            # Create a parameterized SQL query to execute
+            query = 'SELECT * FROM sdm WHERE Column1 > ? OR Column2 < ?'
+            params = (10, 20)
+
+            # Provide the SQL and the statement parameters
+            result_parameterized = sdm.execute_fetch(query, params)
+
         Important:
-            - The default table name is ``'sdm'``, or you can use :meth:`SQLDataModel.get_model_name()` to view the current model alias.
-            - This function is the primary method used by ``SQLDataModel`` methods that are expected to return a new instance.
+            - The default table name is ``'sdm'``, you can use :meth:`SQLDataModel.set_model_name()` to modify the name used by ``SQLDataModel``.
+        
+        Change Log:
+            - Version 0.6.2 (2024-05-15):
+                - Inclusion of :py:attr:`SQLDataModel.table_style` argument in returned ``SQLDataModel`` to inherit all display properties in result.
 
         Note:
+            - Use :meth:`SQLDataModel.set_model_name()` to modify the table name used by the model, default name set as ``'sdm'``.
             - Display properties such as float precision, index column or table styling are also passed to the new instance when not provided in ``kwargs``.
         """
         try:
             res = self.sql_db_conn.execute(sql_query) if sql_params is None else self.sql_db_conn.execute(sql_query, sql_params) 
         except Exception as e:
             raise SQLProgrammingError(
                 SQLDataModel.ErrorFormat(f'SQLProgrammingError: invalid or malformed SQL, provided query failed with error "{e}"')
             ) from None
         fetch_result = res.fetchall()
         fetch_headers = [x[0] for x in res.description]
         if (rows_returned := len(fetch_result)) < 1:
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: nothing to return, provided query returned '{rows_returned}' rows which is insufficient to return or generate a new model from")
             )
-        if not kwargs:
-            return type(self)(fetch_result, headers=fetch_headers, dtypes=self.dtypes, display_max_rows=self.display_max_rows, min_column_width=self.min_column_width, max_column_width=self.max_column_width, column_alignment=self.column_alignment, display_color=self.display_color, display_index=self.display_index, display_float_precision=self.display_float_precision)
-        else:
-            params = {"dtypes":self.dtypes,"display_max_rows":self.display_max_rows, "min_column_width":self.min_column_width, "max_column_width":self.max_column_width, "column_alignment":self.column_alignment, "display_color":self.display_color, "display_index":self.display_index, "display_float_precision":self.display_float_precision}
-            params.update({k:v for k,v in kwargs.items()})
-            return type(self)(fetch_result, headers=fetch_headers, **params)
+        sdm_args = self._get_display_args(include_dtypes=True)
+        if kwargs:
+            sdm_args.update({k:v for k,v in kwargs.items()})
+        return type(self)(fetch_result, headers=fetch_headers, **sdm_args)
 
     def execute_statement(self, sql_stmt:str) -> None:
         """
         Executes an arbitrary SQL query against the current model without the expectation of selection or returned rows.
 
         Parameters:
             ``sql_stmt`` (str): The SQL query to execute.
@@ -11477,32 +11486,45 @@
 
         ```shell
             CREATE TABLE "sdm" ("idx" INTEGER PRIMARY KEY,"first" TEXT,"last" TEXT,"age" INTEGER)
         ```
         """
         return self.sql_db_conn.execute("select sql from sqlite_master").fetchone()[0]
 
-    def _get_display_args(self) -> dict:
+    def _get_display_args(self, include_dtypes:bool=False) -> dict:
         """
         Retrieves the current display configuration settings of the ``SQLDataModel`` with the correct ``kwargs`` for the class :meth:`SQLDataModel.__init__()` method.
 
+        Parameters:
+            ``include_dtypes`` (bool, optional): Whether :py:attr:`SQLDataModel.dtypes` should be included in the result. Default is False, including only display arguments.
+
         Returns:
             ``dict``: A dictionary containing the display configuration settings in the format ``{'setting': 'value'}``.
 
         Display Properties:
             - :py:attr:`SQLDataModel.display_max_rows`: The maximum number of rows to display.
             - :py:attr:`SQLDataModel.min_column_width`: The minimum width of columns when displaying the model.
             - :py:attr:`SQLDataModel.max_column_width`: The maximum width of columns when displaying the model.
             - :py:attr:`SQLDataModel.column_alignment`: The alignment of columns ('left', 'center', 'right' or 'dynamic').
             - :py:attr:`SQLDataModel.display_color`: The color to use when displaying the table, None by default.
             - :py:attr:`SQLDataModel.display_index`: True if displaying index column, False otherwise.
             - :py:attr:`SQLDataModel.display_float_precision`: The precision for displaying floating-point numbers.
             - :py:attr:`SQLDataModel.table_style`: The table styling format to use for strng representations of the model.
-        """        
-        return {"display_max_rows":self.display_max_rows, "min_column_width":self.min_column_width, "max_column_width":self.max_column_width, "column_alignment":self.column_alignment, "display_color":self.display_color, "display_index":self.display_index, "display_float_precision":self.display_float_precision, "table_style":self.table_style}
+        
+        Dtype Property:
+            - :py:attr:`SQLDataModel.dtypes`: A dictionary mapping the current model's columns to their corresponding Python data type.
+        
+        Change Log:
+            - Version 0.6.2 (2024-05-15):
+                - Added ``include_dtypes`` parameter for use by methods such as :meth:`SQLDataModel.min()` and :meth:`SQLDataModel.max()` for operations that require returning the results of SQL fetch statements.
+        """
+        args = {"display_max_rows":self.display_max_rows, "min_column_width":self.min_column_width, "max_column_width":self.max_column_width, "column_alignment":self.column_alignment, "display_color":self.display_color, "display_index":self.display_index, "display_float_precision":self.display_float_precision, "table_style":self.table_style}
+        if include_dtypes:
+            args['dtypes'] = self.dtypes
+        return args
 
     def validate_indicies(self, indicies) -> tuple[int|slice, list[str]]:
         """
         Validates and returns a predictable notation form of indices for accessing rows and columns in the ``SQLDataModel`` from varying indexing input types.
 
         Row indexing:
               - int: Single row index.
```

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/StandardDeviation.py` & `sqldatamodel-0.6.2/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/converters.py` & `sqldatamodel-0.6.2/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/demo.py` & `sqldatamodel-0.6.2/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/exceptions.py` & `sqldatamodel-0.6.2/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel/extensions/str_utils.c` & `sqldatamodel-0.6.2/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel.egg-info/PKG-INFO` & `sqldatamodel-0.6.2/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.6.1
+Version: 0.6.2
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
@@ -339,22 +339,22 @@
 num_epochs = 10
 for epoch in range(num_epochs):
     # Train the model and get the metrics
     train_loss, train_acc = train(model, criterion, optimizer, train_loader, device)
     val_loss, val_acc = validate(model, criterion, val_loader, device)
 
     # Let's store the results first
-    sdm.insert_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
+    sdm.append_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
 
     # Print training results to terminal
     print(f'Epoch [{epoch+1}/{num_epochs}], '
           f'Train Loss: {train_loss:.4f}, Train Acc: {train_acc:.2f}%, '
           f'Val Loss: {val_loss:.4f}, Val Acc: {val_acc:.2f}%')
 ```
-We use the `insert_row()` method to store the results from training, inserting a new row for each epoch. Now that we're storing the data instead of just printing it to the terminal, we can track our results and easily export them into whichever format we need. For this example, let's store them as a `.json` file. All we need is to add one more line at the end of our training loop:
+We use the `append_row()` method to store the results from training, inserting a new row for each epoch. Now that we're storing the data instead of just printing it to the terminal, we can track our results and easily export them into whichever format we need. For this example, let's store them as a `.json` file. All we need is to add one more line at the end of our training loop:
 
 ```python
 # ... Training loop ...
 sdm.to_json('Training-Metrics.json')
 ```
 This will export all the training data stored in our model to a new JSON file `Training-Metrics.json`, trimmed for brevity:
 
@@ -393,15 +393,15 @@
 num_epochs = 10
 for epoch in range(num_epochs):
     # Train the model and get the metrics
     train_loss, train_acc = train(model, criterion, optimizer, train_loader, device)
     val_loss, val_acc = validate(model, criterion, val_loader, device)
 
     # Let's store the results first
-    sdm.insert_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
+    sdm.append_row([epoch+1, train_loss, train_acc, val_loss, val_acc])
 
     # Pretty print last row of training results to terminal
     print(sdm[-1])
 
 # Print all results when training finishes
 print(sdm)
```

### Comparing `sqldatamodel-0.6.1/src/SQLDataModel.egg-info/SOURCES.txt` & `sqldatamodel-0.6.2/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.6.1/tests/test_Future.py` & `sqldatamodel-0.6.2/tests/test_Future.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,80 @@
                 num_checked += 1
             else:
                 assert s_val == f"{x},{y}"
                 num_checked += 1
     assert num_checked == (sdm.row_count * sdm.column_count)
 
 @pytest.mark.core
+def test_setitem_triggers():
+    """Tests append row triggers for setitem and index value vs position sync for row and column indexing."""
+    grid_size = 10 # creates grid_size as (grid_size x grid_size)
+    sdm = SQLDataModel([["F" for _ in range(grid_size)] for _ in range(grid_size)]) # create the grid canvas
+    # create a series of random indicies within grid bounds
+    for i in range(grid_size):
+        # random.seed(i) # set seed to avoid duplication
+        rand_x, rand_y = random.randint(0, grid_size - 1), random.randint(0, grid_size - 1)
+        input_cell = f"({rand_x}, {rand_y})"
+        sdm[rand_x, rand_y] = input_cell
+        output_cell = sdm[rand_x, rand_y].data()
+        assert output_cell == input_cell
+    # test append row trigger within bounds
+    input_row = tuple([f's({grid_size}, {j})' for j in range(grid_size)])
+    sdm[grid_size] = input_row
+    output_row = sdm[-1].data(index=True)
+    expected_row = tuple([grid_size, *input_row])
+    assert output_row == expected_row
+    expected_shape = (grid_size+1,grid_size)
+    output_shape = sdm.shape
+    assert output_shape == expected_shape
+    # create a series of random indicies without index position & value sync
+    canvas = 30
+    subset_grid = 10
+    sdm = SQLDataModel([["F" for _ in range(canvas)] for _ in range(canvas)]) # create the grid canvas
+    sdm = sdm[(canvas-subset_grid):canvas,(canvas-subset_grid):canvas]
+    for i in range(subset_grid):
+        # random.seed(i) # set seed to avoid duplication
+        rand_x, rand_y = random.randint(0, subset_grid - 1), random.randint(0, subset_grid - 1)
+        input_cell = f"({rand_x}, {rand_y})"
+        sdm[rand_x, rand_y] = input_cell
+        output_cell = sdm[rand_x, rand_y].data()
+        assert output_cell == input_cell
+    # test append row trigger outside of original canvas bounds
+    input_row = tuple([f's({canvas}, {j})' for j in range((canvas-subset_grid),canvas)])
+    sdm[canvas-(canvas-subset_grid)] = input_row
+    output_row = sdm[-1].data(index=True)
+    expected_row = tuple([canvas, *input_row])
+    assert output_row == expected_row
+    expected_shape = (canvas-(canvas-subset_grid)+1,canvas-(canvas-subset_grid))
+    output_shape = sdm.shape
+    assert output_shape == expected_shape
+
+@pytest.mark.core
+def test_init_empty(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]  
+    input_dtypes = {'string': 'str', 'int': 'int', 'float': 'float', 'bool': 'int', 'date': 'date', 'bytes': 'bytes', 'nonetype': 'str', 'datetime': 'datetime'}
+    # init from dtypes only
+    sdm = SQLDataModel(dtypes=input_dtypes)
+    for rid, row in enumerate(input_data):
+        sdm[rid] = row
+    output_data = sdm.data(strict_2d=True)
+    assert output_data == input_data
+    output_dtypes = sdm.dtypes
+    assert output_dtypes == input_dtypes
+    # init from headers only
+    sdm = SQLDataModel(headers=input_headers)
+    input_data = [tuple([f"({i},{j})" for j in range(len(input_headers))]) for i in range(len(input_data))]
+    for rid, row in enumerate(input_data):
+        sdm[rid] = row
+    output_data = sdm.data(strict_2d=True)
+    assert output_data == input_data
+    output_headers = sdm.headers
+    assert output_headers == input_headers
+
+@pytest.mark.core
 def test_addition():
     data = [(f"{i}", i, i*1.0) for i in range(1,11)]
     expected_output = [(f"{row[0]}x", row[1]+1, row[2]+0.1, row[1]+1 + row[2]+0.1) for row in data]
     headers = ['str', 'int', 'float']
     sdm = SQLDataModel(data, headers, display_index=False)
     sdm['str concat'] = sdm['str'] + 'x'
     sdm['int scalar'] = sdm['int'] + 1
```

### Comparing `sqldatamodel-0.6.1/tests/test_SQLDataModel.py` & `sqldatamodel-0.6.2/tests/test_SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,80 @@
                 num_checked += 1
             else:
                 assert s_val == f"{x},{y}"
                 num_checked += 1
     assert num_checked == (sdm.row_count * sdm.column_count)
 
 @pytest.mark.core
+def test_setitem_triggers():
+    """Tests append row triggers for setitem and index value vs position sync for row and column indexing."""
+    grid_size = 10 # creates grid_size as (grid_size x grid_size)
+    sdm = SQLDataModel([["F" for _ in range(grid_size)] for _ in range(grid_size)]) # create the grid canvas
+    # create a series of random indicies within grid bounds
+    for i in range(grid_size):
+        # random.seed(i) # set seed to avoid duplication
+        rand_x, rand_y = random.randint(0, grid_size - 1), random.randint(0, grid_size - 1)
+        input_cell = f"({rand_x}, {rand_y})"
+        sdm[rand_x, rand_y] = input_cell
+        output_cell = sdm[rand_x, rand_y].data()
+        assert output_cell == input_cell
+    # test append row trigger within bounds
+    input_row = tuple([f's({grid_size}, {j})' for j in range(grid_size)])
+    sdm[grid_size] = input_row
+    output_row = sdm[-1].data(index=True)
+    expected_row = tuple([grid_size, *input_row])
+    assert output_row == expected_row
+    expected_shape = (grid_size+1,grid_size)
+    output_shape = sdm.shape
+    assert output_shape == expected_shape
+    # create a series of random indicies without index position & value sync
+    canvas = 30
+    subset_grid = 10
+    sdm = SQLDataModel([["F" for _ in range(canvas)] for _ in range(canvas)]) # create the grid canvas
+    sdm = sdm[(canvas-subset_grid):canvas,(canvas-subset_grid):canvas]
+    for i in range(subset_grid):
+        # random.seed(i) # set seed to avoid duplication
+        rand_x, rand_y = random.randint(0, subset_grid - 1), random.randint(0, subset_grid - 1)
+        input_cell = f"({rand_x}, {rand_y})"
+        sdm[rand_x, rand_y] = input_cell
+        output_cell = sdm[rand_x, rand_y].data()
+        assert output_cell == input_cell
+    # test append row trigger outside of original canvas bounds
+    input_row = tuple([f's({canvas}, {j})' for j in range((canvas-subset_grid),canvas)])
+    sdm[canvas-(canvas-subset_grid)] = input_row
+    output_row = sdm[-1].data(index=True)
+    expected_row = tuple([canvas, *input_row])
+    assert output_row == expected_row
+    expected_shape = (canvas-(canvas-subset_grid)+1,canvas-(canvas-subset_grid))
+    output_shape = sdm.shape
+    assert output_shape == expected_shape
+
+@pytest.mark.core
+def test_init_empty(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]  
+    input_dtypes = {'string': 'str', 'int': 'int', 'float': 'float', 'bool': 'int', 'date': 'date', 'bytes': 'bytes', 'nonetype': 'str', 'datetime': 'datetime'}
+    # init from dtypes only
+    sdm = SQLDataModel(dtypes=input_dtypes)
+    for rid, row in enumerate(input_data):
+        sdm[rid] = row
+    output_data = sdm.data(strict_2d=True)
+    assert output_data == input_data
+    output_dtypes = sdm.dtypes
+    assert output_dtypes == input_dtypes
+    # init from headers only
+    sdm = SQLDataModel(headers=input_headers)
+    input_data = [tuple([f"({i},{j})" for j in range(len(input_headers))]) for i in range(len(input_data))]
+    for rid, row in enumerate(input_data):
+        sdm[rid] = row
+    output_data = sdm.data(strict_2d=True)
+    assert output_data == input_data
+    output_headers = sdm.headers
+    assert output_headers == input_headers
+
+@pytest.mark.core
 def test_addition():
     data = [(f"{i}", i, i*1.0) for i in range(1,11)]
     expected_output = [(f"{row[0]}x", row[1]+1, row[2]+0.1, row[1]+1 + row[2]+0.1) for row in data]
     headers = ['str', 'int', 'float']
     sdm = SQLDataModel(data, headers, display_index=False)
     sdm['str concat'] = sdm['str'] + 'x'
     sdm['int scalar'] = sdm['int'] + 1
```

