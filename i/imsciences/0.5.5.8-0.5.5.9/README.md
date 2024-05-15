# Comparing `tmp/imsciences-0.5.5.8.tar.gz` & `tmp/imsciences-0.5.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.8.tar", last modified: Wed May 15 12:37:19 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.9.tar", last modified: Wed May 15 16:06:01 2024, max compression
```

## Comparing `imsciences-0.5.5.8.tar` & `imsciences-0.5.5.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:37:19.383883 imsciences-0.5.5.8/
--rw-rw-rw-   0        0        0     8987 2024-05-15 12:37:19.376882 imsciences-0.5.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     8482 2024-05-15 12:04:13.000000 imsciences-0.5.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 12:37:19.334594 imsciences-0.5.5.8/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.8/imsciences/__init__.py
--rw-rw-rw-   0        0        0    55632 2024-05-15 12:36:55.000000 imsciences-0.5.5.8/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:37:19.373884 imsciences-0.5.5.8/imsciences.egg-info/
--rw-rw-rw-   0        0        0     8987 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 12:37:19.000000 imsciences-0.5.5.8/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 12:37:19.383883 imsciences-0.5.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-15 12:37:07.000000 imsciences-0.5.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:06:01.336023 imsciences-0.5.5.9/
+-rw-rw-rw-   0        0        0     8987 2024-05-15 16:06:01.331635 imsciences-0.5.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8482 2024-05-15 12:04:13.000000 imsciences-0.5.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 16:06:01.306528 imsciences-0.5.5.9/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.5.9/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    55701 2024-05-15 16:04:36.000000 imsciences-0.5.5.9/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:06:01.329636 imsciences-0.5.5.9/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     8987 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:06:01.336023 imsciences-0.5.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-15 16:05:56.000000 imsciences-0.5.5.9/setup.py
```

### Comparing `imsciences-0.5.5.8/PKG-INFO` & `imsciences-0.5.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.8
+Version: 0.5.5.9
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.5.8/README.md` & `imsciences-0.5.5.9/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.5.8/imsciences/datafunctions.py` & `imsciences-0.5.5.9/imsciences/datafunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,15 +750,15 @@
         pandas.DataFrame: DataFrame with additional merged column
         """
         # Specify more than one column must be entered
         if len(col_names) < 2:
             raise ValueError("2 or more columns must be specified to merge")
         
         # Create a new column with the merged columns
-        df[output_column_name] = seperator.join(df[col_names])
+        df[output_column_name] = df[col_names].astype(str).apply(seperator.join, axis=1)
 
         # Add string before 
         if starting_prefix_str is not None:
             df[output_column_name] = starting_prefix_str + df[output_column_name].astype(str)
         
         # Add string after
         if ending_prefix_str is not None:
@@ -1038,8 +1038,11 @@
         # Add note if desired in new column or an existing column
         if add_notes == "Yes":
             note_col = existing_note_col_name if existing_note_col_name else 'Notes'
             if note_col not in df.columns:
                 df[note_col] = None
             df.loc[df_filtered.index, note_col] = note
 
-        return df
+        return df
+    
+class datapull:
+    print("hello")
```

### Comparing `imsciences-0.5.5.8/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.5.9/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.8
+Version: 0.5.5.9
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.5.8/setup.py` & `imsciences-0.5.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.8'
+VERSION = '0.5.5.9'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

