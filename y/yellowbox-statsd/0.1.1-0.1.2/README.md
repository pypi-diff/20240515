# Comparing `tmp/yellowbox_statsd-0.1.1.tar.gz` & `tmp/yellowbox_statsd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox_statsd-0.1.1.tar", max compression
+gzip compressed data, was "yellowbox_statsd-0.1.2.tar", max compression
```

## Comparing `yellowbox_statsd-0.1.1.tar` & `yellowbox_statsd-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/LICENSE
--rw-r--r--   0        0        0     1597 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      144 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/yellowbox_statsd/__init__.py
--rw-r--r--   0        0        0       22 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/yellowbox_statsd/_version.py
--rw-r--r--   0        0        0     9956 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/yellowbox_statsd/metrics.py
--rw-r--r--   0        0        0     4872 2023-05-24 15:34:25.891606 yellowbox_statsd-0.1.1/yellowbox_statsd/statsd.py
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 yellowbox_statsd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-15 13:13:33.523905 yellowbox_statsd-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1710 2024-05-15 13:13:33.527905 yellowbox_statsd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-05-15 13:13:33.527905 yellowbox_statsd-0.1.2/yellowbox_statsd/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-15 13:13:43.715898 yellowbox_statsd-0.1.2/yellowbox_statsd/_version.py
+-rw-r--r--   0        0        0    10974 2024-05-15 13:13:33.527905 yellowbox_statsd-0.1.2/yellowbox_statsd/metrics.py
+-rw-r--r--   0        0        0     4920 2024-05-15 13:13:33.527905 yellowbox_statsd-0.1.2/yellowbox_statsd/statsd.py
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 yellowbox_statsd-0.1.2/PKG-INFO
```

### Comparing `yellowbox_statsd-0.1.1/LICENSE` & `yellowbox_statsd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox_statsd-0.1.1/pyproject.toml` & `yellowbox_statsd-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 [tool.poetry]
 name = "yellowbox-statsd"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Biocatch LTD <serverteam@biocatch.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 yellowbox = { version = ">=0.7.0" }
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.267"
+ruff = ">=0.0.267"
 pytest = "*"
 pytest-cov = "*"
 mypy = ">=1"
-black = "^23.3.0"
 datadog = "^0.45.0"
+aiodogstatsd = "^0.16.0.post0"
+pytest-asyncio = "^0.21.0"
 
 [tool.ruff]
+line-length = 120
+output-format = "full"
+target-version = "py38"
+[tool.ruff.lint]
 # https://beta.ruff.rs/docs/rules/
 select = ["I", "E", "W", "F", "N", "S", "BLE", "COM", "C4", "ISC", "ICN", "G", "PIE", "T20", "PYI", "Q", "SLF", "SIM",
           "ERA", "PGH", "PLC", "PLE", "PLR", "PLW", "RUF", "PT", "UP", "B"]
 ignore = [
+    "ISC001",  # blocked by formatter
     "COM812",  # trailing comma, handled by black
     "UP035",  # deprecated imports
     "PLR0912", # Too many branches
     "S104",  # Possible binding to all interfaces
 ]
-line-length = 120
-show-source = true
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports=true
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 raises-require-match-for = []
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**" = [
     "PT013",  # Found incorrect import of pytest, use simple `import pytest` instead
     "PT004", # Fixture does not return anything, add leading underscore
     "S101",  # asserts
     "PLR2004", # PLR2004 Magic value used in comparison
     "PLR0913",  # PLR0913 Too many arguments to function call
 ]
 
-[tool.ruff.pyupgrade]
+
+[tool.ruff.lint.pyupgrade]
 # Preserve types, even if a file imports `from __future__ import annotations`.
 keep-runtime-typing = true
 
-[tool.black]
-line-length = 120
-
 [tool.coverage.report]
 precision = 2
 exclude_lines = ["pragma: no cover", "raise NotImplementedError", "raise NotImplemented", "if TYPE_CHECKING:", "@overload"]
```

### Comparing `yellowbox_statsd-0.1.1/yellowbox_statsd/metrics.py` & `yellowbox_statsd-0.1.2/yellowbox_statsd/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import (
     Any,
     ClassVar,
     Dict,
     FrozenSet,
     ItemsView,
     Iterable,
+    Iterator,
     KeysView,
     List,
     Mapping,
     Optional,
     Set,
     Tuple,
     Type,
@@ -114,14 +115,21 @@
             return not tags_to_match
         return tags_to_match.issubset(self.tags)
 
     @classmethod
     def from_metric(cls, metric: Metric) -> CapturedMetric:
         return cls(metric.values, metric.sample_rate, metric.tags, metric.metric_timestamp, metric.container_id)
 
+    def _replace_values(self, values: List[str]) -> CapturedMetric:
+        return type(self)(values, self.sample_rate, self.tags, self.metric_timestamp, self.container_id)
+
+    def unbunch(self) -> Iterator[CapturedMetric]:
+        for v in self.values:
+            yield self._replace_values([v])
+
 
 Self = TypeVar("Self", bound="CapturedMetrics")
 
 
 class CapturedMetrics(List[CapturedMetric]):
     def tags(self) -> Iterable[str]:
         s: Set[str] = set()
@@ -144,20 +152,18 @@
 
     def filter_not(
         self: Self, *extra_tags, tags: Union[Iterable[str], Mapping[str, str]] = (), **extra_tags_assigned
     ) -> Self:
         return type(self)(m for m in self if not m.tags_match(*extra_tags, tags=tags, **extra_tags_assigned))
 
     @overload
-    def split(self: Self, tag: str) -> Dict[Optional[str], Self]:
-        ...
+    def split(self: Self, tag: str) -> Dict[Optional[str], Self]: ...
 
     @overload
-    def split(self: Self, tag: Tuple[str, ...]) -> Dict[Tuple[Optional[str], ...], Self]:
-        ...
+    def split(self: Self, tag: Tuple[str, ...]) -> Dict[Tuple[Optional[str], ...], Self]: ...
 
     def split(self: Self, tag: Union[str, Tuple[str, ...]]) -> Dict[Any, Self]:
         if isinstance(tag, str):
 
             def get_keys(metric: CapturedMetric):
                 return metric.tags.get(tag, ()) if metric.tags is not None else ()
 
@@ -172,14 +178,17 @@
             for key in keys:
                 cm = ret.get(key)
                 if cm is None:
                     cm = ret[key] = type(self)()
                 cm.append(metric)
         return ret
 
+    def unbunch(self: Self) -> Self:
+        return type(self)(chain.from_iterable(m.unbunch() for m in self))
+
 
 class CountCapturedMetric(CapturedMetrics):
     def total(self) -> float:
         return sum(float(v) / (m.sample_rate or 1.0) for m in self for v in m.values)
 
 
 class HistogramCapturedMetric(CapturedMetrics):
@@ -208,14 +217,36 @@
                 addant += float(v[1:])
             elif v.startswith("-"):
                 addant -= float(v[1:])
             else:
                 return float(v) + addant
         return addant
 
+    def values(self) -> Iterator[float]:
+        prev = 0.0
+        for m in self:
+            for v in m.values:
+                if v.startswith("+"):
+                    prev += float(v[1:])
+                elif v.startswith("-"):
+                    prev -= float(v[1:])
+                else:
+                    prev = float(v)
+                yield prev
+
+    def min(self, default: Optional[float] = None) -> float:
+        if default is None:
+            return min(self.values())
+        return min(self.values(), default=default)
+
+    def max(self, default: Optional[float] = None) -> float:
+        if default is None:
+            return max(self.values())
+        return max(self.values(), default=default)
+
 
 class SetCapturedMetric(CapturedMetrics):
     def unique(self) -> Set[float]:
         return {float(v) for m in self for v in m.values}
 
 
 class CapturedMetricsCollection(Dict[Tuple[str, str], CapturedMetrics]):
@@ -247,48 +278,38 @@
             else:
                 raise
 
     def count(self, name: str) -> CountCapturedMetric:
         return self[name, "c"]  # type: ignore[return-value]
 
     def get_count(self, name: str, tags=(), **tags_kwargs) -> CountCapturedMetric:
-        return self.get((name, "c"), CountCapturedMetric()).filter(
-            tags=tags, **tags_kwargs
-        )  # type: ignore[return-value]
+        return self.get((name, "c"), CountCapturedMetric()).filter(tags=tags, **tags_kwargs)  # type: ignore[return-value]
 
     def gauge(self, name: str) -> GaugeCapturedMetric:
         return self[name, "g"]  # type: ignore[return-value]
 
     def get_gauge(self, name: str, tags=(), **tags_kwargs) -> GaugeCapturedMetric:
-        return self.get((name, "g"), GaugeCapturedMetric()).filter(
-            tags=tags, **tags_kwargs
-        )  # type: ignore[return-value]
+        return self.get((name, "g"), GaugeCapturedMetric()).filter(tags=tags, **tags_kwargs)  # type: ignore[return-value]
 
     def histogram(self, name: str) -> HistogramCapturedMetric:
         return self[name, "h"]  # type: ignore[return-value]
 
     def get_histogram(self, name: str, tags=(), **tags_kwargs) -> HistogramCapturedMetric:
-        return self.get((name, "h"), HistogramCapturedMetric()).filter(
-            tags=tags, **tags_kwargs
-        )  # type: ignore[return-value]
+        return self.get((name, "h"), HistogramCapturedMetric()).filter(tags=tags, **tags_kwargs)  # type: ignore[return-value]
 
     def set(self, name: str) -> SetCapturedMetric:
         return self[name, "s"]  # type: ignore[return-value]
 
     def get_set(self, name: str, tags=(), **tags_kwargs) -> SetCapturedMetric:
         return self.get((name, "s"), SetCapturedMetric()).filter(tags=tags, **tags_kwargs)  # type: ignore[return-value]
 
     def timing(self, name: str) -> HistogramCapturedMetric:
         return self[name, "ms"]  # type: ignore[return-value]
 
     def get_timing(self, name: str, tags=(), **tags_kwargs) -> HistogramCapturedMetric:
-        return self.get((name, "ms"), HistogramCapturedMetric()).filter(
-            tags=tags, **tags_kwargs
-        )  # type: ignore[return-value]
+        return self.get((name, "ms"), HistogramCapturedMetric()).filter(tags=tags, **tags_kwargs)  # type: ignore[return-value]
 
     def distribution(self, name: str) -> HistogramCapturedMetric:
         return self[name, "d"]  # type: ignore[return-value]
 
     def get_distribution(self, name: str, tags=(), **tags_kwargs) -> HistogramCapturedMetric:
-        return self.get((name, "d"), HistogramCapturedMetric()).filter(
-            tags=tags, **tags_kwargs
-        )  # type: ignore[return-value]
+        return self.get((name, "d"), HistogramCapturedMetric()).filter(tags=tags, **tags_kwargs)  # type: ignore[return-value]
```

### Comparing `yellowbox_statsd-0.1.1/yellowbox_statsd/statsd.py` & `yellowbox_statsd-0.1.2/yellowbox_statsd/statsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import platform
 import subprocess
 from collections.abc import Callable
 from contextlib import contextmanager
+from os import getenv
 from socket import AF_INET, SOCK_DGRAM, socket, timeout
 from threading import Thread
 from traceback import print_exc
 from typing import Any, Iterator, List, Set
 
 from yellowbox import YellowService
 from yellowbox.utils import docker_host_name
@@ -40,15 +41,14 @@
         self.listening_thread.start()
         return super().start()
 
     def stop(self):
         self.should_stop = True
         self.listening_thread.join()
         self.sock.close()
-        return super().stop()
 
     def is_alive(self):
         return self.sock is not None
 
     def add_metric_callback(self, callback: Callable[[Metric], Any]) -> None:
         self.metric_callbacks.add(callback)
 
@@ -103,18 +103,18 @@
                         metric_callback(metric)
                     except Exception:  # noqa: BLE001
                         print("unexpected error when calling message callback")  # noqa: T201
                         print_exc()
 
     def container_host(self):
         uname = platform.uname().release.lower()
-        if ("microsoft" in uname) and ("wsl2" in uname):
+        if ("microsoft" in uname) and ("wsl2" in uname) and not getenv("YB_STATSD_CONTAINER_HOST"):
             # udp mirroring is not supported in wsl2 yet
             # https://github.com/microsoft/WSL/issues/4825
-            # the inference mechanism here can by bypassed by setting the env var YB_STATSD_CONTAINER_HOST
+            # the inference mechanism here can by bypassed by setting the env var YB_STATSD_CONTAINER_HOST to any value
 
             try:
                 proc = subprocess.run(
                     ["/usr/bin/sh", "-c", r'''ip addr show eth0 | grep -oP "(?<=inet\s)\d+(\.\d+){3}"'''],  # noqa: S603
                     capture_output=True,
                     check=True,
                 )
```

### Comparing `yellowbox_statsd-0.1.1/PKG-INFO` & `yellowbox_statsd-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: yellowbox-statsd
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: Biocatch LTD
 Author-email: serverteam@biocatch.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: yellowbox (>=0.7.0)
```

