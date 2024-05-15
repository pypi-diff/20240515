# Comparing `tmp/zboxapi-0.0.3.tar.gz` & `tmp/zboxapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zboxapi-0.0.3.tar", max compression
+gzip compressed data, was "zboxapi-0.0.4.tar", max compression
```

## Comparing `zboxapi-0.0.3.tar` & `zboxapi-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      545 2024-05-10 14:13:39.488068 zboxapi-0.0.3/README.md
--rw-r--r--   0        0        0      896 2024-05-10 14:16:38.496339 zboxapi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-10 14:16:38.504339 zboxapi-0.0.3/src/zboxapi/__init__.py
--rw-r--r--   0        0        0     7041 2024-05-08 17:44:28.545019 zboxapi-0.0.3/src/zboxapi/main.py
--rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 zboxapi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      545 2024-05-10 20:21:05.312952 zboxapi-0.0.4/README.md
+-rw-r--r--   0        0        0      896 2024-05-15 13:43:43.221360 zboxapi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-15 13:43:43.229360 zboxapi-0.0.4/src/zboxapi/__init__.py
+-rw-r--r--   0        0        0     7615 2024-05-15 13:33:43.836917 zboxapi-0.0.4/src/zboxapi/main.py
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 zboxapi-0.0.4/PKG-INFO
```

### Comparing `zboxapi-0.0.3/README.md` & `zboxapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zboxapi-0.0.3/pyproject.toml` & `zboxapi-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zboxapi"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Kelby Valenti <kelby.valenti@gmail.com>", "Timo Sugliani <timo.sugliani@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 zboxapi = "zboxapi.main:launch"
```

### Comparing `zboxapi-0.0.3/src/zboxapi/main.py` & `zboxapi-0.0.4/src/zboxapi/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import contextlib
 import fcntl
+import os
 import re
 import socket
 
 # import ssl
 import subprocess
 import time
 from ipaddress import IPv4Address
 from pathlib import Path
 from typing import IO, Annotated
 
 import uvicorn
 from fastapi import APIRouter, Depends, FastAPI, HTTPException, Security, status
+from fastapi.routing import APIRoute
 from fastapi.security.api_key import APIKey, APIKeyHeader
 from pydantic import AfterValidator, BaseModel
 from pydantic_core import PydanticCustomError
 
 api_key_header = APIKeyHeader(name="access_token", auto_error=False)
 
 
@@ -103,14 +105,25 @@
     return (
         not item["ip"].is_loopback,
         socket.inet_aton(str(item["ip"])),
         item["fqdn"],
     )
 
 
+def simplify_operation_ids(api: FastAPI) -> None:
+    """
+    Update operation IDs so that generated API clients have simpler function
+    names.
+    """
+    for route in api.routes:
+        if isinstance(route, APIRoute) and not route.operation_id:
+            tag = route.tags[0] if route.tags else "default"
+            route.operation_id = f"{tag}_{route.name}"
+
+
 def make_list(obj):
     return obj if isinstance(obj, list) else [obj]
 
 
 def ip_fqdn_str(obj, ip_key="ip", fqdn_key="fqdn"):
     return f"ip={getattr(obj, ip_key)}, fqdn={getattr(obj, fqdn_key)}"
 
@@ -159,100 +172,108 @@
         raise PydanticCustomError("value_error", "Invalid fqdn")
     return value
 
 
 FQDN = Annotated[str, AfterValidator(validate_fqdn)]
 
 
-class DnsCreate(BaseModel):
+class HostsCreate(BaseModel):
     ip: IPv4Address
     fqdn: FQDN
 
 
-class DnsDelete(BaseModel):
+class HostsDelete(BaseModel):
     ip: IPv4Address
     fqdn: FQDN
 
 
-class DnsUpdate(BaseModel):
+class HostsUpdate(BaseModel):
     ip: IPv4Address
     fqdn: FQDN
     new_ip: IPv4Address
     new_fqdn: FQDN
 
 
-class DnsView(BaseModel):
+class HostsView(BaseModel):
     ip: IPv4Address
     fqdn: str
 
 
 hosts_router = APIRouter(prefix="/hosts", tags=["hosts"])
 
 
 @hosts_router.get("")
 def get_hosts(
     ip: IPv4Address | None = None,
     fqdn: str | None = None,
-) -> list[DnsView]:
+) -> list[HostsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
         hosts_lines = filter_hosts_file(hosts_lines, ip, fqdn)
     return hosts_lines
 
 
 @hosts_router.post("")
-def add_hosts(lines_in: list[DnsCreate] | DnsCreate) -> list[DnsView]:
+def add_hosts(lines_in: list[HostsCreate] | HostsCreate) -> list[HostsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
         for line in make_list(lines_in):
             if filter_hosts_file(hosts_lines, line.ip, line.fqdn):
                 raise RecordAlreadyPresent(line)
             hosts_lines.append(ip_fqdn_dict(line))
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
 @hosts_router.put("")
-def update_hosts(lines_in: list[DnsUpdate] | DnsUpdate) -> list[DnsView]:
+def update_hosts(lines_in: list[HostsUpdate] | HostsUpdate) -> list[HostsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
         for line in make_list(lines_in):
             key = ip_fqdn_dict(line)
             if key not in hosts_lines:
                 raise RecordNotFound(line)
             ix = hosts_lines.index(key)
             hosts_lines[ix] = ip_fqdn_dict(line, "new_ip", "new_fqdn")
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
 @hosts_router.delete("")
-def delete_hosts(lines_in: list[DnsDelete] | DnsDelete) -> list[DnsView]:
+def delete_hosts(lines_in: list[HostsDelete] | HostsDelete) -> list[HostsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
         for line in make_list(lines_in):
             key = ip_fqdn_dict(line)
             if key not in hosts_lines:
                 raise RecordNotFound(line)
             hosts_lines.remove(key)
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
-app = FastAPI(title="zPod zBox API", dependencies=[Depends(validate_api_key)])
+zboxapi_root_path = os.getenv("ZBOXAPI_ROOT_PATH", None)
+
+app = FastAPI(
+    title="zBox API",
+    root_path=zboxapi_root_path,
+    dependencies=[Depends(validate_api_key)],
+)
 app.include_router(hosts_router)
+simplify_operation_ids(app)
+
 ZPOD_PASSWORD = get_zpod_password()
 
 
 def launch():
     uvicorn.run(
         app,
-        host="zbox",
+        host="127.0.0.1",
         port=8000,
     )
 
 
 if __name__ == "__main__":
     launch()
```

### Comparing `zboxapi-0.0.3/PKG-INFO` & `zboxapi-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zboxapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: Kelby Valenti
 Author-email: kelby.valenti@gmail.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

