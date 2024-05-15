# Comparing `tmp/onestop_opensign-0.1.4.tar.gz` & `tmp/onestop_opensign-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestop_opensign-0.1.4.tar", last modified: Thu May  9 13:53:36 2024, max compression
+gzip compressed data, was "onestop_opensign-0.1.5.tar", last modified: Tue May 14 18:20:43 2024, max compression
```

## Comparing `onestop_opensign-0.1.4.tar` & `onestop_opensign-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-09 13:53:36.840798 onestop_opensign-0.1.4/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       80 2024-05-08 09:45:22.000000 onestop_opensign-0.1.4/MANIFEST.in
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      411 2024-05-09 13:53:36.840798 onestop_opensign-0.1.4/PKG-INFO
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-09 13:53:36.840798 onestop_opensign-0.1.4/onestop_opensign/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      323 2024-04-30 17:20:54.000000 onestop_opensign-0.1.4/onestop_opensign/__init__.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      515 2024-05-09 13:50:24.000000 onestop_opensign-0.1.4/onestop_opensign/config.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      586 2024-04-30 17:28:13.000000 onestop_opensign-0.1.4/onestop_opensign/extension_init.py
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-09 13:53:36.840798 onestop_opensign-0.1.4/onestop_opensign/fixtures/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      330 2024-04-30 17:32:31.000000 onestop_opensign-0.1.4/onestop_opensign/fixtures/digital_signature_methods.json
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-09 13:53:36.840798 onestop_opensign-0.1.4/onestop_opensign/migrations/
--rw-r--r--   0 edwin     (1000) edwin     (1000)     1999 2024-05-08 08:18:28.000000 onestop_opensign-0.1.4/onestop_opensign/migrations/0001_initial.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      319 2024-05-05 17:00:52.000000 onestop_opensign-0.1.4/onestop_opensign/migrations/__init__.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     4087 2024-05-08 08:53:03.000000 onestop_opensign-0.1.4/onestop_opensign/models.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)    10377 2024-05-08 08:47:37.000000 onestop_opensign-0.1.4/onestop_opensign/provider.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      520 2024-05-02 04:48:23.000000 onestop_opensign-0.1.4/onestop_opensign/urls.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     4057 2024-05-08 08:37:00.000000 onestop_opensign-0.1.4/onestop_opensign/views.py
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-09 13:53:36.840798 onestop_opensign-0.1.4/onestop_opensign.egg-info/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      411 2024-05-09 13:53:36.000000 onestop_opensign-0.1.4/onestop_opensign.egg-info/PKG-INFO
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      558 2024-05-09 13:53:36.000000 onestop_opensign-0.1.4/onestop_opensign.egg-info/SOURCES.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)        1 2024-05-09 13:53:36.000000 onestop_opensign-0.1.4/onestop_opensign.egg-info/dependency_links.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       27 2024-05-09 13:53:36.000000 onestop_opensign-0.1.4/onestop_opensign.egg-info/requires.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       17 2024-05-09 13:53:36.000000 onestop_opensign-0.1.4/onestop_opensign.egg-info/top_level.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       38 2024-05-09 13:53:36.840798 onestop_opensign-0.1.4/setup.cfg
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      961 2024-05-09 13:53:32.000000 onestop_opensign-0.1.4/setup.py
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-14 18:20:43.726665 onestop_opensign-0.1.5/
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       80 2024-05-08 09:45:22.000000 onestop_opensign-0.1.5/MANIFEST.in
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      411 2024-05-14 18:20:43.726665 onestop_opensign-0.1.5/PKG-INFO
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-14 18:20:43.726665 onestop_opensign-0.1.5/onestop_opensign/
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      323 2024-04-30 17:20:54.000000 onestop_opensign-0.1.5/onestop_opensign/__init__.py
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      515 2024-05-09 13:50:24.000000 onestop_opensign-0.1.5/onestop_opensign/config.py
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      586 2024-04-30 17:28:13.000000 onestop_opensign-0.1.5/onestop_opensign/extension_init.py
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-14 18:20:43.726665 onestop_opensign-0.1.5/onestop_opensign/fixtures/
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      330 2024-04-30 17:32:31.000000 onestop_opensign-0.1.5/onestop_opensign/fixtures/digital_signature_methods.json
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-14 18:20:43.726665 onestop_opensign-0.1.5/onestop_opensign/migrations/
+-rw-r--r--   0 edwin     (1000) edwin     (1000)     1999 2024-05-08 08:18:28.000000 onestop_opensign-0.1.5/onestop_opensign/migrations/0001_initial.py
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      319 2024-05-05 17:00:52.000000 onestop_opensign-0.1.5/onestop_opensign/migrations/__init__.py
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)     4087 2024-05-08 08:53:03.000000 onestop_opensign-0.1.5/onestop_opensign/models.py
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)    10579 2024-05-14 18:08:37.000000 onestop_opensign-0.1.5/onestop_opensign/provider.py
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      520 2024-05-02 04:48:23.000000 onestop_opensign-0.1.5/onestop_opensign/urls.py
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)     4057 2024-05-08 08:37:00.000000 onestop_opensign-0.1.5/onestop_opensign/views.py
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2024-05-14 18:20:43.726665 onestop_opensign-0.1.5/onestop_opensign.egg-info/
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      411 2024-05-14 18:20:43.000000 onestop_opensign-0.1.5/onestop_opensign.egg-info/PKG-INFO
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      558 2024-05-14 18:20:43.000000 onestop_opensign-0.1.5/onestop_opensign.egg-info/SOURCES.txt
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)        1 2024-05-14 18:20:43.000000 onestop_opensign-0.1.5/onestop_opensign.egg-info/dependency_links.txt
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       27 2024-05-14 18:20:43.000000 onestop_opensign-0.1.5/onestop_opensign.egg-info/requires.txt
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       17 2024-05-14 18:20:43.000000 onestop_opensign-0.1.5/onestop_opensign.egg-info/top_level.txt
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       38 2024-05-14 18:20:43.726665 onestop_opensign-0.1.5/setup.cfg
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      961 2024-05-14 18:17:43.000000 onestop_opensign-0.1.5/setup.py
```

### Comparing `onestop_opensign-0.1.4/onestop_opensign/config.py` & `onestop_opensign-0.1.5/onestop_opensign/config.py`

 * *Files identical despite different names*

### Comparing `onestop_opensign-0.1.4/onestop_opensign/extension_init.py` & `onestop_opensign-0.1.5/onestop_opensign/extension_init.py`

 * *Files identical despite different names*

### Comparing `onestop_opensign-0.1.4/onestop_opensign/migrations/0001_initial.py` & `onestop_opensign-0.1.5/onestop_opensign/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `onestop_opensign-0.1.4/onestop_opensign/models.py` & `onestop_opensign-0.1.5/onestop_opensign/models.py`

 * *Files identical despite different names*

### Comparing `onestop_opensign-0.1.4/onestop_opensign/provider.py` & `onestop_opensign-0.1.5/onestop_opensign/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,21 +210,27 @@
         """
         widgets = []
         try:
             digital_signing_settings = digital_signature_folder.signing_task_template.digital_signing_settings
             open_sign_settings = digital_signing_settings.settings.get('open_sign', {})
 
             for key, value in open_sign_settings.items():
-                team = base_utils.get_object_or_none(Team, pk=key)
-                _logger.info(f"Checking if signer is in team: {team}, set for signing...")
+                try:
+                    team = base_utils.get_object_or_none(Team, pk=key)
+                    _logger.info(f"Checking if signer is in team: {team}, set for signing...")
+                except Exception as e:
+                    _logger.error(f"Error occurred while getting team: {e}")
+                    team = None
 
-                if team and user in team.members:
+                if user.email == key or (team and user in team.members):
                     widgets.extend(value.get('widgets', []))
+
         except Exception as e:
             _logger.error(f"Error occurred while getting digital signature settings: {e}")
+
         return widgets
 
     def sign_documents(self, digital_signature_folder, request, **kwargs):
         """
         Method that signs document(s) immediately with out sending to a folder
         """
         signers = list(map(lambda user: self.get_signer_details(user, digital_signature_folder), digital_signature_folder.signers.all()))
```

### Comparing `onestop_opensign-0.1.4/onestop_opensign/urls.py` & `onestop_opensign-0.1.5/onestop_opensign/urls.py`

 * *Files identical despite different names*

### Comparing `onestop_opensign-0.1.4/onestop_opensign/views.py` & `onestop_opensign-0.1.5/onestop_opensign/views.py`

 * *Files identical despite different names*

### Comparing `onestop_opensign-0.1.4/onestop_opensign.egg-info/SOURCES.txt` & `onestop_opensign-0.1.5/onestop_opensign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onestop_opensign-0.1.4/setup.py` & `onestop_opensign-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Fixtures folder has been included in Manifest.in file.
 https://stackoverflow.com/questions/1612733/including-non-python-files-with-setup-py
 https://docs.python.org/2/distutils/sourcedist.html#principle
 """
 
 setup(
     name='onestop_opensign',
-    version='0.1.4',
+    version='0.1.5',
     author='OTB Africa',
     author_email='developers@otbafrica.com',
     license='BSD 2-clause',
     description='Package for a onestop extension that integrates with the opensign digital signature service.',
     packages=[
         'onestop_opensign',
         'onestop_opensign.migrations'
```

