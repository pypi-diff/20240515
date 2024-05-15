# Comparing `tmp/brynq_sdk_leapsome-1.0.4.tar.gz` & `tmp/brynq_sdk_leapsome-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_leapsome-1.0.4.tar", last modified: Wed Apr 24 13:20:15 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_leapsome-1.0.5.tar", last modified: Wed May 15 10:11:57 2024, max compression
```

## Comparing `brynq_sdk_leapsome-1.0.4.tar` & `brynq_sdk_leapsome-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk/leapsome/
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-24 13:19:59.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk/leapsome/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4859 2024-04-24 13:19:59.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk/leapsome/api_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2024-04-24 13:19:59.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk/leapsome/sftp_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk_leapsome.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk_leapsome.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      362 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk_leapsome.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk_leapsome.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk_leapsome.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk_leapsome.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/brynq_sdk_leapsome.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 13:20:15.000000 brynq_sdk_leapsome-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-24 13:19:59.000000 brynq_sdk_leapsome-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk/leapsome/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-05-15 10:11:39.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk/leapsome/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5300 2024-05-15 10:11:39.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk/leapsome/api_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2024-05-15 10:11:39.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk/leapsome/sftp_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk_leapsome.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk_leapsome.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      362 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk_leapsome.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk_leapsome.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk_leapsome.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk_leapsome.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/brynq_sdk_leapsome.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 10:11:57.000000 brynq_sdk_leapsome-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-05-15 10:11:39.000000 brynq_sdk_leapsome-1.0.5/setup.py
```

### Comparing `brynq_sdk_leapsome-1.0.4/brynq_sdk/leapsome/api_interface.py` & `brynq_sdk_leapsome-1.0.5/brynq_sdk/leapsome/api_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,10 +84,19 @@
         df_contributors = df[['id', 'contributors']].copy()
         df_contributors = df_contributors.explode('contributors')
         df_contributors = pd.concat([df_contributors.drop(['contributors'], axis=1), df_contributors['contributors'].apply(pd.Series)], axis=1)
         df_contributors = df_contributors.drop(df_contributors.columns[-1], axis=1)
         df_contributors.reset_index(inplace=True, drop=True)
         df_contributors.columns.values[1] = 'user_id'
 
-        df = df.drop(columns=['keyResults', 'contributors'])
+        # And for tags
+        df_tags = df[['id', 'tags']].copy()
+        df_tags = df_tags.explode('tags')
+        df_tags = pd.concat([df_tags.drop(['tags'], axis=1), df_tags['tags'].apply(pd.Series)], axis=1)
+        df_tags = df_tags.drop(df_tags.columns[1], axis=1)
+        df_tags.columns.values[0] = 'objective_id'
+        df_tags = df_tags[df_tags['id'].notna()].copy()
+        df_tags.reset_index(inplace=True, drop=True)
+
+        df = df.drop(columns=['keyResults', 'contributors', 'tags'])
 
         return df, df_key_results, df_contributors
```

### Comparing `brynq_sdk_leapsome-1.0.4/brynq_sdk/leapsome/sftp_interface.py` & `brynq_sdk_leapsome-1.0.5/brynq_sdk/leapsome/sftp_interface.py`

 * *Files identical despite different names*

