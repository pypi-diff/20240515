# Comparing `tmp/healmatcher-0.0.3.tar.gz` & `tmp/healmatcher-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healmatcher-0.0.3.tar", last modified: Tue May 14 19:57:22 2024, max compression
+gzip compressed data, was "dist/healmatcher-0.0.4.tar", last modified: Wed May 15 15:56:00 2024, max compression
```

## Comparing `healmatcher-0.0.3.tar` & `healmatcher-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:57:22.516215 healmatcher-0.0.3/
--rw-r--r--   0 kwanbo     (501) staff       (20)     2053 2024-05-14 19:57:22.516112 healmatcher-0.0.3/PKG-INFO
--rw-r--r--   0 kwanbo     (501) staff       (20)     1466 2024-05-14 19:55:47.000000 healmatcher-0.0.3/README.md
-drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:57:22.515726 healmatcher-0.0.3/healmatcher.egg-info/
--rw-r--r--   0 kwanbo     (501) staff       (20)     2053 2024-05-14 19:57:22.000000 healmatcher-0.0.3/healmatcher.egg-info/PKG-INFO
--rw-r--r--   0 kwanbo     (501) staff       (20)      207 2024-05-14 19:57:22.000000 healmatcher-0.0.3/healmatcher.egg-info/SOURCES.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)        1 2024-05-14 19:57:22.000000 healmatcher-0.0.3/healmatcher.egg-info/dependency_links.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)       20 2024-05-14 19:57:22.000000 healmatcher-0.0.3/healmatcher.egg-info/requires.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)        3 2024-05-14 19:57:22.000000 healmatcher-0.0.3/healmatcher.egg-info/top_level.txt
-drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-14 19:57:22.515961 healmatcher-0.0.3/hm/
--rw-r--r--   0 kwanbo     (501) staff       (20)      106 2024-05-14 18:53:41.000000 healmatcher-0.0.3/hm/__init__.py
--rw-r--r--   0 kwanbo     (501) staff       (20)       38 2024-05-14 19:57:22.516261 healmatcher-0.0.3/setup.cfg
--rw-r--r--   0 kwanbo     (501) staff       (20)     1065 2024-05-14 19:57:19.000000 healmatcher-0.0.3/setup.py
+drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-15 15:56:00.130734 healmatcher-0.0.4/
+-rw-r--r--   0 kwanbo     (501) staff       (20)     2512 2024-05-15 15:56:00.130571 healmatcher-0.0.4/PKG-INFO
+-rw-r--r--   0 kwanbo     (501) staff       (20)     1466 2024-05-15 14:21:45.000000 healmatcher-0.0.4/README.md
+drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-15 15:56:00.129923 healmatcher-0.0.4/healmatcher.egg-info/
+-rw-r--r--   0 kwanbo     (501) staff       (20)     2512 2024-05-15 15:56:00.000000 healmatcher-0.0.4/healmatcher.egg-info/PKG-INFO
+-rw-r--r--   0 kwanbo     (501) staff       (20)      207 2024-05-15 15:56:00.000000 healmatcher-0.0.4/healmatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)        1 2024-05-15 15:56:00.000000 healmatcher-0.0.4/healmatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)       20 2024-05-15 15:56:00.000000 healmatcher-0.0.4/healmatcher.egg-info/requires.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)        3 2024-05-15 15:56:00.000000 healmatcher-0.0.4/healmatcher.egg-info/top_level.txt
+drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-15 15:56:00.130246 healmatcher-0.0.4/hm/
+-rw-r--r--   0 kwanbo     (501) staff       (20)      106 2024-05-15 14:21:45.000000 healmatcher-0.0.4/hm/__init__.py
+-rw-r--r--   0 kwanbo     (501) staff       (20)       38 2024-05-15 15:56:00.130792 healmatcher-0.0.4/setup.cfg
+-rw-r--r--   0 kwanbo     (501) staff       (20)     1065 2024-05-15 15:50:24.000000 healmatcher-0.0.4/setup.py
```

### Comparing `healmatcher-0.0.3/PKG-INFO` & `healmatcher-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 Metadata-Version: 2.1
 Name: healmatcher
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast and simple probabilistic data matching package
+Home-page: UNKNOWN
 Author: Joseph Shim github.com/JosephKBS
 Author-email: <joseph.shim.rok@gmail.com>
+License: UNKNOWN
+Description: # healmatcher
+        - `healmatcher` is a simple but fast probabilistic matching package developed by NYULH HEAL Lab.
+        - Currently, the model supports 4 variables (sex, date of birth, last 4 digits of ssn, and first 2 letters of last name) to run the linkage process
+        
+        
+        ## How to use (example)
+        
+        `pip install healmatcher`
+        
+        
+        ```python
+        # Install package
+        !pip install healmatcher
+        
+        # Load package
+        from hm import hm
+        
+        # create example dataset
+        testa = pd.DataFrame({
+            'sex':[1,2,1,2,1,2,1,2,1,2],
+            'dob':['2012-1-1','2011-12-1','1999-1-1','1998-11-1','2012-11-1','1984-1-1','1982-1-1','1975-1-1','1967-1-1','1954-1-1'],
+            'ssn':[1111,2222,3333,4444,5555,6666,7777,8888,9999,1010],
+            'ln':["as",'ss','zz','rr','ww','wa','tr','tt','hh','gq'],
+            'PROVIDER_NUMBER':[2,1,1,1,1,1,1,1,2,1]
+        })
+        testb = pd.DataFrame({
+            'sex':[2,2,1,1,1,2,1,2,1,1],
+            'dob':['2012-1-1','2001-12-1','1999-1-1','1998-11-1','2012-11-1','1984-1-1','1982-1-1','1975-1-1','1967-1-1','1954-1-1'],
+            'ssn':[1111,2222,3333,4444,5555,6666,7777,8888,9999,1010],
+            'ln':["as",'ls','zz','rr','wb','wa','tr','tt','ha','gq'],
+            'PROVID
+        
+        # Run matching
+        hm(
+            df_a = testa,
+            df_b = testb,
+            col_a=['sex','dob','ssn','ln'],
+            col_b=['sex','dob','ssn','ln'],
+            match_prob_threshold = 0.001,
+            iteration = 20,
+            model2 = True,
+            blocking_rule_for_input = 'PROVIDER_NUMBER',
+            onetoone = True,
+            match_summary = True
+        )
+        ```
+        
+        # Webpage
+        [healmatcher](https://pypi.org/project/healmatcher/)
+        
 Keywords: probabilistic match,probabilistic data match,splink
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-
-# healmatcher
-- `healmatcher` is a simple but fast probabilistic matching package developed by NYULH HEAL Lab.
-- Currently, the model supports 4 variables (sex, date of birth, last 4 digits of ssn, and first 2 letters of last name) to run the linkage process
-
-
-## How to use (example)
-
-`pip install healmatcher`
-
-
-```python
-# Install package
-!pip install healmatcher
-
-# Load package
-from hm import hm
-
-# create example dataset
-testa = pd.DataFrame({
-    'sex':[1,2,1,2,1,2,1,2,1,2],
-    'dob':['2012-1-1','2011-12-1','1999-1-1','1998-11-1','2012-11-1','1984-1-1','1982-1-1','1975-1-1','1967-1-1','1954-1-1'],
-    'ssn':[1111,2222,3333,4444,5555,6666,7777,8888,9999,1010],
-    'ln':["as",'ss','zz','rr','ww','wa','tr','tt','hh','gq'],
-    'PROVIDER_NUMBER':[2,1,1,1,1,1,1,1,2,1]
-})
-testb = pd.DataFrame({
-    'sex':[2,2,1,1,1,2,1,2,1,1],
-    'dob':['2012-1-1','2001-12-1','1999-1-1','1998-11-1','2012-11-1','1984-1-1','1982-1-1','1975-1-1','1967-1-1','1954-1-1'],
-    'ssn':[1111,2222,3333,4444,5555,6666,7777,8888,9999,1010],
-    'ln':["as",'ls','zz','rr','wb','wa','tr','tt','ha','gq'],
-    'PROVID
-
-# Run matching
-hm(
-    df_a = testa,
-    df_b = testb,
-    col_a=['sex','dob','ssn','ln'],
-    col_b=['sex','dob','ssn','ln'],
-    match_prob_threshold = 0.001,
-    iteration = 20,
-    model2 = True,
-    blocking_rule_for_input = 'PROVIDER_NUMBER',
-    onetoone = True,
-    match_summary = True
-)
-```
-
-# Webpage
-[healmatcher](https://pypi.org/project/healmatcher/)
```

### Comparing `healmatcher-0.0.3/README.md` & `healmatcher-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `healmatcher-0.0.3/healmatcher.egg-info/PKG-INFO` & `healmatcher-0.0.4/healmatcher.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 Metadata-Version: 2.1
 Name: healmatcher
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast and simple probabilistic data matching package
+Home-page: UNKNOWN
 Author: Joseph Shim github.com/JosephKBS
 Author-email: <joseph.shim.rok@gmail.com>
+License: UNKNOWN
+Description: # healmatcher
+        - `healmatcher` is a simple but fast probabilistic matching package developed by NYULH HEAL Lab.
+        - Currently, the model supports 4 variables (sex, date of birth, last 4 digits of ssn, and first 2 letters of last name) to run the linkage process
+        
+        
+        ## How to use (example)
+        
+        `pip install healmatcher`
+        
+        
+        ```python
+        # Install package
+        !pip install healmatcher
+        
+        # Load package
+        from hm import hm
+        
+        # create example dataset
+        testa = pd.DataFrame({
+            'sex':[1,2,1,2,1,2,1,2,1,2],
+            'dob':['2012-1-1','2011-12-1','1999-1-1','1998-11-1','2012-11-1','1984-1-1','1982-1-1','1975-1-1','1967-1-1','1954-1-1'],
+            'ssn':[1111,2222,3333,4444,5555,6666,7777,8888,9999,1010],
+            'ln':["as",'ss','zz','rr','ww','wa','tr','tt','hh','gq'],
+            'PROVIDER_NUMBER':[2,1,1,1,1,1,1,1,2,1]
+        })
+        testb = pd.DataFrame({
+            'sex':[2,2,1,1,1,2,1,2,1,1],
+            'dob':['2012-1-1','2001-12-1','1999-1-1','1998-11-1','2012-11-1','1984-1-1','1982-1-1','1975-1-1','1967-1-1','1954-1-1'],
+            'ssn':[1111,2222,3333,4444,5555,6666,7777,8888,9999,1010],
+            'ln':["as",'ls','zz','rr','wb','wa','tr','tt','ha','gq'],
+            'PROVID
+        
+        # Run matching
+        hm(
+            df_a = testa,
+            df_b = testb,
+            col_a=['sex','dob','ssn','ln'],
+            col_b=['sex','dob','ssn','ln'],
+            match_prob_threshold = 0.001,
+            iteration = 20,
+            model2 = True,
+            blocking_rule_for_input = 'PROVIDER_NUMBER',
+            onetoone = True,
+            match_summary = True
+        )
+        ```
+        
+        # Webpage
+        [healmatcher](https://pypi.org/project/healmatcher/)
+        
 Keywords: probabilistic match,probabilistic data match,splink
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-
-# healmatcher
-- `healmatcher` is a simple but fast probabilistic matching package developed by NYULH HEAL Lab.
-- Currently, the model supports 4 variables (sex, date of birth, last 4 digits of ssn, and first 2 letters of last name) to run the linkage process
-
-
-## How to use (example)
-
-`pip install healmatcher`
-
-
-```python
-# Install package
-!pip install healmatcher
-
-# Load package
-from hm import hm
-
-# create example dataset
-testa = pd.DataFrame({
-    'sex':[1,2,1,2,1,2,1,2,1,2],
-    'dob':['2012-1-1','2011-12-1','1999-1-1','1998-11-1','2012-11-1','1984-1-1','1982-1-1','1975-1-1','1967-1-1','1954-1-1'],
-    'ssn':[1111,2222,3333,4444,5555,6666,7777,8888,9999,1010],
-    'ln':["as",'ss','zz','rr','ww','wa','tr','tt','hh','gq'],
-    'PROVIDER_NUMBER':[2,1,1,1,1,1,1,1,2,1]
-})
-testb = pd.DataFrame({
-    'sex':[2,2,1,1,1,2,1,2,1,1],
-    'dob':['2012-1-1','2001-12-1','1999-1-1','1998-11-1','2012-11-1','1984-1-1','1982-1-1','1975-1-1','1967-1-1','1954-1-1'],
-    'ssn':[1111,2222,3333,4444,5555,6666,7777,8888,9999,1010],
-    'ln':["as",'ls','zz','rr','wb','wa','tr','tt','ha','gq'],
-    'PROVID
-
-# Run matching
-hm(
-    df_a = testa,
-    df_b = testb,
-    col_a=['sex','dob','ssn','ln'],
-    col_b=['sex','dob','ssn','ln'],
-    match_prob_threshold = 0.001,
-    iteration = 20,
-    model2 = True,
-    blocking_rule_for_input = 'PROVIDER_NUMBER',
-    onetoone = True,
-    match_summary = True
-)
-```
-
-# Webpage
-[healmatcher](https://pypi.org/project/healmatcher/)
```

### Comparing `healmatcher-0.0.3/setup.py` & `healmatcher-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Fast and simple probabilistic data matching package'
 
 # Setting up
 setup(
         name="healmatcher", 
         version=VERSION,
         author="Joseph Shim github.com/JosephKBS",
```

