# Comparing `tmp/avassa_client-2024.4.1.tar.gz` & `tmp/avassa_client-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avassa_client-2024.4.1.tar", last modified: Mon Apr 15 12:23:06 2024, max compression
+gzip compressed data, was "avassa_client-2024.5.0.tar", last modified: Wed May 15 17:11:11 2024, max compression
```

## Comparing `avassa_client-2024.4.1.tar` & `avassa_client-2024.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-15 12:23:06.048917 avassa_client-2024.4.1/
--rw-r--r--   0 frja       (501) staff       (20)    11343 2023-04-25 10:38:10.000000 avassa_client-2024.4.1/LICENSE
--rw-r--r--   0 frja       (501) staff       (20)    14236 2024-04-15 12:23:06.048590 avassa_client-2024.4.1/PKG-INFO
--rw-r--r--   0 frja       (501) staff       (20)      758 2024-01-15 13:20:32.000000 avassa_client-2024.4.1/README.md
-drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-15 12:23:06.046927 avassa_client-2024.4.1/avassa_client/
--rw-r--r--   0 frja       (501) staff       (20)    10471 2024-04-15 12:20:50.000000 avassa_client-2024.4.1/avassa_client/__init__.py
--rw-r--r--   0 frja       (501) staff       (20)    17620 2024-01-15 13:06:43.000000 avassa_client-2024.4.1/avassa_client/volga.py
-drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-15 12:23:06.048310 avassa_client-2024.4.1/avassa_client.egg-info/
--rw-r--r--   0 frja       (501) staff       (20)    14236 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/PKG-INFO
--rw-r--r--   0 frja       (501) staff       (20)      265 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/SOURCES.txt
--rw-r--r--   0 frja       (501) staff       (20)        1 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/dependency_links.txt
--rw-r--r--   0 frja       (501) staff       (20)       15 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/requires.txt
--rw-r--r--   0 frja       (501) staff       (20)       14 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/top_level.txt
--rw-r--r--   0 frja       (501) staff       (20)      654 2024-04-15 12:22:36.000000 avassa_client-2024.4.1/pyproject.toml
--rw-r--r--   0 frja       (501) staff       (20)       38 2024-04-15 12:23:06.048967 avassa_client-2024.4.1/setup.cfg
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-05-15 17:11:11.101291 avassa_client-2024.5.0/
+-rw-r--r--   0 frja       (501) staff       (20)    11343 2023-04-25 10:38:10.000000 avassa_client-2024.5.0/LICENSE
+-rw-r--r--   0 frja       (501) staff       (20)    14236 2024-05-15 17:11:11.101062 avassa_client-2024.5.0/PKG-INFO
+-rw-r--r--   0 frja       (501) staff       (20)      758 2024-01-15 13:20:32.000000 avassa_client-2024.5.0/README.md
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-05-15 17:11:11.099693 avassa_client-2024.5.0/avassa_client/
+-rw-r--r--   0 frja       (501) staff       (20)    10673 2024-05-15 17:10:45.000000 avassa_client-2024.5.0/avassa_client/__init__.py
+-rw-r--r--   0 frja       (501) staff       (20)    17620 2024-01-15 13:06:43.000000 avassa_client-2024.5.0/avassa_client/volga.py
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-05-15 17:11:11.100823 avassa_client-2024.5.0/avassa_client.egg-info/
+-rw-r--r--   0 frja       (501) staff       (20)    14236 2024-05-15 17:11:11.000000 avassa_client-2024.5.0/avassa_client.egg-info/PKG-INFO
+-rw-r--r--   0 frja       (501) staff       (20)      265 2024-05-15 17:11:11.000000 avassa_client-2024.5.0/avassa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 frja       (501) staff       (20)        1 2024-05-15 17:11:11.000000 avassa_client-2024.5.0/avassa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 frja       (501) staff       (20)       15 2024-05-15 17:11:11.000000 avassa_client-2024.5.0/avassa_client.egg-info/requires.txt
+-rw-r--r--   0 frja       (501) staff       (20)       14 2024-05-15 17:11:11.000000 avassa_client-2024.5.0/avassa_client.egg-info/top_level.txt
+-rw-r--r--   0 frja       (501) staff       (20)      654 2024-05-15 17:10:59.000000 avassa_client-2024.5.0/pyproject.toml
+-rw-r--r--   0 frja       (501) staff       (20)       38 2024-05-15 17:11:11.101329 avassa_client-2024.5.0/setup.cfg
```

### Comparing `avassa_client-2024.4.1/LICENSE` & `avassa_client-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avassa_client-2024.4.1/PKG-INFO` & `avassa_client-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avassa-client
-Version: 2024.4.1
+Version: 2024.5.0
 Summary: Library for integrating with the Avassa APIs
 Author-email: Avassa <info@avassa.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `avassa_client-2024.4.1/README.md` & `avassa_client-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `avassa_client-2024.4.1/avassa_client/__init__.py` & `avassa_client-2024.5.0/avassa_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         self.check_hostname = True
 
     def wrap_socket(self, *args, **kwargs):
         if self._server_hostname is not None:
             kwargs['server_hostname'] = self._server_hostname
         return super().wrap_socket(*args, **kwargs)
 
+    def get_server_hostname(self):
+        return self._server_hostname
+
 
 class Session(object):
     def __init__(self, host: str,
                  token: str,
                  ssl_context: Optional[ssl.SSLContext] = None,
                  user_agent: Optional[str] = None,
                  server_hostname: Optional[str] = None) -> None:
@@ -62,14 +65,16 @@
         self._volga_ws_url = f"wss://{self._base_url.netloc}/v1/ws/volga"
         self._token = token
         if ssl_context:
             if server_hostname is not None:
                 raise ValueError("server_hostname is not applicable when"
                                  " using custom ssl_context")
             self._ssl_context = ssl_context
+            if isinstance(ssl_context, ApiSSLContext):
+                self._server_hostname = ssl_context.get_server_hostname()
         else:
             self._ssl_context = create_ssl_context(server_hostname)
         self._user_agent = user_agent
 
     def auth_header(self) -> Dict[str, str]:
         header = {"Authorization": "Bearer {}".format(self._token)}
         if self._user_agent:
```

### Comparing `avassa_client-2024.4.1/avassa_client/volga.py` & `avassa_client-2024.5.0/avassa_client/volga.py`

 * *Files identical despite different names*

### Comparing `avassa_client-2024.4.1/avassa_client.egg-info/PKG-INFO` & `avassa_client-2024.5.0/avassa_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avassa-client
-Version: 2024.4.1
+Version: 2024.5.0
 Summary: Library for integrating with the Avassa APIs
 Author-email: Avassa <info@avassa.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `avassa_client-2024.4.1/pyproject.toml` & `avassa_client-2024.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avassa-client"
-version = "2024.4.1"
+version = "2024.5.0"
 description = "Library for integrating with the Avassa APIs"
 readme = "README.md"
 authors = [{ name = "Avassa", email = "info@avassa.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

