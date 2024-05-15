# Comparing `tmp/paloalto_panorama_sdk-0.0.7.tar.gz` & `tmp/paloalto_panorama_sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paloalto_panorama_sdk-0.0.7.tar", last modified: Wed May  8 12:26:08 2024, max compression
+gzip compressed data, was "paloalto_panorama_sdk-0.0.8.tar", last modified: Wed May 15 07:47:34 2024, max compression
```

## Comparing `paloalto_panorama_sdk-0.0.7.tar` & `paloalto_panorama_sdk-0.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:08.137727 paloalto_panorama_sdk-0.0.7/
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.7/LICENSE
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.7/MANIFEST.in
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-08 12:26:08.135636 paloalto_panorama_sdk-0.0.7/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)      809 2024-04-29 13:58:58.000000 paloalto_panorama_sdk-0.0.7/README.md
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:07.731671 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/
--rw-r--r--   0 timoriedinger   (501) staff       (20)      185 2024-05-08 12:25:57.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/address_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/address_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      631 2024-05-08 12:05:24.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/device_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/key_manager.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:07.994731 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:16:15.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      735 2024-04-30 08:19:39.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/address_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      926 2024-05-03 05:32:44.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/address_group_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      559 2024-05-08 12:10:05.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/device_group_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     2373 2024-05-08 06:06:03.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      751 2024-05-03 06:29:49.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/service_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      705 2024-05-03 06:23:45.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     2845 2024-05-08 12:12:05.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_sdk.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     4786 2024-05-08 05:09:52.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/security_post_rules_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/service_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/service_manager.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:07.744476 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1180 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/requires.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/top_level.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-05-08 12:26:08.137841 paloalto_panorama_sdk-0.0.7/setup.cfg
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.7/setup.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:08.050080 paloalto_panorama_sdk-0.0.7/tests/
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:08.134544 paloalto_panorama_sdk-0.0.7/tests/PanoramaAPIMock/
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.7/tests/PanoramaAPIMock/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.7/tests/PanoramaAPIMock/panoramaAPIMock.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.7/tests/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.7/tests/test_service.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-15 07:47:34.046999 paloalto_panorama_sdk-0.0.8/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.8/LICENSE
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.8/MANIFEST.in
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-15 07:47:34.046514 paloalto_panorama_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      809 2024-04-29 13:58:58.000000 paloalto_panorama_sdk-0.0.8/README.md
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-15 07:47:34.003796 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      185 2024-05-15 07:44:57.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1766 2024-05-15 07:43:49.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/address_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/address_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      631 2024-05-08 12:05:24.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/device_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/key_manager.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-15 07:47:34.034538 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:16:15.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      735 2024-04-30 08:19:39.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/address_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      926 2024-05-03 05:32:44.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/address_group_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      559 2024-05-08 12:10:05.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/device_group_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     2373 2024-05-08 06:06:03.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      751 2024-05-03 06:29:49.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/service_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      705 2024-05-03 06:23:45.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     2819 2024-05-15 07:44:19.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_sdk.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     4744 2024-05-15 07:44:02.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/security_post_rules_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1805 2024-05-15 07:43:40.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/service_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/service_manager.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-15 07:47:34.013821 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-15 07:47:33.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1180 2024-05-15 07:47:33.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-05-15 07:47:33.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-05-15 07:47:33.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/requires.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-05-15 07:47:33.000000 paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/top_level.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-05-15 07:47:34.047079 paloalto_panorama_sdk-0.0.8/setup.cfg
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.8/setup.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-15 07:47:34.040123 paloalto_panorama_sdk-0.0.8/tests/
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-15 07:47:34.046102 paloalto_panorama_sdk-0.0.8/tests/PanoramaAPIMock/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.8/tests/PanoramaAPIMock/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.8/tests/PanoramaAPIMock/panoramaAPIMock.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.8/tests/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.8/tests/test_service.py
```

### Comparing `paloalto_panorama_sdk-0.0.7/LICENSE` & `paloalto_panorama_sdk-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/PKG-INFO` & `paloalto_panorama_sdk-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paloalto_panorama_sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: This SDK is designed to make it easier to work with the Palo Alto Panorama API.
 Author: Timo Riedinger
 Author-email: timo.riedinger@bechtle.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paloalto_panorama_sdk-0.0.7/README.md` & `paloalto_panorama_sdk-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/address_groups_manager.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/address_groups_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,9 +36,8 @@
                         {
                             'member': members.split('\n')
                         },
                     'description': description
                 }
             ]
         }
-        print(address_group_payload)
         return address_group_payload
```

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/address_manager.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/address_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/device_groups_manager.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/device_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/key_manager.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/key_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/address_data.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/address_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/address_group_data.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/address_group_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/device_group_data.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/device_group_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/service_data.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/service_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_sdk.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/panorama_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from pprint import pprint
 
 from paloalto_panorama_sdk.address_groups_manager import AddressGroupsManager
 from paloalto_panorama_sdk.address_manager import AddressManager
 from paloalto_panorama_sdk.device_groups_manager import DeviceGroupsManager
 from paloalto_panorama_sdk.key_manager import KeyManager
 from paloalto_panorama_sdk.panorama_data_kit.address_data import Address
 from paloalto_panorama_sdk.panorama_data_kit.address_group_data import AddressGroup
```

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/security_post_rules_manager.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/security_post_rules_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
             source_group=security_post_rule.source_member,
             to_zone=security_post_rule.to_member,
             destination_group=security_post_rule.destination_member,
             service=security_post_rule.service_member,
             profile_type=security_post_rule.profile_type,
             profile=security_post_rule.profile_setting
         )
-        print(decoded_security_post_rule)
 
     def list_post_rules(self, location='shared', device_group='TestGroup'):
         params = {'location': location, 'device-group': device_group}
         response = requests.get(url=self.url, headers=self.headers, params=params, verify=self.verify)
         post_rules = json.loads(response.content.decode('utf-8'))
         return post_rules
```

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/service_groups_manager.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/service_groups_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,9 +36,8 @@
                     'members':
                         {
                             'member': members.split('\n')
                         },
                 }
             ]
         }
-        print(service_group_payload)
         return service_group_payload
```

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/service_manager.py` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk/service_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/PKG-INFO` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paloalto-panorama-sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: This SDK is designed to make it easier to work with the Palo Alto Panorama API.
 Author: Timo Riedinger
 Author-email: timo.riedinger@bechtle.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/SOURCES.txt` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/requires.txt` & `paloalto_panorama_sdk-0.0.8/paloalto_panorama_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/setup.py` & `paloalto_panorama_sdk-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/tests/PanoramaAPIMock/panoramaAPIMock.py` & `paloalto_panorama_sdk-0.0.8/tests/PanoramaAPIMock/panoramaAPIMock.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.7/tests/test_service.py` & `paloalto_panorama_sdk-0.0.8/tests/test_service.py`

 * *Files identical despite different names*

