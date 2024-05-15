# Comparing `tmp/ocean_spark_connect-0.3.5.tar.gz` & `tmp/ocean_spark_connect-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocean_spark_connect-0.3.5.tar", max compression
+gzip compressed data, was "ocean_spark_connect-0.3.7.tar", max compression
```

## Comparing `ocean_spark_connect-0.3.5.tar` & `ocean_spark_connect-0.3.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      607 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/README.md
--rw-r--r--   0        0        0       25 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/ocean_spark_connect/__init__.py
--rw-r--r--   0        0        0     4986 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/ocean_spark_connect/inverse_websockify.py
--rw-r--r--   0        0        0    11221 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/ocean_spark_connect/ocean_spark_session.py
--rw-r--r--   0        0        0        0 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/ocean_spark_connect/py.typed
--rw-r--r--   0        0        0      538 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 ocean_spark_connect-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1017 2024-05-15 08:03:47.443426 ocean_spark_connect-0.3.7/README.md
+-rw-r--r--   0        0        0       25 2024-05-15 08:03:47.443426 ocean_spark_connect-0.3.7/ocean_spark_connect/__init__.py
+-rw-r--r--   0        0        0     5448 2024-05-15 08:03:47.443426 ocean_spark_connect-0.3.7/ocean_spark_connect/inverse_websockify.py
+-rw-r--r--   0        0        0    11339 2024-05-15 08:03:47.443426 ocean_spark_connect-0.3.7/ocean_spark_connect/ocean_spark_session.py
+-rw-r--r--   0        0        0        0 2024-05-15 08:03:47.443426 ocean_spark_connect-0.3.7/ocean_spark_connect/py.typed
+-rw-r--r--   0        0        0      537 2024-05-15 08:03:47.447426 ocean_spark_connect-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 ocean_spark_connect-0.3.7/PKG-INFO
```

### Comparing `ocean_spark_connect-0.3.5/ocean_spark_connect/inverse_websockify.py` & `ocean_spark_connect-0.3.7/ocean_spark_connect/inverse_websockify.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,28 +40,30 @@
 
   address 127.0.0.1:15002
 """
 
 import sys
 import os
 import asyncio
+import logging
 import websockets
 
 from typing import Any, List
 
 
 class Proxy:
-    def __init__(self, url: str, token: str, port: int = 15002, addr: str = "0.0.0.0"):
-        if port == "-1" and not addr.startswith("/"):
+    def __init__(self, url: str, token: str, port: int = 15002, addr: str = "0.0.0.0", ping_interval: float = -1.0):
+        if port == -1 and not addr.startswith("/"):
             pid = str(os.getpid())
             rnd = os.urandom(4).hex()
             self.addr = f"/tmp/ocean-spark-{pid}-{rnd}.sock"
         else:
             self.addr = addr
 
+        self.ping_interval = ping_interval
         self.port = port
         self.token = token
         self.url = url
         self.done = False
         self.loop = None
 
     def inverse_websockify(self) -> None:
@@ -74,43 +76,54 @@
             data = await reader()
             if data == b"":
                 break
             future = writer(data)
             if future:
                 await future
 
+    async def ping(self, ws: Any) -> None:
+        while not self.done:
+            await asyncio.sleep(self.ping_interval)
+            await ws.ping()
+
     async def handle_client(self, r: Any, w: Any) -> None:
         peer = w.get_extra_info("peername")
         try:
             async with websockets.connect(
                 self.url,
                 subprotocols=None,
                 extra_headers={"Authorization": f"Bearer {self.token}"},
             ) as ws:
-                print(f"{peer} connected to {self.url} on {self.addr}:{self.port}")
+                logging.debug(f"{peer} connected to {self.url} on {self.addr}:{self.port}")
 
                 def r_reader() -> Any:
                     return r.read(65536)
 
                 tcp_to_ws = self.loop.create_task(self.copy(r_reader, ws.send))
                 ws_to_tcp = self.loop.create_task(self.copy(ws.recv, w.write))
+
+                task_list = [tcp_to_ws, ws_to_tcp]
+                if self.ping_interval > 0:
+                    ping_task = self.loop.create_task(self.ping(ws))
+                    task_list.append(ping_task)
+
                 done, pending = await asyncio.wait(
-                    [tcp_to_ws, ws_to_tcp], return_when=asyncio.FIRST_COMPLETED
+                    task_list, return_when=asyncio.FIRST_COMPLETED
                 )
                 for x in done:
                     try:
                         await x
                     except:
                         pass
                 for x in pending:
                     x.cancel()
         except Exception as e:
-            print(f"{peer} exception:", e)
+            logging.error(f"{peer} exception:", e)
         w.close()
-        print(f"{peer} closed")
+        logging.debug(f"{peer} closed")
 
     async def start(self) -> None:
         if self.addr.startswith("/"):
             await asyncio.start_unix_server(self.handle_client, self.addr)
         else:
             await asyncio.start_server(self.handle_client, self.addr, self.port)
```

### Comparing `ocean_spark_connect-0.3.5/ocean_spark_connect/ocean_spark_session.py` & `ocean_spark_connect-0.3.7/ocean_spark_connect/ocean_spark_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,29 +31,24 @@
                     profile_map[profile] = current_profile
                 elif "=" in line:
                     key, value = line.split("=")
                     current_profile[key.strip()] = value.strip()
     return profile_map
 
 
-teststr = """
-python -c "from pyspark.sql.types import DoubleType; from pyspark.sql.functions import rand; spark.range(10000).select(rand().alias('value')).toPandas()"
-"""
-
-
 class OceanChannelBuilder(ChannelBuilder):
     def __init__(self, url: str, bind_address: str):
         super().__init__(url)
         self._bind_address = bind_address
 
     def toChannel(self) -> grpc.Channel:
         if self._bind_address.startswith("/"):
             channel = grpc.insecure_channel("unix://" + self._bind_address)
         else:
-            channel = grpc.insecure_channel(self.url)
+            channel = super().toChannel()
         return channel
 
 
 def _run_gh_process(query: str):
     process = subprocess.Popen(["gh", "copilot", "suggest", "-t", "shell", query + ""], stdout=subprocess.PIPE)
     cmd = "select random()"
     while True:
@@ -169,61 +164,66 @@
 
     class Builder(RemoteSparkSession.Builder):
         _token: str = None
         _profile: str = None
         _appId: str = None
         _accountId = None
         _clusterId = None
+        _ping_interval: float = -1.0
         _jvm = False
         _channel_builder = False
         _scheme = "wss"
         _host = "api.spotinst.io"
-        _port = "-1"
+        _port = -1
         _bind_address = "0.0.0.0"
 
         def __init__(self):
             super().__init__()
 
-        def use_java(self, value):
+        def use_java(self, value: bool):
             self._jvm = value
             return self
 
-        def appid(self, value):
+        def ping_interval(self, value: float):
+            self._ping_interval = value
+            return self
+
+        def appid(self, value: str):
             self._appId = value
             return self
 
-        def token(self, value):
+        def token(self, value: str):
             self._token = value
             return self
 
-        def profile(self, value):
+        def profile(self, value: str):
             self._profile = value
             return self
 
-        def cluster_id(self, value):
+        def cluster_id(self, value: str):
             self._clusterId = value
             return self
 
-        def account_id(self, value):
+        def account_id(self, value: str):
             self._accountId = value
             return self
 
-        def port(self, value):
+        def port(self, value: int):
             self._port = value
             return self
 
-        def bind_address(self, value):
+        def bind_address(self, value: str):
             self._bind_address = value
             return self
 
-        def host(self, value):
+        def host(self, value: str):
             self._host = value
             return self
 
-        def scheme(self, value):
+        def scheme(self, value: str):
             self._scheme = value
             return self
 
         def getOrCreate(self):
             profile_map = load_profiles()
             if self._appId is not None:
                 if self._clusterId is None:
@@ -242,18 +242,21 @@
                         raise Exception("accountId or profile is required")
                     else:
                         if self._profile not in profile_map:
                             raise Exception(f"Profile {self._profile} not found")
                         self._accountId = profile_map[self._profile]["account"]
 
                 if self._jvm:
+                    if self._port == -1:
+                        self._port = 15002
+
                     _jspark = SparkSession.builder.master("local[1]") \
                         .config("spark.jars.repositories",
                                 "https://us-central1-maven.pkg.dev/ocean-spark/ocean-spark-adapters") \
-                        .config("spark.jars.packages", "com.netapp.spark:clientplugin:1.2.1") \
+                        .config("spark.jars.packages", "com.netapp.spark:clientplugin:1.4.1") \
                         .config("spark.jars.excludes", "org.glassfish:javax.el,log4j:log4j") \
                         .config("spark.plugins", "com.netapp.spark.SparkConnectWebsocketTranscodePlugin") \
                         .config("spark.code.submission.clusterId", f"{self._clusterId}") \
                         .config("spark.code.submission.accountId", f"{self._accountId}") \
                         .config("spark.code.submission.appId", f"{self._appId}") \
                         .config("spark.code.submission.token", f"{self._token}") \
                         .config("spark.code.submission.ports", f"{self._port}") \
@@ -261,15 +264,15 @@
                     SparkContext._active_spark_context = None
                     SparkSession._instantiatedSession = None
 
                     channel_builder = OceanChannelBuilder(f"sc://localhost:{self._port}", self._bind_address)
                     return OceanSparkSession(connection=channel_builder, jspark=_jspark, bind_address=self._bind_address, my_process=None)
                 else:
                     url = f"{self._scheme}://{self._host}/ocean/spark/cluster/{self._clusterId}/app/{self._appId}/connect?accountId={self._accountId}"
-                    _proxy = Proxy(url, self._token, self._port, self._bind_address)
+                    _proxy = Proxy(url, self._token, self._port, self._bind_address, self._ping_interval)
                     _process = Process(target=_proxy.inverse_websockify, args=())
                     _process.start()
 
                     channel_builder = OceanChannelBuilder(f"sc://localhost:{_proxy.port}", _proxy.addr)
                     return OceanSparkSession(connection=channel_builder, jspark=None, bind_address=_proxy.addr, my_process=_process)
```

### Comparing `ocean_spark_connect-0.3.5/pyproject.toml` & `ocean_spark_connect-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocean-spark-connect"
-version = "0.3.5"
+version = "0.3.7"
 description = "Spark Connect adapter for Ocean Spark"
 authors = ["Sigmar Stefansson <sigmar@netapp.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyspark = "^3.4.0"
@@ -12,12 +12,12 @@
 pandas = "^2.0.3"
 pyarrow = "*"
 grpcio = "^1.57.0"
 googleapis-common-protos = "^1.60.0"
 grpcio-status = "^1.57.0"
 
 [tool.setuptools.packages.find]
-where = ["ocean_spark_connect"]
+where = ["ocean_sparkconnect"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ocean_spark_connect-0.3.5/PKG-INFO` & `ocean_spark_connect-0.3.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-spark-connect
-Version: 0.3.5
+Version: 0.3.7
 Summary: Spark Connect adapter for Ocean Spark
 Author: Sigmar Stefansson
 Author-email: sigmar@netapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,24 +15,39 @@
 Requires-Dist: grpcio-status (>=1.57.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pyarrow
 Requires-Dist: pyspark (>=3.4.0,<4.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
 
+# ocean-spark-connect
 ## Wrapper to create Spark Connect session for Spark Applications in Ocean
 
 ```
 from ocean_spark_connect.ocean_spark_session import OceanSparkSession
 
 spark = OceanSparkSession.Builder().cluster_id("osc-cluster").appid("appid").profile("default").getOrCreate()
 spark.sql("select random()").show()
 spark.stop()
 ```
 
+To use periodic ping to keep the session alive, use the ping_interval option (in seconds). 
+The default value is off (-1).
+
+```
+spark = OceanSparkSession.Builder() \
+    .ping_interval(5.0) \
+    .cluster_id("osc-cluster") \
+    .appid("appid") \
+    .profile("default") \
+    .getOrCreate()
+```
+
+To use java Spark plugin for the websocket bridge instead, add the use_java(True) option.
+
 ### Options for OceanSparkSession.Builder with and without default values
 
 In addition to the existing SparkSession.Builder option, the following options are available:
 
 * token
 * profile
 * appid
```

