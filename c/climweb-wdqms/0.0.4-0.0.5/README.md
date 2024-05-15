# Comparing `tmp/climweb_wdqms-0.0.4.tar.gz` & `tmp/climweb_wdqms-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climweb_wdqms-0.0.4.tar", last modified: Tue May 14 22:14:18 2024, max compression
+gzip compressed data, was "climweb_wdqms-0.0.5.tar", last modified: Wed May 15 11:55:07 2024, max compression
```

## Comparing `climweb_wdqms-0.0.4.tar` & `climweb_wdqms-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:18.078684 climweb_wdqms-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-14 22:14:18.078684 climweb_wdqms-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:18.074684 climweb_wdqms-0.0.4/climweb_wdqms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:18.074684 climweb_wdqms-0.0.4/climweb_wdqms/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:18.074684 climweb_wdqms-0.0.4/climweb_wdqms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/management/commands/fetch_transmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:18.078684 climweb_wdqms-0.0.4/climweb_wdqms/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/climweb_wdqms/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:14:18.078684 climweb_wdqms-0.0.4/climweb_wdqms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-14 22:14:18.000000 climweb_wdqms-0.0.4/climweb_wdqms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-14 22:14:18.000000 climweb_wdqms-0.0.4/climweb_wdqms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 22:14:18.000000 climweb_wdqms-0.0.4/climweb_wdqms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 22:14:18.000000 climweb_wdqms-0.0.4/climweb_wdqms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 22:14:18.000000 climweb_wdqms-0.0.4/climweb_wdqms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 22:14:14.000000 climweb_wdqms-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-14 22:14:18.078684 climweb_wdqms-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/management/commands/fetch_transmissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 11:55:07.971765 climweb_wdqms-0.0.5/setup.cfg
```

### Comparing `climweb_wdqms-0.0.4/PKG-INFO` & `climweb_wdqms-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climweb-wdqms
-Version: 0.0.4
+Version: 0.0.5
 Summary: National level WDQMS Summary tool
 Home-page: https://github.com/wmo-raf/climweb-wdqms
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `climweb_wdqms-0.0.4/climweb_wdqms/management/commands/fetch_transmissions.py` & `climweb_wdqms-0.0.5/climweb_wdqms/management/commands/fetch_transmissions.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.4/climweb_wdqms/migrations/0001_initial.py` & `climweb_wdqms-0.0.5/climweb_wdqms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.4/climweb_wdqms/models.py` & `climweb_wdqms-0.0.5/climweb_wdqms/models.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.4/climweb_wdqms/serializers.py` & `climweb_wdqms-0.0.5/climweb_wdqms/serializers.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.4/climweb_wdqms/urls.py` & `climweb_wdqms-0.0.5/climweb_wdqms/urls.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.4/climweb_wdqms/views.py` & `climweb_wdqms-0.0.5/climweb_wdqms/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
         # Aggregate data by month and calculate average received rate
         monthly_data = Transmission.objects.filter(received_date__month=month,
             received_date__year=year, variable=variable
         ).annotate(
             month=TruncMonth('received_date')
         ).values(
-            'month','station__name', 'variable'
+            'month','station__name', 'variable', 'station__wigos_id'
         ).annotate(
             average_received_rate=Avg('received_rate'),
             station_geometry=F('station__geom'),  # Access the geometry field
 
         )
 
         # Convert queryset to list of dictionaries
@@ -259,15 +259,16 @@
             average_received_rate = float(data['average_received_rate']) if data['average_received_rate'] is not None else None
 
             geometry = json.loads(data['station_geometry'].geojson)
 
             feature = {
                 "type": "Feature",
                 "properties": {
-                    "station_name": data['station__name'],
+                    "name": data['station__name'],
+                    "wigos_id": data['station__wigos_id'],
                     "month": data['month'].strftime('%Y-%m'),
                     "variable": data['variable'],
                     "average_received_rate": average_received_rate
                 },
                 "geometry": geometry
             }
             feature_collection["features"].append(feature)
```

### Comparing `climweb_wdqms-0.0.4/climweb_wdqms.egg-info/PKG-INFO` & `climweb_wdqms-0.0.5/climweb_wdqms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climweb-wdqms
-Version: 0.0.4
+Version: 0.0.5
 Summary: National level WDQMS Summary tool
 Home-page: https://github.com/wmo-raf/climweb-wdqms
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `climweb_wdqms-0.0.4/climweb_wdqms.egg-info/SOURCES.txt` & `climweb_wdqms-0.0.5/climweb_wdqms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.4/setup.cfg` & `climweb_wdqms-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climweb-wdqms
-version = 0.0.4
+version = 0.0.5
 description = National level WDQMS Summary tool
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/climweb-wdqms
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

