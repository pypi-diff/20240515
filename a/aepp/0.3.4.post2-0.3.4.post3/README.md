# Comparing `tmp/aepp-0.3.4.post2.tar.gz` & `tmp/aepp-0.3.4.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepp-0.3.4.post2.tar", last modified: Tue May  7 13:42:31 2024, max compression
+gzip compressed data, was "aepp-0.3.4.post3.tar", last modified: Wed May 15 13:14:37 2024, max compression
```

## Comparing `aepp-0.3.4.post2.tar` & `aepp-0.3.4.post3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:31.142091 aepp-0.3.4.post2/
--rw-rw-rw-   0        0        0    10337 2023-05-10 18:38:24.000000 aepp-0.3.4.post2/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-10 18:38:24.000000 aepp-0.3.4.post2/MANIFEST.in
--rw-rw-rw-   0        0        0     4274 2024-05-07 13:42:31.126465 aepp-0.3.4.post2/PKG-INFO
--rw-rw-rw-   0        0        0     3457 2024-03-18 13:57:44.000000 aepp-0.3.4.post2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:31.073678 aepp-0.3.4.post2/aepp/
--rw-rw-rw-   0        0        0     5224 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/aepp/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-07 13:39:17.000000 aepp-0.3.4.post2/aepp/__version__.py
--rw-rw-rw-   0        0        0    17426 2024-02-21 09:35:17.000000 aepp-0.3.4.post2/aepp/accesscontrol.py
--rw-rw-rw-   0        0        0    58818 2024-03-18 13:57:44.000000 aepp-0.3.4.post2/aepp/catalog.py
--rw-rw-rw-   0        0        0     2579 2024-03-18 13:57:44.000000 aepp-0.3.4.post2/aepp/config.py
--rw-rw-rw-   0        0        0    17655 2024-02-21 09:35:17.000000 aepp-0.3.4.post2/aepp/configs.py
--rw-rw-rw-   0        0        0    30327 2024-04-26 09:38:20.000000 aepp-0.3.4.post2/aepp/connector.py
--rw-rw-rw-   0        0        0    42510 2024-02-21 09:35:17.000000 aepp-0.3.4.post2/aepp/customerprofile.py
--rw-rw-rw-   0        0        0    14252 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/dataaccess.py
--rw-rw-rw-   0        0        0    27357 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/dataprep.py
--rw-rw-rw-   0        0        0     8778 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/datasets.py
--rw-rw-rw-   0        0        0    24348 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/destination.py
--rw-rw-rw-   0        0        0     5378 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/destinationinstanceservice.py
--rw-rw-rw-   0        0        0    18629 2023-09-28 14:47:02.000000 aepp-0.3.4.post2/aepp/exportDatasetToDataLandingZone.py
--rw-rw-rw-   0        0        0    76727 2024-05-07 13:37:57.000000 aepp-0.3.4.post2/aepp/flowservice.py
--rw-rw-rw-   0        0        0    13075 2024-03-18 13:57:44.000000 aepp-0.3.4.post2/aepp/hygiene.py
--rw-rw-rw-   0        0        0    20080 2024-02-21 09:35:17.000000 aepp-0.3.4.post2/aepp/identity.py
--rw-rw-rw-   0        0        0    21460 2024-03-25 07:12:28.000000 aepp-0.3.4.post2/aepp/ingestion.py
--rw-rw-rw-   0        0        0     9951 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/observability.py
--rw-rw-rw-   0        0        0    24930 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/policy.py
--rw-rw-rw-   0        0        0     8794 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/privacyservice.py
--rw-rw-rw-   0        0        0    52507 2023-11-02 07:50:24.000000 aepp-0.3.4.post2/aepp/queryservice.py
--rw-rw-rw-   0        0        0    21063 2024-04-11 15:08:07.000000 aepp-0.3.4.post2/aepp/sandboxes.py
--rw-rw-rw-   0        0        0   215461 2024-04-22 12:03:10.000000 aepp-0.3.4.post2/aepp/schema.py
--rw-rw-rw-   0        0        0    42377 2024-04-02 14:45:01.000000 aepp-0.3.4.post2/aepp/segmentation.py
--rw-rw-rw-   0        0        0     7761 2023-10-23 08:56:18.000000 aepp-0.3.4.post2/aepp/sensei.py
--rw-rw-rw-   0        0        0     1200 2023-10-23 08:56:14.000000 aepp-0.3.4.post2/aepp/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:31.126465 aepp-0.3.4.post2/aepp.egg-info/
--rw-rw-rw-   0        0        0     4274 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      928 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 13:42:31.142091 aepp-0.3.4.post2/setup.cfg
--rw-rw-rw-   0        0        0     2206 2023-11-23 12:55:39.000000 aepp-0.3.4.post2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:31.126465 aepp-0.3.4.post2/tests/
--rw-rw-rw-   0        0        0      623 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/__init__.py
--rw-rw-rw-   0        0        0     2246 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/catalog_test.py
--rw-rw-rw-   0        0        0     1238 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/dataaccess_test.py
--rw-rw-rw-   0        0        0     1093 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/datasets_test.py
--rw-rw-rw-   0        0        0     2105 2023-05-23 14:25:29.000000 aepp-0.3.4.post2/tests/destinationinstanceservice_test.py
--rw-rw-rw-   0        0        0     7684 2023-09-28 14:47:02.000000 aepp-0.3.4.post2/tests/exportDatasetToDatalandingZone_test.py
--rw-rw-rw-   0        0        0     4208 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/flowservice_test.py
--rw-rw-rw-   0        0        0     2774 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/schema_test.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:14:37.740993 aepp-0.3.4.post3/
+-rw-rw-rw-   0        0        0    10337 2023-05-10 18:38:24.000000 aepp-0.3.4.post3/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-10 18:38:24.000000 aepp-0.3.4.post3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4274 2024-05-15 13:14:37.737002 aepp-0.3.4.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     3457 2024-03-18 13:57:44.000000 aepp-0.3.4.post3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 13:14:37.672803 aepp-0.3.4.post3/aepp/
+-rw-rw-rw-   0        0        0     5224 2023-05-10 18:04:54.000000 aepp-0.3.4.post3/aepp/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-15 13:10:32.000000 aepp-0.3.4.post3/aepp/__version__.py
+-rw-rw-rw-   0        0        0    17426 2024-02-21 09:35:17.000000 aepp-0.3.4.post3/aepp/accesscontrol.py
+-rw-rw-rw-   0        0        0    58818 2024-03-18 13:57:44.000000 aepp-0.3.4.post3/aepp/catalog.py
+-rw-rw-rw-   0        0        0     2579 2024-03-18 13:57:44.000000 aepp-0.3.4.post3/aepp/config.py
+-rw-rw-rw-   0        0        0    17655 2024-02-21 09:35:17.000000 aepp-0.3.4.post3/aepp/configs.py
+-rw-rw-rw-   0        0        0    30327 2024-04-26 09:38:20.000000 aepp-0.3.4.post3/aepp/connector.py
+-rw-rw-rw-   0        0        0    42510 2024-02-21 09:35:17.000000 aepp-0.3.4.post3/aepp/customerprofile.py
+-rw-rw-rw-   0        0        0    14252 2023-11-02 07:50:23.000000 aepp-0.3.4.post3/aepp/dataaccess.py
+-rw-rw-rw-   0        0        0    27357 2023-11-02 07:50:23.000000 aepp-0.3.4.post3/aepp/dataprep.py
+-rw-rw-rw-   0        0        0     8778 2023-11-02 07:50:23.000000 aepp-0.3.4.post3/aepp/datasets.py
+-rw-rw-rw-   0        0        0    24348 2023-11-02 07:50:23.000000 aepp-0.3.4.post3/aepp/destination.py
+-rw-rw-rw-   0        0        0     5378 2023-11-02 07:50:23.000000 aepp-0.3.4.post3/aepp/destinationinstanceservice.py
+-rw-rw-rw-   0        0        0    18629 2023-09-28 14:47:02.000000 aepp-0.3.4.post3/aepp/exportDatasetToDataLandingZone.py
+-rw-rw-rw-   0        0        0    76727 2024-05-07 13:37:57.000000 aepp-0.3.4.post3/aepp/flowservice.py
+-rw-rw-rw-   0        0        0    13075 2024-03-18 13:57:44.000000 aepp-0.3.4.post3/aepp/hygiene.py
+-rw-rw-rw-   0        0        0    20080 2024-02-21 09:35:17.000000 aepp-0.3.4.post3/aepp/identity.py
+-rw-rw-rw-   0        0        0    21460 2024-03-25 07:12:28.000000 aepp-0.3.4.post3/aepp/ingestion.py
+-rw-rw-rw-   0        0        0     9951 2023-11-02 07:50:23.000000 aepp-0.3.4.post3/aepp/observability.py
+-rw-rw-rw-   0        0        0    24924 2024-05-15 13:10:26.000000 aepp-0.3.4.post3/aepp/policy.py
+-rw-rw-rw-   0        0        0     8794 2023-11-02 07:50:23.000000 aepp-0.3.4.post3/aepp/privacyservice.py
+-rw-rw-rw-   0        0        0    52507 2023-11-02 07:50:24.000000 aepp-0.3.4.post3/aepp/queryservice.py
+-rw-rw-rw-   0        0        0    21063 2024-04-11 15:08:07.000000 aepp-0.3.4.post3/aepp/sandboxes.py
+-rw-rw-rw-   0        0        0   215461 2024-04-22 12:03:10.000000 aepp-0.3.4.post3/aepp/schema.py
+-rw-rw-rw-   0        0        0    42377 2024-04-02 14:45:01.000000 aepp-0.3.4.post3/aepp/segmentation.py
+-rw-rw-rw-   0        0        0     7761 2023-10-23 08:56:18.000000 aepp-0.3.4.post3/aepp/sensei.py
+-rw-rw-rw-   0        0        0     1200 2023-10-23 08:56:14.000000 aepp-0.3.4.post3/aepp/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:14:37.734010 aepp-0.3.4.post3/aepp.egg-info/
+-rw-rw-rw-   0        0        0     4274 2024-05-15 13:14:37.000000 aepp-0.3.4.post3/aepp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      928 2024-05-15 13:14:37.000000 aepp-0.3.4.post3/aepp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 13:14:37.000000 aepp-0.3.4.post3/aepp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-15 13:14:37.000000 aepp-0.3.4.post3/aepp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 13:14:37.000000 aepp-0.3.4.post3/aepp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 13:14:37.741990 aepp-0.3.4.post3/setup.cfg
+-rw-rw-rw-   0        0        0     2206 2023-11-23 12:55:39.000000 aepp-0.3.4.post3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:14:37.730021 aepp-0.3.4.post3/tests/
+-rw-rw-rw-   0        0        0      623 2023-05-10 18:04:54.000000 aepp-0.3.4.post3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2246 2023-05-10 18:04:54.000000 aepp-0.3.4.post3/tests/catalog_test.py
+-rw-rw-rw-   0        0        0     1238 2023-05-10 18:04:54.000000 aepp-0.3.4.post3/tests/dataaccess_test.py
+-rw-rw-rw-   0        0        0     1093 2023-05-10 18:04:54.000000 aepp-0.3.4.post3/tests/datasets_test.py
+-rw-rw-rw-   0        0        0     2105 2023-05-23 14:25:29.000000 aepp-0.3.4.post3/tests/destinationinstanceservice_test.py
+-rw-rw-rw-   0        0        0     7684 2023-09-28 14:47:02.000000 aepp-0.3.4.post3/tests/exportDatasetToDatalandingZone_test.py
+-rw-rw-rw-   0        0        0     4208 2023-05-10 18:04:54.000000 aepp-0.3.4.post3/tests/flowservice_test.py
+-rw-rw-rw-   0        0        0     2774 2023-05-10 18:04:54.000000 aepp-0.3.4.post3/tests/schema_test.py
```

### Comparing `aepp-0.3.4.post2/LICENSE` & `aepp-0.3.4.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/PKG-INFO` & `aepp-0.3.4.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.3.4.post2
+Version: 0.3.4.post3
 Summary: Package to manage AEP API endpoint and some helper functions
 Home-page: https://github.com/adobe/aepp
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `aepp-0.3.4.post2/README.md` & `aepp-0.3.4.post3/README.md`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/__init__.py` & `aepp-0.3.4.post3/aepp/__init__.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/accesscontrol.py` & `aepp-0.3.4.post3/aepp/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/catalog.py` & `aepp-0.3.4.post3/aepp/catalog.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/config.py` & `aepp-0.3.4.post3/aepp/config.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/configs.py` & `aepp-0.3.4.post3/aepp/configs.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/connector.py` & `aepp-0.3.4.post3/aepp/connector.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/customerprofile.py` & `aepp-0.3.4.post3/aepp/customerprofile.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/dataaccess.py` & `aepp-0.3.4.post3/aepp/dataaccess.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/dataprep.py` & `aepp-0.3.4.post3/aepp/dataprep.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/datasets.py` & `aepp-0.3.4.post3/aepp/datasets.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/destination.py` & `aepp-0.3.4.post3/aepp/destination.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/destinationinstanceservice.py` & `aepp-0.3.4.post3/aepp/destinationinstanceservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/exportDatasetToDataLandingZone.py` & `aepp-0.3.4.post3/aepp/exportDatasetToDataLandingZone.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/flowservice.py` & `aepp-0.3.4.post3/aepp/flowservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/hygiene.py` & `aepp-0.3.4.post3/aepp/hygiene.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/identity.py` & `aepp-0.3.4.post3/aepp/identity.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/ingestion.py` & `aepp-0.3.4.post3/aepp/ingestion.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/observability.py` & `aepp-0.3.4.post3/aepp/observability.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/policy.py` & `aepp-0.3.4.post3/aepp/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software distributed under
 #  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 #  OF ANY KIND, either express or implied. See the License for the specific language
 #  governing permissions and limitations under the License.
 
 import aepp
-import typing
+from typing import Union, IO
 from aepp import connector
 import logging
 from .configs import ConnectObject
 import json
 
 class Policy:
     """
@@ -23,15 +23,15 @@
 
     ## logging capability
     loggingEnabled = False
     logger = None
 
     def __init__(
         self,
-        config: typing.Union[dict,ConnectObject] = aepp.config.config_object,
+        config: Union[dict,ConnectObject] = aepp.config.config_object,
         header: dict = aepp.config.header,
         loggingObject: dict = None,
         **kwargs,
     ):
         """
         Instantiate the class to manage DULE rules and statement directly.
         Arguments:
@@ -197,15 +197,15 @@
             raise Exception("Expected a policy id")
         if self.loggingEnabled:
             self.logger.debug(f"Starting getPoliciesCustom")
         path = f"/policies/custom/{policy_id}"
         res = self.connector.getData(self.endpoint + path, headers=self.header)
         return res
 
-    def createPolicy(self, policy: typing.Union(dict, typing.IO) = None):
+    def createPolicy(self, policy: Union[dict, IO] = None):
         """
         Create a custom policy.
         Arguments:
             policy : REQUIRED : A dictionary contaning the policy you would like to implement.
         """
         if self.loggingEnabled:
             self.logger.debug(f"Starting createPolicy")
```

### Comparing `aepp-0.3.4.post2/aepp/privacyservice.py` & `aepp-0.3.4.post3/aepp/privacyservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/queryservice.py` & `aepp-0.3.4.post3/aepp/queryservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/sandboxes.py` & `aepp-0.3.4.post3/aepp/sandboxes.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/schema.py` & `aepp-0.3.4.post3/aepp/schema.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/segmentation.py` & `aepp-0.3.4.post3/aepp/segmentation.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/sensei.py` & `aepp-0.3.4.post3/aepp/sensei.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp/utils.py` & `aepp-0.3.4.post3/aepp/utils.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/aepp.egg-info/PKG-INFO` & `aepp-0.3.4.post3/aepp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.3.4.post2
+Version: 0.3.4.post3
 Summary: Package to manage AEP API endpoint and some helper functions
 Home-page: https://github.com/adobe/aepp
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `aepp-0.3.4.post2/aepp.egg-info/SOURCES.txt` & `aepp-0.3.4.post3/aepp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/setup.py` & `aepp-0.3.4.post3/setup.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/tests/__init__.py` & `aepp-0.3.4.post3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/tests/catalog_test.py` & `aepp-0.3.4.post3/tests/catalog_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/tests/dataaccess_test.py` & `aepp-0.3.4.post3/tests/dataaccess_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/tests/datasets_test.py` & `aepp-0.3.4.post3/tests/datasets_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/tests/destinationinstanceservice_test.py` & `aepp-0.3.4.post3/tests/destinationinstanceservice_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/tests/exportDatasetToDatalandingZone_test.py` & `aepp-0.3.4.post3/tests/exportDatasetToDatalandingZone_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/tests/flowservice_test.py` & `aepp-0.3.4.post3/tests/flowservice_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post2/tests/schema_test.py` & `aepp-0.3.4.post3/tests/schema_test.py`

 * *Files identical despite different names*

