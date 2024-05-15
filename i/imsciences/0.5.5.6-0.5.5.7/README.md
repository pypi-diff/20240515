# Comparing `tmp/imsciences-0.5.5.6.tar.gz` & `tmp/imsciences-0.5.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.6.tar", last modified: Wed May 15 10:13:59 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.7.tar", last modified: Wed May 15 12:02:56 2024, max compression
```

## Comparing `imsciences-0.5.5.6.tar` & `imsciences-0.5.5.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 10:13:59.494105 imsciences-0.5.5.6/
--rw-rw-rw-   0        0        0     9190 2024-05-15 10:13:59.489136 imsciences-0.5.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     8685 2024-05-15 10:13:51.000000 imsciences-0.5.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 10:13:59.457053 imsciences-0.5.5.6/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.6/imsciences/__init__.py
--rw-rw-rw-   0        0        0    56232 2024-05-15 10:13:49.000000 imsciences-0.5.5.6/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:13:59.485589 imsciences-0.5.5.6/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9190 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 10:13:59.000000 imsciences-0.5.5.6/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 10:13:59.494105 imsciences-0.5.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-15 10:13:52.000000 imsciences-0.5.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:02:56.524470 imsciences-0.5.5.7/
+-rw-rw-rw-   0        0        0     8987 2024-05-15 12:02:56.520838 imsciences-0.5.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8482 2024-05-15 12:02:45.000000 imsciences-0.5.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 12:02:56.494214 imsciences-0.5.5.7/imsciences/
+-rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.7/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    55606 2024-05-15 12:02:43.000000 imsciences-0.5.5.7/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:02:56.514932 imsciences-0.5.5.7/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     8987 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 12:02:56.000000 imsciences-0.5.5.7/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 12:02:56.525752 imsciences-0.5.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-15 12:02:47.000000 imsciences-0.5.5.7/setup.py
```

### Comparing `imsciences-0.5.5.6/PKG-INFO` & `imsciences-0.5.5.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: imsciences
-Version: 0.5.5.6
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
@@ -89,17 +74,17 @@
 - **Description**: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.
 - **Usage**: `classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')`
 
 ### 19. `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 - **Description**: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week. In the wide format.
 - **Usage**: `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 
-### 20. `merge_cols_with_seperator(df, col_names,output_column_name = 'Merged')`
-- **Description**: Merge multiple columns in a dataframe into 1 column with a seperator '|'.Can be used if multiple columns are needed for a LUT.
-- **Usage**: `merge_cols_with_seperator(df, ['Campaign','Product'],'Merged Columns')`
+### 20. `merge_cols_with_seperator(self, df, col_names,seperator='_',output_column_name = 'Merged',starting_prefix_str=None,ending_prefix_str=None)`
+- **Description**: Merge multiple columns in a dataframe into 1 column with a seperator.Can be used if multiple columns are needed for a LUT.
+- **Usage**: `merge_cols_with_seperator(df, ['Campaign','Product'],seperator='|','Merged Columns',starting_prefix_str='start_',ending_prefix_str='_end')`
 
 ### 21. `check_sum_of_df_cols_are_equal(df_1,df_2,cols_1,cols_2)`
 - **Description**: Checks if the sum of two columns in two dataframes are the same, and provides the sums of each column and the difference between them.
 - **Usage**: `check_sum_of_df_cols_are_equal(df_1,df_2,'Media Cost','Spend')`
 
 ### 22. `convert_2_df_cols_to_dict(df, key_col, value_col)`
 - **Description**: Can be used to create an LUT. Creates a dictionary using two columns in a dataframe.
@@ -119,12 +104,8 @@
 
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
-- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
-
-### 28. `create_var_names(df,col_names_to_combine,seperator='_',combined_col_name='Variable_Column_Name')`
-- **Description**: Combines dataframe columns containing strings to create a new column containing a variable name.
-- **Usage**: `create_var_names(df,['Media','Metric'],seperator='.',combined_col_name='New Variable Name')`
+- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
```

### Comparing `imsciences-0.5.5.6/README.md` & `imsciences-0.5.5.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: imsciences
+Version: 0.5.5.7
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
@@ -74,17 +89,17 @@
 - **Description**: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.
 - **Usage**: `classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')`
 
 ### 19. `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 - **Description**: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week. In the wide format.
 - **Usage**: `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 
-### 20. `merge_cols_with_seperator(df, col_names,output_column_name = 'Merged')`
-- **Description**: Merge multiple columns in a dataframe into 1 column with a seperator '|'.Can be used if multiple columns are needed for a LUT.
-- **Usage**: `merge_cols_with_seperator(df, ['Campaign','Product'],'Merged Columns')`
+### 20. `merge_cols_with_seperator(self, df, col_names,seperator='_',output_column_name = 'Merged',starting_prefix_str=None,ending_prefix_str=None)`
+- **Description**: Merge multiple columns in a dataframe into 1 column with a seperator.Can be used if multiple columns are needed for a LUT.
+- **Usage**: `merge_cols_with_seperator(df, ['Campaign','Product'],seperator='|','Merged Columns',starting_prefix_str='start_',ending_prefix_str='_end')`
 
 ### 21. `check_sum_of_df_cols_are_equal(df_1,df_2,cols_1,cols_2)`
 - **Description**: Checks if the sum of two columns in two dataframes are the same, and provides the sums of each column and the difference between them.
 - **Usage**: `check_sum_of_df_cols_are_equal(df_1,df_2,'Media Cost','Spend')`
 
 ### 22. `convert_2_df_cols_to_dict(df, key_col, value_col)`
 - **Description**: Can be used to create an LUT. Creates a dictionary using two columns in a dataframe.
@@ -105,11 +120,7 @@
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
-
-### 28. `create_var_names(df,col_names_to_combine,seperator='_',combined_col_name='Variable_Column_Name')`
-- **Description**: Combines dataframe columns containing strings to create a new column containing a variable name.
-- **Usage**: `create_var_names(df,['Media','Metric'],seperator='.',combined_col_name='New Variable Name')`
```

### Comparing `imsciences-0.5.5.6/imsciences/datafunctions.py` & `imsciences-0.5.5.7/imsciences/datafunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,17 @@
 
         print("\n19. aggregate_daily_to_wc_wide")
         print("   - Description: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week.")
         print("   - Usage: aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)")
         print("   - Example: aggregate_daily_to_wc_wide(df, 'date', ['platform'], ['cost', 'impressions', 'clicks'], 'mon', 'average', True)")
 
         print("\n20. merge_cols_with_seperator")
-        print("   - Description: Merge multiple columns in a dataframe into 1 column with a seperator '|'.Can be used if multiple columns are needed for a LUT.")
-        print("   - Usage: merge_cols_with_seperator(df, col_names,output_column_name = 'Merged')")
-        print("   - Example: merge_cols_with_seperator(df, ['Campaign','Product'],'Merged Columns')")        
+        print("   - Description: Merge multiple columns in a dataframe into 1 column with a seperator '_'.Can be used if multiple columns are needed for a LUT.")
+        print("   - Usage: merge_cols_with_seperator(self, df, col_names,seperator='_',output_column_name = 'Merged',starting_prefix_str=None,ending_prefix_str=None)")
+        print("   - Example: merge_cols_with_seperator(df, ['Campaign','Product'],seperator='|','Merged Columns',starting_prefix_str='start_',ending_prefix_str='_end')")        
 
         print("\n21. check_sum_of_df_cols_are_equal")
         print("   - Description: Checks if the sum of two columns in two dataframes are the same, and provides the sums of each column and the difference between them.")
         print("   - Usage: check_sum_of_df_cols_are_equal(df_1,df_2,cols_1,cols_2)")
         print("   - Example: check_sum_of_df_cols_are_equal(df_1,df_2,'Media Cost','Spend')")        
 
         print("\n22. convert_2_df_cols_to_dict")
@@ -144,21 +144,15 @@
         print("   - Description: Changes a dataframe from wide to long format.")
         print("   - Usage: convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')")
         print("   - Example: keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')") 
         
         print("\n27. manually_edit_data")
         print("   - Description: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.")
         print("   - Usage: manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)")
-        print("   - Example: keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')") 
-        
-        print("\n28. create_var_names")
-        print("   - Description: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.")
-        print("   - Usage: create_var_names(df,col_names_to_combine,seperator='_',combined_col_name='Variable_Column_Name')")
-        print("   - Example: create_var_names(df,['Media','Metric'],seperator='.',combined_col_name='New Variable Name')")         
-        
+        print("   - Example: keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')")      
         
     def get_wd_levels(self, levels):
         """
         Gets the current wd of whoever is working on it and gives the options to move the number of levels up.
 
         Parameters:
         - data_frame: pandas DataFrame
@@ -649,25 +643,24 @@
 
         Returns:
         pandas.DataFrame: DataFrame with a new column containing the look up table results.
         """
         
         # Function to find word in string
         def find_word_in_string(x_string, to_find_dict=to_find_dict, default_value=if_not_in_dict):
-            x_string = str(x_string)
             x_string_lower = x_string.lower()
             for key, value in to_find_dict.items():
                 if key.lower() in x_string_lower:
                     return value
             return default_value
         
         # Preprocess DataFrame if multiple columns
         if len(col_names) > 1:
             df["Merged"] = df[col_names].astype(str).apply('|'.join, axis=1)
-            col_names = ["Merged"]
+            col_names = "Merged"
 
         # Apply the inner function to the specified column and create a new column with the results
         df[new_column_name] = df[col_names].apply(find_word_in_string)
         
         # # Drop intermediate column if created
         # if len(col_names) > 1:
         #     df.drop(columns=["Merged"], inplace=True)
@@ -733,36 +726,47 @@
                 wide_df[total_column_name] = wide_df[columns_to_sum].sum(axis=1)
 
         # Reset the index of the final DataFrame
         wide_df = wide_df.reset_index()
 
         return wide_df
 
-    def merge_cols_with_seperator(self, df, col_names,output_column_name = "Merged"):
+    def merge_cols_with_seperator(self, df, col_names,seperator='_',output_column_name = "Merged",starting_prefix_str=None,ending_prefix_str=None):
         """
-        Creates a new column in the dataframe that merges 2 or more columns together with a "|" seperator, possibly to be used for a look up table where multiple columns are being looked up
+        Creates a new column in the dataframe that merges 2 or more columns together with a "_" seperator, possibly to be used for a look up table where multiple columns are being looked up
 
         Parameters:
         df (pandas.DataFrame): Dataframe to make changes to.
         col_names (list): list of columm names ot merge.
+        seperator (str, optional): Name of column outputted. Defaults to "_".
         output_column_name (str, optional): Name of column outputted. Defaults to "Merged".
+        starting_prefix_str (str, optional): string of optional text to be added before the merged column str value
+        ending_prefix_str (str, optional): string of optional text to be added after the merged column str value
 
         Raises:
         ValueError: if more less than two column names are inputted in the list there is nothing to merge on
 
         Returns:
         pandas.DataFrame: DataFrame with additional merged column
         """
         # Specify more than one column must be entered
         if len(col_names) < 2:
             raise ValueError("2 or more columns must be specified to merge")
         
         # Create a new column with the merged columns
-        df[output_column_name] = "|".join(df[col_names])
+        df[output_column_name] = seperator.join(df[col_names])
 
+        # Add string before 
+        if starting_prefix_str is not None:
+            df[output_column_name] = starting_prefix_str + df[output_column_name].astype(str)
+        
+        # Add string after
+        if ending_prefix_str is not None:
+            df[output_column_name] = df[output_column_name].astype(str) + ending_prefix_str
+                    
         return df
 
     def check_sum_of_df_cols_are_equal(self, df_1,df_2,cols_1,cols_2):
         """
         Checks the sum of two different dataframe column or columns are equal
 
         Parameters:
@@ -1033,26 +1037,8 @@
         # Add note if desired in new column or an existing column
         if add_notes == "Yes":
             note_col = existing_note_col_name if existing_note_col_name else 'Notes'
             if note_col not in df.columns:
                 df[note_col] = None
             df.loc[df_filtered.index, note_col] = note
 
-        return df
-    
-    def create_var_names(self,df,col_names_to_combine,seperator="_",combined_col_name="Variable_Column_Name"):
-        """
-        Combines dataframe columns containing strings to create a new column containing a variable name
-
-        Parameters:
-            df (pandas.DataFrame): The DataFrame containing the data.
-            col_names_to_combine (list of str): List of the column names on which to combine the strings
-            seperator (str, optional): The seperator to combine all the strings on to create the variable names. Defaults to "_".
-            combined_col_name (str, optional): The name of the final combined variable name column. Defaults to "Variable_Column_Name".
-
-        Returns:
-            pandas.DataFrame: DataFrame with a new column containing the combined variable name.
-        """
-        df = df.copy()
-        df[combined_col_name] = df[col_names_to_combine].astype(str).apply(seperator.join, axis=1)
-        
         return df
```

### Comparing `imsciences-0.5.5.6/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.5.7/imsciences.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.6
+Version: 0.5.5.7
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -89,17 +89,17 @@
 - **Description**: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.
 - **Usage**: `classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')`
 
 ### 19. `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 - **Description**: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week. In the wide format.
 - **Usage**: `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 
-### 20. `merge_cols_with_seperator(df, col_names,output_column_name = 'Merged')`
-- **Description**: Merge multiple columns in a dataframe into 1 column with a seperator '|'.Can be used if multiple columns are needed for a LUT.
-- **Usage**: `merge_cols_with_seperator(df, ['Campaign','Product'],'Merged Columns')`
+### 20. `merge_cols_with_seperator(self, df, col_names,seperator='_',output_column_name = 'Merged',starting_prefix_str=None,ending_prefix_str=None)`
+- **Description**: Merge multiple columns in a dataframe into 1 column with a seperator.Can be used if multiple columns are needed for a LUT.
+- **Usage**: `merge_cols_with_seperator(df, ['Campaign','Product'],seperator='|','Merged Columns',starting_prefix_str='start_',ending_prefix_str='_end')`
 
 ### 21. `check_sum_of_df_cols_are_equal(df_1,df_2,cols_1,cols_2)`
 - **Description**: Checks if the sum of two columns in two dataframes are the same, and provides the sums of each column and the difference between them.
 - **Usage**: `check_sum_of_df_cols_are_equal(df_1,df_2,'Media Cost','Spend')`
 
 ### 22. `convert_2_df_cols_to_dict(df, key_col, value_col)`
 - **Description**: Can be used to create an LUT. Creates a dictionary using two columns in a dataframe.
@@ -120,11 +120,7 @@
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
-
-### 28. `create_var_names(df,col_names_to_combine,seperator='_',combined_col_name='Variable_Column_Name')`
-- **Description**: Combines dataframe columns containing strings to create a new column containing a variable name.
-- **Usage**: `create_var_names(df,['Media','Metric'],seperator='.',combined_col_name='New Variable Name')`
```

### Comparing `imsciences-0.5.5.6/setup.py` & `imsciences-0.5.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.6'
+VERSION = '0.5.5.7'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

