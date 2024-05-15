# Comparing `tmp/pih-ad-0.15.tar.gz` & `tmp/pih-ad-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ad-0.15.tar", last modified: Wed Apr 10 04:39:41 2024, max compression
+gzip compressed data, was "pih-ad-0.16.tar", last modified: Wed May 15 03:47:20 2024, max compression
```

## Comparing `pih-ad-0.15.tar` & `pih-ad-0.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 04:39:41.409116 pih-ad-0.15/
-drwxrwxrwx   0        0        0        0 2024-04-10 04:39:41.031712 pih-ad-0.15/ActiveDirectoryService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-ad-0.15/ActiveDirectoryService/__init__.py
--rw-rw-rw-   0        0        0      157 2024-02-10 00:14:06.000000 pih-ad-0.15/ActiveDirectoryService/__main__.py
--rw-rw-rw-   0        0        0    18020 2024-04-10 04:37:37.000000 pih-ad-0.15/ActiveDirectoryService/api.py
--rw-rw-rw-   0        0        0     1601 2024-04-10 04:38:49.000000 pih-ad-0.15/ActiveDirectoryService/const.py
--rw-rw-rw-   0        0        0    15355 2024-03-11 05:44:07.000000 pih-ad-0.15/ActiveDirectoryService/service.py
--rw-rw-rw-   0        0        0      340 2024-04-10 04:39:41.362239 pih-ad-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 04:39:41.330990 pih-ad-0.15/pih_ad.egg-info/
--rw-rw-rw-   0        0        0      340 2024-04-10 04:39:40.000000 pih-ad-0.15/pih_ad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-10 04:39:40.000000 pih-ad-0.15/pih_ad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 04:39:40.000000 pih-ad-0.15/pih_ad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-10 04:39:40.000000 pih-ad-0.15/pih_ad.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-10 04:39:40.000000 pih-ad-0.15/pih_ad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-10 04:39:40.000000 pih-ad-0.15/pih_ad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 04:39:41.409116 pih-ad-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 03:47:20.258792 pih-ad-0.16/
+drwxrwxrwx   0        0        0        0 2024-05-15 03:47:19.668133 pih-ad-0.16/ActiveDirectoryService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-ad-0.16/ActiveDirectoryService/__init__.py
+-rw-rw-rw-   0        0        0      157 2024-02-10 00:14:06.000000 pih-ad-0.16/ActiveDirectoryService/__main__.py
+-rw-rw-rw-   0        0        0    18100 2024-05-14 14:30:34.000000 pih-ad-0.16/ActiveDirectoryService/api.py
+-rw-rw-rw-   0        0        0     1580 2024-05-15 03:46:44.000000 pih-ad-0.16/ActiveDirectoryService/const.py
+-rw-rw-rw-   0        0        0    15730 2024-05-15 03:46:05.000000 pih-ad-0.16/ActiveDirectoryService/service.py
+-rw-rw-rw-   0        0        0      340 2024-05-15 03:47:20.217172 pih-ad-0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 03:47:20.154637 pih-ad-0.16/pih_ad.egg-info/
+-rw-rw-rw-   0        0        0      340 2024-05-15 03:47:18.000000 pih-ad-0.16/pih_ad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-15 03:47:19.000000 pih-ad-0.16/pih_ad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 03:47:18.000000 pih-ad-0.16/pih_ad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-15 03:47:18.000000 pih-ad-0.16/pih_ad.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-05-15 03:47:18.000000 pih-ad-0.16/pih_ad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-15 03:47:18.000000 pih-ad-0.16/pih_ad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 03:47:20.280805 pih-ad-0.16/setup.cfg
```

### Comparing `pih-ad-0.15/ActiveDirectoryService/api.py` & `pih-ad-0.16/ActiveDirectoryService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import ipih
 
 from pih import A
 from pih.consts.errors import NotAccesable
 from pih.collections import FullName, User
 from ActiveDirectoryService.const import *
-from pih.tools import if_else, j, n, nn, lw, ne
+from pih.tools import if_else, j, n, nn, lw, ne, escs
 
 
 class ActiveDirectoryApi:
     DEFAULT_AD_QUERY: ADQuery = ADQuery()
 
     @staticmethod
     def get_printer_list(driver_name: str | None = None) -> list[dict[str, str]]:
@@ -59,25 +59,27 @@
         )
 
     @staticmethod
     def get_shared_printer_list() -> list[dict[str, str]]:
         ad_query: ADQuery = ADQuery()
         ad_query.execute_query(
             attributes=A.CT_FC.PRINTER.ITEM.get_name_list(),
-            where_clause=(f"objectCategory = 'printqueue'"),
+            where_clause=j(("objectCategory = ", escs("printqueue"))),
         )
         query_result = [] if ad_query.get_row_count() == 0 else ad_query.get_results()
         result: list[dict[str, str]] = []
         for item in query_result:
             result.append(item)
         return result
 
     @staticmethod
     def get_computer_description_list(dn: str) -> list[dict[str, Any]]:
-        property_container: ADContainer = ADContainer.from_dn(A.CT_AD.PROPERTY_COMPUTER_DN)
+        property_container: ADContainer = ADContainer.from_dn(
+            A.CT_AD.PROPERTY_COMPUTER_DN
+        )
         property_list: list[ADGroup] = property_container.get_children(False)
         computer_property_map: dict[str, int] = defaultdict(int)
         property_item: ADGroup
         for property_item in property_list:
             property_member_list: list[ADComputer] = ADGroup.from_dn(
                 property_item.dn
             ).get_members()
@@ -217,18 +219,18 @@
         search_attribute: str,
         search_value: str,
         fields: list[str],
         base_dn: str = A.CT_AD.ACTIVE_USERS_CONTAINER_DN,
         ad_query=DEFAULT_AD_QUERY,
     ) -> dict[str, Any] | None:
         if search_attribute.find("name") != -1:
-            if search_value != "*":
-                search_value = f"*{search_value}*"
+            if search_value != ANY_SYMBOL:
+                search_value = j((ANY_SYMBOL, search_value, ANY_SYMBOL))
         if search_value == "":
-            search_value = "*"
+            search_value = ANY_SYMBOL
         ad_query.execute_query(
             attributes=fields,
             base_dn=base_dn,
             where_clause=f"objectClass = 'user' and objectCategory = 'person' and {search_attribute} = '{search_value}'",
         )
         if ad_query.get_row_count() == 0:
             return None
@@ -441,14 +443,15 @@
         @staticmethod
         def user_remove(user_dn: str) -> bool:
             try:
                 ADUser.from_dn(user_dn).delete()
                 return True
             except:
                 return False
+
         @staticmethod
         def user_set_telephone_number(user_dn: str, telephone: str) -> bool:
             ActiveDirectoryApi.user_set_telephone_number(user_dn, telephone)
             return True
 
         @staticmethod
         def user_set_password(user_dn: str, password: str) -> bool:
@@ -459,8 +462,8 @@
         def user_move(user_dn: str, container_dn: str) -> bool:
             ActiveDirectoryApi.user_move(user_dn, container_dn)
             return True
 
         @staticmethod
         def user_set_status(user_dn: str, status: str, container_dn: str) -> bool:
             ActiveDirectoryApi.user_set_dn(user_dn, status, container_dn)
-            return True
+            return True
```

### Comparing `pih-ad-0.15/ActiveDirectoryService/const.py` & `pih-ad-0.16/ActiveDirectoryService/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "ActiveDirectory"
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.15"
+VERSION: str = "0.16"
 
 PACKAGES: tuple[str, ...] = ("pyad", "pywin32", "wmi")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Active directory service",
     host=HOST.NAME,
@@ -46,15 +46,15 @@
         "get_user_list_by_property",
     ),
     version=VERSION,
     standalone_name="ad",
     use_standalone=True,
 )
 
-ANY_SYMBOL: str = "*"
+
 
 
 class UserExistanceStatus(Enum):
     EXISTS = 1
     INACTIVE = -1
     NOT_EXISTS = 0
```

### Comparing `pih-ad-0.15/ActiveDirectoryService/service.py` & `pih-ad-0.16/ActiveDirectoryService/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import ipih
 
-from pih import A, PIHThreadPoolExecutor, thread
+from pih import A, PIHThreadPoolExecutor, thread, strdict
 from ActiveDirectoryService.const import SD
 
 
-ISOLATED = False
-
-SC = A.CT_SC
-
 from typing import Any
 from pih.collections import FullName, Result
-from pih.tools import ParameterList, e, n, ne, while_excepted, one
+from pih.tools import ParameterList, e, n, ne, while_excepted, one, lw
+
+
+ISOLATED = True
+
+SC = A.CT_SC
 
 
 class DH:
     computer_cache: dict[str, dict[str, Any]] = {}
     computer_description_list: list[dict[str, Any]] = []
     computer_lock: bool = False
     user_cache: dict[str, dict[str, Any]] = {}
     user_lock: bool = False
 
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
-       
+
         from pih.consts.errors import NotAccesable
         from ActiveDirectoryService.api import ActiveDirectoryApi as Api
-        
+
         from concurrent.futures import as_completed
         import pythoncom
-        
+
         def service_call_handler(sc: SC, pl: ParameterList) -> Any:
             with A.ER.detect(pythoncom.CoUninitialize):
                 pythoncom.CoInitialize()
                 if sc == SC.heart_beat:
-                    if (
-                        A.SE.life_time.seconds % A.CT.CACHE.TTL.WORKSTATIONS
-                    ) == 0:
+                    if (A.SE.life_time.seconds % A.CT.CACHE.TTL.WORKSTATIONS) == 0:
                         update_computer_cache()
                         return
                     if (A.SE.life_time.seconds % A.CT.CACHE.TTL.USERS) == 0:
                         update_users_cache()
                         return
                 if sc == SC.drop_user_cache:
                     update_users_cache()
@@ -54,28 +53,39 @@
                 if sc == SC.get_user_by_full_name:
                     return get_user_by_attribute(
                         A.CT_FNC.SEARCH_ATTRIBUTE_NAME,
                         A.D.fullname_to_string(pl.next(FullName())),
                         pl.next(),
                     )
                 if sc == SC.get_users_by_name:
-                    value: str = pl.next()
-                    value = value.lower()
+                    value: str | None = pl.next()
+                    value = lw(value)
                     active: bool | None = pl.next()
                     cached: bool | None = pl.next()
+                    strict_comparison: bool | None = pl.next()
                     cached = A.D.check_not_none(cached, cached, A.S_U.use_cache())
                     if cached:
+                        user_cache_list: list[strdict] = A.D.as_list(DH.user_cache)
+
+                        def filter_function(item: strdict | Any) -> bool:
+                            if isinstance(item, dict):
+                                name: str = item[A.CT_FNC.SEARCH_ATTRIBUTE_NAME]
+                                return (
+                                    A.D.contains(name, value)
+                                    if strict_comparison
+                                    else A.D.full_right_intersection_by_tokens(name, value)
+                                )
+                            return False
+
                         return create_user_result(
-                            A.D.filter(
-                                lambda item: isinstance(item, dict)
-                                and item[A.CT_FNC.SEARCH_ATTRIBUTE_NAME]
-                                .lower()
-                                .find(value)
-                                != -1,
-                                A.D.as_list(DH.user_cache),
+                            user_cache_list
+                            if e(value)
+                            else A.D.filter(
+                                filter_function,
+                                user_cache_list,
                             )
                         )
                     return get_user_by_attribute(
                         A.CT_FNC.SEARCH_ATTRIBUTE_NAME, value, active
                     )
                 if sc == SC.get_user_by_login:
                     value: str = pl.next()
@@ -198,61 +208,56 @@
         def get_computer_list_by_container_dn(value: str | None = None) -> dict:
             computer_cache: dict[str, dict[str, Any]] = DH.computer_cache
             if e(computer_cache):
                 update_computer_cache()
             return A.D.filter(
                 lambda item: True if n(value) else item[A.CT_FNC.DN] == value,
                 [computer_cache[computer_name] for computer_name in computer_cache],
-            ) # type: ignore
+            )  # type: ignore
 
         def get_computer_discription_list_by_container_dn(
             value: str | None = None,
         ) -> dict[str, dict[str, Any]]:
             computer_description_list: list[dict[str, Any]] = (
                 DH.computer_description_list
             )
             if e(computer_description_list):
                 update_computer_cache()
             return A.D.filter(
                 lambda item: True if n(value) else item[A.CT_FNC.DN] == value,
                 computer_description_list,
-            ) # type: ignore
+            )  # type: ignore
 
         def create_user_result(data: Any) -> Result:
             return Result(A.CT_FC.AD.USER, data)
 
         def update_computer_cache() -> None:
             if not DH.computer_lock:
                 DH.computer_lock = True
                 with A.ER.detect():
-                    DH.computer_description_list = (
-                        Api.get_computer_description_list(
-                            A.CT_AD.WORKSTATIONS_CONTAINER_DN
-                        )
-                        + Api.get_computer_description_list(
-                            A.CT_AD.SERVERS_CONTAINER_DN
-                        )
-                    )
+                    DH.computer_description_list = Api.get_computer_description_list(
+                        A.CT_AD.WORKSTATIONS_CONTAINER_DN
+                    ) + Api.get_computer_description_list(A.CT_AD.SERVERS_CONTAINER_DN)
                     computer_cache: dict[str, dict[str, Any]] = {}
                     with PIHThreadPoolExecutor(
                         max_workers=len(DH.computer_description_list)
                     ) as executor:
 
                         future_to_computer = {
                             executor.submit(
                                 Api.get_user_login_by_workstation_name_via_query,
                                 value=computer_description_item[A.CT_FNC.NAME],
                                 active=True,
                             ): computer_description_item
                             for computer_description_item in DH.computer_description_list
                         }
-                        for future_computer in as_completed(future_to_computer): # type: ignore
+                        for future_computer in as_completed(future_to_computer):  # type: ignore
                             computer: dict[str, Any] = future_to_computer[
                                 future_computer
-                            ] # type: ignore
+                            ]  # type: ignore
                             computer_name: str = computer[A.CT_FNC.NAME].lower()
                             computer_cache[computer_name] = computer
                             exception: BaseException | None = (
                                 future_computer.exception()
                             )
                             if e(exception):
                                 computer[A.CT_FNC.ACCESSABLE] = True
@@ -261,15 +266,15 @@
                                 if ne(login_list):
                                     computer[A.CT_FNC.LOGIN] = login_list[0]
                             else:
                                 if isinstance(exception, NotAccesable):
                                     computer[A.CT_FNC.ACCESSABLE] = False
                                     computer[A.CT_FNC.ACTIVE_USERS_LOGIN] = None
                                 else:
-                                    raise exception # type: ignore
+                                    raise exception  # type: ignore
                 DH.computer_cache = computer_cache
                 DH.computer_lock = False
 
         def get_user_by_attribute(
             attribute: str,
             value: str,
             active: bool | None = None,
@@ -295,27 +300,27 @@
                     while True:
                         with A.ER.detect():
                             result: list[dict[str, Any]] = get_user_by_attribute(
                                 A.CT_FNC.SEARCH_ATTRIBUTE_LOGIN,
                                 value or A.CT_AD.SEARCH_ALL_PATTERN,
                                 active,
                                 False,
-                            ) # type: ignore
+                            )  # type: ignore
 
                             def every_action(user_data: dict[str, Any]) -> None:
                                 LDH.user_cache |= {
                                     user_data[A.CT_UP.LOGIN].lower(): user_data
                                 }
 
-                            A.D.every(every_action, result) # type: ignore
+                            A.D.every(every_action, result)  # type: ignore
                             break
                     if n(value):
                         DH.user_cache = LDH.user_cache
                     else:
-                        DH.user_cache[value] = (lambda item: item, one)[ # type: ignore
+                        DH.user_cache[value] = (lambda item: item, one)[  # type: ignore
                             len(LDH.user_cache) == 1
                         ](A.D.as_list(LDH.user_cache))
                 DH.user_lock = False
 
         def update_users_cache() -> None:
             fetch_user_by_login(None)
 
@@ -326,20 +331,20 @@
 
             def start_action() -> None:
                 pythoncom.CoInitialize()
                 update_users_cache()
                 update_computer_cache()
                 pythoncom.CoUninitialize()
 
-            thread(start_action) # type: ignore
+            thread(start_action)  # type: ignore
 
         A.SRV_A.serve(
             SD,
             service_call_handler,
-            service_starts_handler, # type: ignore
+            service_starts_handler,  # type: ignore
             isolate=ISOLATED,
             as_standalone=as_standalone,
         )
 
 
 if __name__ == "__main__":
     start()
```

