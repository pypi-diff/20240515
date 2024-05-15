# Comparing `tmp/imsciences-0.5.5.3.tar.gz` & `tmp/imsciences-0.5.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.3.tar", last modified: Fri May 10 12:41:04 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.4.tar", last modified: Tue May 14 14:52:44 2024, max compression
```

## Comparing `imsciences-0.5.5.3.tar` & `imsciences-0.5.5.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 12:41:04.189970 imsciences-0.5.5.3/
--rw-rw-rw-   0        0        0     7464 2024-05-10 12:41:04.184958 imsciences-0.5.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     6959 2024-05-10 09:52:39.000000 imsciences-0.5.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 12:41:04.147746 imsciences-0.5.5.3/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.3/imsciences/__init__.py
--rw-rw-rw-   0        0        0    44950 2024-05-10 12:40:01.000000 imsciences-0.5.5.3/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:41:04.180494 imsciences-0.5.5.3/imsciences.egg-info/
--rw-rw-rw-   0        0        0     7464 2024-05-10 12:41:03.000000 imsciences-0.5.5.3/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-10 12:41:03.000000 imsciences-0.5.5.3/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 12:41:03.000000 imsciences-0.5.5.3/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 12:41:03.000000 imsciences-0.5.5.3/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 12:41:03.000000 imsciences-0.5.5.3/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 12:41:04.190976 imsciences-0.5.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-10 12:39:57.000000 imsciences-0.5.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:52:44.251054 imsciences-0.5.5.4/
+-rw-rw-rw-   0        0        0     8855 2024-05-14 14:52:44.246164 imsciences-0.5.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8350 2024-05-14 14:45:39.000000 imsciences-0.5.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 14:52:44.218266 imsciences-0.5.5.4/imsciences/
+-rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.4/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    54723 2024-05-14 14:47:52.000000 imsciences-0.5.5.4/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:52:44.241809 imsciences-0.5.5.4/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     8855 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 14:52:44.251054 imsciences-0.5.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-14 14:45:41.000000 imsciences-0.5.5.4/setup.py
```

### Comparing `imsciences-0.5.5.3/PKG-INFO` & `imsciences-0.5.5.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.3
+Version: 0.5.5.4
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -108,7 +108,19 @@
 ### 23. `create_FY_and_H_columns(df, index_col, start_date, starting_FY,short_format='No',half_years='No',combined_FY_and_H='No')`
 - **Description**: Used to create a financial year, half year, and financial half year column.
 - **Usage**: `create_FY_and_H_columns(df, 'Week (M-S)', '2022-10-03', 'FY2023',short_format='Yes',half_years='Yes',combined_FY_and_H='Yes')`
 
 ### 24. `keyword_lookup_replacement(df, col, replacement_rows, cols_to_merge, replacement_lookup_dict,output_column_name='Updated Column')`
 - **Description**: Essentially provides an if statement with a xlookup if a value is something. Updates certain chosen values in a specified column of the DataFrame based on a lookup dictionary.
 - **Usage**: `keyword_lookup_replacement(df, 'channel', 'Paid Search Generic', ['channel','segment','product'], qlik_dict_for_channel,output_column_name='Channel New')`
+
+### 25. `create_new_version_of_col_using_LUT(df, keys_col,value_col, dict_for_specific_changes, new_col_name='New Version of Old Col')`
+- **Description**: Creates a new column in a dataframe, which takes an old column and uses a lookup table to changes values in the new column to reflect the lookup table. The lookup is based on a column in the dataframe.
+- **Usage**: `keyword_lookup_replacement(df, '*Campaign Name','Campaign Type',search_campaign_name_retag_lut,'Campaign Name New')`
+
+### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
+- **Description**: Changes a dataframe from wide to long format.
+- **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
+
+### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
+- **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
+- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
```

### Comparing `imsciences-0.5.5.3/README.md` & `imsciences-0.5.5.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -92,8 +92,20 @@
 
 ### 23. `create_FY_and_H_columns(df, index_col, start_date, starting_FY,short_format='No',half_years='No',combined_FY_and_H='No')`
 - **Description**: Used to create a financial year, half year, and financial half year column.
 - **Usage**: `create_FY_and_H_columns(df, 'Week (M-S)', '2022-10-03', 'FY2023',short_format='Yes',half_years='Yes',combined_FY_and_H='Yes')`
 
 ### 24. `keyword_lookup_replacement(df, col, replacement_rows, cols_to_merge, replacement_lookup_dict,output_column_name='Updated Column')`
 - **Description**: Essentially provides an if statement with a xlookup if a value is something. Updates certain chosen values in a specified column of the DataFrame based on a lookup dictionary.
-- **Usage**: `keyword_lookup_replacement(df, 'channel', 'Paid Search Generic', ['channel','segment','product'], qlik_dict_for_channel,output_column_name='Channel New')`
+- **Usage**: `keyword_lookup_replacement(df, 'channel', 'Paid Search Generic', ['channel','segment','product'], qlik_dict_for_channel,output_column_name='Channel New')`
+
+### 25. `create_new_version_of_col_using_LUT(df, keys_col,value_col, dict_for_specific_changes, new_col_name='New Version of Old Col')`
+- **Description**: Creates a new column in a dataframe, which takes an old column and uses a lookup table to changes values in the new column to reflect the lookup table. The lookup is based on a column in the dataframe.
+- **Usage**: `keyword_lookup_replacement(df, '*Campaign Name','Campaign Type',search_campaign_name_retag_lut,'Campaign Name New')`
+
+### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
+- **Description**: Changes a dataframe from wide to long format.
+- **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
+
+### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
+- **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
+- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
```

### Comparing `imsciences-0.5.5.3/imsciences/datafunctions.py` & `imsciences-0.5.5.4/imsciences/datafunctions.py`

 * *Files 16% similar despite different names*

```diff
@@ -131,15 +131,29 @@
         print("   - Example: create_FY_and_H_columns(df, 'Week (M-S)', '2022-10-03', 'FY2023',short_format='Yes',half_years='Yes',combined_FY_and_H='Yes')")        
         
         print("\n24. keyword_lookup_replacement")
         print("   - Description: Essentially provides an if statement with a xlookup if a value is something. Updates certain chosen values in a specified column of the DataFrame based on a lookup dictionary.")
         print("   - Usage: keyword_lookup_replacement(df, col, replacement_rows, cols_to_merge, replacement_lookup_dict,output_column_name='Updated Column')")
         print("   - Example: keyword_lookup_replacement(df, 'channel', 'Paid Search Generic', ['channel','segment','product'], qlik_dict_for_channel,output_column_name='Channel New')")        
 
-
+        print("\n25. create_new_version_of_col_using_LUT")
+        print("   - Description: Creates a new column in a dataframe, which takes an old column and uses a lookup table to changes values in the new column to reflect the lookup table. The lookup is based on a column in the dataframe.")
+        print("   - Usage: create_new_version_of_col_using_LUT(df, keys_col,value_col, dict_for_specific_changes, new_col_name='New Version of Old Col')")
+        print("   - Example: keyword_lookup_replacement(df, '*Campaign Name','Campaign Type',search_campaign_name_retag_lut,'Campaign Name New')")        
+
+        print("\n26. convert_df_wide_2_long")
+        print("   - Description: Changes a dataframe from wide to long format.")
+        print("   - Usage: convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')")
+        print("   - Example: keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')") 
+        
+        print("\n27. manually_edit_data")
+        print("   - Description: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.")
+        print("   - Usage: manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)")
+        print("   - Example: keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')") 
+        
     def get_wd_levels(self, levels):
         """
         Gets the current wd of whoever is working on it and gives the options to move the number of levels up.
 
         Parameters:
         - data_frame: pandas DataFrame
             The input data frame.
@@ -627,54 +641,35 @@
         if_not_in_dict (str, optional): default value if no substring matches are found in the look up table dictionary. Defaults to "Other".
         new_column_name (str, optional): name of new column. Defaults to "Mapping".
 
         Returns:
         pandas.DataFrame: DataFrame with a new column containing the look up table results.
         """
         
-        # Define the inner function for classification
+        # Function to find word in string
         def find_word_in_string(x_string, to_find_dict=to_find_dict, default_value=if_not_in_dict):
             x_string_lower = x_string.lower()
             for key, value in to_find_dict.items():
                 if key.lower() in x_string_lower:
                     return value
             return default_value
+        
+        # Preprocess DataFrame if multiple columns
+        if len(col_names) > 1:
+            df["Merged"] = df[col_names].astype(str).apply('|'.join, axis=1)
+            col_names = ["Merged"]
 
-        # Check if there is multiple columns to look up on
-        if len(col_names) == 1:
+        # Apply the inner function to the specified column and create a new column with the results
+        df[new_column_name] = df[col_names].apply(find_word_in_string)
+        
+        # # Drop intermediate column if created
+        # if len(col_names) > 1:
+        #     df.drop(columns=["Merged"], inplace=True)
 
-            # Create copy of df to avoid SettingWithCopyWarning warning
-            df_2 = df.copy()
-            
-            try:
-                # Apply the inner function to the specified column and create a new column with the results
-                df_2[new_column_name] = df_2.loc[:,''.join(col_names)].apply(find_word_in_string)
-                
-            # Raise an error if list has not been inputted for column names
-            except TypeError:
-                print("Error: Column Names even if only one must be specified as a list, so must be inputted as e.g." + str(["Product"]) + ". to_find_dict must be specified as dictionary")
-                
-            
-        # Check if there is multiple columns to look up on
-        if len(col_names) > 1:
-            
-            # Create copy of df to avoid SettingWithCopyWarning warning
-            df_2 = df.copy()
-            
-            try:
-                # Apply a lambda function to join the chosen columns togther with a seperator
-                df_2["Merged"] = df_2.loc[:,col_names].apply(lambda row: '|'.join(row.values.astype(str)), axis=1)
-            
-            except TypeError:
-                print("Error: Column Names even if only one must be specified as a list, so must be inputted as e.g." + str(["Product"]) + ". to_find_dict must be specified as dictionary")
-            
-            # Apply the inner function to the specified column and create a new column with the results
-            df_2[new_column_name] = df_2.loc[:,"Merged"].apply(find_word_in_string)
-            
-        return df_2
+        return df
 
     def aggregate_daily_to_wc_wide(self, df : pd.DataFrame, date_column : str, group_columns : list[str], sum_columns : list[str], wc : str = 'sun', aggregation : str = 'sum', include_totals : bool = False) -> pd.DataFrame:
         """
         Aggregates daily data into weekly data, starting on a specified day of the week, 
         and groups the data by additional specified columns. It aggregates specified numeric columns 
         by summing, averaging, or counting them, and pivots the data to create separate columns for each combination 
         of the group columns and sum columns. NaN values are replaced with 0 and the index is reset. 
@@ -692,16 +687,14 @@
         - wc: string
             The week commencing day (e.g., 'sun' for Sunday, 'mon' for Monday).
         - aggregation: string, optional (default 'sum')
             Aggregation method, either 'sum', 'average', or 'count'.
         - include_totals: boolean, optional (default False)
             If True, include total columns for each sum_column.
 
-
-
         Returns:
         - pandas DataFrame
             A new DataFrame with weekly aggregated data. The index is reset,
             and columns represent the grouped and aggregated metrics. The DataFrame 
             is in wide format, with separate columns for each combination of 
             grouped metrics.
         """
@@ -875,8 +868,166 @@
                 merged_value = x['Merged']  
                 if merged_value in replacement_lookup_dict:
                     return replacement_lookup_dict[merged_value]
             return x[col]
         
         df[output_column_name] = df.apply(replace_values, axis=1)
         
+        return df
+    
+    def create_new_version_of_col_using_LUT(self, df, keys_col,value_col, dict_for_specific_changes, new_col_name="New Version of Old Col"):
+        """
+        Creates a new column in a dataframe, which takes an old column and uses a lookup table to changes values in the new column to reflect the lookup table. 
+        The lookup is based on a column in the dataframe. Can only input one column and output one new column.
+
+        Parameters:
+            df (pandas.DataFrame): The DataFrame containing the data.
+            keys_col (str): The name of the column which the LUT will be refercing to ouput a value.
+            value_col (str): The name of the column which the new column will be based off. If a key in the key column is not found in the LUT, the values from this column are used instead.
+            dict_for_specific_changes (dict): The LUT which the keys_col will be mapped on to find any values that need changing in the new column.
+            new_col_name (str, optional): This is the name of the new column being generated. Defaults to "New Version of Old Col".
+
+        Returns:
+        pandas.DataFrame: DataFrame with a new column which is similar to the old column, except for where changes have been made to reflect the lookup table.
+        """
+    
+        # Extract columns to change using new dictionary
+        smaller_df = df[[keys_col,value_col]]
+
+        # Use the new dictionary to create a new LUT
+        smaller_df_with_LUT = self.apply_lookup_table_for_columns(smaller_df,[keys_col,value_col],dict_for_specific_changes)
+        
+        # In a new column, keep values from the old column that don't need updating as they are not in the dictionary, and replace values that do need updating with values from the dictionary based on the keys
+        smaller_df_with_LUT["Updated Col"]=smaller_df_with_LUT.apply(lambda x: x['Mapping'] if x['Mapping'] != "Other" else x[value_col],axis=1)
+
+        # Drop the extra unecessary cols
+        smaller_df_with_LUT.drop([keys_col,'Mapping'],axis=1,inplace=True)
+        
+        # # Output dataframes as dictionary to be used in a LUT
+        new_dict = self.convert_2_df_cols_to_dict(smaller_df_with_LUT,value_col,"Updated Col")
+
+        # # Use new dictionary to create a new version of an old column
+        df_final = self.apply_lookup_table_for_columns(df,[keys_col],new_dict,"other",new_col_name)
+        
+        return df_final
+    
+    def convert_df_wide_2_long(self, df,value_cols,variable_col_name='Stacked',value_col_name='Value'):
+        """
+        Changes a dataframe from wide to long format.
+
+        Args:
+            df (pandas.DataFrame): The DataFrame containing the data.
+            value_cols (list of str or str if only one): list of column names which are to be transformed from several columns into one.
+            variable_col_name (str, optional): Name of new variables column, which contains the names of the columns which have been stacked into one. Defaults to 'Stacked'.
+            value_col_name (str, optional): Name of the new value column which contains all the data from the stacked columns. Defaults to 'Value'.
+
+        Returns:
+            pandas.DataFrame:: Returns dataframe transformed from long to wide.
+            
+        Raises:
+            ValueError: If number of column names to be depivoted is less than 2, then this function is not neccesary.
+        """
+        
+        # Check length of value cols is greater than 1
+        if len(value_cols) < 2:
+            raise ValueError("Number of inputs in list must be greater than 1")
+        
+        # Find the columns that are not to be depivoted into one column
+        id_vars = list(set(df.columns.tolist()) - set(value_cols))
+        
+        # Melt all columns chosen into one column
+        df_final = pd.melt(df, id_vars,value_cols,var_name=variable_col_name,value_name=value_col_name)
+        
+        return df_final
+    
+    def manually_edit_data(self, df, filters_dict, col_to_change, new_value, change_in_existing_df_col="No", new_col_to_change_name='New', manual_edit_col_name=None, add_notes="No", existing_note_col_name=None, note=None):
+        """
+        Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe
+
+        Args:
+            df (pandas.DataFrame): The DataFrame containing the data.
+            filters_dict (dict): Dictionary of conditions for the boolean mask i.e. what to filter your df on to get to your chosen cell
+            col_to_change (str): String name of column to edit
+            new_value (any): Value of new input for cell
+            change_in_existing_df_col (str, optional): Input of Yes or No to describe whether to make the change in an existing column. Defaults to "No".
+            new_col_to_change_name (str, optional): Name of the new column to copy the column being edited into and to make the change in. Defaults to 'New'.
+            manual_edit_col_name (str, optional): Name of the current manual edits column, if one is not specified it will be created. Defaults to None.
+            add_notes (str, optional): Gives the option to create a new notes column. Defaults to "No".
+            existing_note_col_name (str, optional): If there is an existing notes column this can be specified. Defaults to None.
+            note (str), optional): The string of the note to be added to the column. Defaults to None.
+
+        Raises:
+            TypeError: The column for the column to change can only be specified as one column as it is a string not a list
+            ValueError: You can only input the values of "Yes" or "No" for whether to make the change in existing column
+            ValueError: You can only input the values of "Yes" or "No" for whether to make a new notes column
+
+        Returns:
+            pandas.DataFrame: Dataframe with manual changes added
+        """
+        # Raise type error if more than one col is supported
+        if isinstance(col_to_change, list):
+            raise TypeError("Col to change must be specified as a string, not a list")
+        
+        # Raises value error if input is invalid for change_in_existing_df_col
+        if change_in_existing_df_col not in ["Yes", "No"]:
+            raise ValueError("Invalid input value for change_in_existing_df_col. Allowed values are: ['Yes', 'No']")
+        
+        # Raises value error if input is invalid for add_notes_col
+        if add_notes not in ["Yes", "No"]:
+            raise ValueError("Invalid input value for add_notes. Allowed values are: ['Yes', 'No']")
+
+        # Create list of conditions 
+        mask = pd.Series(True, index=df.index)
+        for col, cond in filters_dict.items():
+            cond = cond.strip()
+            operator, value = cond.split(maxsplit=1)
+            
+            # If value is a string condition make sure to check if there are new lines
+            if "'" in value:
+                value = value.strip().strip("'\"")
+            # If not a string e.g. datetime or number condition you need to transform the string into a value
+            else:
+                value = eval(value)  
+
+            if operator == "==":
+                temp_mask = (df[col] == value)
+            elif operator == "!=":
+                temp_mask = (df[col] != value)
+            elif operator == ">=":
+                temp_mask = (df[col] >= value)
+            elif operator == "<=":
+                temp_mask = (df[col] <= value)
+            elif operator == ">":
+                temp_mask = (df[col] > value)
+            elif operator == "<":
+                temp_mask = (df[col] < value)                          
+            mask &= temp_mask
+
+        # Create the filtered df by applying the conditions
+        df_filtered = df[mask]
+
+        # Create a new column to add the changes if desired, else edit in the current chosen column
+        col_to_update = col_to_change if change_in_existing_df_col == "Yes" else new_col_to_change_name
+        if change_in_existing_df_col == "No" and new_col_to_change_name not in df.columns:
+            df = df.copy()
+            df[new_col_to_change_name] = df[col_to_change]
+            
+        # Update the new cell in the chosen column
+        df.loc[df_filtered.index, col_to_update] = new_value
+
+        # Add in manual edit column if desired or specify where one already is
+        if manual_edit_col_name:
+            if manual_edit_col_name not in df.columns:
+                df[manual_edit_col_name] = 0
+            df.loc[df_filtered.index, manual_edit_col_name] = 1
+        elif not manual_edit_col_name and 'Manual Changes' not in df.columns:
+            df['Manual Changes'] = 0
+            df.loc[df_filtered.index, 'Manual Changes'] = 1
+
+        # Add note if desired in new column or an existing column
+        if add_notes == "Yes":
+            note_col = existing_note_col_name if existing_note_col_name else 'Notes'
+            if note_col not in df.columns:
+                df[note_col] = None
+            df.loc[df_filtered.index, note_col] = note
+
         return df
```

### Comparing `imsciences-0.5.5.3/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.5.4/imsciences.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.3
+Version: 0.5.5.4
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -108,7 +108,19 @@
 ### 23. `create_FY_and_H_columns(df, index_col, start_date, starting_FY,short_format='No',half_years='No',combined_FY_and_H='No')`
 - **Description**: Used to create a financial year, half year, and financial half year column.
 - **Usage**: `create_FY_and_H_columns(df, 'Week (M-S)', '2022-10-03', 'FY2023',short_format='Yes',half_years='Yes',combined_FY_and_H='Yes')`
 
 ### 24. `keyword_lookup_replacement(df, col, replacement_rows, cols_to_merge, replacement_lookup_dict,output_column_name='Updated Column')`
 - **Description**: Essentially provides an if statement with a xlookup if a value is something. Updates certain chosen values in a specified column of the DataFrame based on a lookup dictionary.
 - **Usage**: `keyword_lookup_replacement(df, 'channel', 'Paid Search Generic', ['channel','segment','product'], qlik_dict_for_channel,output_column_name='Channel New')`
+
+### 25. `create_new_version_of_col_using_LUT(df, keys_col,value_col, dict_for_specific_changes, new_col_name='New Version of Old Col')`
+- **Description**: Creates a new column in a dataframe, which takes an old column and uses a lookup table to changes values in the new column to reflect the lookup table. The lookup is based on a column in the dataframe.
+- **Usage**: `keyword_lookup_replacement(df, '*Campaign Name','Campaign Type',search_campaign_name_retag_lut,'Campaign Name New')`
+
+### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
+- **Description**: Changes a dataframe from wide to long format.
+- **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
+
+### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
+- **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
+- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
```

### Comparing `imsciences-0.5.5.3/setup.py` & `imsciences-0.5.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.3'
+VERSION = '0.5.5.4'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

