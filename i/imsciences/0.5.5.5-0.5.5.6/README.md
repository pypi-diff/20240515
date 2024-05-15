# Comparing `tmp/imsciences-0.5.5.5.tar.gz` & `tmp/imsciences-0.5.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.5.tar", last modified: Wed May 15 09:16:40 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.6.tar", last modified: Wed May 15 10:13:59 2024, max compression
```

## Comparing `imsciences-0.5.5.5.tar` & `imsciences-0.5.5.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:16:40.189691 imsciences-0.5.5.5/
--rw-rw-rw-   0        0        0     8855 2024-05-15 09:16:40.182204 imsciences-0.5.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     8350 2024-05-14 14:45:39.000000 imsciences-0.5.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 09:16:40.158360 imsciences-0.5.5.5/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.5/imsciences/__init__.py
--rw-rw-rw-   0        0        0    54723 2024-05-15 09:12:25.000000 imsciences-0.5.5.5/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:16:40.182204 imsciences-0.5.5.5/imsciences.egg-info/
--rw-rw-rw-   0        0        0     8855 2024-05-15 09:16:39.000000 imsciences-0.5.5.5/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-15 09:16:40.000000 imsciences-0.5.5.5/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:16:39.000000 imsciences-0.5.5.5/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 09:16:39.000000 imsciences-0.5.5.5/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 09:16:39.000000 imsciences-0.5.5.5/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 09:16:40.189691 imsciences-0.5.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-15 09:15:45.000000 imsciences-0.5.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:13:59.494105 imsciences-0.5.5.6/
+-rw-rw-rw-   0        0        0     9190 2024-05-15 10:13:59.489136 imsciences-0.5.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8685 2024-05-15 10:13:51.000000 imsciences-0.5.5.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 10:13:59.457053 imsciences-0.5.5.6/imsciences/
+-rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.6/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    56232 2024-05-15 10:13:49.000000 imsciences-0.5.5.6/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:13:59.485589 imsciences-0.5.5.6/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9190 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 10:13:59.494105 imsciences-0.5.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-15 10:13:52.000000 imsciences-0.5.5.6/setup.py
```

### Comparing `imsciences-0.5.5.5/PKG-INFO` & `imsciences-0.5.5.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.5
+Version: 0.5.5.6
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -120,7 +120,11 @@
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
+
+### 28. `create_var_names(df,col_names_to_combine,seperator='_',combined_col_name='Variable_Column_Name')`
+- **Description**: Combines dataframe columns containing strings to create a new column containing a variable name.
+- **Usage**: `create_var_names(df,['Media','Metric'],seperator='.',combined_col_name='New Variable Name')`
```

### Comparing `imsciences-0.5.5.5/README.md` & `imsciences-0.5.5.6/imsciences.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: imsciences
+Version: 0.5.5.6
+Summary: IMS Data Processing Package
+Author: IMS
+Author-email: cam@im-sciences.com
+Keywords: python,data processing
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
 # IMS Package Documentation
 
 The IMS package is a python library for processing incoming data into a format that can be used for projects. IMS processing offers a variety of functions to manipulate and analyze data efficiently. Here are the functionalities provided by the package:
 
 ### 1. `get_wd_levels(levels)`
 - **Description**: Get the working directory with the option of moving up parents.
 - **Usage**: `get_wd_levels(levels)`
@@ -104,8 +119,12 @@
 
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
-- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
+- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
+
+### 28. `create_var_names(df,col_names_to_combine,seperator='_',combined_col_name='Variable_Column_Name')`
+- **Description**: Combines dataframe columns containing strings to create a new column containing a variable name.
+- **Usage**: `create_var_names(df,['Media','Metric'],seperator='.',combined_col_name='New Variable Name')`
```

### Comparing `imsciences-0.5.5.5/imsciences/datafunctions.py` & `imsciences-0.5.5.6/imsciences/datafunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,20 @@
         print("   - Example: keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')") 
         
         print("\n27. manually_edit_data")
         print("   - Description: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.")
         print("   - Usage: manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)")
         print("   - Example: keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')") 
         
+        print("\n28. create_var_names")
+        print("   - Description: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.")
+        print("   - Usage: create_var_names(df,col_names_to_combine,seperator='_',combined_col_name='Variable_Column_Name')")
+        print("   - Example: create_var_names(df,['Media','Metric'],seperator='.',combined_col_name='New Variable Name')")         
+        
+        
     def get_wd_levels(self, levels):
         """
         Gets the current wd of whoever is working on it and gives the options to move the number of levels up.
 
         Parameters:
         - data_frame: pandas DataFrame
             The input data frame.
@@ -643,14 +649,15 @@
 
         Returns:
         pandas.DataFrame: DataFrame with a new column containing the look up table results.
         """
         
         # Function to find word in string
         def find_word_in_string(x_string, to_find_dict=to_find_dict, default_value=if_not_in_dict):
+            x_string = str(x_string)
             x_string_lower = x_string.lower()
             for key, value in to_find_dict.items():
                 if key.lower() in x_string_lower:
                     return value
             return default_value
         
         # Preprocess DataFrame if multiple columns
@@ -1026,8 +1033,26 @@
         # Add note if desired in new column or an existing column
         if add_notes == "Yes":
             note_col = existing_note_col_name if existing_note_col_name else 'Notes'
             if note_col not in df.columns:
                 df[note_col] = None
             df.loc[df_filtered.index, note_col] = note
 
+        return df
+    
+    def create_var_names(self,df,col_names_to_combine,seperator="_",combined_col_name="Variable_Column_Name"):
+        """
+        Combines dataframe columns containing strings to create a new column containing a variable name
+
+        Parameters:
+            df (pandas.DataFrame): The DataFrame containing the data.
+            col_names_to_combine (list of str): List of the column names on which to combine the strings
+            seperator (str, optional): The seperator to combine all the strings on to create the variable names. Defaults to "_".
+            combined_col_name (str, optional): The name of the final combined variable name column. Defaults to "Variable_Column_Name".
+
+        Returns:
+            pandas.DataFrame: DataFrame with a new column containing the combined variable name.
+        """
+        df = df.copy()
+        df[combined_col_name] = df[col_names_to_combine].astype(str).apply(seperator.join, axis=1)
+        
         return df
```

### Comparing `imsciences-0.5.5.5/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.5.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: imsciences
-Version: 0.5.5.5
-Summary: IMS Data Processing Package
-Author: IMS
-Author-email: cam@im-sciences.com
-Keywords: python,data processing
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
 # IMS Package Documentation
 
 The IMS package is a python library for processing incoming data into a format that can be used for projects. IMS processing offers a variety of functions to manipulate and analyze data efficiently. Here are the functionalities provided by the package:
 
 ### 1. `get_wd_levels(levels)`
 - **Description**: Get the working directory with the option of moving up parents.
 - **Usage**: `get_wd_levels(levels)`
@@ -120,7 +105,11 @@
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
+
+### 28. `create_var_names(df,col_names_to_combine,seperator='_',combined_col_name='Variable_Column_Name')`
+- **Description**: Combines dataframe columns containing strings to create a new column containing a variable name.
+- **Usage**: `create_var_names(df,['Media','Metric'],seperator='.',combined_col_name='New Variable Name')`
```

### Comparing `imsciences-0.5.5.5/setup.py` & `imsciences-0.5.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.5'
+VERSION = '0.5.5.6'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

