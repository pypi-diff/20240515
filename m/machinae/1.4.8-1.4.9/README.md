# Comparing `tmp/machinae-1.4.8.tar.gz` & `tmp/machinae-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/machinae-1.4.8.tar", last modified: Thu May  9 12:48:11 2019, max compression
+gzip compressed data, was "dist/machinae-1.4.9.tar", last modified: Wed Nov 25 23:07:42 2020, max compression
```

## Comparing `machinae-1.4.8.tar` & `machinae-1.4.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-09 12:48:11.000000 machinae-1.4.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12349 2019-05-09 12:47:12.000000 machinae-1.4.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1409 2019-05-09 12:47:12.000000 machinae-1.4.8/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-05-09 12:48:11.000000 machinae-1.4.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    15595 2019-05-09 12:48:11.000000 machinae-1.4.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-09 12:48:11.000000 machinae-1.4.8/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8572 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6683 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/outputs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2021 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae/sites/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2784 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/sites/html.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2020 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/sites/csv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6854 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/sites/json.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/sites/ipwhois.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2836 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/sites/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/sites/rss.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5677 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/sites/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1696 2019-05-09 12:47:12.000000 machinae-1.4.8/src/machinae/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    15595 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      556 2019-05-09 12:48:11.000000 machinae-1.4.8/src/machinae.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-25 23:07:42.000000 machinae-1.4.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15729 2020-11-25 23:07:42.000000 machinae-1.4.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12459 2020-11-25 23:07:01.000000 machinae-1.4.9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-11-25 23:07:42.000000 machinae-1.4.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1409 2020-11-25 23:07:01.000000 machinae-1.4.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-25 23:07:42.000000 machinae-1.4.9/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-25 23:07:42.000000 machinae-1.4.9/src/machinae/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2021 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8572 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6683 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/outputs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-25 23:07:42.000000 machinae-1.4.9/src/machinae/sites/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2836 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/sites/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5677 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/sites/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2020 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/sites/csv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2784 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/sites/html.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/sites/ipwhois.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6861 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/sites/json.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/sites/rss.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1696 2020-11-25 23:07:01.000000 machinae-1.4.9/src/machinae/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-25 23:07:42.000000 machinae-1.4.9/src/machinae.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15729 2020-11-25 23:07:41.000000 machinae-1.4.9/src/machinae.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      556 2020-11-25 23:07:42.000000 machinae-1.4.9/src/machinae.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-25 23:07:41.000000 machinae-1.4.9/src/machinae.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-11-25 23:07:41.000000 machinae-1.4.9/src/machinae.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-25 23:07:41.000000 machinae-1.4.9/src/machinae.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      116 2020-11-25 23:07:41.000000 machinae-1.4.9/src/machinae.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-11-25 23:07:41.000000 machinae-1.4.9/src/machinae.egg-info/top_level.txt
```

### Comparing `machinae-1.4.8/README.md` & `machinae-1.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -236,19 +236,22 @@
 - Add option for per-otype request settings
 - Add custom per-site output for error codes
 
 
 Version History
 ---------------
 
+### Version 1.4.9 (2020-11-25) ###
+- Fix bug in JSON as_time processing when time is an epoch time, but str type
+
 ### Version 1.4.1 (2018-08-31) ###
 - New Features
     - Automatically Defangs output
     - MISP Support (example added to machinae.yml)
-    
+
 ### Version 1.4.0 (2016-04-20) ###
 - New features
     - "-a"/"--auth" option for passing an auth config file
         - Thanks johannestaas for the submission
     - "-H"/"--http-proxy" option, and environment support, for HTTP proxies
 - New sites
     - Passivetotal (various forms, thanks johannestaas)
```

### Comparing `machinae-1.4.8/setup.py` & `machinae-1.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #this should hopefully allow us to have a more pypi friendly, always up to date readme
 readMeDir = path.abspath(path.dirname(__file__))
 with open(path.join(readMeDir, 'README.md'), encoding='utf-8') as readFile:
     long_desc = readFile.read()
 
 
-VERSION = '1.4.8'
+VERSION = '1.4.9'
 
 setup(
     name='machinae',
     version=VERSION,
     author='Steve McMaster',
     author_email='mcmaster@hurricanelabs.com',
     package_dir={'': 'src'},
```

### Comparing `machinae-1.4.8/PKG-INFO` & `machinae-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machinae
-Version: 1.4.8
+Version: 1.4.9
 Summary: Machinae Security Intelligence Collector
 Home-page: http://hurricanelabs.github.io/machinae/
 Author: Steve McMaster
 Author-email: mcmaster@hurricanelabs.com
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/HurricaneLabs/machinae.svg?branch=master)](https://travis-ci.org/HurricaneLabs/machinae)
         [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/2344/badge)](https://bestpractices.coreinfrastructure.org/projects/2344)
@@ -244,19 +244,22 @@
         - Add option for per-otype request settings
         - Add custom per-site output for error codes
         
         
         Version History
         ---------------
         
+        ### Version 1.4.9 (2020-11-25) ###
+        - Fix bug in JSON as_time processing when time is an epoch time, but str type
+        
         ### Version 1.4.1 (2018-08-31) ###
         - New Features
             - Automatically Defangs output
             - MISP Support (example added to machinae.yml)
-            
+        
         ### Version 1.4.0 (2016-04-20) ###
         - New features
             - "-a"/"--auth" option for passing an auth config file
                 - Thanks johannestaas for the submission
             - "-H"/"--http-proxy" option, and environment support, for HTTP proxies
         - New sites
             - Passivetotal (various forms, thanks johannestaas)
```

### Comparing `machinae-1.4.8/src/machinae/cmd.py` & `machinae-1.4.9/src/machinae/cmd.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/outputs.py` & `machinae-1.4.9/src/machinae/outputs.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/__init__.py` & `machinae-1.4.9/src/machinae/__init__.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/sites/html.py` & `machinae-1.4.9/src/machinae/sites/html.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/sites/csv.py` & `machinae-1.4.9/src/machinae/sites/csv.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/sites/json.py` & `machinae-1.4.9/src/machinae/sites/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 )
 
             if "format" in parser:
                 if parser["format"] == "as_list":
                     val = ", ".join(map(str, val))
                 elif parser["format"] == "as_time":
                     try:
-                        dt = datetime.datetime.fromtimestamp(val)
+                        dt = datetime.datetime.fromtimestamp(float(val))
                     #pylint: disable=bare-except
                     #Will be cleaned up in future refactor -- I hate mcmaster
                     except:
                         dt = parse(val)
                     val = dt.isoformat()
             result_dict[key] = val
```

### Comparing `machinae-1.4.8/src/machinae/sites/ipwhois.py` & `machinae-1.4.9/src/machinae/sites/ipwhois.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/sites/__init__.py` & `machinae-1.4.9/src/machinae/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/sites/rss.py` & `machinae-1.4.9/src/machinae/sites/rss.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/sites/base.py` & `machinae-1.4.9/src/machinae/sites/base.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae/utils.py` & `machinae-1.4.9/src/machinae/utils.py`

 * *Files identical despite different names*

### Comparing `machinae-1.4.8/src/machinae.egg-info/PKG-INFO` & `machinae-1.4.9/src/machinae.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machinae
-Version: 1.4.8
+Version: 1.4.9
 Summary: Machinae Security Intelligence Collector
 Home-page: http://hurricanelabs.github.io/machinae/
 Author: Steve McMaster
 Author-email: mcmaster@hurricanelabs.com
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/HurricaneLabs/machinae.svg?branch=master)](https://travis-ci.org/HurricaneLabs/machinae)
         [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/2344/badge)](https://bestpractices.coreinfrastructure.org/projects/2344)
@@ -244,19 +244,22 @@
         - Add option for per-otype request settings
         - Add custom per-site output for error codes
         
         
         Version History
         ---------------
         
+        ### Version 1.4.9 (2020-11-25) ###
+        - Fix bug in JSON as_time processing when time is an epoch time, but str type
+        
         ### Version 1.4.1 (2018-08-31) ###
         - New Features
             - Automatically Defangs output
             - MISP Support (example added to machinae.yml)
-            
+        
         ### Version 1.4.0 (2016-04-20) ###
         - New features
             - "-a"/"--auth" option for passing an auth config file
                 - Thanks johannestaas for the submission
             - "-H"/"--http-proxy" option, and environment support, for HTTP proxies
         - New sites
             - Passivetotal (various forms, thanks johannestaas)
```

### Comparing `machinae-1.4.8/src/machinae.egg-info/SOURCES.txt` & `machinae-1.4.9/src/machinae.egg-info/SOURCES.txt`

 * *Files identical despite different names*

