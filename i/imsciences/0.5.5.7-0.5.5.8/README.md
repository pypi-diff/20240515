# Comparing `tmp/imsciences-0.5.5.7.tar.gz` & `tmp/imsciences-0.5.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.7.tar", last modified: Wed May 15 12:02:56 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.8.tar", last modified: Wed May 15 12:37:19 2024, max compression
```

## Comparing `imsciences-0.5.5.7.tar` & `imsciences-0.5.5.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:02:56.524470 imsciences-0.5.5.7/
--rw-rw-rw-   0        0        0     8987 2024-05-15 12:02:56.520838 imsciences-0.5.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     8482 2024-05-15 12:02:45.000000 imsciences-0.5.5.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 12:02:56.494214 imsciences-0.5.5.7/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.7/imsciences/__init__.py
--rw-rw-rw-   0        0        0    55606 2024-05-15 12:02:43.000000 imsciences-0.5.5.7/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:02:56.514932 imsciences-0.5.5.7/imsciences.egg-info/
--rw-rw-rw-   0        0        0     8987 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 12:02:56.525752 imsciences-0.5.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-15 12:02:47.000000 imsciences-0.5.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:37:19.383883 imsciences-0.5.5.8/
+-rw-rw-rw-   0        0        0     8987 2024-05-15 12:37:19.376882 imsciences-0.5.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8482 2024-05-15 12:04:13.000000 imsciences-0.5.5.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 12:37:19.334594 imsciences-0.5.5.8/imsciences/
+-rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.8/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    55632 2024-05-15 12:36:55.000000 imsciences-0.5.5.8/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:37:19.373884 imsciences-0.5.5.8/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     8987 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 12:37:19.383883 imsciences-0.5.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-15 12:37:07.000000 imsciences-0.5.5.8/setup.py
```

### Comparing `imsciences-0.5.5.7/PKG-INFO` & `imsciences-0.5.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.7
+Version: 0.5.5.8
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.5.7/README.md` & `imsciences-0.5.5.8/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.5.7/imsciences/datafunctions.py` & `imsciences-0.5.5.8/imsciences/datafunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import plotly.express as px
 import plotly.graph_objs as go
 from dateutil.parser import parse
 import numpy as np
 from datetime import datetime
 import datetime
+import re
 from datetime import datetime, timedelta
 
 class dataprocessing:
     
     def help(self):
         print("This is the help section. The functions in the package are as follows:")
 
@@ -640,34 +641,34 @@
         to_find_dict (dict): your look up table, where keys are the values being looked up, and the values are the resulting mappings. 
         if_not_in_dict (str, optional): default value if no substring matches are found in the look up table dictionary. Defaults to "Other".
         new_column_name (str, optional): name of new column. Defaults to "Mapping".
 
         Returns:
         pandas.DataFrame: DataFrame with a new column containing the look up table results.
         """
-        
-        # Function to find word in string
-        def find_word_in_string(x_string, to_find_dict=to_find_dict, default_value=if_not_in_dict):
-            x_string_lower = x_string.lower()
-            for key, value in to_find_dict.items():
-                if key.lower() in x_string_lower:
-                    return value
-            return default_value
+
+        # Create regex pattern from the dictionary keys
+        regex_pattern = "|".join(re.escape(key) for key in to_find_dict.keys())
         
         # Preprocess DataFrame if multiple columns
         if len(col_names) > 1:
             df["Merged"] = df[col_names].astype(str).apply('|'.join, axis=1)
-            col_names = "Merged"
+            col_to_use = "Merged"
+        else:
+            col_to_use = col_names[0]
 
-        # Apply the inner function to the specified column and create a new column with the results
-        df[new_column_name] = df[col_names].apply(find_word_in_string)
+        # Extract the first match using the regex pattern
+        matches = df[col_to_use].str.extract(f'({regex_pattern})', expand=False, flags=re.IGNORECASE)
         
-        # # Drop intermediate column if created
-        # if len(col_names) > 1:
-        #     df.drop(columns=["Merged"], inplace=True)
+        # Map the matches to the corresponding values in the dictionary
+        df[new_column_name] = matches.str.lower().map({k.lower(): v for k, v in to_find_dict.items()}).fillna(if_not_in_dict)
+        
+        # Drop intermediate column if created
+        if len(col_names) > 1:
+            df.drop(columns=["Merged"], inplace=True)
 
         return df
 
     def aggregate_daily_to_wc_wide(self, df : pd.DataFrame, date_column : str, group_columns : list[str], sum_columns : list[str], wc : str = 'sun', aggregation : str = 'sum', include_totals : bool = False) -> pd.DataFrame:
         """
         Aggregates daily data into weekly data, starting on a specified day of the week, 
         and groups the data by additional specified columns. It aggregates specified numeric columns
```

### Comparing `imsciences-0.5.5.7/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.5.8/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.7
+Version: 0.5.5.8
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.5.7/setup.py` & `imsciences-0.5.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.7'
+VERSION = '0.5.5.8'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

