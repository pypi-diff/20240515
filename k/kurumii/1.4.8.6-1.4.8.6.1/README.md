# Comparing `tmp/kurumii-1.4.8.6.tar.gz` & `tmp/kurumii-1.4.8.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurumii-1.4.8.6.tar", last modified: Tue May 14 12:38:01 2024, max compression
+gzip compressed data, was "kurumii-1.4.8.6.1.tar", last modified: Wed May 15 16:02:55 2024, max compression
```

## Comparing `kurumii-1.4.8.6.tar` & `kurumii-1.4.8.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 12:38:01.722028 kurumii-1.4.8.6/
--rw-rw-rw-   0        0        0      309 2024-05-14 12:38:01.722028 kurumii-1.4.8.6/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 12:38:01.707311 kurumii-1.4.8.6/kurumii/
--rw-rw-rw-   0        0        0     4003 2024-05-14 12:36:01.000000 kurumii-1.4.8.6/kurumii/__init__.py
--rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8.6/kurumii/additional_functions.py
--rw-rw-rw-   0        0        0      805 2024-05-14 12:35:38.000000 kurumii-1.4.8.6/kurumii/api_request.py
--rw-rw-rw-   0        0        0    15433 2024-05-13 11:39:32.000000 kurumii-1.4.8.6/kurumii/ascii.py
--rw-rw-rw-   0        0        0    46861 2024-05-12 11:40:47.000000 kurumii-1.4.8.6/kurumii/colors.py
--rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8.6/kurumii/data_manipulation.py
--rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 kurumii-1.4.8.6/kurumii/database.py
--rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8.6/kurumii/files.py
--rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8.6/kurumii/id.py
--rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8.6/kurumii/jsonify.py
--rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8.6/kurumii/keyboard.py
--rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8.6/kurumii/print_additions.py
--rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8.6/kurumii/profanities.py
--rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8.6/kurumii/youtube.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:38:01.719723 kurumii-1.4.8.6/kurumii.egg-info/
--rw-rw-rw-   0        0        0      309 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 12:38:01.722028 kurumii-1.4.8.6/setup.cfg
--rw-rw-rw-   0        0        0      388 2024-05-14 12:37:57.000000 kurumii-1.4.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:02:55.676751 kurumii-1.4.8.6.1/
+-rw-rw-rw-   0        0        0      311 2024-05-15 16:02:55.675765 kurumii-1.4.8.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 16:02:55.658800 kurumii-1.4.8.6.1/kurumii/
+-rw-rw-rw-   0        0        0     4003 2024-05-14 12:36:01.000000 kurumii-1.4.8.6.1/kurumii/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8.6.1/kurumii/additional_functions.py
+-rw-rw-rw-   0        0        0      805 2024-05-14 12:35:38.000000 kurumii-1.4.8.6.1/kurumii/api_request.py
+-rw-rw-rw-   0        0        0    15433 2024-05-13 11:39:32.000000 kurumii-1.4.8.6.1/kurumii/ascii.py
+-rw-rw-rw-   0        0        0    46884 2024-05-15 16:01:28.000000 kurumii-1.4.8.6.1/kurumii/colors.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8.6.1/kurumii/data_manipulation.py
+-rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 kurumii-1.4.8.6.1/kurumii/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8.6.1/kurumii/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8.6.1/kurumii/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8.6.1/kurumii/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8.6.1/kurumii/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8.6.1/kurumii/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8.6.1/kurumii/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8.6.1/kurumii/youtube.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:02:55.672762 kurumii-1.4.8.6.1/kurumii.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-05-15 16:02:55.000000 kurumii-1.4.8.6.1/kurumii.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-15 16:02:55.000000 kurumii-1.4.8.6.1/kurumii.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:02:55.000000 kurumii-1.4.8.6.1/kurumii.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-15 16:02:55.000000 kurumii-1.4.8.6.1/kurumii.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 16:02:55.000000 kurumii-1.4.8.6.1/kurumii.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 16:02:55.676751 kurumii-1.4.8.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      390 2024-05-15 16:01:41.000000 kurumii-1.4.8.6.1/setup.py
```

### Comparing `kurumii-1.4.8.6/kurumii/__init__.py` & `kurumii-1.4.8.6.1/kurumii/__init__.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/additional_functions.py` & `kurumii-1.4.8.6.1/kurumii/additional_functions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/api_request.py` & `kurumii-1.4.8.6.1/kurumii/api_request.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/ascii.py` & `kurumii-1.4.8.6.1/kurumii/ascii.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/colors.py` & `kurumii-1.4.8.6.1/kurumii/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1298,15 +1298,15 @@
                 response = input(f"No colors under '{color_name}' found. Did you mean '{suggestion}'? (yes/no): ")
                 if "y" in response.lower():
                     return (f"No colors under '{color_name}' found. Did you mean '{suggestion}'?", suggestion)
                 else:
                     return (f"No colors under '{color_name}' found.", suggestion)
             else:
                 return (f"No colors under '{color_name}' found. Did you mean '{suggestion}'?", suggestion)
-    return (f"No colors under '{color_name}' found.", None)
+    return (f"No colors under '{color_name}' found.", "No color suggestion found")
 
 
 def verify_hex_color(color_code):
     """
     Verify if the input string represents a hexadecimal color code.
 
     Args:
```

### Comparing `kurumii-1.4.8.6/kurumii/data_manipulation.py` & `kurumii-1.4.8.6.1/kurumii/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/database.py` & `kurumii-1.4.8.6.1/kurumii/database.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/files.py` & `kurumii-1.4.8.6.1/kurumii/files.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/id.py` & `kurumii-1.4.8.6.1/kurumii/id.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/jsonify.py` & `kurumii-1.4.8.6.1/kurumii/jsonify.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/keyboard.py` & `kurumii-1.4.8.6.1/kurumii/keyboard.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/print_additions.py` & `kurumii-1.4.8.6.1/kurumii/print_additions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/profanities.py` & `kurumii-1.4.8.6.1/kurumii/profanities.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.6/kurumii/youtube.py` & `kurumii-1.4.8.6.1/kurumii/youtube.py`

 * *Files identical despite different names*

