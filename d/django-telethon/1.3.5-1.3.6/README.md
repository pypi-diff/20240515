# Comparing `tmp/django_telethon-1.3.5.tar.gz` & `tmp/django_telethon-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_telethon-1.3.5.tar", last modified: Wed May 15 20:43:03 2024, max compression
+gzip compressed data, was "django_telethon-1.3.6.tar", last modified: Wed May 15 20:46:51 2024, max compression
```

## Comparing `django_telethon-1.3.5.tar` & `django_telethon-1.3.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:03.962345 django_telethon-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 20:43:00.000000 django_telethon-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 20:43:00.000000 django_telethon-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-15 20:43:03.962345 django_telethon-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-15 20:43:00.000000 django_telethon-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:03.958345 django_telethon-1.3.5/django_telethon/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:03.958345 django_telethon-1.3.5/django_telethon/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:03.958345 django_telethon-1.3.5/django_telethon/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/management/commands/runtelegram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:03.962345 django_telethon-1.3.5/django_telethon/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:03.962345 django_telethon-1.3.5/django_telethon/models/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/models/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/models/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/models/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/models/sentfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/models/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-15 20:43:00.000000 django_telethon-1.3.5/django_telethon/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:03.962345 django_telethon-1.3.5/django_telethon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-15 20:43:03.000000 django_telethon-1.3.5/django_telethon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 20:43:03.000000 django_telethon-1.3.5/django_telethon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:43:03.000000 django_telethon-1.3.5/django_telethon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 20:43:03.000000 django_telethon-1.3.5/django_telethon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 20:43:03.000000 django_telethon-1.3.5/django_telethon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 20:43:00.000000 django_telethon-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:43:03.962345 django_telethon-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-15 20:43:00.000000 django_telethon-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:51.291104 django_telethon-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 20:46:48.000000 django_telethon-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 20:46:48.000000 django_telethon-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-15 20:46:51.291104 django_telethon-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-15 20:46:48.000000 django_telethon-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:51.287104 django_telethon-1.3.6/django_telethon/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:51.287104 django_telethon-1.3.6/django_telethon/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:51.287104 django_telethon-1.3.6/django_telethon/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/management/commands/runtelegram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:51.287104 django_telethon-1.3.6/django_telethon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:51.287104 django_telethon-1.3.6/django_telethon/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/models/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/models/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/models/sentfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/models/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-15 20:46:48.000000 django_telethon-1.3.6/django_telethon/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:46:51.287104 django_telethon-1.3.6/django_telethon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-15 20:46:51.000000 django_telethon-1.3.6/django_telethon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 20:46:51.000000 django_telethon-1.3.6/django_telethon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:46:51.000000 django_telethon-1.3.6/django_telethon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 20:46:51.000000 django_telethon-1.3.6/django_telethon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 20:46:51.000000 django_telethon-1.3.6/django_telethon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 20:46:48.000000 django_telethon-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:46:51.291104 django_telethon-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-15 20:46:48.000000 django_telethon-1.3.6/setup.py
```

### Comparing `django_telethon-1.3.5/LICENSE` & `django_telethon-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/PKG-INFO` & `django_telethon-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-telethon
-Version: 1.3.5
+Version: 1.3.6
 Summary: Telethon for django
 Home-page: https://github.com/ali-zahedi/django-telethon
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_telethon-1.3.5/README.md` & `django_telethon-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/admin.py` & `django_telethon-1.3.6/django_telethon/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         'phone',
         'name',
     )
     actions = ('send_a_test_message',)
 
     @admin.action(description="Send a test message")
     def send_a_test_message(self, request, queryset):
-        queryset = queryset.selected_related('client_session')
+        queryset = queryset.select_related('client_session')
         for entity in queryset:
             entity_id = entity.entity_id
             # TODO: try to handle this method inside the package
             payload = {
                 'fn': 'send_message',
                 'msg': f'Check **{entity}**',
                 'parser': 'md',
```

### Comparing `django_telethon-1.3.5/django_telethon/default_settings.py` & `django_telethon-1.3.6/django_telethon/default_settings.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/management/commands/runtelegram.py` & `django_telethon-1.3.6/django_telethon/management/commands/runtelegram.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/migrations/0001_initial.py` & `django_telethon-1.3.6/django_telethon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/models/entities.py` & `django_telethon-1.3.6/django_telethon/models/entities.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/models/login.py` & `django_telethon-1.3.6/django_telethon/models/login.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/models/sentfiles.py` & `django_telethon-1.3.6/django_telethon/models/sentfiles.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/models/sessions.py` & `django_telethon-1.3.6/django_telethon/models/sessions.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/models/states.py` & `django_telethon-1.3.6/django_telethon/models/states.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/rabbitmq.py` & `django_telethon-1.3.6/django_telethon/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/receivers.py` & `django_telethon-1.3.6/django_telethon/receivers.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/sessions.py` & `django_telethon-1.3.6/django_telethon/sessions.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/utils.py` & `django_telethon-1.3.6/django_telethon/utils.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon/views.py` & `django_telethon-1.3.6/django_telethon/views.py`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/django_telethon.egg-info/PKG-INFO` & `django_telethon-1.3.6/django_telethon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-telethon
-Version: 1.3.5
+Version: 1.3.6
 Summary: Telethon for django
 Home-page: https://github.com/ali-zahedi/django-telethon
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_telethon-1.3.5/django_telethon.egg-info/SOURCES.txt` & `django_telethon-1.3.6/django_telethon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/pyproject.toml` & `django_telethon-1.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_telethon-1.3.5/setup.py` & `django_telethon-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-telethon',
-    version='v1.3.5',
+    version='v1.3.6',
     packages=find_packages(),
     include_package_data=True,
     license='BSD License',
     description='Telethon for django',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/ali-zahedi/django-telethon',
```

