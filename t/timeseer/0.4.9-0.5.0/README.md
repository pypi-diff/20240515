# Comparing `tmp/timeseer-0.4.9.tar.gz` & `tmp/timeseer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseer-0.4.9.tar", last modified: Fri Feb 23 20:12:45 2024, max compression
+gzip compressed data, was "timeseer-0.5.0.tar", last modified: Tue May 14 14:39:59 2024, max compression
```

## Comparing `timeseer-0.4.9.tar` & `timeseer-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:12:45.109644 timeseer-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-02-23 20:12:45.109644 timeseer-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-02-23 20:12:35.000000 timeseer-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-23 20:12:35.000000 timeseer-0.4.9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:12:45.105644 timeseer-0.4.9/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13514 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/data_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/data_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/data_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/data_uploader_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/filters_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/filters_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-23 20:12:35.000000 timeseer-0.4.9/internal/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:12:45.105644 timeseer-0.4.9/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 20:12:35.000000 timeseer-0.4.9/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-02-23 20:12:35.000000 timeseer-0.4.9/metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-23 20:12:35.000000 timeseer-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 20:12:45.109644 timeseer-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 20:12:35.000000 timeseer-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:12:45.105644 timeseer-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-02-23 20:12:35.000000 timeseer-0.4.9/tests/test_filter_event_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-02-23 20:12:35.000000 timeseer-0.4.9/tests/test_filter_series_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-02-23 20:12:35.000000 timeseer-0.4.9/tests/test_filter_series_pyarrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:12:45.109644 timeseer-0.4.9/timeseer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-02-23 20:12:45.000000 timeseer-0.4.9/timeseer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-23 20:12:45.000000 timeseer-0.4.9/timeseer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 20:12:45.000000 timeseer-0.4.9/timeseer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-23 20:12:45.000000 timeseer-0.4.9/timeseer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-23 20:12:45.000000 timeseer-0.4.9/timeseer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:39:59.944018 timeseer-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-14 14:39:59.944018 timeseer-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-05-14 14:39:53.000000 timeseer-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-14 14:39:53.000000 timeseer-0.5.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:39:59.944018 timeseer-0.5.0/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19713 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/data_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/data_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/data_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/data_uploader_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/filters_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/filters_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-14 14:39:53.000000 timeseer-0.5.0/internal/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:39:59.944018 timeseer-0.5.0/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:39:53.000000 timeseer-0.5.0/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-14 14:39:53.000000 timeseer-0.5.0/metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 14:39:53.000000 timeseer-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:39:59.944018 timeseer-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 14:39:53.000000 timeseer-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:39:59.944018 timeseer-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-14 14:39:53.000000 timeseer-0.5.0/tests/test_filter_event_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-05-14 14:39:53.000000 timeseer-0.5.0/tests/test_filter_series_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-14 14:39:53.000000 timeseer-0.5.0/tests/test_filter_series_pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:39:59.944018 timeseer-0.5.0/timeseer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-14 14:39:59.000000 timeseer-0.5.0/timeseer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-14 14:39:59.000000 timeseer-0.5.0/timeseer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:39:59.000000 timeseer-0.5.0/timeseer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 14:39:59.000000 timeseer-0.5.0/timeseer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 14:39:59.000000 timeseer-0.5.0/timeseer.egg-info/top_level.txt
```

### Comparing `timeseer-0.4.9/PKG-INFO` & `timeseer-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseer
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python SDK for Timeseer.AI
 Author-email: "Timeseer.AI" <pypi@timeseer.ai>
 License: Copyright Timeseer.AI 2023
 Project-URL: Homepage, https://timeseer.ai/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `timeseer-0.4.9/README.md` & `timeseer-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/__init__.py` & `timeseer-0.5.0/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,21 +53,22 @@
     Metadata,
     SeriesSearch,
     SeriesSelector,
 )
 
 from timeseer_client.internal import (
     AugmentationStrategy,
+    DataSubstitutionCursor,
     EventFrame,
     ProcessType,
     Statistic,
     TimeseerClientException,
     UnknownAugmentationStrategyException,
 )
-from timeseer_client.internal.client import Client
+from timeseer_client.internal.client import Client, TLSOptions
 from timeseer_client.internal.data_services import DataServices, DataServiceSelector
 from timeseer_client.internal.data_sets import DataSets
 from timeseer_client.internal.data_substitutions import (
     apply_data_substitution,
     mask_event_frames,  # noqa: F401
 )
 from timeseer_client.internal.filters import filter_event_frames, filter_series
@@ -79,17 +80,19 @@
 
 register_custom_fields(Metadata)
 
 
 __all__ = [
     "AugmentationStrategy",
     "Client",
+    "TLSOptions",
     "DataServices",
     "DataServiceSelector",
     "DataSets",
+    "DataSubstitutionCursor",
     "DataType",
     "Dictionary",
     "EventFrame",
     "Flows",
     "InterpolationType",
     "Metadata",
     "ProcessType",
```

### Comparing `timeseer-0.4.9/internal/data_services.py` & `timeseer-0.5.0/internal/data_services.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 """Python client for Timeseer Data Services."""
 
 import time
 from dataclasses import dataclass
 from datetime import datetime
+from http import HTTPMethod
 from typing import Any, Dict, List, Optional, Union
 
 import pyarrow as pa
 from kukur import Metadata, SeriesSelector
 
 from timeseer_client.internal import (
     DataSubstitution,
+    DataSubstitutionCursor,
     DataSubstitutionData,
+    DataSubstitutionResponse,
     EventFrame,
-    JSONFlightClient,
+    ServerReturnedException,
     Statistic,
     TimeoutException,
+    TimeseerClient,
     TimeseerClientException,
+    parse_json_exception_message,
+    parse_json_response,
 )
 
 
 class DataServiceEvaluationFailedException(TimeseerClientException):
     """Thrown when a data service evaluation fails."""
 
     def __init__(self, name: str, view_name: str):
@@ -53,49 +59,52 @@
 class DataServices:
     """Data Services provide access to analysis results, time series data and statistics.
 
     Args:
         client: the Timeseer Client
     """
 
-    __client: JSONFlightClient
+    __client: TimeseerClient
 
-    def __init__(self, client: JSONFlightClient):
+    def __init__(self, client: TimeseerClient):
         self.__client = client
 
     def list(self) -> List[str]:
         """Return a list containing all the Data Service names."""
-        return self.__client.do_action("data_services/list", {})
+        response = self.__client.request(HTTPMethod.GET, "data-services")
+        return [data_service["name"] for data_service in parse_json_response(response)]
 
     def get(self, data_service_name: str) -> List[DataServiceSelector]:
         """Return a list containing a selector for each series set in a data service."""
-        return [
-            DataServiceSelector.from_data(data)
-            for data in self.__client.do_action(
-                "data_services/get", {"dataServiceName": data_service_name}
-            )
-        ]
+        response = self.__client.request(
+            HTTPMethod.GET,
+            "data-services/views",
+            query={"dataServiceName": data_service_name},
+        )
+        selector_data = parse_json_response(response)
+        return [DataServiceSelector.from_data(data) for data in selector_data]
 
     def wait_for_all_evaluations(
         self, data_service_name: str, *, timeout_seconds: float = 60.0
     ) -> None:
         """Wait until all the evaluations of a Data Service are complete.
 
         Args:
             data_service_name: The name of the Data Service to wait for.
             timeout_seconds: The number of seconds to wait until the evaluation is complete. (optional, keyword only)
 
         Raises:
             DataServiceEvaluationsFailedException when a failure is reported.
         """
-        body = {"dataServiceName": data_service_name}
+        query = {"dataServiceName": data_service_name}
         while timeout_seconds > 0:
-            job_states = self.__client.do_action(
-                "data_services/get_all_view_states", body
+            response = self.__client.request(
+                HTTPMethod.GET, "data-services/state", query=query
             )
+            job_states = parse_json_response(response)
             if all(
                 job_state["completed"] == job_state["total"] for job_state in job_states
             ):
                 if any(job_state["failed"] > 0 for job_state in job_states):
                     raise DataServiceEvaluationsFailedException(data_service_name)
                 return
             time.sleep(0.2)
@@ -111,17 +120,23 @@
         Args:
             data_service: The series set in a Data Service to wait for.
             timeout_seconds: The number of seconds to wait until the evaluation is complete. (optional, keyword only)
 
         Raises:
             DataServiceEvaluationFailedException when a failure is reported.
         """
-        body = {"dataService": data_service.to_data()}
+        query = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
+        }
         while timeout_seconds > 0:
-            job_state = self.__client.do_action("data_services/get_view_state", body)
+            response = self.__client.request(
+                HTTPMethod.GET, "data-services/view/state", query=query
+            )
+            job_state = parse_json_response(response)
             if job_state["completed"] == job_state["total"]:
                 if job_state["failed"] > 0:
                     raise DataServiceEvaluationFailedException(
                         data_service.name, data_service.series_set_name
                     )
                 return
             time.sleep(1)
@@ -148,166 +163,301 @@
             end_date: the end date of the data
                 Defaults to end date of the data service.
 
         Returns::
             A pyarrow Table with three columns: 'ts', 'value' and 'quality'.
         """
         body = {
-            "query": "data_services/get_data",
-            "dataService": data_service.to_data(),
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
             "selector": selector.to_data(),
             "startDate": start_date.isoformat() if start_date is not None else None,
             "endDate": end_date.isoformat() if end_date is not None else None,
         }
-        return self.__client.do_get(body)
+
+        response = self.__client.request(
+            HTTPMethod.POST,
+            "data-services/view/get-data",
+            body=body,
+            headers={
+                "Accept": "application/vnd.apache.arrow.stream",
+            },
+        )
+        if response.status not in [200, 201]:
+            raise ServerReturnedException(parse_json_exception_message(response))
+        buffer = response.read()
+        reader = pa.ipc.RecordBatchStreamReader(buffer)
+        return reader.read_all()
 
     def list_data_substitutions(  # noqa: PLR0913
         self,
         data_service: DataServiceSelector,
-        selector: SeriesSelector,
+        selector: Optional[SeriesSelector] = None,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
-        last_updated_date: Optional[datetime] = None,
-    ) -> List[DataSubstitution]:
+        last_modified_date: Optional[datetime] = None,
+        cursor: Optional[DataSubstitutionCursor] = None,
+    ) -> DataSubstitutionResponse:
         """List data substitutions for a Series in a data service.
 
         Args:
             data_service: The series set in the Data Service to look for data in.
             selector: Return data for the time series selected by this selector.
             start_date: The start date of the period of interest for the substitutions.
             end_date: The end date of the period of interest for the substitutions.
-            last_updated_date: Only list substitutions updated on or after the specified date.
+            last_modified_date: Only list substitutions updated on or after the specified date.
+            cursor: Only list substitutions newer than the substitution pointed to by the cursor.
 
         Returns::
             A list of `DataSubstitution`s
         """
         body = {
-            "dataService": data_service.to_data(),
-            "selector": selector.to_data(),
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
+            "selector": selector.to_data() if selector is not None else None,
             "startDate": start_date.isoformat() if start_date is not None else None,
             "endDate": end_date.isoformat() if end_date is not None else None,
-            "lastUpdatedDate": (
-                last_updated_date.isoformat() if last_updated_date is not None else None
+            "lastModifiedDate": (
+                last_modified_date.isoformat()
+                if last_modified_date is not None
+                else None
             ),
+            "cursor": cursor.to_data() if cursor is not None else None,
         }
-        return [
-            DataSubstitution.from_data(substitution_data)
-            for substitution_data in self.__client.do_action(
-                "data_services/list_data_substitutions", body
-            )
-        ]
+        response = self.__client.request(
+            HTTPMethod.POST, "data-services/view/data-substitutions", body=body
+        )
+        response_data = parse_json_response(response)
+        return DataSubstitutionResponse(
+            (
+                DataSubstitutionCursor.from_data(response_data["cursor"])
+                if response_data["cursor"] is not None
+                else None
+            ),
+            [
+                DataSubstitution.from_data(substitution_data)
+                for substitution_data in response_data["substitutions"]
+            ],
+        )
 
     def get_substitution_data(
         self, data_service: DataServiceSelector, data_substitution: DataSubstitution
     ) -> DataSubstitutionData:
         """Get the stored data for a given data substitution.
 
         Args:
             data_service: The series set in the Data Service to look for data in.
             data_substitution: The data substitution to query the data for.
 
         Returns::
             A pyarrow Table with three columns: 'ts', 'value' and 'quality'.
         """
-        body = {
-            "query": "data_services/get_substitution_data",
-            "dataService": data_service.to_data(),
-            "dataSubstitutionId": data_substitution.db_id,
+        query = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
+            "dataSubstitutionId": str(data_substitution.db_id),
         }
+
+        response = self.__client.request(
+            HTTPMethod.GET,
+            "data-services/view/get-substitution-data",
+            query=query,
+            headers={
+                "Accept": "application/vnd.apache.arrow.stream",
+            },
+        )
+        if response.status not in [200, 201]:
+            raise ServerReturnedException(parse_json_exception_message(response))
+        buffer = response.read()
+        reader = pa.ipc.RecordBatchStreamReader(buffer)
         return DataSubstitutionData(
-            data_substitution.start_date,
-            data_substitution.end_date,
-            self.__client.do_get(body),
+            data_substitution.start_date, data_substitution.end_date, reader.read_all()
         )
 
     def get_kpi_scores(self, data_service: DataServiceSelector) -> Dict[str, int]:
         """Get the kpi scores of a Data Service.
 
         Args:
             data_service: The series set in the Data Service to return scores for.
 
         Returns::
             The score per KPI as a percentage.
         """
-        body = {
-            "dataService": data_service.to_data(),
+        query = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
         }
-        return self.__client.do_action("data_services/get_kpi_scores", body)
+        response = self.__client.request(
+            HTTPMethod.GET, "data-services/view/kpi-scores", query=query
+        )
+        return parse_json_response(response)
 
     def convert_to_event_frame(self, table: pa.Table) -> List[EventFrame]:
         """Convert a PyArrow table to an EventFrame object."""
         return [EventFrame.from_row(data) for data in table.to_pylist()]
 
     def get_event_frames(  # noqa: PLR0913
         self,
         data_service: DataServiceSelector,
         selector: Optional[SeriesSelector] = None,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
         frame_type: Optional[Union[str, List[str]]] = None,
+        last_modified_date: Optional[datetime] = None,
     ) -> pa.Table:
         """Get all event frames matching the given criteria.
 
         Args:
             data_service: The series set in the Data Service to return event frames for.
             selector: the time series to which the event frames are linked.
             start_date: the start date of the range to find overlapping event frames in.
                 Defaults to start date of the data service.
             end_date: the end date of the range to find overlapping event frames in.
                 Defaults to end date of the data service.
             frame_type: the type or types of event frames to search for. Finds all types when empty.
+            last_modified_date: only include event frames modified on or later than this timestamp.
 
         Returns::
-            A pyarrow Table with 6 columns.
+            A pyarrow Table with 9 columns.
             The first column ('start_date') contains the start date.
             The second column ('end_date') contains the end date.
             The third column ('type') contains the type of the returned event frame as a string.
             The fourth column ('explanation') can contain the explanation for an event frame as a string.
             The fifth column ('status') can contain the status of an event frame as a string.
             Columns 6 contains possible multiple references for the event frame.
             the seventh column contains the properties of the event frame.
-            The eight column contains the uuid of the event frame.
+            The eighth column contains the uuid of the event frame.
+            The ninth column contains the last modified timestamp of the event frame.
         """
-        query: Dict[str, Any] = {
-            "query": "data_services/get_event_frames",
-            "dataService": data_service.to_data(),
+        body: Dict[str, Any] = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
             "selector": selector.to_data() if selector is not None else None,
             "startDate": start_date.isoformat() if start_date is not None else None,
             "endDate": end_date.isoformat() if end_date is not None else None,
+            "lastModifiedDate": (
+                last_modified_date.isoformat()
+                if last_modified_date is not None
+                else None
+            ),
         }
 
         if frame_type is not None:
-            query["type"] = frame_type
+            body["type"] = frame_type
 
-        return self.__client.do_get(query)
+        response = self.__client.request(
+            HTTPMethod.POST,
+            "data-services/view/event-frames",
+            body=body,
+            headers={
+                "Accept": "application/vnd.apache.arrow.stream",
+            },
+        )
+        if response.status not in [200, 201]:
+            raise ServerReturnedException(parse_json_exception_message(response))
+        buffer = response.read()
+        reader = pa.ipc.RecordBatchStreamReader(buffer)
+        return reader.read_all()
 
     def update_event_frame(self, event_frame: EventFrame):
         """Update the properties on an event frame.
 
         Args:
             event_frame: The event frame to be updated.
         """
-        data = {
+        body = {
             "eventFrame": event_frame.to_data(),
         }
-        return self.__client.do_action("data_services/update_event_frame", data)
+        self.__client.request(
+            HTTPMethod.POST, "data-services/view/event-frames/update", body=body
+        )
+
+    def create_multivariate_event_frame(  # noqa: PLR0913
+        self,
+        data_service: DataServiceSelector,
+        start_date: datetime,
+        end_date: datetime,
+        frame_type: str,
+    ):
+        """Create a multivariate event frame.
+
+        Args:
+            data_service: The series set in the data_service to create an event frame for.
+            start_date: the start date of the range to find overlapping event frames in.
+                Defaults to start date of the data service.
+            end_date: the end date of the range to find overlapping event frames in.
+                Defaults to end date of the data service.
+            frame_type: the type or types of event frames to search for. Finds all types when empty.
+        """
+        event_frame = {
+            "type": frame_type,
+            "startDate": start_date.isoformat(),
+            "endDate": end_date.isoformat(),
+        }
+
+        body = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
+            "eventFrames": [event_frame],
+        }
+        self.__client.request(
+            HTTPMethod.POST, "data-services/view/event-frames/create", body=body
+        )
+
+    def create_event_frame(  # noqa: PLR0913
+        self,
+        data_service: DataServiceSelector,
+        selector: SeriesSelector,
+        start_date: datetime,
+        end_date: datetime,
+        frame_type: str,
+    ):
+        """Create an event frame.
+
+        Args:
+            data_service: the series set in the data_service to create an event frame for.
+            selector: the time series to which the event frame is linked.
+            start_date: the start date of the event frame.
+            end_date: the end date of the event frame.
+            frame_type: the type of the event frame.
+        """
+        event_frame = {
+            "type": frame_type,
+            "startDate": start_date.isoformat(),
+            "endDate": end_date.isoformat(),
+        }
+
+        body = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
+            "selector": selector.to_data(),
+            "eventFrames": [event_frame],
+        }
+        self.__client.request(
+            HTTPMethod.POST, "data-services/view/event-frames/create", body=body
+        )
 
     def list_series(self, data_service: DataServiceSelector) -> List[SeriesSelector]:
         """Return all series in a Data Service Series Set.
 
         Args:
             data_service: The series set in the Data Service to list series for.
 
         Returns::
             A list of `SeriesSelector`s.
         """
-        query = {"dataService": data_service.to_data()}
+        query = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
+        }
+        response = self.__client.request(
+            HTTPMethod.GET, "data-services/view/series", query=query
+        )
         return [
-            SeriesSelector.from_data(data)
-            for data in self.__client.do_action("data_services/list_series", query)
+            SeriesSelector.from_data(data) for data in parse_json_response(response)
         ]
 
     def get_statistics(
         self,
         data_service: DataServiceSelector,
         selector: Optional[SeriesSelector] = None,
     ) -> List[Statistic]:
@@ -318,37 +468,44 @@
         Args:
             data_service: The series set in the Data Service to return statistics for.
             selector: The time series to return statistics for. (optional, keyword-only)
 
         Returns::
             A list of `Statistic`s.
         """
-        query: Dict[str, Any] = {"dataService": data_service.to_data()}
+        body: Dict[str, Any] = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
+        }
 
         if selector is not None:
-            query["selector"] = selector.to_data()
+            body["selector"] = selector.to_data()
 
-        return [
-            Statistic.from_data(data)
-            for data in self.__client.do_action("data_services/get_statistics", query)
-        ]
+        response = self.__client.request(
+            HTTPMethod.POST, "data-services/view/statistics", body=body
+        )
+        return [Statistic.from_data(data) for data in parse_json_response(response)]
 
     def get_calculated_metadata(
         self, data_service: DataServiceSelector, selector: SeriesSelector
     ) -> Metadata:
         """Return calculated metadata for a series in a Data Service.
 
         Args:
             data_service: The series set in a Data Service where the calculated metadata is kept.
             selector: The time series to return calculated metadata for.
 
         Returns::
             A `Metadata` object with the calculated metadata that's available.
         """
-        query = {
-            "dataService": data_service.to_data(),
+        body: Dict[str, Any] = {
+            "dataServiceName": data_service.name,
+            "dataServiceViewName": data_service.series_set_name,
             "selector": selector.to_data(),
         }
+        response = self.__client.request(
+            HTTPMethod.POST, "data-services/view/calculated-metadata", body=body
+        )
         return Metadata.from_data(
-            self.__client.do_action("data_services/get_calculated_metadata", query),
+            parse_json_response(response),
             selector,
         )
```

### Comparing `timeseer-0.4.9/internal/data_sets.py` & `timeseer-0.5.0/internal/data_sets.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Python client for Timeseer Data Sets."""
 
+from http import HTTPMethod
 from typing import Any, List, Tuple
 
 import pyarrow as pa
 from kukur import Metadata
 
 from timeseer_client.internal import (
-    JSONFlightClient,
     MissingTimezoneException,
+    TimeseerClient,
     UnsupportedDataFormatException,
+    parse_json_response,
 )
 
 HAS_PANDAS = True
 try:
     import pandas as pd
 
     from timeseer_client.internal import data_uploader_pandas
@@ -24,31 +26,32 @@
 class DataSets:
     """Data Sets are fixed collections of time series and their data in a specific time range.
 
     Args:
         client: the Timeseer Client
     """
 
-    __client: JSONFlightClient
+    __client: TimeseerClient
 
-    def __init__(self, client: JSONFlightClient):
+    def __init__(self, client: TimeseerClient):
         self.__client = client
 
     def list(self) -> List[str]:
         """Return a list containing all the data set names."""
-        return self.__client.do_action("data_sets/list", {})
+        response = self.__client.request(HTTPMethod.GET, "data-sets")
+        return [data_service["name"] for data_service in parse_json_response(response)]
 
     def remove_data(self, name: str):
         """Removes all data in a data set.
 
         Args:
             name: The name of the data set.
         """
         body = {"name": name}
-        self.__client.do_action("data_sets/remove_data", body)
+        self.__client.request(HTTPMethod.POST, "data-sets/remove-data", body=body)
 
     def upload_data(
         self,
         many_series: List[Tuple[Metadata, Any]],
     ):
         """Upload time series data to a Data Set.
 
@@ -66,15 +69,15 @@
             if isinstance(table, pa.Table):
                 data = _ensure_utc_timezone(table)
             elif HAS_PANDAS and isinstance(table, pd.DataFrame):
                 data = data_uploader_pandas.to_pyarrow_table(table)
             else:
                 raise UnsupportedDataFormatException()
             metadata_json = metadata.to_data()
-            self.__client.do_put({"metadata": metadata_json}, data)
+            self.__client.do_put(metadata_json, data)
 
 
 def _ensure_utc_timezone(table: pa.Table) -> pa.Table:
     if table.schema.field("ts").type.tz is None:
         raise MissingTimezoneException()
 
     return table.set_column(
```

### Comparing `timeseer-0.4.9/internal/data_substitutions.py` & `timeseer-0.5.0/internal/data_substitutions.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/internal/data_uploader_pandas.py` & `timeseer-0.5.0/internal/data_uploader_pandas.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/internal/filters.py` & `timeseer-0.5.0/internal/filters.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/internal/filters_arrow.py` & `timeseer-0.5.0/internal/filters_arrow.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/internal/filters_pandas.py` & `timeseer-0.5.0/internal/filters_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         return event_frames
 
     filtered = event_frames.loc[
         (event_frames["start_date"] > pd.to_datetime(end_date))
         | (event_frames["end_date"] > pd.to_datetime(start_date))
     ].copy()
 
-    filtered.loc[
-        filtered["start_date"] < pd.to_datetime(start_date), "start_date"
-    ] = pd.to_datetime(start_date)
-    filtered.loc[
-        filtered["end_date"] > pd.to_datetime(end_date), "end_date"
-    ] = pd.to_datetime(end_date)
+    filtered.loc[filtered["start_date"] < pd.to_datetime(start_date), "start_date"] = (
+        pd.to_datetime(start_date)
+    )
+    filtered.loc[filtered["end_date"] > pd.to_datetime(end_date), "end_date"] = (
+        pd.to_datetime(end_date)
+    )
     return filtered
 
 
 def _hold_last_value(
     series: pd.DataFrame, out_of_event_frames: List[bool]
 ) -> pd.DataFrame:
     last_acceptable = None
@@ -119,17 +119,17 @@
                         - series["ts"][index - (series_to_filter_count + 1)]
                     )
                     time_interpolation = numerator / denominator
                     new_value = (
                         last_acceptable * (1 - time_interpolation)
                         + series["value"][index] * time_interpolation
                     )
-                    series.loc[
-                        index - (series_to_filter_count - element), "value"
-                    ] = new_value
+                    series.loc[index - (series_to_filter_count - element), "value"] = (
+                        new_value
+                    )
             if last_acceptable is None:
                 remove_first_elements = series_to_filter_count
 
             last_acceptable = series["value"][index]
             series_to_filter_count = 0
         else:
             series_to_filter_count = series_to_filter_count + 1
```

### Comparing `timeseer-0.4.9/internal/flows.py` & `timeseer-0.5.0/internal/flows.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 """Python client for Timeseer Flows."""
 
 import time
 from datetime import datetime
-from typing import Dict, List, Optional
+from http import HTTPMethod
+from typing import Any, Dict, List, Optional
 
 from kukur import SeriesSelector
 
-from timeseer_client.internal import JSONFlightClient, TimeseerClientException
+from timeseer_client.internal import (
+    TimeseerClient,
+    TimeseerClientException,
+    parse_json_response,
+)
 
 
 class FlowEvaluationFailedException(TimeseerClientException):
     """Thrown when a flow evaluation fails."""
 
-    def __init__(self, flow_name: str | None):
+    def __init__(self, flow_name: Optional[str]):
         if flow_name is None:
             super().__init__("flow evaluation failed.")
         else:
             super().__init__(f'evaluation for flow "{flow_name}" failed.')
 
 
 class Flows:
     """Flows run modules to process time series data.
 
     Args:
         client: the Timeseer Client
     """
 
-    __client: JSONFlightClient
+    __client: TimeseerClient
 
-    def __init__(self, client: JSONFlightClient):
+    def __init__(self, client: TimeseerClient):
         self.__client = client
 
     def list(self) -> List[str]:
         """Return a list containing all the flow names."""
-        return self.__client.do_action("flows/list", {})
+        response = self.__client.request(HTTPMethod.GET, "flows")
+        return [flow["name"] for flow in parse_json_response(response)]
 
     def evaluate(self, flow_name: str, *, block=True):
         """Evaluate a flow.
 
         Args:
             flow_name: the name of the flow to evaluate
             block: block until the evaluation completes (keyword-only, default True)
@@ -63,49 +69,65 @@
             existing_flow_name: the name of the flow to duplicate.
             new_flow_name: the name of the duplicated flow.
             series_set_names: the names of the existing series sets to be used in the flow. (Optional).
             start_date: the start date of the flow (Optional).
             end_date: the end date of the flow (Optional).
             data_set_name: the name of the data set to use for the flow (Optional).
         """
-        body: Dict = {
-            "existingFlowName": existing_flow_name,
+        body: Dict[str, Any] = {
+            "name": existing_flow_name,
             "newFlowName": new_flow_name,
-            "seriesSetNames": series_set_names,
-            "dataSetName": data_set_name,
         }
+        if series_set_names is not None:
+            body["seriesSetNames"] = series_set_names
         if start_date is not None:
             body["startDate"] = start_date.isoformat()
         if end_date is not None:
             body["endDate"] = end_date.isoformat()
-        self.__client.do_action("flows/duplicate", body)
+        if data_set_name is not None:
+            body["dataSetName"] = data_set_name
+        self.__client.request(
+            HTTPMethod.POST,
+            "flows/duplicate",
+            body=body,
+        )
 
 
 def evaluate_flow(
-    client: JSONFlightClient,
+    client: TimeseerClient,
     flow_name: str,
     *,
     limitations: Optional[List[SeriesSelector]] = None,
     block=True,
 ):
     """Trigger an evaluation of the flow with the given name."""
-    flow: Dict = {"flowName": flow_name}
+    body: Dict = {"name": flow_name}
     if limitations is not None:
-        flow["limitations"] = [selector.to_data() for selector in limitations]
-    response = client.do_action("flows/evaluate", flow)
+        body["limitations"] = [selector.to_data() for selector in limitations]
+    http_response = client.request(
+        HTTPMethod.POST,
+        "flows/evaluate",
+        body=body,
+    )
+    response = parse_json_response(http_response)
     if block:
         wait_for_flow_evaluation(client, response, flow_name)
 
 
 def wait_for_flow_evaluation(
-    client: JSONFlightClient, response: Dict, flow_name: str | None = None
+    client: TimeseerClient, response: Dict, flow_name: Optional[str] = None
 ):
     """Repeatedly query for the flow evaluation state of the given flow evaluation group."""
     while True:
-        state = client.do_action("flows/get_evaluation_state", response)
+        http_response = client.request(
+            HTTPMethod.POST,
+            "flows/evaluate/state",
+            body=response,
+        )
+        state = parse_json_response(http_response)
         if (
             state["completed"] == state["total"]
             and state["blockCompleted"] == state["blockTotal"]
         ):
             if (
                 state["failed"] > 0
                 or state["blockFailed"] > 0
```

### Comparing `timeseer-0.4.9/internal/profile.py` & `timeseer-0.5.0/internal/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Convenience functions to profile a time series."""
 
 from typing import Dict, List, Tuple
 
 from kukur import Metadata, SeriesSelector
 from pyarrow import Table
 
-from timeseer_client.internal import JSONFlightClient
+from timeseer_client.internal import TimeseerClient
 from timeseer_client.internal.data_services import DataServices, DataServiceSelector
 from timeseer_client.internal.data_sets import DataSets
 from timeseer_client.internal.flows import Flows
 from timeseer_client.internal.resources import Resources
 
 
 def profile(
-    client: JSONFlightClient, name: str, many_series: List[Tuple[Metadata, Table]]
+    client: TimeseerClient, name: str, many_series: List[Tuple[Metadata, Table]]
 ) -> List[Dict[str, str]]:
     """Profile time series.
 
     This creates a Data Set, Flow and Data Service with the given name.
     Waits until the flow has been evaluated.
 
     Args:
```

### Comparing `timeseer-0.4.9/internal/resources.py` & `timeseer-0.5.0/internal/resources.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 """Python client for Timeseer resources."""
 
 import json
 import time
+from http import HTTPMethod
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 import kukur.config
 
 try:
     import yaml
 
     HAS_YAML = True
 except ImportError:
     HAS_YAML = False
 
 from timeseer_client.internal import (
-    JSONFlightClient,
     MissingModuleException,
+    ServerReturnedException,
     TimeoutException,
+    TimeseerClient,
+    parse_json_response,
 )
 
 
 class Resources:
     """Resources are the main organizational structures within Timeseer.
 
     Args:
         client: the Timeseer Client
     """
 
-    __client: JSONFlightClient
+    __client: TimeseerClient
 
-    def __init__(self, client: JSONFlightClient):
+    def __init__(self, client: TimeseerClient):
         self.__client = client
 
     def list(self, *, resource_type: Optional[str] = None) -> List[Dict]:
         """List all defined resources.
 
         Args:
             resource_type: Only list resources of this type (optional, keyword-only)
 
         Returns:
             A list of dictionaries of resource 'name' and 'type'.
         """
-        body = {}
+        query = {}
         if resource_type is not None:
-            body["resourceType"] = resource_type
-        return self.__client.do_action("resources/list", body)
+            query["type"] = resource_type
+        response = self.__client.request(HTTPMethod.GET, "resources", query=query)
+        return parse_json_response(response)
 
     def create(
         self,
         resources: Optional[List[Dict]] = None,
         *,
         resource: Optional[Dict] = None,
         path: Optional[Union[Path, str]] = None,
@@ -76,30 +80,28 @@
                 if not HAS_YAML:
                     raise MissingModuleException("PyYAML")
                 all_resources.extend(_read_yaml(path))
             elif path.suffix == ".toml":
                 all_resources.extend(_read_toml(path))
             elif path.suffix == ".json":
                 all_resources.extend(_read_json(path))
-        body = {
-            "resources": all_resources,
-        }
-
-        self.__client.do_action("resources/create", body)
+        body = {"resources": all_resources}
+        self.__client.request(HTTPMethod.POST, "resources", body=body)
 
     def read(self, resource: Dict[str, str]) -> Dict:
         """Return a resource definition.
 
         Args:
             resource: Dictionary of resource 'type' and 'name'
 
         Returns:
             The resource definition.
         """
-        return self.__client.do_action("resources/read", resource)
+        response = self.__client.request(HTTPMethod.GET, "resources", query=resource)
+        return parse_json_response(response)
 
     def delete(
         self,
         resources: Optional[List[Dict]] = None,
         *,
         resource: Optional[Dict] = None,
         timeout_seconds: int = 60,
@@ -125,18 +127,19 @@
 
         body = {
             "resources": all_resources,
         }
 
         message = None
         while timeout_seconds > 0:
-            response = self.__client.do_action("resources/delete", body)
-            if response is None:
+            try:
+                self.__client.request(HTTPMethod.DELETE, "resources", body=body)
                 return
-            message = response.get("message")
+            except ServerReturnedException as err:
+                message = str(err)
             timeout_seconds = timeout_seconds - 1
             time.sleep(1)
 
         raise TimeoutException(message)
 
 
 def _read_yaml(path: Path) -> List[Dict]:
```

### Comparing `timeseer-0.4.9/internal/sources.py` & `timeseer-0.5.0/internal/sources.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """Python client for Timeseer Sources."""
 
 import time
+from http import HTTPMethod
 
-from timeseer_client.internal import JSONFlightClient
+from timeseer_client.internal import TimeseerClient, parse_json_response
 
 
 class Sources:
     """Sources provide access to timeseries and metadata.
 
     Args:
         client: the Timeseer Client
     """
 
-    __client: JSONFlightClient
+    __client: TimeseerClient
 
-    def __init__(self, client: JSONFlightClient):
+    def __init__(self, client: TimeseerClient):
         self.__client = client
 
     def update(self, source_name: str, *, block=True):
         """Update a source.
 
         Args:
             source_name: the name of the source to analyze
             block: block until the update completes (keyword-only, default True)
         """
-        self.__client.do_action("sources/update", {"sourceName": source_name})
+        self.__client.request(
+            HTTPMethod.POST, "sources/update", query={"sourceName": source_name}
+        )
 
         if block:
             self.wait_for_update(source_name)
 
     def wait_for_update(self, source_name: str):
         """Wait until the metadata update of the given source completes.
 
         Args:
             source_name: the name of the source to analyze
         """
         while True:
-            state = self.__client.do_action(
-                "sources/get_update_state", {"sourceName": source_name}
+            response = self.__client.request(
+                HTTPMethod.GET, "sources/update", query={"sourceName": source_name}
             )
+            state = parse_json_response(response)
             if state["completed"] == state["total"]:
                 break
             time.sleep(0.2)
```

### Comparing `timeseer-0.4.9/metadata/fields.py` & `timeseer-0.5.0/metadata/fields.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/pyproject.toml` & `timeseer-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/tests/test_filter_event_frames.py` & `timeseer-0.5.0/tests/test_filter_event_frames.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/tests/test_filter_series_pandas.py` & `timeseer-0.5.0/tests/test_filter_series_pandas.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/tests/test_filter_series_pyarrow.py` & `timeseer-0.5.0/tests/test_filter_series_pyarrow.py`

 * *Files identical despite different names*

### Comparing `timeseer-0.4.9/timeseer.egg-info/PKG-INFO` & `timeseer-0.5.0/timeseer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseer
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python SDK for Timeseer.AI
 Author-email: "Timeseer.AI" <pypi@timeseer.ai>
 License: Copyright Timeseer.AI 2023
 Project-URL: Homepage, https://timeseer.ai/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `timeseer-0.4.9/timeseer.egg-info/SOURCES.txt` & `timeseer-0.5.0/timeseer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

