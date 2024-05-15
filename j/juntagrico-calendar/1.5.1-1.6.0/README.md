# Comparing `tmp/juntagrico_calendar-1.5.1.tar.gz` & `tmp/juntagrico_calendar-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juntagrico_calendar-1.5.1.tar", last modified: Sat Mar  5 18:14:39 2022, max compression
+gzip compressed data, was "juntagrico_calendar-1.6.0.tar", last modified: Wed May 15 21:09:37 2024, max compression
```

## Comparing `juntagrico_calendar-1.5.1.tar` & `juntagrico_calendar-1.6.0.tar`

### file list

```diff
@@ -1,57 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.263219 juntagrico_calendar-1.5.1/juntagrico_calendar/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/dao/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/dao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/entity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/juntagricoapp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.263219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3881 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/css/jobcalendar.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.263219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.263219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/bootstrap/main.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/bootstrap/main.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/core/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/core/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/core/locales/de.js
--rw-r--r--   0 runner    (1001) docker     (121)    14357 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/core/main.min.css
--rw-r--r--   0 runner    (1001) docker     (121)   126428 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/core/main.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/daygrid/
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    27128 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/list/
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/list/main.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     6209 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/list/main.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     6588 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/static/js/jobcalendar.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.263219 juntagrico_calendar-1.5.1/juntagrico_calendar/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/templates/cal/
--rwxr-xr-x   0 runner    (1001) docker     (121)      405 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/templates/cal/job_calendar.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/templates/cal/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/templates/cal/snippets/content_snippet.html
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/templates/cal/snippets/scripts_snippet.html
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/templates/cal/snippets/styles_snippet.html
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/util/temporal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2875 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/juntagrico_calendar/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/juntagrico_calendar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-03-05 18:14:39.000000 juntagrico_calendar-1.5.1/juntagrico_calendar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-03-05 18:14:39.000000 juntagrico_calendar-1.5.1/juntagrico_calendar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-05 18:14:39.000000 juntagrico_calendar-1.5.1/juntagrico_calendar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-05 18:14:39.000000 juntagrico_calendar-1.5.1/juntagrico_calendar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-03-05 18:14:39.000000 juntagrico_calendar-1.5.1/juntagrico_calendar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-05 18:14:39.267219 juntagrico_calendar-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-03-05 18:14:24.000000 juntagrico_calendar-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.433444 juntagrico_calendar-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-05-15 21:09:37.433444 juntagrico_calendar-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.425444 juntagrico_calendar-1.6.0/juntagrico_calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.425444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/css/jobcalendar.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.425444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.425444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/bootstrap/main.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/bootstrap/main.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/core/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/core/locales/de.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14357 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/core/main.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   126428 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/core/main.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/daygrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    27128 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/list/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/list/main.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/list/main.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/static/js/jobcalendar.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.425444 juntagrico_calendar-1.6.0/juntagrico_calendar/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/templates/cal/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/templates/cal/job_calendar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/templates/cal/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/templates/cal/snippets/content_snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/templates/cal/snippets/scripts_snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/templates/cal/snippets/styles_snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/util/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/juntagrico_calendar/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:09:37.429444 juntagrico_calendar-1.6.0/juntagrico_calendar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-05-15 21:09:37.000000 juntagrico_calendar-1.6.0/juntagrico_calendar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-15 21:09:37.000000 juntagrico_calendar-1.6.0/juntagrico_calendar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:09:37.000000 juntagrico_calendar-1.6.0/juntagrico_calendar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:09:37.000000 juntagrico_calendar-1.6.0/juntagrico_calendar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 21:09:37.000000 juntagrico_calendar-1.6.0/juntagrico_calendar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 21:09:23.000000 juntagrico_calendar-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:09:37.433444 juntagrico_calendar-1.6.0/setup.cfg
```

### Comparing `juntagrico_calendar-1.5.1/LICENSE` & `juntagrico_calendar-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/css/jobcalendar.css` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/css/jobcalendar.css`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/bootstrap/main.min.js` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/bootstrap/main.min.js`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/core/locales/de.js` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/core/locales/de.js`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/core/main.min.css` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/core/main.min.css`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/core/main.min.js` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/core/main.min.js`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.css` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.css`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.js` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.js`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/list/main.min.css` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/list/main.min.css`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/external/fullcalendar/list/main.min.js` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/external/fullcalendar/list/main.min.js`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/static/js/jobcalendar.js` & `juntagrico_calendar-1.6.0/juntagrico_calendar/static/js/jobcalendar.js`

 * *Files identical despite different names*

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar/views.py` & `juntagrico_calendar-1.6.0/juntagrico_calendar/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     print(now)
     start = get_datetime_from_iso8601_string(request.GET.get('start'),  now)
     end = get_datetime_from_iso8601_string(request.GET.get('end'), start + timedelta(days=7))
     search = request.GET.get('search')
 
     if search is None:
         jobs = Job.objects.filter(time__range=(start, end))
-    elif search is not '':
+    elif search != '':
         # if search term is passed, only search in parts, that frontend can't find
         jobtypes = JobType.objects.filter(recuringjob__time__range=(start, end))\
             .distinct().filter(description__iregex=search)
         rjobs = RecuringJob.objects.filter(time__range=(start, end), type__in=jobtypes)
         otjobs = OneTimeJob.objects.filter(time__range=(start, end), description__iregex=search)
         jobs = list(otjobs) + list(rjobs)
     else:
```

### Comparing `juntagrico_calendar-1.5.1/juntagrico_calendar.egg-info/SOURCES.txt` & `juntagrico_calendar-1.6.0/juntagrico_calendar.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
-setup.py
 juntagrico_calendar/__init__.py
-juntagrico_calendar/admin.py
-juntagrico_calendar/juntagricoapp.py
+juntagrico_calendar/apps.py
 juntagrico_calendar/urls.py
 juntagrico_calendar/views.py
 juntagrico_calendar.egg-info/PKG-INFO
 juntagrico_calendar.egg-info/SOURCES.txt
 juntagrico_calendar.egg-info/dependency_links.txt
 juntagrico_calendar.egg-info/requires.txt
 juntagrico_calendar.egg-info/top_level.txt
-juntagrico_calendar/dao/__init__.py
-juntagrico_calendar/entity/__init__.py
-juntagrico_calendar/migrations/__init__.py
 juntagrico_calendar/static/css/jobcalendar.css
 juntagrico_calendar/static/external/fullcalendar/bootstrap/main.min.css
 juntagrico_calendar/static/external/fullcalendar/bootstrap/main.min.js
 juntagrico_calendar/static/external/fullcalendar/core/main.min.css
 juntagrico_calendar/static/external/fullcalendar/core/main.min.js
 juntagrico_calendar/static/external/fullcalendar/core/locales/de.js
 juntagrico_calendar/static/external/fullcalendar/daygrid/main.min.css
```

