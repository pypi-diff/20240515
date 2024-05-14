# Comparing `tmp/sdss_tpm_multicast_client-0.1.1.tar.gz` & `tmp/sdss_tpm_multicast_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_tpm_multicast_client-0.1.1.tar", max compression
+gzip compressed data, was "sdss_tpm_multicast_client-0.2.0.tar", max compression
```

## Comparing `sdss_tpm_multicast_client-0.1.1.tar` & `sdss_tpm_multicast_client-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1253 2023-10-25 02:31:14.699965 sdss_tpm_multicast_client-0.1.1/README.md
--rw-r--r--   0        0        0     1398 2023-10-25 02:31:14.700442 sdss_tpm_multicast_client-0.1.1/build.py
--rw-r--r--   0        0        0     1298 2023-10-25 02:31:14.704187 sdss_tpm_multicast_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      444 2023-10-25 02:31:14.704826 sdss_tpm_multicast_client-0.1.1/src/tpm_multicast_client/__init__.py
--rw-r--r--   0        0        0      899 2023-10-25 02:31:14.705456 sdss_tpm_multicast_client-0.1.1/src/tpm_multicast_client/__main__.py
--rw-r--r--   0        0        0     3021 2023-10-25 02:31:14.705934 sdss_tpm_multicast_client-0.1.1/src/tpm_multicast_client/client.py
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 sdss_tpm_multicast_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1836 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1801 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      448 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/__init__.py
+-rw-r--r--   0        0        0      899 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/__main__.py
+-rw-r--r--   0        0        0     3031 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/client.py
+-rw-r--r--   0        0        0     6534 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/unpack.py
+-rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 sdss_tpm_multicast_client-0.2.0/PKG-INFO
```

### Comparing `sdss_tpm_multicast_client-0.1.1/pyproject.toml` & `sdss_tpm_multicast_client-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 [tool.poetry]
 name = "sdss-tpm-multicast-client"
-version = "0.1.1"
+version = "0.2.0"
 description = "TPM multicast client"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD 3-Clause"
 readme = "README.md"
 packages = [
     { include = "tpm_multicast_client", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10,<4.0"
 sdsstools = "^1.0.0"
 
-[tool.poetry.build]
-script = "build.py"
-generate-setup-file = false
-
 [tool.poetry.group.dev.dependencies]
 ipython = ">=8.0.0"
 ipdb = ">=0.13.3"
-black = {version = ">=21.10b0", allow-prereleases = true}
-ruff = "^0.0.289"
+black = ">=21.10"
+ruff = ">=0.1.0"
+pytest = ">=5.2.2"
+pytest-cov = ">=2.8.1"
+pytest-mock = ">=1.13.0"
+pytest-sugar = ">=0.9.2"
+coverage = {version = ">=5.0", extras = ["toml"]}
 
 [tool.poetry.scripts]
 tpm-multicast-client = "tpm_multicast_client.__main__:tpm_multicast_client"
 
 [tool.black]
 line-length = 88
 target-version = ['py312']
 fast = true
 
 [tool.ruff]
 line-length = 88
 target-version = 'py312'
+exclude = ["typings/"]
+
+[tool.ruff.lint]
 select = ["E", "F", "I"]
 unfixable = ["F841"]
-exclude = ["typings/"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403", "E402"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["tpm_multicast_client"]
 lines-after-imports = 2
 section-order = ["future", "standard-library", "typing", "third-party", "sdss", "first-party", "local-folder"]
 
-[tool.ruff.isort.sections]
+[tool.ruff.lint.isort.sections]
 typing = ["typing"]
 sdss = ["sdsstools"]
 
+[tool.pytest.ini_options]
+addopts = "--cov tpm_multicast_client --cov-report xml --cov-report html --cov-report term -W ignore"
+asyncio_mode = "auto"
+
+[tool.coverage.run]
+branch = true
+include = ["src/tpm_multicast_client/*"]
+omit = [
+    "**/__init__.py",
+    "**/tpm_multicast_client/__main__.py",
+    "**/tpm_multicast_client/client.py",
+]
+
+[tool.coverage.report]
+exclude_lines = [
+    "if TYPE_CHECKING:",
+    "# pragma: no cover"
+]
+
 [build-system]
 requires = ["poetry-core", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sdss_tpm_multicast_client-0.1.1/src/tpm_multicast_client/__main__.py` & `sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_tpm_multicast_client-0.1.1/src/tpm_multicast_client/client.py` & `sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import asyncio
 import socket
 import struct
 import warnings
 
 from typing import Awaitable, Callable
 
-from tpm_multicast_client.tpmdgram import data2dict
+from tpm_multicast_client.unpack import unpack_tpm_data
 
 
 CallbackType = Callable[[dict], None | Awaitable[None]]
 
 MCAST_GRP = "224.1.1.1"
 MCAST_PORT = 2007
 IS_ALL_GROUPS = True
@@ -51,15 +51,15 @@
         self.callback = callback
         self.loop = loop
 
         self.is_closed = asyncio.Future()
 
     def datagram_received(self, data, _):
         try:
-            dd = data2dict(data)
+            dd = unpack_tpm_data(data)
             if asyncio.iscoroutinefunction(self.callback):
                 asyncio.create_task(self.callback(dd))
             else:
                 self.loop.call_soon(self.callback, dd)
         except Exception as ee:
             warnings.warn(f"Failed decoding message from multicast: {ee}", UserWarning)
```

### Comparing `sdss_tpm_multicast_client-0.1.1/PKG-INFO` & `sdss_tpm_multicast_client-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 Metadata-Version: 2.1
 Name: sdss-tpm-multicast-client
-Version: 0.1.1
+Version: 0.2.0
 Summary: TPM multicast client
 License: BSD 3-Clause
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # tpm_multicast_client
 
-Listens to the TPM multicast stream and unpack the status dictionary using Jeff Hagen's `tpmdgram` code.
+![Versions](https://img.shields.io/badge/python->=3.10-blue)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Test](https://github.com/sdss/tpm-multicast-client/actions/workflows/test.yml/badge.svg)](https://github.com/sdss/tpm-multicast-client/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/sdss/tpm-multicast-client/graph/badge.svg?token=eOF9ZykYgu)](https://codecov.io/gh/sdss/tpm-multicast-client)
+
+Listens to the TPM multicast stream and unpack the data into a status dictionary. This is a Python-only implementation of Jeff Hagen's ``tpmdgram.c``.
 
 ## Installation
 
 To install with `pip` do
 
 ```console
 pip install sdss-tpm-multicast-client
 ```
 
 To install from source do
 
 ```console
+pip install .
+```
+
+or, for development,
+
+```console
 poetry install
 ```
 
 More information on developing with Poetry can be found [here](https://python-poetry.org).
 
 ## Usage
```

