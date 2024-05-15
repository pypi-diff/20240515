# Comparing `tmp/purgatory-1.0.3.tar.gz` & `tmp/purgatory-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purgatory-1.0.3.tar", max compression
+gzip compressed data, was "purgatory-2.0.0.tar", max compression
```

## Comparing `purgatory-1.0.3.tar` & `purgatory-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1523 2021-12-28 07:38:48.830707 purgatory-1.0.3/LICENSE
--rw-r--r--   0        0        0     3410 2023-07-23 15:11:39.521798 purgatory-1.0.3/README.rst
--rw-r--r--   0        0        0     1590 2023-07-29 13:03:59.770700 purgatory-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1199 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/__init__.py
--rw-r--r--   0        0        0       85 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/messages/__init__.py
--rw-r--r--   0        0        0      304 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/messages/base.py
--rw-r--r--   0        0        0      221 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/messages/commands.py
--rw-r--r--   0        0        0      554 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/messages/events.py
--rw-r--r--   0        0        0     7510 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/model.py
--rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/py.typed
--rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/_async/__init__.py
--rw-r--r--   0        0        0     5795 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/_async/circuitbreaker.py
--rw-r--r--   0        0        0     1633 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/_async/message_handlers.py
--rw-r--r--   0        0        0     3723 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/_async/messagebus.py
--rw-r--r--   0        0        0     4614 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/service/_async/repository.py
--rw-r--r--   0        0        0     1833 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/service/_async/unit_of_work.py
--rw-r--r--   0        0        0      274 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/service/_redis.py
--rw-r--r--   0        0        0        0 2023-07-29 13:03:55.197350 purgatory-1.0.3/src/purgatory/service/_sync/__init__.py
--rw-r--r--   0        0        0     5663 2023-07-29 13:03:55.200683 purgatory-1.0.3/src/purgatory/service/_sync/circuitbreaker.py
--rw-r--r--   0        0        0     1573 2023-07-29 13:03:55.754019 purgatory-1.0.3/src/purgatory/service/_sync/message_handlers.py
--rw-r--r--   0        0        0     3692 2023-07-29 13:03:55.204017 purgatory-1.0.3/src/purgatory/service/_sync/messagebus.py
--rw-r--r--   0        0        0     4433 2023-07-29 13:03:55.780686 purgatory-1.0.3/src/purgatory/service/_sync/repository.py
--rw-r--r--   0        0        0     1746 2023-07-29 13:03:55.207350 purgatory-1.0.3/src/purgatory/service/_sync/unit_of_work.py
--rw-r--r--   0        0        0      945 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/service/typing.py
--rw-r--r--   0        0        0      383 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/typing.py
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 purgatory-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1523 2021-12-28 07:38:48.830707 purgatory-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3410 2023-07-23 15:11:39.521798 purgatory-2.0.0/README.rst
+-rw-r--r--   0        0        0     1518 2024-05-15 06:42:21.907614 purgatory-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1083 2024-05-15 06:32:39.992052 purgatory-2.0.0/src/purgatory/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/domain/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/domain/messages/__init__.py
+-rw-r--r--   0        0        0      304 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/domain/messages/base.py
+-rw-r--r--   0        0        0      221 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/domain/messages/commands.py
+-rw-r--r--   0        0        0      554 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/domain/messages/events.py
+-rw-r--r--   0        0        0     7511 2024-05-15 06:32:39.992052 purgatory-2.0.0/src/purgatory/domain/model.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/py.typed
+-rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/service/_async/__init__.py
+-rw-r--r--   0        0        0     5795 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/service/_async/circuitbreaker.py
+-rw-r--r--   0        0        0     1633 2023-05-10 11:55:56.516868 purgatory-2.0.0/src/purgatory/service/_async/message_handlers.py
+-rw-r--r--   0        0        0     3726 2024-05-15 06:32:39.992052 purgatory-2.0.0/src/purgatory/service/_async/messagebus.py
+-rw-r--r--   0        0        0     4614 2023-05-10 11:55:56.520201 purgatory-2.0.0/src/purgatory/service/_async/repository.py
+-rw-r--r--   0        0        0     1834 2024-05-15 06:32:39.992052 purgatory-2.0.0/src/purgatory/service/_async/unit_of_work.py
+-rw-r--r--   0        0        0      274 2023-05-10 11:55:56.520201 purgatory-2.0.0/src/purgatory/service/_redis.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:42:16.970960 purgatory-2.0.0/src/purgatory/service/_sync/__init__.py
+-rw-r--r--   0        0        0     5663 2024-05-15 06:42:16.970960 purgatory-2.0.0/src/purgatory/service/_sync/circuitbreaker.py
+-rw-r--r--   0        0        0     1573 2024-05-15 06:42:17.617625 purgatory-2.0.0/src/purgatory/service/_sync/message_handlers.py
+-rw-r--r--   0        0        0     3695 2024-05-15 06:42:16.977626 purgatory-2.0.0/src/purgatory/service/_sync/messagebus.py
+-rw-r--r--   0        0        0     4433 2024-05-15 06:42:17.660958 purgatory-2.0.0/src/purgatory/service/_sync/repository.py
+-rw-r--r--   0        0        0     1747 2024-05-15 06:42:16.977626 purgatory-2.0.0/src/purgatory/service/_sync/unit_of_work.py
+-rw-r--r--   0        0        0      946 2024-05-15 06:32:39.995385 purgatory-2.0.0/src/purgatory/service/typing.py
+-rw-r--r--   0        0        0      383 2023-05-10 11:55:56.520201 purgatory-2.0.0/src/purgatory/typing.py
+-rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 purgatory-2.0.0/PKG-INFO
```

### Comparing `purgatory-1.0.3/LICENSE` & `purgatory-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/README.rst` & `purgatory-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/pyproject.toml` & `purgatory-2.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,57 +12,57 @@
 homepage = "https://github.com/mardiros/purgatory"
 license = "BSD-derived"
 name = "purgatory"
 packages = [
   {include = "purgatory", from = "src"},
 ]
 readme = "README.rst"
-version = "1.0.3"
+version = "2.0.0"
 
 [tool.pyright]
 include = ["src"]
 typeCheckingMode = "strict"
 
 [[tool.mypy.overrides]]
 module = "purgatory.*"
 disallow_untyped_defs = true
 disallow_any_generics = true
 
 [tool.poetry.dependencies]
-python = "^3.7"
-redis = {version = "^4.6.0", optional = true}
+python = "^3.8"
+redis = {version = "^5.0.4", optional = true}
 
 [tool.poetry.extras]
-aioredis = ["redis"]  # kept for compat
 redis = ["redis"]
 
+[tool.poetry.group.dev]
+optional = true
+
 [tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
+black = "^24.4.2"
 coverage = {version = "^6.2", extras = ["toml"]}
 flake8 = "^5.0.4"
-furo = "^2022"
+furo = "^2024.5.6"
 isort = "^5.10.1"
+mypy = "^1.4.1"
 pytest = "^7.1.3"
 pytest-asyncio = "^0.21.1"
 pytest-cov = "^4.1.0"
-Sphinx = "^4.3.2"
+redis = "^5.0.4"
+Sphinx = "^7.0.1"
 sphinx-autodoc-typehints = "^1.12.0"
-tomlkit = "^0.12.1"
-unasync = "^0.5.0"
-redis = "^4.6.0"
-mypy = "^1.4.1"
-typing-extensions = "^4.7.1"
+tomlkit = "^0.12.5"
 types-redis = "^4.6.0"
-types-setuptools = "^68.0.0"
+typing-extensions = "^4.7.1"
+unasync = "^0.6.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.coverage.report]
 exclude_lines = [
   "except ImportError:",
-  "except pkg_resources.DistributionNotFound:",
 ]
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `purgatory-1.0.3/src/purgatory/__init__.py` & `purgatory-2.0.0/src/purgatory/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-import pkg_resources
+from importlib import metadata
 
-try:
-    __version__ = pkg_resources.get_distribution("purgatory").version
-except pkg_resources.DistributionNotFound:
-    # read the doc does not support poetry
-    pass
+__version__ = metadata.version("purgatory")
 
 
 from purgatory.domain.messages import Event
 from purgatory.domain.messages.events import (
     CircuitBreakerCreated,
     CircuitBreakerFailed,
     CircuitBreakerRecovered,
```

### Comparing `purgatory-1.0.3/src/purgatory/domain/messages/events.py` & `purgatory-2.0.0/src/purgatory/domain/messages/events.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/src/purgatory/domain/model.py` & `purgatory-2.0.0/src/purgatory/domain/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Circuit breaker state model.
 
 The state model is implemented using the State pattern from the Gang Of Four.
 """
+
 import abc
 import time
 from dataclasses import dataclass
 from types import TracebackType
 from typing import Callable, List, Optional, Tuple, Type, Union, cast
 
 from purgatory.domain.messages.base import Event
```

### Comparing `purgatory-1.0.3/src/purgatory/service/_async/circuitbreaker.py` & `purgatory-2.0.0/src/purgatory/service/_async/circuitbreaker.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/src/purgatory/service/_async/message_handlers.py` & `purgatory-2.0.0/src/purgatory/service/_async/message_handlers.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/src/purgatory/service/_async/messagebus.py` & `purgatory-2.0.0/src/purgatory/service/_async/messagebus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Propagate commands and events to every registered handles.
 
 """
+
 import logging
 from collections import defaultdict
 from typing import Any, Dict, List, Type, TypeVar, cast
 
 from purgatory.domain.messages.base import Command, Event, Message
 
 from ..typing import AsyncCommandHandler, AsyncEventHandler, AsyncMessageHandler
@@ -22,17 +23,17 @@
 
 
 class AsyncMessageRegistry:
     """Store all the handlers for commands an events."""
 
     def __init__(self) -> None:
         self.commands_registry: Dict[Type[Command], AsyncCommandHandler[Command]] = {}
-        self.events_registry: Dict[
-            Type[Event], List[AsyncEventHandler[Event]]
-        ] = defaultdict(list)
+        self.events_registry: Dict[Type[Event], List[AsyncEventHandler[Event]]] = (
+            defaultdict(list)
+        )
 
     def add_listener(
         self, msg_type: Type[Message], callback: AsyncMessageHandler[Any, Any]
     ) -> None:
         if issubclass(msg_type, Command):
             if msg_type in self.commands_registry:
                 raise ConfigurationError(
```

### Comparing `purgatory-1.0.3/src/purgatory/service/_async/repository.py` & `purgatory-2.0.0/src/purgatory/service/_async/repository.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/src/purgatory/service/_async/unit_of_work.py` & `purgatory-2.0.0/src/purgatory/service/_async/unit_of_work.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit of work"""
+
 from __future__ import annotations
 
 import abc
 from types import TracebackType
 from typing import Generator, Optional, Type
 
 from purgatory.domain.messages import Message
```

### Comparing `purgatory-1.0.3/src/purgatory/service/_sync/circuitbreaker.py` & `purgatory-2.0.0/src/purgatory/service/_sync/circuitbreaker.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/src/purgatory/service/_sync/message_handlers.py` & `purgatory-2.0.0/src/purgatory/service/_sync/message_handlers.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/src/purgatory/service/_sync/messagebus.py` & `purgatory-2.0.0/src/purgatory/service/_sync/messagebus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Propagate commands and events to every registered handles.
 
 """
+
 import logging
 from collections import defaultdict
 from typing import Any, Dict, List, Type, TypeVar, cast
 
 from purgatory.domain.messages.base import Command, Event, Message
 
 from ..typing import SyncCommandHandler, SyncEventHandler, SyncMessageHandler
@@ -22,17 +23,17 @@
 
 
 class SyncMessageRegistry:
     """Store all the handlers for commands an events."""
 
     def __init__(self) -> None:
         self.commands_registry: Dict[Type[Command], SyncCommandHandler[Command]] = {}
-        self.events_registry: Dict[
-            Type[Event], List[SyncEventHandler[Event]]
-        ] = defaultdict(list)
+        self.events_registry: Dict[Type[Event], List[SyncEventHandler[Event]]] = (
+            defaultdict(list)
+        )
 
     def add_listener(
         self, msg_type: Type[Message], callback: SyncMessageHandler[Any, Any]
     ) -> None:
         if issubclass(msg_type, Command):
             if msg_type in self.commands_registry:
                 raise ConfigurationError(
```

### Comparing `purgatory-1.0.3/src/purgatory/service/_sync/repository.py` & `purgatory-2.0.0/src/purgatory/service/_sync/repository.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.3/src/purgatory/service/_sync/unit_of_work.py` & `purgatory-2.0.0/src/purgatory/service/_sync/unit_of_work.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit of work"""
+
 from __future__ import annotations
 
 import abc
 from types import TracebackType
 from typing import Generator, Optional, Type
 
 from purgatory.domain.messages import Message
```

### Comparing `purgatory-1.0.3/src/purgatory/service/typing.py` & `purgatory-2.0.0/src/purgatory/service/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Propagate commands and events to every registered handles.
 
 """
+
 import logging
 from typing import Any, Callable, Coroutine, TypeVar, Union
 
 from purgatory.domain.messages.base import Command, Event
 
 from ._async.unit_of_work import AsyncAbstractUnitOfWork
 from ._sync.unit_of_work import SyncAbstractUnitOfWork
```

### Comparing `purgatory-1.0.3/PKG-INFO` & `purgatory-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: purgatory
-Version: 1.0.3
+Version: 2.0.0
 Summary: A circuit breaker implementation for asyncio
 Home-page: https://github.com/mardiros/purgatory
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: aioredis
 Provides-Extra: redis
-Requires-Dist: redis (>=4.6.0,<5.0.0) ; extra == "aioredis" or extra == "redis"
+Requires-Dist: redis (>=5.0.4,<6.0.0) ; extra == "redis"
 Description-Content-Type: text/x-rst
 
 Purgatory
 =========
 
 .. image:: https://github.com/mardiros/purgatory/actions/workflows/gh-pages.yml/badge.svg
    :target: https://mardiros.github.io/purgatory/
```

