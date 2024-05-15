# Comparing `tmp/django_rest_aggregation-0.1.0.tar.gz` & `tmp/django_rest_aggregation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rest_aggregation-0.1.0.tar", last modified: Wed Apr 17 08:18:22 2024, max compression
+gzip compressed data, was "django_rest_aggregation-0.2.0.tar", last modified: Wed May 15 06:35:47 2024, max compression
```

## Comparing `django_rest_aggregation-0.1.0.tar` & `django_rest_aggregation-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:18:22.282509 django_rest_aggregation-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-17 08:18:22.278509 django_rest_aggregation-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:18:22.282509 django_rest_aggregation-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:18:22.278509 django_rest_aggregation-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:18:22.278509 django_rest_aggregation-0.1.0/src/django_rest_aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:18:22.278509 django_rest_aggregation-0.1.0/src/django_rest_aggregation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-17 08:18:22.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 08:18:22.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:18:22.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 08:18:22.000000 django_rest_aggregation-0.1.0/src/django_rest_aggregation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:18:22.278509 django_rest_aggregation-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    30023 2024-04-17 08:18:16.000000 django_rest_aggregation-0.1.0/tests/test_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:35:47.014516 django_rest_aggregation-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-05-15 06:35:47.014516 django_rest_aggregation-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:35:47.014516 django_rest_aggregation-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:35:47.010516 django_rest_aggregation-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:35:47.014516 django_rest_aggregation-0.2.0/src/django_rest_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:35:47.014516 django_rest_aggregation-0.2.0/src/django_rest_aggregation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-05-15 06:35:47.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 06:35:47.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:35:47.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 06:35:47.000000 django_rest_aggregation-0.2.0/src/django_rest_aggregation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:35:47.014516 django_rest_aggregation-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    30050 2024-05-15 06:35:38.000000 django_rest_aggregation-0.2.0/tests/test_aggregation.py
```

### Comparing `django_rest_aggregation-0.1.0/LICENSE` & `django_rest_aggregation-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rest_aggregation-0.1.0/PKG-INFO` & `django_rest_aggregation-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_rest_aggregation
-Version: 0.1.0
+Version: 0.2.0
 Summary: A DRF mixin for aggregation endpoints
 Author-email: Simon Legtenborg <simon.legtenborg@singular-it.de>
 Project-URL: Homepage, https://github.com/singularit-de/django-rest-aggregation/
 Project-URL: Bug Tracker, https://github.com/singularit-de/django-rest-aggregation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,17 +26,17 @@
 - grouping by multiple fields
 - filtering and ordering
 
 ---
 
 ## Installation
 
-To install, use pip: &#10060;
+To install, use pip
 
-    pip install [COMING SOON] 
+    pip install django-rest-aggregation
 
 ## Quickstart
 
 Inherit the **AggregationMixin** in your ViewSet.
 
 ```python
 from django_rest_aggregation.mixins import AggregationMixin
```

### Comparing `django_rest_aggregation-0.1.0/README.md` & `django_rest_aggregation-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 - grouping by multiple fields
 - filtering and ordering
 
 ---
 
 ## Installation
 
-To install, use pip: &#10060;
+To install, use pip
 
-    pip install [COMING SOON] 
+    pip install django-rest-aggregation
 
 ## Quickstart
 
 Inherit the **AggregationMixin** in your ViewSet.
 
 ```python
 from django_rest_aggregation.mixins import AggregationMixin
```

### Comparing `django_rest_aggregation-0.1.0/pyproject.toml` & `django_rest_aggregation-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_rest_aggregation"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name = "Simon Legtenborg", email = "simon.legtenborg@singular-it.de" },
 ]
 description = "A DRF mixin for aggregation endpoints"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `django_rest_aggregation-0.1.0/src/django_rest_aggregation/aggregator.py` & `django_rest_aggregation-0.2.0/src/django_rest_aggregation/aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.core.exceptions import FieldDoesNotExist
 from django.db import models
+from django.db.models import Case, When, Value
 from rest_framework.exceptions import ValidationError
 from rest_framework.request import Request
 
 from django_rest_aggregation.enums import Aggregation
 
 
 def get_filtered_params(request):
@@ -79,15 +80,17 @@
         self.model = queryset.model
         self.aggregation_name = aggregation_name
 
     def get_aggregated_queryset(self):
         self.validate_params()
 
         if (group_by := self.params.get("group_by", ["group"])) == ["group"]:
-            self.queryset = self.queryset.annotate(group=models.Value("all", output_field=models.CharField()))
+            self.queryset = self.queryset.annotate(group=Case(
+                When(pk__isnull=False, then=Value("all")),
+                default=Value("test")))
 
         return self.queryset.values(*group_by).annotate(**get_annotation(self.params, self.aggregation_name))
 
     def validate_params(self):
         # check if aggregation is in params and is valid
         if (aggregation := self.params.get("aggregation", None)) is None:
             raise ValidationError({"error": "'aggregation' is required"})
```

### Comparing `django_rest_aggregation-0.1.0/src/django_rest_aggregation/enums.py` & `django_rest_aggregation-0.2.0/src/django_rest_aggregation/enums.py`

 * *Files identical despite different names*

### Comparing `django_rest_aggregation-0.1.0/src/django_rest_aggregation/filter.py` & `django_rest_aggregation-0.2.0/src/django_rest_aggregation/filter.py`

 * *Files identical despite different names*

### Comparing `django_rest_aggregation-0.1.0/src/django_rest_aggregation/mixins.py` & `django_rest_aggregation-0.2.0/src/django_rest_aggregation/mixins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,36 @@
+from django_filters.rest_framework import DjangoFilterBackend
 from rest_framework.decorators import action
 from rest_framework.response import Response
 
 from .aggregator import Aggregator
 from .filter import ValueFilter
 from .serializers import AggregationSerializer
 
 
 class AggregationMixin:
     @action(methods=["get"], detail=False, url_path="aggregation", url_name="aggregation")
     def aggregation(self, request):
-        queryset = self.filter_queryset(self.get_queryset()).order_by()
+        queryset = self.get_queryset().order_by()
+
+        if DjangoFilterBackend in self.filter_backends:
+            queryset = DjangoFilterBackend().filter_queryset(request, queryset, self)
 
         aggregator = Aggregator(request, queryset, self.get_aggregation_name())
         filtered_queryset = self.filter_aggregated_queryset(aggregator.get_aggregated_queryset())
 
+        context = {
+            "request": request,
+            "name": self.get_aggregation_name()
+        }
         page = self.paginate_queryset(filtered_queryset)
         if page is not None:
-            serializer = self.get_aggregation_serializer_class(page, many=True)
+            serializer = self.get_aggregation_serializer_class(page, many=True, context=context)
             return self.get_paginated_response(serializer.data)
-        serializer = self.get_aggregation_serializer_class(filtered_queryset, many=True)
+        serializer = self.get_aggregation_serializer_class(filtered_queryset, many=True, context=context)
         return Response(serializer.data)
 
     def get_aggregation_serializer_class(self, *args, **kwargs):
         serializer = getattr(self, "aggregation_serializer_class", None)
         if serializer is not None:
             return serializer(*args, **kwargs)
         return AggregationSerializer(*args, **kwargs)
@@ -31,20 +39,20 @@
         name = getattr(self, "aggregation_name", None)
         if isinstance(name, str):
             return name
         return "value"
 
     def filter_aggregated_queryset(self, queryset):
         ordering_fields = getattr(self, "ordering_fields", [])
-        valid_fields = queryset[0].keys()
+        valid_fields = queryset[0].keys() if queryset.exists() else []
 
         if ordering_fields == "__all__":
             ordering_fields = valid_fields
         else:
-            ordering_fields = list(set(ordering_fields).intersection(set(queryset[0].keys())))
+            ordering_fields = list(set(ordering_fields).intersection(set(valid_fields)))
 
         if (fields := getattr(self, "aggregated_filterset_fields", None)) is not None:
             ValueFilter.set_filter_fields(fields, self.get_aggregation_name())
         filterset_class = getattr(self, "aggregated_filterset_class", ValueFilter)
 
         helper_view = HelperView(ordering_fields, filterset_class)
```

### Comparing `django_rest_aggregation-0.1.0/src/django_rest_aggregation.egg-info/PKG-INFO` & `django_rest_aggregation-0.2.0/src/django_rest_aggregation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_rest_aggregation
-Version: 0.1.0
+Version: 0.2.0
 Summary: A DRF mixin for aggregation endpoints
 Author-email: Simon Legtenborg <simon.legtenborg@singular-it.de>
 Project-URL: Homepage, https://github.com/singularit-de/django-rest-aggregation/
 Project-URL: Bug Tracker, https://github.com/singularit-de/django-rest-aggregation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,17 +26,17 @@
 - grouping by multiple fields
 - filtering and ordering
 
 ---
 
 ## Installation
 
-To install, use pip: &#10060;
+To install, use pip
 
-    pip install [COMING SOON] 
+    pip install django-rest-aggregation
 
 ## Quickstart
 
 Inherit the **AggregationMixin** in your ViewSet.
 
 ```python
 from django_rest_aggregation.mixins import AggregationMixin
```

### Comparing `django_rest_aggregation-0.1.0/tests/test_aggregation.py` & `django_rest_aggregation-0.2.0/tests/test_aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import datetime
+
 from django.db import connection
 from rest_framework.test import APITestCase
 
 from tests.models import Author, Book, Store
 
 
 class TestBasicFunctionality(APITestCase):
@@ -148,15 +150,15 @@
         # Minimum of DateField
         response = self.client.get(
             "/book/aggregation/",
             {"aggregation": "minimum", "aggregation_field": "pubdate"},
             format="json",
         )
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(response.data, [{"group": "all", "value": "2020-01-01"}])
+        self.assertEqual(response.data, [{"group": "all", "value": datetime.date(2020, 1, 1)}])
 
     def test_maximum(self):
         # Maximum of IntegerField
         response = self.client.get(
             "/book/aggregation/",
             {"aggregation": "maximum", "aggregation_field": "pages"},
             format="json",
@@ -185,15 +187,15 @@
         # Maximum of DateField
         response = self.client.get(
             "/book/aggregation/",
             {"aggregation": "maximum", "aggregation_field": "pubdate"},
             format="json",
         )
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(response.data, [{"group": "all", "value": "2020-01-05"}])
+        self.assertEqual(response.data, [{"group": "all", "value": datetime.date(2020, 1, 5)}])
 
 
 class TestGroupingAndAnnotations(APITestCase):
     def setUp(self):
         self.author = Author(name="John", age=20)
         self.author.save()
         self.author2 = Author(name="Jane", age=30)
@@ -880,20 +882,20 @@
                 "ordering": "CustomizedValue",
             },
             format="json",
         )
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.data["results"], [])
 
-    def test_sqlite_exception(self):
-        # throws exception if sqlite version is less than
+    def test_pagiation_count(self):
         response = self.client.get(
-            "/book/aggregation/",
+            "/customized_book/aggregation/",
             {
                 "aggregation": "sum",
                 "aggregation_field": "price",
-                "value__gte": 1,
+                "ordering": "CustomizedValue",
+                "CustomizedValue__lte": 0,
             },
             format="json",
         )
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(response.data, [{"group": "all", "value": 10.55}])
+        self.assertEqual(response.data["count"], 0)
```

