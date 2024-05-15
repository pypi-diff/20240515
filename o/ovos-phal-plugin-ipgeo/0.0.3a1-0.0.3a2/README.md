# Comparing `tmp/ovos-phal-plugin-ipgeo-0.0.3a1.tar.gz` & `tmp/ovos-phal-plugin-ipgeo-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-phal-plugin-ipgeo-0.0.3a1.tar", last modified: Fri Mar 15 22:00:59 2024, max compression
+gzip compressed data, was "ovos-phal-plugin-ipgeo-0.0.3a2.tar", last modified: Wed May 15 17:05:05 2024, max compression
```

## Comparing `ovos-phal-plugin-ipgeo-0.0.3a1.tar` & `ovos-phal-plugin-ipgeo-0.0.3a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:00:59.293065 ovos-phal-plugin-ipgeo-0.0.3a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-15 22:00:56.000000 ovos-phal-plugin-ipgeo-0.0.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-15 22:00:56.000000 ovos-phal-plugin-ipgeo-0.0.3a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-15 22:00:59.293065 ovos-phal-plugin-ipgeo-0.0.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 22:00:56.000000 ovos-phal-plugin-ipgeo-0.0.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:00:59.293065 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo/
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-15 22:00:56.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-15 22:00:56.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:00:59.293065 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-15 22:00:59.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-15 22:00:59.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 22:00:59.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-15 22:00:59.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-15 22:00:59.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-15 22:00:59.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 22:00:59.000000 ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-15 22:00:56.000000 ovos-phal-plugin-ipgeo-0.0.3a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 22:00:59.293065 ovos-phal-plugin-ipgeo-0.0.3a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-03-15 22:00:56.000000 ovos-phal-plugin-ipgeo-0.0.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:05:05.348074 ovos-phal-plugin-ipgeo-0.0.3a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-15 17:05:02.000000 ovos-phal-plugin-ipgeo-0.0.3a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 17:05:02.000000 ovos-phal-plugin-ipgeo-0.0.3a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 17:05:05.348074 ovos-phal-plugin-ipgeo-0.0.3a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 17:05:02.000000 ovos-phal-plugin-ipgeo-0.0.3a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:05:05.344074 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-15 17:05:02.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 17:05:02.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:05:05.348074 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 17:05:05.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-15 17:05:05.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:05:05.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 17:05:05.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 17:05:05.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 17:05:05.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:05:05.000000 ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 17:05:02.000000 ovos-phal-plugin-ipgeo-0.0.3a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:05:05.348074 ovos-phal-plugin-ipgeo-0.0.3a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-05-15 17:05:02.000000 ovos-phal-plugin-ipgeo-0.0.3a2/setup.py
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.3a1/LICENSE` & `ovos-phal-plugin-ipgeo-0.0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-ipgeo-0.0.3a1/PKG-INFO` & `ovos-phal-plugin-ipgeo-0.0.3a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-ipgeo
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: A PHAL plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-ipgeo
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo/__init__.py` & `ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,17 +35,20 @@
         if self.web_config.get("location") and \
                 (message is None or not message.data.get('overwrite')):
             LOG.debug("Skipping overwrite of existing location")
             return
         # geolocate from ip address
         try:
             location = self.ip_geolocate()
+            if not location:
+                raise ValueError(f"Got empty location: {location}")
             LOG.info(f"Got location: {location}")
             self.web_config["location"] = location
             self.web_config.store()
+            LOG.debug(f"Updated {self.web_config.path}")
             self.bus.emit(Message("configuration.updated"))
             if message:
                 LOG.debug("Emitting location update response")
                 self.bus.emit(message.response(
                     data={'location': location}))
             return
         except ConnectionError as e:
@@ -58,13 +61,23 @@
                 data={'error': True}))
 
     @staticmethod
     def ip_geolocate(ip=None):
         try:
             # configured backend may throw some errors if its down
             api = GeolocationApi()
+        except Exception as e:
+            LOG.exception("Failed to create Geolocation API")
+            api = GeolocationApi(backend_type=BackendType.OFFLINE)
+        try:
             return api.get_ip_geolocation(ip)
         except Exception as e:
             LOG.exception("Backend Geolocation API error!")
+        try:
             # force offline backend api (direct call)
-            api = GeolocationApi(backend_type=BackendType.OFFLINE)
-            return api.get_ip_geolocation(ip)
+            if api.backend_type != BackendType.OFFLINE:
+                return (GeolocationApi(backend_type=BackendType.OFFLINE)
+                        .get_ip_geolocation(ip))
+        except Exception as e:
+            LOG.error(e)
+            # Raise this exception since we won't return anything valid
+            raise e
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.3a1/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO` & `ovos-phal-plugin-ipgeo-0.0.3a2/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-ipgeo
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: A PHAL plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-ipgeo
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.3a1/setup.py` & `ovos-phal-plugin-ipgeo-0.0.3a2/setup.py`

 * *Files identical despite different names*

