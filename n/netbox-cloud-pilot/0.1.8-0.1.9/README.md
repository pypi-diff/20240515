# Comparing `tmp/netbox-cloud-pilot-0.1.8.tar.gz` & `tmp/netbox-cloud-pilot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cloud-pilot-0.1.8.tar", last modified: Fri Jan 12 12:04:47 2024, max compression
+gzip compressed data, was "netbox-cloud-pilot-0.1.9.tar", last modified: Fri Jan 12 21:44:08 2024, max compression
```

## Comparing `netbox-cloud-pilot-0.1.8.tar` & `netbox-cloud-pilot-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:47.450487 netbox-cloud-pilot-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-01-12 12:04:47.450487 netbox-cloud-pilot-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:47.446487 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:47.446487 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    36945 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13926 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    31143 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/iaas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:47.446487 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/nb_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:47.442487 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:47.446487 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:47.446487 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/env_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/env_node_groups.html
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/plugin_store.html
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/netboxconfiguration.html
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/netboxdbbackup.html
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/nodelogs.html
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_disable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_enable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_uninstall.html
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugins_store.html
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20506 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:04:47.450487 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-01-12 12:04:47.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-12 12:04:47.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 12:04:47.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 12:04:47.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-12 12:04:47.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-12 12:04:47.000000 netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 12:04:47.450487 netbox-cloud-pilot-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-12 12:04:39.000000 netbox-cloud-pilot-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:08.179295 netbox-cloud-pilot-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-01-12 21:44:08.179295 netbox-cloud-pilot-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:08.175295 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:08.175295 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36945 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14459 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31143 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/iaas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:08.175295 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/nb_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:08.171295 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:08.179295 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:08.179295 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/env_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/env_node_groups.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/plugin_store.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/netboxconfiguration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/netboxdbbackup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/nodelogs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_disable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_enable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_uninstall.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugins_store.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20506 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:44:08.179295 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-01-12 21:44:08.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-12 21:44:08.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 21:44:08.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 21:44:08.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-12 21:44:08.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-12 21:44:08.000000 netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 21:44:08.179295 netbox-cloud-pilot-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-12 21:44:00.000000 netbox-cloud-pilot-0.1.9/setup.py
```

### Comparing `netbox-cloud-pilot-0.1.8/PKG-INFO` & `netbox-cloud-pilot-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cloud-pilot
-Version: 0.1.8
+Version: 0.1.9
 Summary: Enhances NetBox on CloudMyDC's VAP with advanced management and control features.
 Home-page: https://github.com/Onemind-Services-LLC/netbox-cloud-pilot/
 Download-URL: https://github.com/Onemind-Services-LLC/netbox-cloud-pilot/
 Author: Abhimanyu Saharan
 Author-email: asaharan@onemindservices.com
 Maintainer: Abhimanyu Saharan
 Maintainer-email: asaharan@onemindservices.com
```

### Comparing `netbox-cloud-pilot-0.1.8/README.md` & `netbox-cloud-pilot-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/__init__.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/constants.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/constants.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/forms.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,7 +414,22 @@
 
 class ConfirmationForm(_ConfirmationForm):
     """
     A generic confirmation form. The form is not valid unless the `confirm` field is checked.
     """
 
     name = forms.CharField(widget=forms.HiddenInput())
+
+    def clean(self):
+        super().clean()
+
+        if not get_workers_for_queue('default'):
+            raise ValidationError(
+                "No RQ workers operating on the 'default' queue are currently active in the environment."
+            )
+
+        instance = NetBoxConfiguration.objects.first()
+        env = instance.get_env()
+
+        # Ensure no actions are currently running on the environment
+        if env.get_actions():
+            raise ValidationError("There are currently actions running on the environment.")
```

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/iaas.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/iaas.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/migrations/0001_initial.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/models.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -328,24 +328,34 @@
         except CroniterError as e:
             raise ValidationError({"crontab": e})
 
     @property
     def cron(self):
         return " ".join(croniter(self.crontab).expressions)
 
-    def list_backups(self):
+    @property
+    def get_master_node(self):
         node_groups = self.netbox_env.get_env_storage().get_node_groups()
         master_node = None
         for node_group in node_groups:
             master_node = node_group.get("node", {})
             break
 
+        return master_node
+
+    def list_backups(self):
+        master_node = self.get_master_node
         if not master_node:
             return []
 
+        # Always update restic
+        self.netbox_env.get_env_storage().execute_cmd(
+            node_id=master_node.get("id"), command="/usr/bin/restic self-update 2>&1"
+        )
+
         result = self.netbox_env.get_env_storage().execute_cmd(
             node_id=master_node.get("id"), command="/root/getBackupsAllEnvs.sh"
         )[0]
 
         if backups := json.loads(result.get("out", "")).get("backups", {}).get(self.netbox_env.env_name, []):
             # Cache backups in case next time it returns empty
             cache.set(f"netbox_db_backups_{self.pk}", backups, timeout=60 * 60)
```

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/navigation.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/nb_settings.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/nb_settings.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/tables.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/env_info.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/env_info.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/env_node_groups.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/env_node_groups.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/plugin_store.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/inc/plugin_store.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/netboxconfiguration.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/netboxconfiguration.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/netboxdbbackup.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/netboxdbbackup.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/nodelogs.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/nodelogs.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_disable.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_disable.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_enable.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_enable.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_uninstall.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugin_uninstall.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugins_store.html` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/templates/netbox_cloud_pilot/plugins_store.html`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/urls.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/utils.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot/views.py` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/PKG-INFO` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cloud-pilot
-Version: 0.1.8
+Version: 0.1.9
 Summary: Enhances NetBox on CloudMyDC's VAP with advanced management and control features.
 Home-page: https://github.com/Onemind-Services-LLC/netbox-cloud-pilot/
 Download-URL: https://github.com/Onemind-Services-LLC/netbox-cloud-pilot/
 Author: Abhimanyu Saharan
 Author-email: asaharan@onemindservices.com
 Maintainer: Abhimanyu Saharan
 Maintainer-email: asaharan@onemindservices.com
```

### Comparing `netbox-cloud-pilot-0.1.8/netbox_cloud_pilot.egg-info/SOURCES.txt` & `netbox-cloud-pilot-0.1.9/netbox_cloud_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cloud-pilot-0.1.8/setup.py` & `netbox-cloud-pilot-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 readme = os.path.join(os.path.dirname(__file__), 'README.md')
 
 with open(readme) as fh:
     long_description = fh.read()
 
 setup(
     name="netbox-cloud-pilot",
-    version="0.1.8",
+    version="0.1.9",
     description="Enhances NetBox on CloudMyDC's VAP with advanced management and control features.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Onemind-Services-LLC/netbox-cloud-pilot/",
     download_url="https://github.com/Onemind-Services-LLC/netbox-cloud-pilot/",
     author="Abhimanyu Saharan",
     author_email="asaharan@onemindservices.com",
```

