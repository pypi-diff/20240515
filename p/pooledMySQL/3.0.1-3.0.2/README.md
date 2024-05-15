# Comparing `tmp/pooledmysql-3.0.1.tar.gz` & `tmp/pooledmysql-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pooledmysql-3.0.1.tar", last modified: Sun Apr 28 17:04:37 2024, max compression
+gzip compressed data, was "pooledmysql-3.0.2.tar", last modified: Wed May 15 16:10:04 2024, max compression
```

## Comparing `pooledmysql-3.0.1.tar` & `pooledmysql-3.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:04:37.541029 pooledmysql-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-28 17:04:37.541029 pooledmysql-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-28 17:04:33.000000 pooledmysql-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:04:37.541029 pooledmysql-3.0.1/pooledMySQL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-28 17:04:33.000000 pooledmysql-3.0.1/pooledMySQL.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-28 17:04:33.000000 pooledmysql-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:04:37.541029 pooledmysql-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:04.908075 pooledmysql-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-15 16:10:04.908075 pooledmysql-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 16:10:00.000000 pooledmysql-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:04.908075 pooledmysql-3.0.2/pooledMySQL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-15 16:10:04.000000 pooledmysql-3.0.2/pooledMySQL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-15 16:10:04.000000 pooledmysql-3.0.2/pooledMySQL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:10:04.000000 pooledmysql-3.0.2/pooledMySQL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:10:04.000000 pooledmysql-3.0.2/pooledMySQL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 16:10:04.000000 pooledmysql-3.0.2/pooledMySQL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-15 16:10:00.000000 pooledmysql-3.0.2/pooledMySQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-15 16:10:00.000000 pooledmysql-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:10:04.908075 pooledmysql-3.0.2/setup.cfg
```

### Comparing `pooledmysql-3.0.1/PKG-INFO` & `pooledmysql-3.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pooledMySQL
-Version: 3.0.1
+Version: 3.0.2
 Summary: A simple way to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 Author-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/pooledMySQL
 Keywords: mysql,pool,threadedmysql,pooledmysql,multithreaded,thread,database,sql
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: mysql_connector_python
 Requires-Dist: customisedLogs
 
-# pooledMySQL v3.0.1
+# pooledMySQL v3.0.2
 
 ```pip install pooledMySQL --upgrade```
 
 ###### <br>A well maintained program to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 
 
 <br>To install:
```

### Comparing `pooledmysql-3.0.1/README.md` & `pooledmysql-3.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pooledMySQL v3.0.1
+# pooledMySQL v3.0.2
 
 ```pip install pooledMySQL --upgrade```
 
 ###### <br>A well maintained program to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 
 
 <br>To install:
```

### Comparing `pooledmysql-3.0.1/pooledMySQL.egg-info/PKG-INFO` & `pooledmysql-3.0.2/pooledMySQL.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pooledMySQL
-Version: 3.0.1
+Version: 3.0.2
 Summary: A simple way to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 Author-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/pooledMySQL
 Keywords: mysql,pool,threadedmysql,pooledmysql,multithreaded,thread,database,sql
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: mysql_connector_python
 Requires-Dist: customisedLogs
 
-# pooledMySQL v3.0.1
+# pooledMySQL v3.0.2
 
 ```pip install pooledMySQL --upgrade```
 
 ###### <br>A well maintained program to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 
 
 <br>To install:
```

### Comparing `pooledmysql-3.0.1/pooledMySQL.py` & `pooledmysql-3.0.2/pooledMySQL.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 __packagename__ = "pooledmysql"
 
 
 def updatePackage():
     from time import sleep
     from json import loads
     import http.client
@@ -91,15 +91,15 @@
                        PRIMARY KEY (`_id`),
                        UNIQUE INDEX `_id_UNIQUE` (`_id` ASC) VISIBLE)
                        ''', commit_required=True))
         """
         pass
 
 
-    def defaultErrorWriter(self, category:str="", text:str="", extras:str="", ignoreLog:bool=False):
+    def __defaultErrorWriter(self, category:str= "", text:str= "", extras:str= "", ignoreLog:bool=False):
         """
         Default function to write MySQL logs to terminal and logfile
         :param category: Category of the error
         :param text: Main text of the error
         :param extras: Additional text
         :param ignoreLog: Boolean specifying if logging for current execution be ignored from log file
         """
@@ -140,26 +140,26 @@
                     _appendAfterUse = True
                     _connectionFound = True
                 try:
                     data = connObj.execute(syntax)
                 except Exception as e:
                     data = None
                     if not catchErrors:
-                        self.defaultErrorWriter("EXECUTION FAIL", repr(e), syntax, ignoreLog=not logIntoFile)
+                        self.__defaultErrorWriter("EXECUTION FAIL", repr(e), syntax, ignoreLog=not logIntoFile)
                         raise e
                 if _destroyAfterUse:
-                    connObj.safeDeleteConnection()
+                    connObj.__safeDeleteConnection()
                 elif _appendAfterUse:
                     _old = len(self.__connections)
                     self.__connections.append(connObj)
                     _new = len(self.__connections)
                     self.__logger.info("MYSQL-POOL", "NEW", f"Total Connections: {_old}->{_new}")
                 return data
             except Exception as e:
-                self.defaultErrorWriter("CONNECTION FAIL", repr(e))
+                self.__defaultErrorWriter("CONNECTION FAIL", repr(e))
                 if not catchErrors:
                     raise e
                 Imports.sleep(0.5)
 
 
     class __connectionWrapper:
         def __init__(self, connection:Imports.PooledMySQLConnection|Imports.MySQLConnectionAbstract, cleanupCallback, logger:Imports.LogManager):
@@ -188,20 +188,20 @@
                 self.idle = False
                 try:
                     self.raw.ping(True, 1, 1)
                     self.lastUsed = Imports.time()
                     self.logger.skip("PING", f"Success. Waiting {self.maxSendKeepAliveAfter} secs")
                 except Imports.MySQLConnector.InterfaceError:
                     self.logger.skip("PING", f"Failed. Deleting connection")
-                    self.safeDeleteConnection()
+                    self.__safeDeleteConnection()
                 self.idle = True
-            self.safeDeleteConnection()
+            self.__safeDeleteConnection()
 
 
-        def safeDeleteConnection(self):
+        def __safeDeleteConnection(self):
             """
             Safely close and cleanup itself
             :return:
             """
             self.alive = False
             self.cleanupCallback(self)
             self.raw.disconnect()
```

### Comparing `pooledmysql-3.0.1/pyproject.toml` & `pooledmysql-3.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pooledMySQL"
-version = "3.0.1"
+version = "3.0.2"
 description = "A simple way to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually."
 
 readme = "README.md"
 authors = [{ name = "Bhindi", email = "bhaskarpanja93@gmail.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

