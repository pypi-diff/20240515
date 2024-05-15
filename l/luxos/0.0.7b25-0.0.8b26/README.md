# Comparing `tmp/luxos-0.0.7b25.tar.gz` & `tmp/luxos-0.0.8b26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.7b25.tar", last modified: Fri May 10 16:43:08 2024, max compression
+gzip compressed data, was "luxos-0.0.8b26.tar", last modified: Wed May 15 14:35:56 2024, max compression
```

## Comparing `luxos-0.0.7b25.tar` & `luxos-0.0.8b26.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:43:08.040315 luxos-0.0.7b25/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-10 16:43:08.040315 luxos-0.0.7b25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-10 16:42:37.000000 luxos-0.0.7b25/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-10 16:43:06.000000 luxos-0.0.7b25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:43:08.040315 luxos-0.0.7b25/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:43:08.032316 luxos-0.0.7b25/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:43:08.036316 luxos-0.0.7b25/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 16:43:06.000000 luxos-0.0.7b25/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:43:08.040315 luxos-0.0.7b25/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:43:08.040315 luxos-0.0.7b25/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/scripts/luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-10 16:42:37.000000 luxos-0.0.7b25/src/luxos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:43:08.040315 luxos-0.0.7b25/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-10 16:43:08.000000 luxos-0.0.7b25/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-10 16:43:08.000000 luxos-0.0.7b25/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:43:08.000000 luxos-0.0.7b25/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 16:43:08.000000 luxos-0.0.7b25/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 16:43:08.000000 luxos-0.0.7b25/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 16:43:08.000000 luxos-0.0.7b25/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:43:08.040315 luxos-0.0.7b25/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-10 16:42:37.000000 luxos-0.0.7b25/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-10 16:42:37.000000 luxos-0.0.7b25/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-10 16:42:37.000000 luxos-0.0.7b25/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 16:42:37.000000 luxos-0.0.7b25/tests/test_luxos_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-10 16:42:37.000000 luxos-0.0.7b25/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-10 16:42:37.000000 luxos-0.0.7b25/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.927947 luxos-0.0.8b26/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-15 14:35:56.927947 luxos-0.0.8b26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-15 14:35:24.000000 luxos-0.0.8b26/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-15 14:35:54.000000 luxos-0.0.8b26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:35:56.927947 luxos-0.0.8b26/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.919947 luxos-0.0.8b26/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.923947 luxos-0.0.8b26/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 14:35:54.000000 luxos-0.0.8b26/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.923947 luxos-0.0.8b26/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.923947 luxos-0.0.8b26/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.927947 luxos-0.0.8b26/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.927947 luxos-0.0.8b26/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_utils.py
```

### Comparing `luxos-0.0.7b25/PKG-INFO` & `luxos-0.0.8b26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.7b25
+Version: 0.0.8b26
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.7b25/README.md` & `luxos-0.0.8b26/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/pyproject.toml` & `luxos-0.0.8b26/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.7b25"
+version = "0.0.8b26"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.7b25/src/luxos/api.json` & `luxos-0.0.8b26/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/api.py` & `luxos-0.0.8b26/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/asyncops.py` & `luxos-0.0.8b26/src/luxos/asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/cli/v1.py` & `luxos-0.0.8b26/src/luxos/cli/v1.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/exceptions.py` & `luxos-0.0.8b26/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/misc.py` & `luxos-0.0.8b26/src/luxos/misc.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,28 +13,32 @@
         if n < 1:
             raise ValueError("n must be at least one")
         it = iter(iterable)
         while batch := tuple(itertools.islice(it, n)):
             yield batch
 
 
-def iter_ip_ranges(txt: str) -> Generator[str, None, None]:
+def iter_ip_ranges(
+    txt: str, gsep: str = ":", rsep: str = "-"
+) -> Generator[str, None, None]:
     """iterate over ip ranges
 
     for ip in iter_ip_ranges("127.0.0.1-127.0.0.3:127.0.0.15"):
         print(ip)
 
     127.0.0.1
     127.0.0.2
     127.0.0.3
     127.0.0.15
+
+    NOTE: use the `:` (gsep) to separate ips groups, and `-` (rsep) to define a range.
     """
 
-    for segment in txt.split(":"):
-        start, _, end = segment.partition("-")
+    for segment in txt.split(gsep):
+        start, _, end = segment.partition(rsep)
         if not end:
             yield start
         else:
             cur = ipaddress.IPv4Address(start)
             last = ipaddress.IPv4Address(end)
             while cur <= last:
                 yield str(cur)
```

### Comparing `luxos-0.0.7b25/src/luxos/scripts/async_luxos.py` & `luxos-0.0.8b26/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/scripts/health_checker.py` & `luxos-0.0.8b26/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/scripts/luxos.py` & `luxos-0.0.8b26/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/text.py` & `luxos-0.0.8b26/src/luxos/text.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/src/luxos/utils.py` & `luxos-0.0.8b26/src/luxos/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,33 @@
 from pathlib import Path
 from typing import Any, Callable
 
 from luxos.asyncops import rexec  # noqa: F401
 import luxos.misc
 
 
+def ip_ranges(txt: str, gsep: str = ":", rsep: str = "-") -> list[str]:
+    """return a list of ips given a text expression.
+
+    Eg.
+        >>> for ip in ip_ranges("127.0.0.1"):
+        ...     print(ip)
+        127.0.0.1
+
+        >>> for ip in ip_ranges("127.0.0.1-127.0.0.3"):
+        ...     print(ip)
+        127.0.0.1
+        127.0.0.2
+        127.0.0.3
+
+    NOTE: use the `:` (gsep) to separate ips groups, and `-` (rsep) to define a range.
+    """
+    return list(luxos.misc.iter_ip_ranges(txt, gsep, rsep))
+
+
 def load_ips_from_csv(path: Path | str, port: int = 4028) -> list[tuple[str, int]]:
     from luxos.scripts.luxos import load_ip_list_from_csv
 
     result = []
     for ip in load_ip_list_from_csv(str(path)):
         result.append((ip, port))
     return result
```

### Comparing `luxos-0.0.7b25/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.8b26/src/luxos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.7b25
+Version: 0.0.8b26
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.7b25/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.8b26/src/luxos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 src/luxos.egg-info/top_level.txt
 src/luxos/cli/__init__.py
 src/luxos/cli/v1.py
 src/luxos/scripts/__init__.py
 src/luxos/scripts/async_luxos.py
 src/luxos/scripts/health_checker.py
 src/luxos/scripts/luxos.py
+tests/test_asyncops.py
 tests/test_cli.py
 tests/test_luxos.py
-tests/test_luxos_asyncops.py
-tests/test_luxos_misc.py
+tests/test_misc.py
 tests/test_text.py
 tests/test_utils.py
```

### Comparing `luxos-0.0.7b25/tests/test_cli.py` & `luxos-0.0.8b26/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/tests/test_luxos_asyncops.py` & `luxos-0.0.8b26/tests/test_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/tests/test_luxos_misc.py` & `luxos-0.0.8b26/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/tests/test_text.py` & `luxos-0.0.8b26/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b25/tests/test_utils.py` & `luxos-0.0.8b26/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,7 +87,22 @@
     addresses = [(index, None) for index in range(10_000)]
     expected = {
         f"received by ('{host}', {port}): hello world {index}" for index, _ in addresses
     }
 
     ret = await utils.launch(addresses, call, batch=100)
     assert set(ret) == expected
+
+
+def test_util_ip_ranges():
+    assert set(utils.ip_ranges("127.0.0.1")) == {"127.0.0.1"}
+    assert set(utils.ip_ranges("127.0.0.1->127.0.0.3", gsep="\n", rsep="->")) == {
+        "127.0.0.1",
+        "127.0.0.2",
+        "127.0.0.3",
+    }
+    assert set(utils.ip_ranges("127.0.0.1-127.0.0.3\n127.0.0.15", gsep="\n")) == {
+        "127.0.0.1",
+        "127.0.0.2",
+        "127.0.0.3",
+        "127.0.0.15",
+    }
```

