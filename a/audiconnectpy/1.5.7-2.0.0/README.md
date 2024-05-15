# Comparing `tmp/audiconnectpy-1.5.7.tar.gz` & `tmp/audiconnectpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.5.7.tar", last modified: Fri May 10 17:52:06 2024, max compression
+gzip compressed data, was "audiconnectpy-2.0.0.tar", last modified: Wed May 15 16:11:03 2024, max compression
```

## Comparing `audiconnectpy-1.5.7.tar` & `audiconnectpy-2.0.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:52:06.591498 audiconnectpy-1.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:52:06.587498 audiconnectpy-1.5.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:52:06.587498 audiconnectpy-1.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:52:06.587498 audiconnectpy-1.5.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-10 17:52:06.591498 audiconnectpy-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:52:06.591498 audiconnectpy-1.5.7/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21270 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24559 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24226 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12014 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:52:06.591498 audiconnectpy-1.5.7/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-10 17:52:06.000000 audiconnectpy-1.5.7/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-10 17:52:06.000000 audiconnectpy-1.5.7/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:52:06.000000 audiconnectpy-1.5.7/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:52:06.000000 audiconnectpy-1.5.7/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 17:52:06.000000 audiconnectpy-1.5.7/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 17:52:06.000000 audiconnectpy-1.5.7/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:52:06.591498 audiconnectpy-1.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:52:06.591498 audiconnectpy-1.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 17:51:55.000000 audiconnectpy-1.5.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.061576 audiconnectpy-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.061576 audiconnectpy-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.061576 audiconnectpy-2.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22121 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26295 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:02.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 16:11:03.000000 audiconnectpy-2.0.0/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.065575 audiconnectpy-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-15 16:10:51.000000 audiconnectpy-2.0.0/tests/conftest.py
```

### Comparing `audiconnectpy-1.5.7/.github/dependabot.yml` & `audiconnectpy-2.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/.github/workflows/auto-approve.yml` & `audiconnectpy-2.0.0/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.0.0/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.0.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/.github/workflows/release.yml` & `audiconnectpy-2.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/.gitignore` & `audiconnectpy-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/.pre-commit-config.yaml` & `audiconnectpy-2.0.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.3
+    rev: v0.4.4
     hooks:
       - id: ruff
         args:
           - --fix
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
```

### Comparing `audiconnectpy-1.5.7/LICENSE` & `audiconnectpy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/PKG-INFO` & `audiconnectpy-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.5.7
+Version: 2.0.0
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8.1
 Requires-Dist: bs4>=0.0.2
+Requires-Dist: mashumaro>=3.13
 
 # audiconnectpy
 
 [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/cyr-ius/audiconnectpy/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/cyr-ius/audiconnectpy)](https://github.com/cyr-ius/audiconnectpy/releases/latest)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/audiconnectpy?label=PyPI%20Downloads)](https://pypi.org/project/audiconnectpy/)
```

### Comparing `audiconnectpy-1.5.7/README.md` & `audiconnectpy-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/audiconnectpy/actions.py` & `audiconnectpy-2.0.0/audiconnectpy/vehicle.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,180 @@
-"""Audi actions."""
+"""Vehicle class."""
 
 from __future__ import annotations
 
 import asyncio
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from datetime import datetime
+import logging
 from typing import Any, Literal
 
-from .auth import Auth
+from mashumaro import DataClassDictMixin, field_options
+
 from .const import (
     BRAND,
     FAILED,
     MAX_RESPONSE_ATTEMPTS,
     REQUEST_FAILED,
     REQUEST_STATUS_SLEEP,
     REQUEST_SUCCESSFUL,
     SUCCEEDED,
+    SUCCESSFUL,
 )
 from .exceptions import HttpRequestError, TimeoutExceededError
-from .helpers import ExtendedDict, spin_hash
+from .helpers import ExtendedDict, remove_value, spin_hash
+from .model import Location, Model, Position
+
+_LOGGER = logging.getLogger(__name__)
+
+
+class Globals:
+    """Global variables."""
+
+    def __init__(self, unit: str) -> None:
+        """Initilaze."""
+        global UNIT_SYSTEM  # pylint: disable=global-variable-undefined
+        UNIT_SYSTEM = f"{unit}"  # type: ignore
 
 
 @dataclass
-class AudiActions:
-    """Actions on vehicle."""
+class Vehicles(DataClassDictMixin):
+    """Vehicles."""
+
+    user_vehicles: list[Vehicle] = field(
+        metadata=field_options(alias="userVehicles"), default=None
+    )
+
+
+@dataclass
+class Vehicle(DataClassDictMixin):
+    """Vehicle class."""
 
-    auth: Auth
     vin: str
-    url: str
-    url_setter: str
-    country: str
-    api_level: dict[str, int]
-    spin: str | None
+    csid: str
+    nickname: str | None = None
+    last_access: datetime | None = None
+    uris: dict[str, str] = field(init=False)
+    spin: str = field(init=False)
+    auth: str = field(init=False)
+    infos: dict[str, Any] | None = field(
+        metadata=field_options(alias="vehicle"), default=None
+    )
+    capabilities: dict[str, Any] | None = field(init=False, default=None)
+    position: Position | None = field(init=False, default=None)
+    location: Location | None = field(init=False, default=None)
+
+    @property
+    def api_level(self) -> dict[str, int]:
+        """Return API Level."""
+        return {
+            "climatisation": 2,  # 2 or 3
+            "ventilation": 1,  # 1 or other
+            "charger": 1,  # 1 or 2 or 3 (json)
+            "windows_heating": 1,  # 1 or 2 (json)
+        }
+
+    def set_api_level(
+        self,
+        mode: Literal["climatisation", "ventilation", "charger", "window_heating"],
+        value: int,
+    ) -> None:
+        """Set API Level."""
+        if mode in self.api_level.keys():
+            self.api_level[mode] = int(value)
+
+    async def async_update(self) -> None:
+        """Update data vehicle."""
+
+        # Selective status
+        data = await self.async_get_selectivestatus()
+        data = remove_value(data)
+        vehicle_model = Model.from_dict(data)
+
+        for attr in vehicle_model.to_dict():
+            obj = getattr(vehicle_model, attr, None)
+            setattr(self, attr, obj)
+
+        self.last_access = vehicle_model.access.access_status.car_captured_timestamp
+
+        # Capabilities
+        capabilities = await self.async_get_capabilities()
+        self.capabilities = capabilities.get("capabilities")
+
+        # Position
+        position = await self.async_get_position()
+        self.position = Position.from_dict(position.get("data"))
+
+        # Locations (here.com)
+        location = await self.async_get_location()
+        self.location = Location.from_dict(
+            {
+                "proprietaries": [
+                    item
+                    for item in location.get("data", [])
+                    if "proprietaryData" not in item
+                ],
+                "addresses": [
+                    item
+                    for item in location.get("data", [])
+                    if "proprietaryData" in item
+                ],
+            }
+        )
+
+    async def async_get_location(self) -> ExtendedDict:
+        """Get destination data."""
+        headers = await self.auth.async_get_headers(token_type="here")
+        data = await self.auth.get(f"{self.uris['here_url']}/location", headers=headers)
+        return data
+
+    async def async_get_position(self) -> ExtendedDict:
+        """Get position data."""
+        headers = await self.auth.async_get_headers(token_type="idk")
+        data = await self.auth.get(
+            f"{self.uris['cv_url']}/vehicles/{self.vin}/parkingposition",
+            headers=headers,
+        )
+        return data
+
+    async def async_get_capabilities(self) -> ExtendedDict:
+        """Get capabilities."""
+        headers = await self.auth.async_get_headers(token_type="idk")
+        data = await self.auth.get(
+            f"{self.uris['cv_url']}/vehicles/{self.vin}/capabilities",
+            headers=headers,
+        )
+        return data
+
+    async def async_get_selectivestatus(
+        self, jobs: list[str] | None = None
+    ) -> ExtendedDict:
+        """Get capabilities."""
+        if not jobs:
+            headers = await self.auth.async_get_headers(token_type="idk")
+            capabilities = await self.auth.get(
+                f"{self.uris['cv_url']}/vehicles/{self.vin}/selectivestatus?jobs=userCapabilities",
+                headers=headers,
+            )
+            dict_values = (
+                capabilities.get("userCapabilities", {})
+                .get("capabilitiesStatus", {})
+                .get("value", [])
+            )
+            self.capabilities = [
+                d for capability in dict_values if (d := capability.get("id"))
+            ]
+
+        str_jobs = ",".join(self.capabilities)
+        headers = await self.auth.async_get_headers(token_type="idk")
+        data = await self.auth.get(
+            f"{self.uris['cv_url']}/vehicles/{self.vin}/selectivestatus?jobs={str_jobs},userCapabilities",
+            headers=headers,
+        )
+        return data
 
     async def async_set_lock(self, lock: bool) -> None:
         """Set lock."""
         security_token = await self._async_get_security_token(
             "rlu_v1/operations/" + ("LOCK" if lock else "UNLOCK")
         )
         headers = await self.auth.async_get_action_headers(
@@ -43,23 +183,23 @@
         )
         data: str | dict[str, Any] = (
             '<?xml version="1.0" encoding= "UTF-8" ?>'
             + f'<rluAction xmlns="http://audi.de/connect/rlu"><action>{"lock" if lock else "unlock"}</action></rluAction>'
         )
 
         rsp = await self.auth.post(
-            f"{self.url}/bs/rlu/v1/{BRAND}/{self.country}/vehicles/{self.vin}/actions",
+            f"{self.uris['url']}/bs/rlu/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
         rsp = rsp if rsp else ExtendedDict()
         request_id = rsp.getr("rluActionResponse.requestId")
         await self._async_check_request(
-            f"{self.url}/bs/rlu/v1/{BRAND}/{self.country}/vehicles/{self.vin}/requests/{request_id}/status",
+            f"{self.uris['url']}/bs/rlu/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/requests/{request_id}/status",
             "lock vehicle" if lock else "unlock vehicle",
             REQUEST_SUCCESSFUL,
             REQUEST_FAILED,
             "requestStatusResponse.status",
         )
 
     async def async_set_climater(
@@ -112,23 +252,23 @@
                 }
                 if start
                 else {"action": {"type": "stopClimatisation"}}
             )
             use_json = True
 
         rsp = await self.auth.post(
-            f"{self.url}/bs/climatisation/v1/{BRAND}/{self.country}/vehicles/{self.vin}/climater/actions",
+            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
             use_json=use_json,
         )
         rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self._async_check_request(
-            f"{self.url}/bs/climatisation/v1/{BRAND}/{self.country}/vehicles/{self.vin}/climater/actions/{actionid}",
+            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "start climatisation" if start else "stop climatisation",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_climater_temp(
@@ -182,23 +322,23 @@
                             "zoneSettings": {"zoneSetting": zone_settings},
                         },
                     },
                 }
             }
             use_json = True
         rsp = await self.auth.post(
-            f"{self.url}/bs/climatisation/v1/{BRAND}/{self.country}/vehicles/{self.vin}/climater/actions",
+            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
             use_json=use_json,
         )
         rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self._async_check_request(
-            f"{self.url}/bs/climatisation/v1/{BRAND}/{self.country}/vehicles/{self.vin}/climater/actions/{actionid}",
+            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "set target temperature",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_pre_heating(self, start: bool, duration: int = 60) -> None:
@@ -231,15 +371,15 @@
                 }
                 if start
                 else {"performAction": {"quickstop": {"active": False}}}
             )
             use_json = True
 
         await self.auth.post(
-            f"{self.url}/bs/rs/v1/{BRAND}/{self.country}/vehicles/{self.vin}/action",
+            f"{self.uris['url']}/bs/rs/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/action",
             headers=headers,
             data=data,
             use_json=use_json,
         )
 
     async def async_set_ventilation(self, start: bool, duration: int = 60) -> None:
         """Set ventilation."""
@@ -280,15 +420,15 @@
                 }
                 if start
                 else {"performAction": {"quickstop": {"active": False}}}
             )
             use_json = True
 
         await self.auth.post(
-            f"{self.url}/bs/rs/v1/{BRAND}/{self.country}/vehicles/{self.vin}/action",
+            f"{self.uris['url']}/bs/rs/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/action",
             headers=headers,
             data=data,
             use_json=use_json,
         )
 
     async def async_set_battery_charger(self, start: bool, timer: bool = False) -> None:
         """Set battery charger."""
@@ -320,23 +460,23 @@
             headers = await self.auth.async_get_action_headers(
                 "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
             )
             data = f'<?xml version="1.0" encoding="UTF-8" ?><action><type>{"start" if start else "stop"}</type></action>'
             use_json = False
 
         rsp = await self.auth.post(
-            f"{self.url}/bs/batterycharge/v1/{BRAND}/{self.country}/vehicles/{self.vin}/charger/actions",
+            f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions",
             headers=headers,
             data=data,
             use_json=use_json,
         )
         rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self._async_check_request(
-            f"{self.url}/bs/batterycharge/v1/{BRAND}/{self.country}/vehicles/{self.vin}/charger/actions/{actionid}",
+            f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions/{actionid}",
             "start charger" if start else "stop charger",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_charger_max(self, current: float = 32) -> None:
@@ -357,23 +497,23 @@
             data = (
                 '<?xml version="1.0" encoding="UTF-8" ?><action><type>setSettings</type>'
                 + f"<settings><maxChargeCurrent>{current}</maxChargeCurrent></settings></action>"
             )
             use_json = False
 
         rsp = await self.auth.post(
-            f"{self.url}/bs/batterycharge/v1/{BRAND}/{self.country}/vehicles/{self.vin}/charger/actions",
+            f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions",
             headers=headers,
             data=data,
             use_json=use_json,
         )
         rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self._async_check_request(
-            f"{self.url}/bs/batterycharge/v1/{BRAND}/{self.country}/vehicles/{self.vin}/charger/actions/{actionid}",
+            f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions/{actionid}",
             "set charger max current",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_window_heating(self, start: bool) -> None:
@@ -392,35 +532,35 @@
             )
             data = (
                 '<?xml version="1.0" encoding= "UTF-8" ?>'
                 + f"<action><type>{'startWindowHeating' if start else 'stopWindowHeating'}</type></action>"
             )
             use_json = False
         rsp = await self.auth.post(
-            f"{self.url}/bs/climatisation/v1/{BRAND}/{self.country}/vehicles/{self.vin}/climater/actions",
+            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
             use_json=use_json,
         )
         rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self._async_check_request(
-            f"{self.url}/bs/climatisation/v1/{BRAND}/{self.country}/vehicles/{self.vin}/climater/actions/{actionid}",
+            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "start window heating" if start else "stop window heating",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_honkflash(
         self, mode: Literal["honk", "flash"], duration: int = 15
     ) -> None:
         """Set honk and flash light."""
         rsp_position = await self.auth.get(
-            f"{self.url}/bs/cf/v1/{BRAND}/{self.country}/vehicles/{self.vin}/position"
+            f"{self.uris['url']}/bs/cf/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/position"
         )
         rsp_position = rsp_position if rsp_position else ExtendedDict()
         position = rsp_position.getr("findCarResponse.Position.carCoordinate")
         headers = await self.auth.async_get_action_headers("application/json", None)
         data: str | dict[str, Any] = {
             "honkAndFlashRequest": {
                 "serviceOperationCode": "HONK_AND_FLASH"
@@ -430,75 +570,75 @@
                 "userPosition": {
                     "latitude": position["latitude"],
                     "longitude": position["longitude"],
                 },
             }
         }
         await self.auth.post(
-            f"{self.url}/bs/rhf/v1/{BRAND}/{self.country}/vehicles/{self.vin}/honkAndFlash",
+            f"{self.uris['url']}/bs/rhf/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/honkAndFlash",
             headers=headers,
             data=data,
         )
 
     async def async_refresh_vehicle_data(self) -> None:
         """Refresh vehicle data."""
         headers = await self.auth.async_get_headers(token_type="idk")
-        region = "emea" if self.country.upper() != "US" else "na"
         data = await self.auth.post(
-            f"https://{region}.bff.cariad.digital/vehicle/v1/vehicles/{self.vin}/vehiclewakeup",
+            f"{self.uris['cv_url']}/vehicles/{self.vin}/vehiclewakeup",
             headers=headers,
         )
         data = data if data else ExtendedDict()
         request_id: str = data.getr("data.requestID")
         await self._async_pending_request(
-            f"https://{region}.bff.cariad.digital/vehicle/v1/vehicles/{self.vin}/pendingrequests",
+            f"{self.uris['cv_url']}/vehicles/{self.vin}/pendingrequests",
             "refresh vehicle data",
-            "successful",
-            "failed",
+            SUCCESSFUL,
+            FAILED,
             request_id,
         )
 
-    async def _async_check_request(
-        self, url: str, action: str, success: str, failed: str, path: str
+    async def _async_pending_request(
+        self, url: str, action: str, success: str, failed: str, request_id: str
     ) -> None:
         """Check request succeeded."""
         stauts_good = False
         for _ in range(MAX_RESPONSE_ATTEMPTS):
             await asyncio.sleep(REQUEST_STATUS_SLEEP)
 
-            rsp = await self.auth.get(url)
+            headers = await self.auth.async_get_headers(token_type="idk")
+            rsp = await self.auth.get(url, headers=headers)
 
-            status = rsp.getr(path)
+            status = None
+            if rsp and (data := rsp.get("data")):
+                for item in data:
+                    if item.get("id") == request_id:
+                        status = item.get("status")
+                        break
 
             if status is None or (failed is not None and status == failed):
                 raise HttpRequestError(("Cannot %s, return code '%s'", action, status))
 
             if status == success:
                 stauts_good = True
                 break
 
         if stauts_good is False:
             raise TimeoutExceededError(("Cannot %s, operation timed out", action))
 
-    async def _async_pending_request(
-        self, url: str, action: str, success: str, failed: str, request_id: str
+    async def _async_check_request(
+        self, url: str, action: str, success: str, failed: str, path: str
     ) -> None:
         """Check request succeeded."""
         stauts_good = False
-        headers = await self.auth.async_get_headers(token_type="idk")
-
         for _ in range(MAX_RESPONSE_ATTEMPTS):
             await asyncio.sleep(REQUEST_STATUS_SLEEP)
-            rsp = await self.auth.get(url, headers=headers)
-            status = None
-            if rsp and (data := rsp.get("data")):
-                for item in data:
-                    if item.get("id") == request_id:
-                        status = item.get("status")
-                        break
+
+            rsp = await self.auth.get(url)
+
+            status = rsp.getr(path)
 
             if status is None or (failed is not None and status == failed):
                 raise HttpRequestError(("Cannot %s, return code '%s'", action, status))
 
             if status == success:
                 stauts_good = True
                 break
@@ -509,15 +649,15 @@
     async def _async_get_security_token(self, action: str) -> Any:
         """Get security token."""
         self.spin = "" if self.spin is None else self.spin
 
         # Challenge
         headers = await self.auth.async_get_headers(token_type="mbb", okhttp=True)
         rsp = await self.auth.get(
-            f"{self.url_setter}/rolesrights/authorization/v2/vehicles/{self.vin}/services/{action}/security-pin-auth-requested",
+            f"{self.uris['url_setter']}/rolesrights/authorization/v2/vehicles/{self.vin}/services/{action}/security-pin-auth-requested",
             headers=headers,
         )
         rsp = rsp if rsp else ExtendedDict()
         sec_token = rsp.getr("securityPinAuthInfo.securityToken")
         challenge: str = rsp.getr(
             "securityPinAuthInfo.securityPinTransmission.challenge"
         )
@@ -532,12 +672,12 @@
                 },
                 "securityToken": sec_token,
             }
         }
 
         headers["Content-Type"] = "application/json"
         body = await self.auth.post(
-            f"{self.url_setter}/rolesrights/authorization/v2/security-pin-auth-completed",
+            f"{self.uris['url_setter']}/rolesrights/authorization/v2/security-pin-auth-completed",
             headers=headers,
             data=data,
         )
         return body["securityToken"]
```

### Comparing `audiconnectpy-1.5.7/audiconnectpy/auth.py` & `audiconnectpy-2.0.0/audiconnectpy/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import aiohttp
 from aiohttp.hdrs import METH_GET, METH_POST, METH_PUT
 import async_timeout
 from bs4 import BeautifulSoup
 
 from .exceptions import (
     AudiException,
+    AuthorizationError,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
 )
 from .helpers import ExtendedDict, json_loads
 
 TIMEOUT = 120
@@ -46,31 +47,23 @@
         self, session: aiohttp.ClientSession, proxy: str | None = None
     ) -> None:
         """Initialize."""
         self._session = session
         self.__proxy: dict[str, str] | None = (
             {"http": proxy, "https": proxy} if proxy else None
         )
-        self._audi_baseurl = ""
-        self._mbb_baseurl = MBB_URL
-        self._token_endpoint_url = ""
-        self._authorization_endpoint_url = ""
-        self._revocation_endpoint_url = ""
-        self.profil_url = ""
 
-        self._client_id = CLIENT_ID
-        self._x_client_id = ""
+        self._x_client_id: str | None = None
         self.user_id = ""
-        self.language = ""
-        self._country = ""
         self._mbb_token: dict[str, Any] = {}
         self._here_token: dict[str, Any] = {}
         self._mbb_token_expired: datetime | None = None
         self._idk_token: dict[str, str] = {}
         self._audi_token: dict[str, str] = {}
+        self.uris: dict[str, str] = {}
 
     async def request(
         self,
         method: str,
         url: str,
         data: Any | None = None,
         headers: dict[str, str] | None = None,
@@ -153,37 +146,34 @@
             data = json.dumps(data)
         response = await self.request(
             METH_POST, url, headers=headers, data=data, **kwargs
         )
         return response
 
     async def async_connect(
-        self, username: str, password: str, country: str, tries: int = 3
-    ) -> bool:
+        self, username: str, password: str, uris: dict[str, str], tries: int = 3
+    ) -> None:
         """Connect to API."""
         try:
-            self._country = country
+            self.uris = uris
             await self._async_login(username, password)
-        except HttpRequestError as error:  # pylint: disable=broad-except
+        except HttpRequestError as error:
             if tries > 1:
                 _LOGGER.warning(
                     "Login to Audi service failed, trying again in %s seconds [ERROR:%s]",
                     DELAY,
                     str(error),
                 )
                 await asyncio.sleep(DELAY)
-                return await self.async_connect(username, password, country, tries - 1)
-            _LOGGER.error("Login to Audi service failed: %s ", str(error))
-            return False
-        else:
-            return True
+                return await self.async_connect(username, password, uris, tries - 1)
+
+            raise AuthorizationError("Login to Audi service failed: %s ", error)
 
     async def _async_login(self, user: str, password: str) -> None:
         """Request login."""
-        await self._async_retrieve_url_service()
 
         # Generate code_challenge
         code_verifier = str(base64.urlsafe_b64encode(os.urandom(32)), "utf-8").strip(
             "="
         )
         code_challenge = str(
             base64.urlsafe_b64encode(
@@ -193,37 +183,37 @@
         ).strip("=")
         code_challenge_method = "S256"
 
         # login page
         headers = await self.async_get_headers()
         idk_data = {
             "response_type": "code",
-            "client_id": self._client_id,
+            "client_id": self.uris["client_id"],
             "redirect_uri": "myaudi:///",
             "scope": "address badge birthdate birthplace email gallery mbb name nationalIdentifier nationality nickname phone picture profession profile vin openid",
             "state": str(uuid.uuid4()),
             "nonce": str(uuid.uuid4()),
             "prompt": "login",
             "code_challenge": code_challenge,
             "code_challenge_method": code_challenge_method,
-            "ui_locales": f"{self.language}-{self.language} {self.language}",
+            "ui_locales": f"{self.uris['language']}-{self.uris['language']} {self.uris['language']}",
         }
         idk_rsp, idk_rsptxt = await self.request(
             "GET",
-            self._authorization_endpoint_url,
+            self.uris["authorization_endpoint"],
             None,
             headers=headers,
             params=idk_data,
             raw_reply=True,
             raw_rsp=True,
         )
 
         # form_data with email
         submit_data = self._get_hidden_html_input_form_data(idk_rsptxt, {"email": user})
-        submit_url = self._get_post_url(idk_rsptxt, self._authorization_endpoint_url)
+        submit_url = self._get_post_url(idk_rsptxt, self.uris["authorization_endpoint"])
         # send email
         email_rsptxt = await self.request(
             "POST",
             submit_url,
             submit_data,
             headers=headers,
             cookies=idk_rsp.cookies,
@@ -366,58 +356,14 @@
                 self._here_token = await self._async_get_here_token(
                     id_token=self._idk_token["id_token"]
                 )
 
             except AudiException as error:  # pylint: disable=broad-except
                 _LOGGER.error("Refresh token failed: %s", str(error))
 
-    async def _async_retrieve_url_service(self) -> None:
-        """Get urls for request."""
-        # Get markets to get language
-        markets_json = await self.request("GET", f"{MARKET_URL}/markets", None)
-
-        country_spec = markets_json.getr("countries.countrySpecifications")
-        if self._country.upper() not in country_spec:
-            raise AudiException("Country not found")
-
-        self.language = country_spec.get(self._country.upper(), {}).get(
-            "defaultLanguage"
-        )
-
-        # Get market config to get client_id , Authorization base url and mbbOAuth base url
-        market_json = await self.request(
-            "GET", f"{MARKET_URL}/market/{self._country.upper()}/{self.language}", None
-        )
-
-        self._client_id = market_json.get("idkClientIDAndroidLive", CLIENT_ID)
-        self._audi_baseurl = market_json.get(
-            "myAudiAuthorizationServerProxyServiceURLProduction", ""
-        )
-        self.profil_url = (
-            market_json.get("idkCustomerProfileMicroserviceBaseURLLive", "") + "/v3"
-        )
-        openid_url = market_json.get("idkLoginServiceConfigurationURLProduction", "")
-        self._mbb_baseurl = market_json.get("mbbOAuthBaseURLLive", MBB_URL)
-
-        _LOGGER.debug("Client id: %s", self._client_id)
-        _LOGGER.debug("Audi Base Url: %s", self._audi_baseurl)
-        _LOGGER.debug("MBB Base Url: %s", self._mbb_baseurl)
-        _LOGGER.debug("IDK Base Url: %s", openid_url)
-
-        # Get openId config to get authorizationEndpoint, tokenEndpoint, RevocationEndpoint
-        openid_json = await self.request("GET", openid_url, None)
-
-        self._authorization_endpoint_url = openid_json.get("authorization_endpoint", "")
-        self._token_endpoint_url = openid_json.get("token_endpoint", "")
-        self._revocation_endpoint_url = openid_json.get("revocation_endpoint", "")
-
-        _LOGGER.debug("AuthEndpoint: %s", self._authorization_endpoint_url)
-        _LOGGER.debug("TokenEndpoint: %s", self._token_endpoint_url)
-        _LOGGER.debug("RevocationEndpoint: %s", self._revocation_endpoint_url)
-
     async def async_get_action_headers(
         self, content_type: str, security_token: str | None, x_security: bool = False
     ) -> dict[str, str]:
         """Return header for vehicle action."""
         headers = {
             "Content-Type": content_type,
             "User-Agent": "okhttp/3.11.0",
@@ -431,15 +377,15 @@
 
         headers = await self.async_get_headers(token_type="mbb", headers=headers)
 
         return headers
 
     async def async_get_headers(
         self,
-        token_type: Literal["idk", "mbb", "audi"] | None = None,
+        token_type: Literal["idk", "mbb", "audi", "here"] | None = None,
         headers: dict[str, Any] | None = None,
         okhttp: bool = False,
         security_token: str | None = None,
     ) -> dict[str, str]:
         """Get simple headers."""
         defaults = {
             "Accept": "application/json",
@@ -528,67 +474,67 @@
             "grant_type": "id_token",
             "token": kwargs.get("id_token"),
             "stage": "live",
             "config": "myaudi",
         }
         azs_token_json = await self.request(
             "POST",
-            self._audi_baseurl + "/token",
+            self.uris["audi_url"] + "/token",
             json.dumps(asz_req_data),
             headers=headers,
             allow_redirects=False,
         )
         _LOGGER.debug("AZS Token: %s", azs_token_json)
         return azs_token_json
 
     async def _async_get_idk_token(self, **kwargs: Any) -> Any:
         """Get IDK Token."""
-        refresh_token = kwargs.get("refresh_token")
-        code = kwargs.get("code")
-        code_verifier = kwargs.get("code_verifier")
         headers = {
             "Accept": "application/json",
             "Accept-Charset": "utf-8",
             "User-Agent": HDR_USER_AGENT,
             "Content-Type": "application/x-www-form-urlencoded",
         }
         # IDK token request data
-        if refresh_token:
+        if "refresh_token" in kwargs:
             idk_data = {
-                "client_id": self._client_id,
+                "client_id": self.uris["client_id"],
                 "grant_type": "refresh_token",
-                "refresh_token": refresh_token,
+                "refresh_token": kwargs.get("refresh_token"),
                 "response_type": "token id_token",
             }
         else:
             idk_data = {
-                "client_id": self._client_id,
+                "client_id": self.uris["client_id"],
                 "grant_type": "authorization_code",
-                "code": code,
+                "code": kwargs.get("code"),
                 "redirect_uri": "myaudi:///",
                 "response_type": "token id_token",
-                "code_verifier": code_verifier,
+                "code_verifier": kwargs.get("code_verifier"),
             }
 
         # IDK token request
         encoded_idk_data = urlencode(idk_data, encoding="utf-8").replace("+", "%20")
 
         idk_token_json = await self.post(
-            self._token_endpoint_url,
+            self.uris["token_endpoint"],
             encoded_idk_data,
             headers=headers,
             allow_redirects=False,
             use_json=False,
         )
         _LOGGER.debug("IDK Token: %s", idk_token_json)
 
         return idk_token_json
 
-    async def _async_register_idk(self) -> Any:
-        """Register IDK."""
+    async def _async_register_idk(self) -> str:
+        """Register IDK.
+
+        Return X-Client-ID
+        """
         # mbboauth client register
         headers = {
             "Accept": "application/json",
             "Accept-Charset": "utf-8",
             "User-Agent": HDR_USER_AGENT,
             "Content-Type": "application/json",
         }
@@ -597,20 +543,20 @@
             "platform": "google",
             "client_brand": "Audi",
             "appName": "myAudi",
             "appVersion": HDR_XAPP_VERSION,
             "appId": "de.myaudi.mobile.assistant",
         }
         mbboauth_client_reg_json = await self.post(
-            self._mbb_baseurl + "/mobile/register/v1",
+            self.uris["mbb_url"] + "/mobile/register/v1",
             mbboauth_reg_data,
             headers=headers,
             allow_redirects=False,
         )
-        return mbboauth_client_reg_json.get("client_id")
+        return str(mbboauth_client_reg_json.get("client_id", ""))
 
     async def _async_get_mbb_token(self, **kwargs: Any) -> Any:
         """Authentication to mbboauth-1d.prd.ece.vwg-connect.com."""
         headers = {
             "Accept": "application/json",
             "Accept-Charset": "utf-8",
             "User-Agent": HDR_USER_AGENT,
@@ -632,15 +578,15 @@
                 "token": kwargs.get("id_token"),
                 "scope": "sc2:fal",
             }
         encoded_mbboauth_data = urlencode(mbboauth_data, encoding="utf-8").replace(
             "+", "%20"
         )
         mbboauth_json = await self.post(
-            self._mbb_baseurl + "/mobile/oauth2/v1/token",
+            self.uris["mbb_url"] + "/mobile/oauth2/v1/token",
             encoded_mbboauth_data,
             headers=headers,
             allow_redirects=False,
             use_json=False,
         )
         _LOGGER.debug("MBB Token: %s", mbboauth_json)
         return mbboauth_json
@@ -667,15 +613,15 @@
                 "scope": "sc2:here_a_t21-s",
             }
 
         encoded_hereoauth_data = urlencode(hereoauth_data, encoding="utf-8").replace(
             "+", "%20"
         )
         hereoauth_json = await self.post(
-            self._mbb_baseurl + "/mobile/oauth2/v1/token",
+            self.uris["mbb_url"] + "/mobile/oauth2/v1/token",
             encoded_hereoauth_data,
             headers=headers,
             allow_redirects=False,
             use_json=False,
         )
         _LOGGER.debug("Here Token: %s", hereoauth_json)
         return hereoauth_json
```

### Comparing `audiconnectpy-1.5.7/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.0.0/audiconnectpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.5.7
+Version: 2.0.0
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8.1
 Requires-Dist: bs4>=0.0.2
+Requires-Dist: mashumaro>=3.13
 
 # audiconnectpy
 
 [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/cyr-ius/audiconnectpy/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/cyr-ius/audiconnectpy)](https://github.com/cyr-ius/audiconnectpy/releases/latest)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/audiconnectpy?label=PyPI%20Downloads)](https://pypi.org/project/audiconnectpy/)
```

### Comparing `audiconnectpy-1.5.7/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.0.0/audiconnectpy.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 .github/dependabot.yml
 .github/workflows/auto-approve.yml
 .github/workflows/pythonpackage.yml
 .github/workflows/pythonpublish.yml
 .github/workflows/release.yml
 .vscode/settings.json
 audiconnectpy/__init__.py
-audiconnectpy/actions.py
 audiconnectpy/api.py
 audiconnectpy/auth.py
 audiconnectpy/const.py
 audiconnectpy/exceptions.py
 audiconnectpy/helpers.py
-audiconnectpy/models.py
-audiconnectpy/services.py
+audiconnectpy/model.py
 audiconnectpy/vehicle.py
 audiconnectpy.egg-info/PKG-INFO
 audiconnectpy.egg-info/SOURCES.txt
 audiconnectpy.egg-info/dependency_links.txt
 audiconnectpy.egg-info/not-zip-safe
 audiconnectpy.egg-info/requires.txt
 audiconnectpy.egg-info/top_level.txt
-tests/__init__.py
+tests/__init__.py
+tests/conftest.py
```

### Comparing `audiconnectpy-1.5.7/example.py` & `audiconnectpy-2.0.0/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.7/pyproject.toml` & `audiconnectpy-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 requires-python = ">=3.10.0"
 dependencies    = [
     "aiohttp>=3.8.1",
     "bs4>=0.0.2",
+    "mashumaro>=3.13",
 ]
 
 [tool.setuptools_scm]
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = false
```

