# Comparing `tmp/gaarf-exporter-1.0.0.dev1.tar.gz` & `tmp/gaarf-exporter-1.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaarf-exporter-1.0.0.dev1.tar", last modified: Tue May 14 07:25:05 2024, max compression
+gzip compressed data, was "gaarf-exporter-1.0.0.dev2.tar", last modified: Tue May 14 12:39:14 2024, max compression
```

## Comparing `gaarf-exporter-1.0.0.dev1.tar` & `gaarf-exporter-1.0.0.dev2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6443 2024-03-26 12:03:46.000000 gaarf-exporter-1.0.0.dev1/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.103046 gaarf-exporter-1.0.0.dev1/gaarf_exporter/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1293 2024-05-13 21:01:08.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/alert.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/alert_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2395 2024-05-02 16:45:02.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/bootstrap.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      450 2024-05-13 15:50:58.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/conversion_action.yaml
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      672 2024-05-13 19:59:40.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/disapprovals.yaml
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      433 2024-05-13 15:50:58.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/mapping.yaml
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      340 2024-05-13 12:26:59.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/performance.yaml
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6541 2024-05-14 07:00:12.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     8246 2024-05-14 06:59:31.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/main.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2825 2024-05-08 08:46:57.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/query_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    16979 2024-05-13 21:10:46.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/target.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/util.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1017 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1848 2024-05-14 06:43:50.000000 gaarf-exporter-1.0.0.dev1/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:38:01.000000 gaarf-exporter-1.0.0.dev1/tests/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/tests/end-to-end/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/end-to-end/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3308 2024-05-14 07:17:45.000000 gaarf-exporter-1.0.0.dev1/tests/end-to-end/test_gaarf_exporter.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/tests/unit/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/unit/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_alerts.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6493 2024-05-14 06:59:03.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2024-05-08 08:46:57.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_query_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    19671 2024-05-13 20:58:11.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_target.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 12:39:14.905019 gaarf-exporter-1.0.0.dev2/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-05-14 12:39:14.905019 gaarf-exporter-1.0.0.dev2/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6443 2024-03-26 12:03:46.000000 gaarf-exporter-1.0.0.dev2/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 12:39:14.901019 gaarf-exporter-1.0.0.dev2/gaarf_exporter/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1293 2024-05-13 21:01:08.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/alert.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/alert_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2395 2024-05-02 16:45:02.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/bootstrap.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 12:39:14.901019 gaarf-exporter-1.0.0.dev2/gaarf_exporter/collector_definitions/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      450 2024-05-13 15:50:58.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/collector_definitions/conversion_action.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3424 2024-05-14 10:37:10.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/collector_definitions/disapprovals.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2495 2024-05-14 12:22:35.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/collector_definitions/mapping.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4622 2024-05-14 11:02:43.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/collector_definitions/performance.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7078 2024-05-14 09:34:11.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8246 2024-05-14 08:34:31.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/main.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2825 2024-05-08 08:46:57.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/query_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    18710 2024-05-14 12:23:03.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/target.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter/util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 12:39:14.901019 gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-05-14 12:39:14.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1017 2024-05-14 12:39:14.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-05-14 12:39:14.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-05-14 12:39:14.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-05-14 12:39:14.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-05-14 12:39:14.000000 gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-05-14 12:39:14.905019 gaarf-exporter-1.0.0.dev2/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1848 2024-05-14 12:39:11.000000 gaarf-exporter-1.0.0.dev2/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 12:39:14.901019 gaarf-exporter-1.0.0.dev2/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:38:01.000000 gaarf-exporter-1.0.0.dev2/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 12:39:14.901019 gaarf-exporter-1.0.0.dev2/tests/end-to-end/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev2/tests/end-to-end/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3308 2024-05-14 07:17:45.000000 gaarf-exporter-1.0.0.dev2/tests/end-to-end/test_gaarf_exporter.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 12:39:14.905019 gaarf-exporter-1.0.0.dev2/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev2/tests/unit/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev2/tests/unit/test_alerts.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6444 2024-05-14 12:19:36.000000 gaarf-exporter-1.0.0.dev2/tests/unit/test_collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev2/tests/unit/test_exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2024-05-08 08:46:57.000000 gaarf-exporter-1.0.0.dev2/tests/unit/test_query_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    19764 2024-05-14 12:23:03.000000 gaarf-exporter-1.0.0.dev2/tests/unit/test_target.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev2/tests/unit/test_util.py
```

### Comparing `gaarf-exporter-1.0.0.dev1/PKG-INFO` & `gaarf-exporter-1.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaarf-exporter
-Version: 1.0.0.dev1
+Version: 1.0.0.dev2
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gaarf-exporter-1.0.0.dev1/README.md` & `gaarf-exporter-1.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/alert.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/alert.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/alert_elements.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/alert_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/bootstrap.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/collectors.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/collectors.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,21 +117,32 @@
     """Initializes CollectorSet based on provided collectors."""
     self._collectors = collectors or set()
     self._service_collectors = service_collectors
 
   @property
   def collectors(self) -> set[query_target.Collector]:
     """Return customized or original collectors of the CollectorSet."""
-    if self._service_collectors:
-      _service_collectors = set()
-      for collector in self._collectors:
-        if service_collector := collector.generate_service_collector():
-          _service_collectors.add(service_collector)
-      self._collectors = self._collectors.union(_service_collectors)
     self.deduplicate_collectors()
+    if self._service_collectors:
+      has_service_collector = any([
+          isinstance(collector, query_target.ServiceCollector)
+          for collector in self._collectors
+      ])
+      if not has_service_collector:
+        valid_collector_levels = [
+            collector.level
+            for collector in self._collectors
+            if collector.level != query_target.CollectorLevel.UNKNOWN
+        ]
+        if valid_collector_levels:
+          default_service_collector = (
+              query_target.create_default_service_collector(
+                  min(valid_collector_levels)))
+          self._collectors.add(default_service_collector)
+
     return self._collectors
 
   def deduplicate_collectors(self) -> None:
     """Dedupicates collectors in the set.
 
     If there are similar collectors in the list return only those with
     the lowest level.
@@ -183,15 +194,19 @@
 
 def define_collectors(path: str):
   _registry: dict = defaultdict(dict)
   files = [file for file in glob.glob(path)]
   results = [_read_files(file) for file in files]
   for data in results:
     for collector_data in data:
-      coll = query_target.Collector.from_definition(collector_data)
+      if collector_data.get('type') == 'service':
+        coll = query_target.ServiceCollector.from_definition(collector_data)
+      else:
+        coll = query_target.Collector.from_definition(collector_data)
       _registry[coll.name] = coll
-      for subregistry in collector_data.get('registries'):
-        _registry[subregistry].update({coll.name: coll})
+      if subregistries := collector_data.get('registries'):
+        for subregistry in subregistries:
+          _registry[subregistry].update({coll.name: coll})
       if 'has_conversion_split' in collector_data:
         conv_coll = coll.create_conv_collector()
         _registry[conv_coll.name] = conv_coll
   return _registry
```

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/exporter.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/main.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/main.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/query_elements.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/query_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/target.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,21 +155,21 @@
     resource_name: Name of resource to get data from (used in FROM statement).
     query: Full text of the query to be sent to Google Ads API.
     suffix: Optional custom identifier to the target.
   """
 
   def __init__(self,
                name: str | None = None,
-               metrics: str | list[query_elements.Field] | None = None,
+               metrics: str | Sequence[query_elements.Field] | None = None,
                level: CollectorLevel | None = CollectorLevel.AD_GROUP,
                resource_name: str | None = None,
-               dimensions: str | list[query_elements.Field] | None = None,
-               filters: str | None = None,
+               dimensions: str | Sequence[query_elements.Field] | None = None,
+               filters: str | Sequence[str] | None = None,
                suffix: str | None = None,
-               query: strr | None = None) -> None:
+               query: str | None = None) -> None:
     """Initializes Collector.
 
     Args:
       name: Unique identifier of a target.
       metrics: All metrics (started with `metrics.`) associated with the target.
       level: Minimal entity level in the target (ad_group, campaign, customer).
       resource_name: Name of resource to get data from (used in FROM statement).
@@ -177,15 +177,15 @@
       filters: Text conditions for limiting the query.
       suffix: Optional custom identifier to the target.
       query: Full query_text.
     """
     self.name = name
     self._level = level
     self._resource_name = resource_name
-    self._filters = filters
+    self._filters = filters or set()
     self._metrics = self._init_fields(metrics, 'metrics')
     self._dimensions = self._init_fields(dimensions)
     self.suffix = suffix if suffix else name
     self._query = query
 
   @classmethod
   def from_definition(cls, definition: dict) -> Collector:
@@ -241,17 +241,28 @@
 
   @dimensions.setter
   def dimensions(self, values: Sequence[query_elements.Field]) -> None:
     """Changes saved dimensions of a target."""
     self._dimensions = values
 
   @property
-  def filters(self) -> str:
+  def filters(self) -> set[str]:
     """Returns filters or default placeholder."""
-    return self._filters or 'segments.date DURING TODAY'
+    if isinstance(self._filters, str):
+      self._filters = set(self._filters.split(' AND '))
+    else:
+      self._filters = set(self._filters)
+    if isinstance(self, ServiceCollector):
+      return self._filters
+    # TODO (amarkin): Adding default filter hurts customization by dates. And wierd.
+    if not self._filters:
+      self._filters.add('segments.date DURING TODAY')
+    elif not any('segments.date' in _filter for _filter in self._filters):
+      self._filters.add('segments.date DURING TODAY')
+    return self._filters
 
   @filters.setter
   def filters(self, values: str) -> None:
     """Changes saved dimensions of a target."""
     self._filters = values
 
   def _init_fields(self,
@@ -344,19 +355,15 @@
       return '\n'
     dimensions_info = ',\n'.join(
         [field.to_query_field() for field in sorted(dimensions)])
     return f'{dimensions_info},\n'
 
   @property
   def _formatted_filters(self) -> str:
-    if not self._filters:
-      return 'segments.date DURING TODAY'
-    if isinstance(self._filters, MutableSequence):
-      return ' AND '.join(self._filters)
-    return self._filters
+    return ' AND '.join(self.filters)
 
   @property
   def resource_name(self) -> str:
     """Gets resource_name or infers it from target level."""
     if self._resource_name:
       return self._resource_name
     if level_info := self.level_info:
@@ -376,16 +383,17 @@
   def customize(self, kwargs: dict[str, str]) -> None:
     if level := kwargs.get('level'):
       self.level = CollectorLevel[level.upper()]
     if (start_date := kwargs.get('start_date')) and (end_date :=
                                                      kwargs.get('end_date')):
       start_date = gaarf_utils.convert_date(start_date)
       end_date = gaarf_utils.convert_date(end_date)
-      self.filters = self.filters.replace(
-          'DURING TODAY', f"BETWEEN '{start_date}' AND '{end_date}'")
+      if not self.filters or 'segments.date DURING TODAY' in self.filters:
+        self.filters.remove('segments.date DURING TODAY')
+        self.filters.add(f"segments.date BETWEEN '{start_date}' AND '{end_date}'")
       n_days = (datetime.strptime(end_date, '%Y-%m-%d') -
                 datetime.strptime(start_date, '%Y-%m-%d')).days + 1
       self.dimensions.add(query_elements.Field(str(n_days), 'n_days'))
 
   def is_similar(self, other: Collector) -> bool:
     """Compares similarity between two collectors.
 
@@ -441,18 +449,15 @@
         ])
         if filters:
           filters = filters + ' AND ' + level_info.active_entities_filter
         else:
           filters = level_info.active_entities_filter
 
     return ServiceCollector(
-        name='mapping',
-        dimensions=dimensions,
-        level=level,
-        filters=filters)
+        name='mapping', dimensions=dimensions, level=level, filters=filters)
 
   def __eq__(self, other: Collector) -> bool:
     """Compares two targets based on similarity, resource_name and level."""
     if not self.is_similar(other):
       return False
     if self.level != other.level:
       return False
@@ -469,14 +474,17 @@
     if self.level.value > other.level.value:
       return True
     return False
 
   def __hash__(self):
     return hash(self.query)
 
+  def __repr__(self) -> str:
+    return f'Collector(name="{self.name}")'
+
 
 class ServiceCollector(Collector):
   """Helper class for targets without metrics."""
 
   @property
   def metrics(self) -> set[query_elements.Field]:
     """Returns default info metric."""
@@ -484,7 +492,40 @@
         query_elements.Field(name='1', alias='info'),
     }
 
   @metrics.setter
   def metrics(self, value: query_elements.Field) -> None:
     """Ensures that metrics cannot be overwritten."""
     raise ValueError('Cannot change value of "metrics"!')
+
+
+def create_default_service_collector(
+    level: CollectorLevel) -> ServiceCollector | None:
+  """Generates correct ServiceCollector based on provided level.
+
+   Based on level (AD_GROUP, CAMPAIGN, ACCOUNT, etc.) corresponding
+   ServiceCollector is created that contains all necessary mapping information
+   downstream. I.e. if 'level=AD_GROUP' then information on ad_group, campaign
+   and customer will be included in to the mapping.
+
+   Returns:
+    ServiceCollector called 'mapping' for an appropriate level.
+
+  """
+  if level == CollectorLevel.MCC:
+    level = CollectorLevel.CUSTOMER
+  dimensions = set()
+  filters = set()
+
+  for target_level in CollectorLevel:
+    if (target_level
+        not in (CollectorLevel.MCC, CollectorLevel.AD_GROUP_AD_ASSET) and
+        level <= target_level and (level_info := LEVELS.get(target_level))):
+      dimensions.update([
+          query_elements.Field(name=level_info.id, alias=level_info.id_alias),
+          query_elements.Field(
+              name=level_info.name, alias=level_info.name_alias)
+      ])
+      filters.add(level_info.active_entities_filter)
+
+  return ServiceCollector(
+      name='mapping', dimensions=dimensions, level=level, filters=filters)
```

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter/util.py` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter/util.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/PKG-INFO` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaarf-exporter
-Version: 1.0.0.dev1
+Version: 1.0.0.dev2
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/SOURCES.txt` & `gaarf-exporter-1.0.0.dev2/gaarf_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/setup.py` & `gaarf-exporter-1.0.0.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / 'README.md').read_text()
 
 setup(
   name='gaarf-exporter',
-  version='1.0.0.dev1',
+  version='1.0.0.dev2',
   long_description=README,
   long_description_content_type='text/markdown',
   author='Google Inc. (gTech gPS CSE team)',
   author_email='no-reply@google.com',
   license='Apache 2.0',
   classifiers=[
     'Programming Language :: Python :: 3 :: Only',
```

### Comparing `gaarf-exporter-1.0.0.dev1/tests/end-to-end/test_gaarf_exporter.py` & `gaarf-exporter-1.0.0.dev2/tests/end-to-end/test_gaarf_exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/tests/unit/test_alerts.py` & `gaarf-exporter-1.0.0.dev2/tests/unit/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/tests/unit/test_collectors.py` & `gaarf-exporter-1.0.0.dev2/tests/unit/test_collectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,17 +176,16 @@
   def test_load_collectors_gets_collector_by_name(self, registry):
     perf = registry.collectors.get('performance')
     assert perf.name == 'performance'
     assert perf.query
 
   def test_load_collectors_gets_collector_by_subregistry_name(self, registry):
     default_registry = registry.collectors.get('default')
-    assert len(default_registry) == 4
+    assert len(default_registry) == 3
     assert default_registry.get('performance').name == 'performance'
-    assert default_registry.get('mapping').query
 
   def test_load_collectors_gets_conversion_split_collector(self, registry):
     perf = registry.collectors.get('performance_conversion_split')
     assert perf.query
 
   def test_load_collectors_gets_correct_collector_query(self, registry):
     collector = registry.find_collectors('performance')
```

### Comparing `gaarf-exporter-1.0.0.dev1/tests/unit/test_exporter.py` & `gaarf-exporter-1.0.0.dev2/tests/unit/test_exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/tests/unit/test_query_elements.py` & `gaarf-exporter-1.0.0.dev2/tests/unit/test_query_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-1.0.0.dev1/tests/unit/test_target.py` & `gaarf-exporter-1.0.0.dev2/tests/unit/test_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
         SELECT
             ad_group_ad.ad.id AS ad_id,
             campaign.id AS campaign_id,
             ad_group_ad.policy_summary.approval_status AS approval_status,
             ad_group_ad.policy_summary.review_status AS review_status,
         FROM ad_group_ad
         WHERE campaign.status = ENABLED
+            AND segments.date DURING TODAY
             AND ad_group.status = ENABLED
             AND ad_group_ad.status = ENABLED
             AND ad_group_ad.policy_summary.approval_status != APPROVED
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     @pytest.mark.skip('Obsolete')
@@ -344,16 +345,20 @@
     def test_dimensions_returns_correct_fields(self):
       target = query_target.Collector(dimensions='segments.date')
       assert target.dimensions == {
           query_elements.Field(name='segments.date', alias=None),
       }
 
     @pytest.mark.parametrize('filters,expected_filter', [
-        ('segments.date DURING YESTERDAY', 'segments.date DURING YESTERDAY'),
-        (None, 'segments.date DURING TODAY'),
+        ('segments.date DURING YESTERDAY', {
+            'segments.date DURING YESTERDAY',
+        }),
+        (None, {
+            'segments.date DURING TODAY',
+        }),
     ])
     def test_filters_returns_correct_expression(self, filters, expected_filter):
       target = query_target.Collector(filters=filters)
 
       assert target.filters == expected_filter
 
     def test_resource_name_returns_correct_expression_for_explicit_resource_name(
```

### Comparing `gaarf-exporter-1.0.0.dev1/tests/unit/test_util.py` & `gaarf-exporter-1.0.0.dev2/tests/unit/test_util.py`

 * *Files identical despite different names*

