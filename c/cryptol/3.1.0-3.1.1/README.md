# Comparing `tmp/cryptol-3.1.0.tar.gz` & `tmp/cryptol-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptol-3.1.0.tar", max compression
+gzip compressed data, was "cryptol-3.1.1.tar", max compression
```

## Comparing `cryptol-3.1.0.tar` & `cryptol-3.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2024-01-31 18:59:53.874057 cryptol-3.1.0/LICENSE
--rw-r--r--   0        0        0     6969 2024-01-31 18:59:53.874057 cryptol-3.1.0/README.md
--rw-r--r--   0        0        0     1242 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/__init__.py
--rw-r--r--   0        0        0    21322 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/bitvector.py
--rw-r--r--   0        0        0    12827 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/commands.py
--rw-r--r--   0        0        0    27251 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/connection.py
--rw-r--r--   0        0        0    18605 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/cryptoltypes.py
--rw-r--r--   0        0        0     4476 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/custom_fstring.py
--rw-r--r--   0        0        0      355 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/file_deps.py
--rw-r--r--   0        0        0      561 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/opaque.py
--rw-r--r--   0        0        0        0 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/py.typed
--rw-r--r--   0        0        0     4115 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/quoting.py
--rw-r--r--   0        0        0    12886 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/single_connection.py
--rw-r--r--   0        0        0     3178 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/solver.py
--rw-r--r--   0        0        0    21146 2024-01-31 18:59:53.874057 cryptol-3.1.0/cryptol/synchronous.py
--rw-r--r--   0        0        0      228 2024-01-31 18:59:53.874057 cryptol-3.1.0/mypy.ini
--rw-r--r--   0        0        0      579 2024-02-05 19:49:23.215660 cryptol-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     7728 1970-01-01 00:00:00.000000 cryptol-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-15 21:56:19.663926 cryptol-3.1.1/LICENSE
+-rw-r--r--   0        0        0     7169 2024-05-15 20:12:21.031449 cryptol-3.1.1/README.md
+-rw-r--r--   0        0        0     1223 2024-05-15 20:12:21.031691 cryptol-3.1.1/cryptol/__init__.py
+-rw-r--r--   0        0        0    21322 2024-02-12 21:22:56.844300 cryptol-3.1.1/cryptol/bitvector.py
+-rw-r--r--   0        0        0    12827 2024-04-09 15:08:48.255190 cryptol-3.1.1/cryptol/commands.py
+-rw-r--r--   0        0        0    27212 2024-05-15 20:12:21.032106 cryptol-3.1.1/cryptol/connection.py
+-rw-r--r--   0        0        0    18605 2024-02-05 18:28:12.159796 cryptol-3.1.1/cryptol/cryptoltypes.py
+-rw-r--r--   0        0        0     4476 2024-02-05 18:28:12.159896 cryptol-3.1.1/cryptol/custom_fstring.py
+-rw-r--r--   0        0        0      355 2024-04-08 17:47:20.949833 cryptol-3.1.1/cryptol/file_deps.py
+-rw-r--r--   0        0        0      561 2024-02-05 18:28:12.160005 cryptol-3.1.1/cryptol/opaque.py
+-rw-r--r--   0        0        0        0 2024-02-05 18:28:12.160026 cryptol-3.1.1/cryptol/py.typed
+-rw-r--r--   0        0        0     4115 2024-02-12 21:22:56.844915 cryptol-3.1.1/cryptol/quoting.py
+-rw-r--r--   0        0        0    12886 2024-02-12 21:22:56.845136 cryptol-3.1.1/cryptol/single_connection.py
+-rw-r--r--   0        0        0     3178 2024-02-05 18:28:12.160269 cryptol-3.1.1/cryptol/solver.py
+-rw-r--r--   0        0        0    21146 2024-02-12 21:22:56.845283 cryptol-3.1.1/cryptol/synchronous.py
+-rw-r--r--   0        0        0      338 2024-05-15 21:56:19.664149 cryptol-3.1.1/mypy.ini
+-rw-r--r--   0        0        0      628 2024-05-15 21:56:36.146979 cryptol-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8046 1970-01-01 00:00:00.000000 cryptol-3.1.1/PKG-INFO
```

### Comparing `cryptol-3.1.0/LICENSE` & `cryptol-3.1.1/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2013-2021 Galois Inc.
+Copyright (c) 2013-2024 Galois Inc.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
   * Redistributions of source code must retain the above copyright
```

### Comparing `cryptol-3.1.0/README.md` & `cryptol-3.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -190,7 +190,12 @@
 
 ```
 cryptol.connect(url="http://localhost:8080/", reset_server=True)
 ```
 
 will connect to a Cryptol server running at `http://localhost:8080/` and will
 guarantee any previous state on the server is cleared.
+
+
+## Supported Python Versions
+
+Currently, `cryptol-remote-api` officially supports python `3.12`. The `cryptol-remote-api` Docker image currently uses Python 3.10 and will be updated in issue #1661.
```

### Comparing `cryptol-3.1.0/cryptol/__init__.py` & `cryptol-3.1.1/cryptol/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import base64
 import os
 from enum import Enum
 from dataclasses import dataclass
-from distutils.spawn import find_executable
+from shutil import which
 from typing import Any, List, NoReturn, Optional, Union
 from typing_extensions import Literal
 
 import argo_client.interaction as argo
 from argo_client.interaction import HasProtocolState
 from argo_client.connection import DynamicSocketProcess, ServerConnection, ServerProcess, StdIOProcess, HttpProcess
 from . import cryptoltypes
```

### Comparing `cryptol-3.1.0/cryptol/bitvector.py` & `cryptol-3.1.1/cryptol/bitvector.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/cryptol/commands.py` & `cryptol-3.1.1/cryptol/commands.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/cryptol/connection.py` & `cryptol-3.1.1/cryptol/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from __future__ import annotations
 
 import os
 import sys
-from distutils.spawn import find_executable
+from shutil import which
 from typing import Any, List, Optional, Union, TextIO
 from typing_extensions import Literal
 
 import argo_client.interaction as argo
 from argo_client.connection import DynamicSocketProcess, ServerConnection, ServerProcess, StdIOProcess, HttpProcess
 from .custom_fstring import *
 from .quoting import *
@@ -73,25 +73,25 @@
     # User-passed url?
     if c is None and url is not None:
         c = CryptolConnection(ServerConnection(HttpProcess(url, verify=verify)), cryptol_path, log_dest=log_dest)
     # Check `CRYPTOL_SERVER` env var if no connection identified yet
     if c is None:
         command = os.getenv('CRYPTOL_SERVER')
         if command is not None:
-            command = find_executable(command)
+            command = which(command)
             if command is not None:
                 c = CryptolConnection(command+" socket", cryptol_path=cryptol_path, log_dest=log_dest, timeout=timeout)
     # Check `CRYPTOL_SERVER_URL` env var if no connection identified yet
     if c is None:
         url = os.getenv('CRYPTOL_SERVER_URL')
         if url is not None:
             c = CryptolConnection(ServerConnection(HttpProcess(url,verify=verify)), cryptol_path, log_dest=log_dest, timeout=timeout)
     # Check if `cryptol-remote-api` is in the PATH if no connection identified yet
     if c is None:
-        command = find_executable('cryptol-remote-api')
+        command = which('cryptol-remote-api')
         if command is not None:
             c = CryptolConnection(command+" socket", cryptol_path=cryptol_path, log_dest=log_dest, timeout=timeout)
     # Raise an error if still no connection identified yet
     if c is not None:
         if reset_server:
             CryptolResetServer(c)
         return c
```

### Comparing `cryptol-3.1.0/cryptol/cryptoltypes.py` & `cryptol-3.1.1/cryptol/cryptoltypes.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/cryptol/custom_fstring.py` & `cryptol-3.1.1/cryptol/custom_fstring.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/cryptol/opaque.py` & `cryptol-3.1.1/cryptol/opaque.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/cryptol/quoting.py` & `cryptol-3.1.1/cryptol/quoting.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/cryptol/single_connection.py` & `cryptol-3.1.1/cryptol/single_connection.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/cryptol/solver.py` & `cryptol-3.1.1/cryptol/solver.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/cryptol/synchronous.py` & `cryptol-3.1.1/cryptol/synchronous.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.1.0/PKG-INFO` & `cryptol-3.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: cryptol
-Version: 3.1.0
+Version: 3.1.1
 Summary: Cryptol client for the Cryptol RPC server
 License: BSD License
 Keywords: cryptography,verification
 Author: Galois, Inc.
 Author-email: cryptol-team@galois.com
 Requires-Python: >=3.8.0,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: BitVector (>=3.4.9,<4.0.0)
-Requires-Dist: argo-client (==0.0.11)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: argo-client (==0.0.12)
+Requires-Dist: requests (>=2.31.0)
+Requires-Dist: types-requests (>=2.31.0)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
+Requires-Dist: urllib3 (>=2.2.0)
 Description-Content-Type: text/markdown
 
 # Cryptol Python Client
 
 In-development Python client for Cryptol. Currently tested on Linux and MacOS --
 at present there may be some minor issues running the Python Client in a Windows
 environment that need to be addressed (e.g., some Python process management methods
@@ -212,7 +215,12 @@
 ```
 cryptol.connect(url="http://localhost:8080/", reset_server=True)
 ```
 
 will connect to a Cryptol server running at `http://localhost:8080/` and will
 guarantee any previous state on the server is cleared.
 
+
+## Supported Python Versions
+
+Currently, `cryptol-remote-api` officially supports python `3.12`. The `cryptol-remote-api` Docker image currently uses Python 3.10 and will be updated in issue #1661.
+
```

