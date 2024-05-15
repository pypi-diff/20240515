# Comparing `tmp/tplinkrouterc6u-4.0.1.tar.gz` & `tmp/tplinkrouterc6u-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tplinkrouterc6u-4.0.1.tar", last modified: Mon Apr 22 18:10:44 2024, max compression
+gzip compressed data, was "tplinkrouterc6u-4.0.2.tar", last modified: Wed May 15 07:22:27 2024, max compression
```

## Comparing `tplinkrouterc6u-4.0.1.tar` & `tplinkrouterc6u-4.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:10:44.535619 tplinkrouterc6u-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-04-22 18:10:44.535619 tplinkrouterc6u-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:10:44.535619 tplinkrouterc6u-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:10:44.531619 tplinkrouterc6u-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30473 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/test/test_client_deco.py
--rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/test/test_client_mr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:10:44.531619 tplinkrouterc6u-4.0.1/tplinkrouterc6u/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48732 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 18:10:40.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:10:44.535619 tplinkrouterc6u-4.0.1/tplinkrouterc6u.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-04-22 18:10:44.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-22 18:10:44.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:10:44.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 18:10:44.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 18:10:44.000000 tplinkrouterc6u-4.0.1/tplinkrouterc6u.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:22:27.229189 tplinkrouterc6u-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30473 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/test/test_client_deco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/test/test_client_mr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/tplinkrouterc6u/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48732 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/top_level.txt
```

### Comparing `tplinkrouterc6u-4.0.1/LICENSE` & `tplinkrouterc6u-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.1/PKG-INFO` & `tplinkrouterc6u-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplinkrouterc6u
-Version: 4.0.1
+Version: 4.0.2
 Summary: TP-Link Router API
 Home-page: https://github.com/AlexandrErohin/TP-Link-Archer-C6U
 Author: Alex Erohin
 Author-email: alexanderErohin@yandex.ru
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tplinkrouterc6u-4.0.1/README.md` & `tplinkrouterc6u-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.1/setup.py` & `tplinkrouterc6u-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tplinkrouterc6u",
-    version="4.0.1",
+    version="4.0.2",
     author="Alex Erohin",
     author_email="alexanderErohin@yandex.ru",
     description="TP-Link Router API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AlexandrErohin/TP-Link-Archer-C6U",
     packages=setuptools.find_packages(),
```

### Comparing `tplinkrouterc6u-4.0.1/test/test_client.py` & `tplinkrouterc6u-4.0.2/test/test_client.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.1/test/test_client_deco.py` & `tplinkrouterc6u-4.0.2/test/test_client_deco.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.1/test/test_client_mr.py` & `tplinkrouterc6u-4.0.2/test/test_client_mr.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.1/tplinkrouterc6u/client.py` & `tplinkrouterc6u-4.0.2/tplinkrouterc6u/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 
 
 class TplinkBaseRouter(AbstractRouter, TplinkRequest):
     _smart_network = True
     _perf_status = True
 
     def __init__(self, host: str, password: str, username: str = 'admin', logger: Logger = None,
-                 verify_ssl: bool = True, timeout: int = 10) -> None:
+                 verify_ssl: bool = True, timeout: int = 30) -> None:
         super().__init__(host, password, username, logger, verify_ssl, timeout)
 
         self._url_firmware = 'admin/firmware?form=upgrade&operation=read'
         self._url_ipv4_reservations = 'admin/dhcps?form=reservation&operation=load'
         self._url_ipv4_dhcp_leases = 'admin/dhcps?form=client&operation=load'
         referer = '{}/webpages/index.html'.format(self.host)
         self._headers_request = {'Referer': referer}
@@ -464,25 +464,25 @@
         elif data.startswith('iot_6'):
             result = Connection.IOT_6G
         return result
 
 
 class TplinkRouter(TplinkEncryption, TplinkBaseRouter):
     def __init__(self, host: str, password: str, username: str = 'admin', logger: Logger = None,
-                 verify_ssl: bool = True, timeout: int = 10) -> None:
+                 verify_ssl: bool = True, timeout: int = 30) -> None:
         super().__init__(host, password, username, logger, verify_ssl, timeout)
 
         self._url_firmware = 'admin/firmware?form=upgrade'
         self._url_ipv4_reservations = 'admin/dhcps?form=reservation'
         self._url_ipv4_dhcp_leases = 'admin/dhcps?form=client'
 
 
 class TPLinkDecoClient(TplinkEncryption, AbstractRouter):
     def __init__(self, host: str, password: str, username: str = 'admin', logger: Logger = None,
-                 verify_ssl: bool = True, timeout: int = 10) -> None:
+                 verify_ssl: bool = True, timeout: int = 30) -> None:
         super().__init__(host, password, username, logger, verify_ssl, timeout)
 
         self._headers_request = {'Content-Type': 'application/json'}
         self._headers_login = {'Content-Type': 'application/json'}
         self._data_block = 'result'
         self.devices = []
 
@@ -747,15 +747,15 @@
             self.type = type
             self.oid = oid
             self.stack = stack
             self.pstack = pstack
             self.attrs = attrs
 
     def __init__(self, host: str, password: str, username: str = 'admin', logger: Logger = None,
-                 verify_ssl: bool = True, timeout: int = 10) -> None:
+                 verify_ssl: bool = True, timeout: int = 30) -> None:
         super().__init__(host, password, username, logger, verify_ssl, timeout)
 
         self.req = requests.Session()
         self._token = None
         self._hash = hashlib.md5((self.username + self.password).encode()).hexdigest()
         self._nn = None
         self._ee = None
@@ -1247,14 +1247,14 @@
         # format expected raw request data
         return signature, encrypted_data
 
 
 class TplinkRouterProvider:
     @staticmethod
     def get_client(host: str, password: str, username: str = 'admin', logger: Logger = None,
-                   verify_ssl: bool = True, timeout: int = 10) -> AbstractRouter | None:
+                   verify_ssl: bool = True, timeout: int = 30) -> AbstractRouter | None:
         for client in [TPLinkMRClient, TplinkC6V4Router, TPLinkDecoClient, TplinkRouter, TplinkC1200Router]:
             router = client(host, password, username, logger, verify_ssl, timeout)
             if router.supports():
                 return router
 
         return None
```

### Comparing `tplinkrouterc6u-4.0.1/tplinkrouterc6u/dataclass.py` & `tplinkrouterc6u-4.0.2/tplinkrouterc6u/dataclass.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.1/tplinkrouterc6u/encryption.py` & `tplinkrouterc6u-4.0.2/tplinkrouterc6u/encryption.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.1/tplinkrouterc6u/enum.py` & `tplinkrouterc6u-4.0.2/tplinkrouterc6u/enum.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.1/tplinkrouterc6u.egg-info/PKG-INFO` & `tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplinkrouterc6u
-Version: 4.0.1
+Version: 4.0.2
 Summary: TP-Link Router API
 Home-page: https://github.com/AlexandrErohin/TP-Link-Archer-C6U
 Author: Alex Erohin
 Author-email: alexanderErohin@yandex.ru
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

