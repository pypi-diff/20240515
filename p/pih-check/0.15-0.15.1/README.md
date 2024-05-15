# Comparing `tmp/pih-check-0.15.tar.gz` & `tmp/pih-check-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-check-0.15.tar", last modified: Wed Apr 10 01:37:32 2024, max compression
+gzip compressed data, was "pih-check-0.15.1.tar", last modified: Wed May 15 13:25:42 2024, max compression
```

## Comparing `pih-check-0.15.tar` & `pih-check-0.15.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:37:32.406320 pih-check-0.15/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:37:31.921939 pih-check-0.15/CheckerService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-check-0.15/CheckerService/__init__.py
--rw-rw-rw-   0        0        0      149 2024-02-12 04:26:31.000000 pih-check-0.15/CheckerService/__main__.py
--rw-rw-rw-   0        0        0    19805 2024-04-09 23:55:43.000000 pih-check-0.15/CheckerService/api.py
--rw-rw-rw-   0        0        0     1390 2024-04-10 01:35:32.000000 pih-check-0.15/CheckerService/const.py
--rw-rw-rw-   0        0        0     6723 2024-03-27 00:18:20.000000 pih-check-0.15/CheckerService/service.py
--rw-rw-rw-   0        0        0      269 2024-04-10 01:37:32.375084 pih-check-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:37:32.296946 pih-check-0.15/pih_check.egg-info/
--rw-rw-rw-   0        0        0      269 2024-04-10 01:37:31.000000 pih-check-0.15/pih_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-04-10 01:37:31.000000 pih-check-0.15/pih_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:37:31.000000 pih-check-0.15/pih_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-10 01:37:31.000000 pih-check-0.15/pih_check.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 01:37:31.000000 pih-check-0.15/pih_check.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 01:37:31.000000 pih-check-0.15/pih_check.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:37:32.406320 pih-check-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 13:25:42.985128 pih-check-0.15.1/
+drwxrwxrwx   0        0        0        0 2024-05-15 13:25:42.545251 pih-check-0.15.1/CheckerService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-check-0.15.1/CheckerService/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-02-12 04:26:31.000000 pih-check-0.15.1/CheckerService/__main__.py
+-rw-rw-rw-   0        0        0    19805 2024-04-09 23:55:43.000000 pih-check-0.15.1/CheckerService/api.py
+-rw-rw-rw-   0        0        0     1395 2024-05-15 12:41:24.000000 pih-check-0.15.1/CheckerService/const.py
+-rw-rw-rw-   0        0        0     6723 2024-03-27 00:18:20.000000 pih-check-0.15.1/CheckerService/service.py
+-rw-rw-rw-   0        0        0      271 2024-05-15 13:25:42.938016 pih-check-0.15.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 13:25:42.890035 pih-check-0.15.1/pih_check.egg-info/
+-rw-rw-rw-   0        0        0      271 2024-05-15 13:25:41.000000 pih-check-0.15.1/pih_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-15 13:25:42.000000 pih-check-0.15.1/pih_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 13:25:42.000000 pih-check-0.15.1/pih_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-15 13:25:42.000000 pih-check-0.15.1/pih_check.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 13:25:42.000000 pih-check-0.15.1/pih_check.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 13:25:42.000000 pih-check-0.15.1/pih_check.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 13:25:43.000534 pih-check-0.15.1/setup.cfg
```

### Comparing `pih-check-0.15/CheckerService/api.py` & `pih-check-0.15.1/CheckerService/api.py`

 * *Files identical despite different names*

### Comparing `pih-check-0.15/CheckerService/const.py` & `pih-check-0.15.1/CheckerService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pih.collections.service import ServiceDescription
 from pih.collections import ResourceStatus, ComputerDescription, SiteResourceStatus
 
 NAME: str = "Checker"
 
 HOST = Hosts.BACKUP_WORKER.NAME
 
-VERSION: str = "0.15"
+VERSION: str = "0.15.1"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Checker service",
     host=HOST,
     commands=("get_resource_status_list",),
     standalone_name="check",
@@ -28,17 +28,17 @@
         ResourceStatus(), A.CT_R_D.INTERNET
     )
 
     VPN_PACS_SPB: ResourceStatus = A.D.fill_data_from_source(
         ResourceStatus(), A.CT_R_D.VPN_PACS_SPB
     )
 
-    PACS_SPB: ResourceStatus = A.D.fill_data_from_source(
-        ResourceStatus(), A.CT_R_D.PACS_SPB
-    )
+    #PACS_SPB: ResourceStatus = A.D.fill_data_from_source(
+    #    ResourceStatus(), A.CT_R_D.PACS_SPB
+    #)
 
     SITE: list[SiteResourceStatus] = []
 
     WAPPI: list[ResourceStatus] = []
 
     WS: list[ResourceStatus] = []
```

### Comparing `pih-check-0.15/CheckerService/service.py` & `pih-check-0.15.1/CheckerService/service.py`

 * *Files identical despite different names*

