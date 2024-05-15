# Comparing `tmp/sarcharts-0.1.9.tar.gz` & `tmp/sarcharts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.1.9.tar", last modified: Tue May 14 15:42:44 2024, max compression
+gzip compressed data, was "sarcharts-0.2.0.tar", last modified: Tue May 14 15:54:05 2024, max compression
```

## Comparing `sarcharts-0.1.9.tar` & `sarcharts-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.460326 sarcharts-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.464326 sarcharts-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 15:42:39.000000 sarcharts-0.1.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-14 15:42:39.000000 sarcharts-0.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:42:44.000000 sarcharts-0.1.9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 15:42:44.000000 sarcharts-0.1.9/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 15:42:39.000000 sarcharts-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-14 15:42:44.468326 sarcharts-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 15:42:39.000000 sarcharts-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.464326 sarcharts-0.1.9/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 15:42:39.000000 sarcharts-0.1.9/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-14 15:42:39.000000 sarcharts-0.1.9/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 15:42:39.000000 sarcharts-0.1.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.464326 sarcharts-0.1.9/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.464326 sarcharts-0.1.9/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/css/sarcharts.css
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/css/ul-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/html/img/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/img/chevron.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/ul-select.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 15:42:44.472326 sarcharts-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 15:42:39.000000 sarcharts-0.1.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-14 15:42:39.000000 sarcharts-0.1.9/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-14 15:42:39.000000 sarcharts-0.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.920699 sarcharts-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.924699 sarcharts-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 15:54:00.000000 sarcharts-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-14 15:54:00.000000 sarcharts-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:54:05.000000 sarcharts-0.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 15:54:05.000000 sarcharts-0.2.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 15:54:00.000000 sarcharts-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-14 15:54:05.928699 sarcharts-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 15:54:00.000000 sarcharts-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.924699 sarcharts-0.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 15:54:00.000000 sarcharts-0.2.0/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-14 15:54:00.000000 sarcharts-0.2.0/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 15:54:00.000000 sarcharts-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.924699 sarcharts-0.2.0/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.920699 sarcharts-0.2.0/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/css/sarcharts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/css/ul-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/html/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/img/chevron.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/html/js/ul-select.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-14 15:54:00.000000 sarcharts-0.2.0/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:54:05.928699 sarcharts-0.2.0/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 15:54:05.000000 sarcharts-0.2.0/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 15:54:05.928699 sarcharts-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 15:54:00.000000 sarcharts-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-14 15:54:00.000000 sarcharts-0.2.0/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-14 15:54:00.000000 sarcharts-0.2.0/tox.ini
```

### Comparing `sarcharts-0.1.9/.github/workflows/python-publish.yml` & `sarcharts-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/.pylintrc` & `sarcharts-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/LICENSE` & `sarcharts-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/PKG-INFO` & `sarcharts-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.9
+Version: 0.2.0
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.1.9/README.md` & `sarcharts-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/doc/README.md` & `sarcharts-0.2.0/doc/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/doc/sarcharts.png` & `sarcharts-0.2.0/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/__init__.py` & `sarcharts-0.2.0/sarcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/html/css/sarcharts.css` & `sarcharts-0.2.0/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/html/css/ul-select.css` & `sarcharts-0.2.0/sarcharts/html/css/ul-select.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/html/js/chart.umd.js` & `sarcharts-0.2.0/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.2.0/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/html/js/hammer.min.js` & `sarcharts-0.2.0/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/html/js/jquery.js` & `sarcharts-0.2.0/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/html/js/ul-select.js` & `sarcharts-0.2.0/sarcharts/html/js/ul-select.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/lib/chartjs.py` & `sarcharts-0.2.0/sarcharts/lib/chartjs.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/lib/progressbar.py` & `sarcharts-0.2.0/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/lib/sadf.py` & `sarcharts-0.2.0/sarcharts/lib/sadf.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/lib/util.py` & `sarcharts-0.2.0/sarcharts/lib/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,14 +73,11 @@
         return datetime.datetime.strptime(d, format)
     except ValueError:
         debug(args, 'E', f"ERROR: date '{d}' doesn't match {format}.")
 
 
 def in_date_range(args, d):
     d = valid_date(args, d)
-    print(args.fromdate)
     if d >= args.fromdate and d <= args.todate:
-        print("si")
         return True
     else:
-        print("no")
         return False
```

### Comparing `sarcharts-0.1.9/sarcharts/templates/chart.html` & `sarcharts-0.2.0/sarcharts/templates/chart.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts/templates/header.html` & `sarcharts-0.2.0/sarcharts/templates/header.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.2.0/sarcharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.9
+Version: 0.2.0
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.1.9/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.2.0/sarcharts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/setup.cfg` & `sarcharts-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/setup.py` & `sarcharts-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.9/tox.ini` & `sarcharts-0.2.0/tox.ini`

 * *Files identical despite different names*

