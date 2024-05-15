# Comparing `tmp/PheTK-0.1.39.tar.gz` & `tmp/PheTK-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PheTK-0.1.39.tar", last modified: Fri May  3 02:32:54 2024, max compression
+gzip compressed data, was "PheTK-0.1.40.tar", last modified: Wed May 15 03:01:46 2024, max compression
```

## Comparing `PheTK-0.1.39.tar` & `PheTK-0.1.40.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-03 02:32:54.343148 PheTK-0.1.39/
--rw-r--r--   0 trantac  (1207383791) 1360859114    35149 2024-03-25 02:28:38.000000 PheTK-0.1.39/LICENSE
--rw-r--r--   0 trantac  (1207383791) 1360859114    16955 2024-05-03 02:32:54.342949 PheTK-0.1.39/PKG-INFO
--rw-r--r--   0 trantac  (1207383791) 1360859114    16673 2024-05-03 02:30:12.000000 PheTK-0.1.39/README.md
--rw-r--r--   0 trantac  (1207383791) 1360859114       38 2024-05-03 02:32:54.343198 PheTK-0.1.39/setup.cfg
--rw-r--r--   0 trantac  (1207383791) 1360859114      950 2024-05-03 02:19:17.000000 PheTK-0.1.39/setup.py
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-03 02:32:54.296621 PheTK-0.1.39/src/
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-03 02:32:54.307269 PheTK-0.1.39/src/PheTK/
--rw-r--r--   0 trantac  (1207383791) 1360859114    16572 2024-03-25 02:28:39.000000 PheTK-0.1.39/src/PheTK/Cohort.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     8713 2024-03-25 02:28:39.000000 PheTK-0.1.39/src/PheTK/Demo.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    28199 2024-04-12 00:30:56.000000 PheTK-0.1.39/src/PheTK/PheWAS.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     5120 2024-04-12 00:30:56.000000 PheTK-0.1.39/src/PheTK/Phecode.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    35458 2024-04-12 00:30:56.000000 PheTK-0.1.39/src/PheTK/Plot.py
--rw-r--r--   0 trantac  (1207383791) 1360859114        0 2024-03-25 02:28:37.000000 PheTK-0.1.39/src/PheTK/__init__.py
--rw-r--r--   0 trantac  (1207383791) 1360859114      526 2024-04-12 02:27:18.000000 PheTK-0.1.39/src/PheTK/_paths.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    10177 2024-04-12 00:30:56.000000 PheTK-0.1.39/src/PheTK/_queries.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     4208 2024-03-25 17:23:44.000000 PheTK-0.1.39/src/PheTK/_utils.py
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-03 02:32:54.337084 PheTK-0.1.39/src/PheTK/phecode/
--rw-r--r--   0 trantac  (1207383791) 1360859114 17510731 2024-03-25 02:28:37.000000 PheTK-0.1.39/src/PheTK/phecode/phecode12.csv
--rw-r--r--   0 trantac  (1207383791) 1360859114 11150857 2024-03-25 02:28:37.000000 PheTK-0.1.39/src/PheTK/phecode/phecodeX.csv
--rw-r--r--   0 trantac  (1207383791) 1360859114  1393896 2024-03-25 02:28:39.000000 PheTK-0.1.39/src/PheTK/phecode/phecodeX_WHO.csv
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-03 02:32:54.310903 PheTK-0.1.39/src/PheTK.egg-info/
--rw-r--r--   0 trantac  (1207383791) 1360859114    16955 2024-05-03 02:32:54.000000 PheTK-0.1.39/src/PheTK.egg-info/PKG-INFO
--rw-r--r--   0 trantac  (1207383791) 1360859114      469 2024-05-03 02:32:54.000000 PheTK-0.1.39/src/PheTK.egg-info/SOURCES.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114        1 2024-05-03 02:32:54.000000 PheTK-0.1.39/src/PheTK.egg-info/dependency_links.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114      120 2024-05-03 02:32:54.000000 PheTK-0.1.39/src/PheTK.egg-info/requires.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114        6 2024-05-03 02:32:54.000000 PheTK-0.1.39/src/PheTK.egg-info/top_level.txt
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.284661 PheTK-0.1.40/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    35149 2024-03-25 02:28:38.000000 PheTK-0.1.40/LICENSE
+-rw-r--r--   0 trantac  (1207383791) 1360859114    17202 2024-05-15 03:01:46.284440 PheTK-0.1.40/PKG-INFO
+-rw-r--r--   0 trantac  (1207383791) 1360859114    16920 2024-05-15 03:00:29.000000 PheTK-0.1.40/README.md
+-rw-r--r--   0 trantac  (1207383791) 1360859114       38 2024-05-15 03:01:46.284758 PheTK-0.1.40/setup.cfg
+-rw-r--r--   0 trantac  (1207383791) 1360859114      950 2024-05-15 03:00:29.000000 PheTK-0.1.40/setup.py
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.239976 PheTK-0.1.40/src/
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.248034 PheTK-0.1.40/src/PheTK/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    16590 2024-05-15 03:00:29.000000 PheTK-0.1.40/src/PheTK/Cohort.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     8713 2024-03-25 02:28:39.000000 PheTK-0.1.40/src/PheTK/Demo.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    28199 2024-05-15 02:39:18.000000 PheTK-0.1.40/src/PheTK/PheWAS.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     5120 2024-05-15 02:39:18.000000 PheTK-0.1.40/src/PheTK/Phecode.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    35458 2024-05-15 02:39:18.000000 PheTK-0.1.40/src/PheTK/Plot.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114        0 2024-03-25 02:28:37.000000 PheTK-0.1.40/src/PheTK/__init__.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114      526 2024-05-12 19:15:55.000000 PheTK-0.1.40/src/PheTK/_paths.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    10177 2024-05-15 02:39:18.000000 PheTK-0.1.40/src/PheTK/_queries.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     4208 2024-03-25 17:23:44.000000 PheTK-0.1.40/src/PheTK/_utils.py
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.277615 PheTK-0.1.40/src/PheTK/phecode/
+-rw-r--r--   0 trantac  (1207383791) 1360859114 17510731 2024-03-25 02:28:37.000000 PheTK-0.1.40/src/PheTK/phecode/phecode12.csv
+-rw-r--r--   0 trantac  (1207383791) 1360859114 11150857 2024-03-25 02:28:37.000000 PheTK-0.1.40/src/PheTK/phecode/phecodeX.csv
+-rw-r--r--   0 trantac  (1207383791) 1360859114  1393896 2024-03-25 02:28:39.000000 PheTK-0.1.40/src/PheTK/phecode/phecodeX_WHO.csv
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-05-15 03:01:46.252902 PheTK-0.1.40/src/PheTK.egg-info/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    17202 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/PKG-INFO
+-rw-r--r--   0 trantac  (1207383791) 1360859114      469 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/SOURCES.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114        1 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/dependency_links.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114      120 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/requires.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114        6 2024-05-15 03:01:46.000000 PheTK-0.1.40/src/PheTK.egg-info/top_level.txt
```

### Comparing `PheTK-0.1.39/LICENSE` & `PheTK-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/PKG-INFO` & `PheTK-0.1.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: PheTK
-Version: 0.1.39
+Version: 0.1.40
 Summary: The Phenotype Toolkit
 Home-page: https://github.com/nhgritctran/PheTK
 Author: Tam Tran
 Author-email: PheTK@mail.nih.gov
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PheTK - The Phenotype Toolkit
 The official repository of PheTK.
 
-Current version: 0.1.39
+Current version: 0.1.40
 
 ## Changelog:
 
+___version 0.1.40 (14 May 2024):___
+- Fixed an incorrect printout text check in `.by_genotype()` in Cohort module when a variant is not found. 
+This is only an aesthetic fix to avoid confusion, and does not affect previously generated cohorts.
+
 ___version 0.1.39 (02 May 2024):___
 - Added lxml as a required dependency during installation as it might not be preinstalled in some platforms.
 
 ___version 0.1.38 (11 Apr 2024):___
-- Updated default _All of Us_ common variant matrix table (ACAF) file path used by .by_genotype() method in Cohort module
+- Updated default _All of Us_ common variant matrix table (ACAF) file path used by `.by_genotype()` method in Cohort module
 with _All of Us_ updated path.
 - Updated README to add some minimum VM configuration suggestions.
 
 ___version 0.1.37 (04 Apr 2024):___
 - Removed SNOMED codes from SQL query (_ehr_dx_code_query_) generating _ehr_length_, _dx_code_occurrence_count_, 
-_dx_condition_count_, and _age_at_last_event_ covariates in _.add_covariates()_ method in Cohort module.
+_dx_condition_count_, and _age_at_last_event_ covariates in `.add_covariates()` method in Cohort module.
   - This was to make it consistent with ICD event query for phecode mapping, 
     i.e., only ICD9CM and ICD10CM would be used as vocabulary_id for these queries.
   - For _All of Us_ users, this change should affect less than 2% of covariate data previously generated 
-  by _.add_covariates()_ method from version 0.1.36 or earlier, and should not significantly change previous analysis results.
+  by `.add_covariates()` method from version 0.1.36 or earlier, and should not significantly change previous analysis results.
 
 ## 1. INSTALLATION
 PheTK can be installed using pip install command in a terminal (Python 3.7 or newer):
 
 ```
 pip install PheTK
 ```
```

### Comparing `PheTK-0.1.39/README.md` & `PheTK-0.1.40/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # PheTK - The Phenotype Toolkit
 The official repository of PheTK.
 
-Current version: 0.1.39
+Current version: 0.1.40
 
 ## Changelog:
 
+___version 0.1.40 (14 May 2024):___
+- Fixed an incorrect printout text check in `.by_genotype()` in Cohort module when a variant is not found. 
+This is only an aesthetic fix to avoid confusion, and does not affect previously generated cohorts.
+
 ___version 0.1.39 (02 May 2024):___
 - Added lxml as a required dependency during installation as it might not be preinstalled in some platforms.
 
 ___version 0.1.38 (11 Apr 2024):___
-- Updated default _All of Us_ common variant matrix table (ACAF) file path used by .by_genotype() method in Cohort module
+- Updated default _All of Us_ common variant matrix table (ACAF) file path used by `.by_genotype()` method in Cohort module
 with _All of Us_ updated path.
 - Updated README to add some minimum VM configuration suggestions.
 
 ___version 0.1.37 (04 Apr 2024):___
 - Removed SNOMED codes from SQL query (_ehr_dx_code_query_) generating _ehr_length_, _dx_code_occurrence_count_, 
-_dx_condition_count_, and _age_at_last_event_ covariates in _.add_covariates()_ method in Cohort module.
+_dx_condition_count_, and _age_at_last_event_ covariates in `.add_covariates()` method in Cohort module.
   - This was to make it consistent with ICD event query for phecode mapping, 
     i.e., only ICD9CM and ICD10CM would be used as vocabulary_id for these queries.
   - For _All of Us_ users, this change should affect less than 2% of covariate data previously generated 
-  by _.add_covariates()_ method from version 0.1.36 or earlier, and should not significantly change previous analysis results.
+  by `.add_covariates()` method from version 0.1.36 or earlier, and should not significantly change previous analysis results.
 
 ## 1. INSTALLATION
 PheTK can be installed using pip install command in a terminal (Python 3.7 or newer):
 
 ```
 pip install PheTK
 ```
```

### Comparing `PheTK-0.1.39/setup.py` & `PheTK-0.1.40/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read contents of the README.md file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PheTK',
-    version='0.1.39',
+    version='0.1.40',
     python_requires='>=3.7',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     package_data={
         '': ['*.*'],
         'PheTK': ['phecode/*'],
     },
```

### Comparing `PheTK-0.1.39/src/PheTK/Cohort.py` & `PheTK-0.1.40/src/PheTK/Cohort.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             print("\033[1mMulti-allelic detected! Splitting...")
             mt = hl.split_multi(mt)
             mt.row.show()
 
         # keep variant of interest
         mt = mt.filter_rows((mt.locus == variant["locus"]) &
                             (mt.alleles == variant["alleles"]))
-        if mt:
+        if mt.count_rows() >= 1:
             print()
             print(f"\033[1mVariant {variant_string} found!")
             mt.row.show()
 
             # export to polars
             spark_df = mt.entries().select("GT").to_spark()
             polars_df = _utils.spark_to_polars(spark_df)
```

### Comparing `PheTK-0.1.39/src/PheTK/Demo.py` & `PheTK-0.1.40/src/PheTK/Demo.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/PheWAS.py` & `PheTK-0.1.40/src/PheTK/PheWAS.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/Phecode.py` & `PheTK-0.1.40/src/PheTK/Phecode.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/Plot.py` & `PheTK-0.1.40/src/PheTK/Plot.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/_paths.py` & `PheTK-0.1.40/src/PheTK/_paths.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/_queries.py` & `PheTK-0.1.40/src/PheTK/_queries.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/_utils.py` & `PheTK-0.1.40/src/PheTK/_utils.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/phecode/phecode12.csv` & `PheTK-0.1.40/src/PheTK/phecode/phecode12.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/phecode/phecodeX.csv` & `PheTK-0.1.40/src/PheTK/phecode/phecodeX.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK/phecode/phecodeX_WHO.csv` & `PheTK-0.1.40/src/PheTK/phecode/phecodeX_WHO.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.39/src/PheTK.egg-info/PKG-INFO` & `PheTK-0.1.40/src/PheTK.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: PheTK
-Version: 0.1.39
+Version: 0.1.40
 Summary: The Phenotype Toolkit
 Home-page: https://github.com/nhgritctran/PheTK
 Author: Tam Tran
 Author-email: PheTK@mail.nih.gov
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PheTK - The Phenotype Toolkit
 The official repository of PheTK.
 
-Current version: 0.1.39
+Current version: 0.1.40
 
 ## Changelog:
 
+___version 0.1.40 (14 May 2024):___
+- Fixed an incorrect printout text check in `.by_genotype()` in Cohort module when a variant is not found. 
+This is only an aesthetic fix to avoid confusion, and does not affect previously generated cohorts.
+
 ___version 0.1.39 (02 May 2024):___
 - Added lxml as a required dependency during installation as it might not be preinstalled in some platforms.
 
 ___version 0.1.38 (11 Apr 2024):___
-- Updated default _All of Us_ common variant matrix table (ACAF) file path used by .by_genotype() method in Cohort module
+- Updated default _All of Us_ common variant matrix table (ACAF) file path used by `.by_genotype()` method in Cohort module
 with _All of Us_ updated path.
 - Updated README to add some minimum VM configuration suggestions.
 
 ___version 0.1.37 (04 Apr 2024):___
 - Removed SNOMED codes from SQL query (_ehr_dx_code_query_) generating _ehr_length_, _dx_code_occurrence_count_, 
-_dx_condition_count_, and _age_at_last_event_ covariates in _.add_covariates()_ method in Cohort module.
+_dx_condition_count_, and _age_at_last_event_ covariates in `.add_covariates()` method in Cohort module.
   - This was to make it consistent with ICD event query for phecode mapping, 
     i.e., only ICD9CM and ICD10CM would be used as vocabulary_id for these queries.
   - For _All of Us_ users, this change should affect less than 2% of covariate data previously generated 
-  by _.add_covariates()_ method from version 0.1.36 or earlier, and should not significantly change previous analysis results.
+  by `.add_covariates()` method from version 0.1.36 or earlier, and should not significantly change previous analysis results.
 
 ## 1. INSTALLATION
 PheTK can be installed using pip install command in a terminal (Python 3.7 or newer):
 
 ```
 pip install PheTK
 ```
```

