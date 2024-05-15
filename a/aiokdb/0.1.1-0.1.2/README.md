# Comparing `tmp/aiokdb-0.1.1.tar.gz` & `tmp/aiokdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokdb-0.1.1.tar", last modified: Tue May 14 08:12:34 2024, max compression
+gzip compressed data, was "aiokdb-0.1.2.tar", last modified: Wed May 15 09:16:52 2024, max compression
```

## Comparing `aiokdb-0.1.1.tar` & `aiokdb-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.108641 aiokdb-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.104641 aiokdb-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.104641 aiokdb-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-14 08:12:24.000000 aiokdb-0.1.1/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 08:12:24.000000 aiokdb-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-14 08:12:24.000000 aiokdb-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-14 08:12:24.000000 aiokdb-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-14 08:12:34.108641 aiokdb-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-14 08:12:24.000000 aiokdb-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.104641 aiokdb-0.1.1/aiokdb/
--rw-r--r--   0 runner    (1001) docker     (127)    29541 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/format.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-14 08:12:24.000000 aiokdb-0.1.1/aiokdb/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.108641 aiokdb-0.1.1/aiokdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-14 08:12:34.000000 aiokdb-0.1.1/aiokdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 08:12:34.000000 aiokdb-0.1.1/aiokdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:12:34.000000 aiokdb-0.1.1/aiokdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 08:12:34.000000 aiokdb-0.1.1/aiokdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-14 08:12:24.000000 aiokdb-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 08:12:24.000000 aiokdb-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:12:34.108641 aiokdb-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:34.108641 aiokdb-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_client_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-14 08:12:24.000000 aiokdb-0.1.1/test/test_serialization_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:16:52.075650 aiokdb-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:16:52.067650 aiokdb-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:16:52.071650 aiokdb-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-15 09:16:45.000000 aiokdb-0.1.2/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-15 09:16:45.000000 aiokdb-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-15 09:16:45.000000 aiokdb-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 09:16:45.000000 aiokdb-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-15 09:16:52.075650 aiokdb-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-15 09:16:45.000000 aiokdb-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:16:52.071650 aiokdb-0.1.2/aiokdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    29938 2024-05-15 09:16:45.000000 aiokdb-0.1.2/aiokdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-15 09:16:45.000000 aiokdb-0.1.2/aiokdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 09:16:45.000000 aiokdb-0.1.2/aiokdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 09:16:45.000000 aiokdb-0.1.2/aiokdb/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-15 09:16:45.000000 aiokdb-0.1.2/aiokdb/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:16:45.000000 aiokdb-0.1.2/aiokdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-15 09:16:45.000000 aiokdb-0.1.2/aiokdb/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-15 09:16:45.000000 aiokdb-0.1.2/aiokdb/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:16:52.075650 aiokdb-0.1.2/aiokdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-15 09:16:52.000000 aiokdb-0.1.2/aiokdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 09:16:52.000000 aiokdb-0.1.2/aiokdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:16:52.000000 aiokdb-0.1.2/aiokdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 09:16:52.000000 aiokdb-0.1.2/aiokdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 09:16:45.000000 aiokdb-0.1.2/check.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-15 09:16:45.000000 aiokdb-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 09:16:45.000000 aiokdb-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 09:16:52.075650 aiokdb-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:16:52.075650 aiokdb-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:16:45.000000 aiokdb-0.1.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-15 09:16:45.000000 aiokdb-0.1.2/test/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-15 09:16:45.000000 aiokdb-0.1.2/test/test_client_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-15 09:16:45.000000 aiokdb-0.1.2/test/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-15 09:16:45.000000 aiokdb-0.1.2/test/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-15 09:16:45.000000 aiokdb-0.1.2/test/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-15 09:16:45.000000 aiokdb-0.1.2/test/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-15 09:16:45.000000 aiokdb-0.1.2/test/test_serialization_examples.py
```

### Comparing `aiokdb-0.1.1/.github/workflows/check.yml` & `aiokdb-0.1.2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/.github/workflows/publish.yml` & `aiokdb-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/.gitignore` & `aiokdb-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/LICENSE` & `aiokdb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/PKG-INFO` & `aiokdb-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pure Python asyncio connector to KDB
 Author-email: Chris Shucksmith <chris@shucksmith.co.uk>
 Project-URL: Homepage, https://github.com/TeaEngineering/aiokdb
 Project-URL: Issues, https://github.com/TeaEngineering/aiokdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -68,12 +68,11 @@
 
 ## Tests
 
 The unit tests in `test/test_rpc.py` will use a real KDB binary to test against (over RPC) if you set `KDB_PYTEST_SERVICE` to a URL of the form `kdb://user:password@hostname:port`, otherwise that test is skipped and they are self contained.
 
 * Formatting with `ruff check .`
 * Formatting with `ruff format .`
-* imports `isort --check --profile black .`
 * Check type annotations with `mypy --strict .`
 * Run `pytest .` in the root directory
```

### Comparing `aiokdb-0.1.1/README.md` & `aiokdb-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,12 +54,11 @@
 
 ## Tests
 
 The unit tests in `test/test_rpc.py` will use a real KDB binary to test against (over RPC) if you set `KDB_PYTEST_SERVICE` to a URL of the form `kdb://user:password@hostname:port`, otherwise that test is skipped and they are self contained.
 
 * Formatting with `ruff check .`
 * Formatting with `ruff format .`
-* imports `isort --check --profile black .`
 * Check type annotations with `mypy --strict .`
 * Run `pytest .` in the root directory
```

### Comparing `aiokdb-0.1.1/aiokdb/__init__.py` & `aiokdb-0.1.2/aiokdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,17 @@
 
     def i(self, i: int) -> "KObj":
         raise self._te()
 
     def j(self, j: int) -> "KObj":
         raise self._te()
 
+    def uu(self, uu: uuid.UUID) -> "KObj":
+        raise self._te()
+
     # atom getters
     def aB(self) -> bool:
         raise self._te()
 
     def aG(self) -> int:
         raise self._te()
 
@@ -322,14 +325,20 @@
 
     def j(self, j: int) -> KObj:
         if self.t not in [-TypeEnum.KJ, -TypeEnum.KP]:
             raise ValueError(f"wrong type {self._tn()} for j()")
         self.data = struct.pack("q", j)
         return self
 
+    def uu(self, uu: uuid.UUID) -> KObj:
+        if self.t not in [-TypeEnum.UU]:
+            raise ValueError(f"wrong type {self._tn()} for uu()")
+        self.data = uu.bytes
+        return self
+
     # atom getters
     def aB(self) -> bool:
         if self.t not in [-TypeEnum.KB]:
             raise ValueError(f"wrong type {self._tn()} for aB")
         return self.aG() == 1
 
     def aG(self) -> int:
@@ -715,21 +724,21 @@
         for i in range(sz):
             obj, offset = _d9_unpackfrom(data, offset)
             self._k.append(obj)
         return self, offset
 
 
 class KUUIDArray(KRangedType):
-    def __init__(self, t: int = TypeEnum.UU) -> None:
+    def __init__(self, t: int = TypeEnum.UU, sz: int = 0, attr: int = 0) -> None:
         super().__init__(TypeEnum.UU)
         self._u: list[uuid.UUID] = []
 
     def _paysz(self) -> int:
         # sum sizes nested ks
-        return 2 + 4 + 8 * len(self._u)
+        return 2 + 4 + 16 * len(self._u)
 
     def _databytes(self) -> bytes:
         parts = [struct.pack("<bBI", self.t, self.attrib, len(self._u))]
         parts.extend(uu.bytes for uu in self._u)
         return b"".join(parts)
 
     def kU(self) -> MutableSequence[uuid.UUID]:
@@ -823,14 +832,18 @@
     return KObjAtom(-TypeEnum.KJ).j(i)
 
 
 def ks(s: str) -> KObj:
     return KSymAtom(-TypeEnum.KS).ss(s)
 
 
+def kuu(uu: uuid.UUID) -> KObj:
+    return KObjAtom(-TypeEnum.UU).uu(uu)
+
+
 # vector constructors
 VECTOR_CONSTUCTORS: dict[TypeEnum, Type[KObj]] = {
     TypeEnum.K: KObjArray,
     TypeEnum.KB: KByteArray,
     TypeEnum.KG: KByteArray,
     TypeEnum.KH: KShortArray,
     TypeEnum.KI: KIntArray,
@@ -977,14 +990,17 @@
         return self.kvalue().kvalue().kK()
 
 
 def krr(msg: str) -> KObj:
     return KSymAtom(TypeEnum.KRR).ss(msg)
 
 
+kNil = ka(TypeEnum.NIL)
+
+
 class KException(Exception):
     pass
 
 
 def xd(kkeys: KObj, kvalues: KObj, sorted: bool = False) -> KDict:
     if sorted:
         return KDict(kkeys, kvalues, TypeEnum.SD)
```

### Comparing `aiokdb-0.1.1/aiokdb/cli.py` & `aiokdb-0.1.2/aiokdb/cli.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/aiokdb/client.py` & `aiokdb-0.1.2/aiokdb/client.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/aiokdb/extras.py` & `aiokdb-0.1.2/aiokdb/extras.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/aiokdb/format.py` & `aiokdb-0.1.2/aiokdb/format.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/aiokdb/server.py` & `aiokdb-0.1.2/aiokdb/server.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/aiokdb/socket.py` & `aiokdb-0.1.2/aiokdb/socket.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/aiokdb.egg-info/PKG-INFO` & `aiokdb-0.1.2/aiokdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pure Python asyncio connector to KDB
 Author-email: Chris Shucksmith <chris@shucksmith.co.uk>
 Project-URL: Homepage, https://github.com/TeaEngineering/aiokdb
 Project-URL: Issues, https://github.com/TeaEngineering/aiokdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -68,12 +68,11 @@
 
 ## Tests
 
 The unit tests in `test/test_rpc.py` will use a real KDB binary to test against (over RPC) if you set `KDB_PYTEST_SERVICE` to a URL of the form `kdb://user:password@hostname:port`, otherwise that test is skipped and they are self contained.
 
 * Formatting with `ruff check .`
 * Formatting with `ruff format .`
-* imports `isort --check --profile black .`
 * Check type annotations with `mypy --strict .`
 * Run `pytest .` in the root directory
```

### Comparing `aiokdb-0.1.1/aiokdb.egg-info/SOURCES.txt` & `aiokdb-0.1.2/aiokdb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 LICENSE
 README.md
+check.sh
 pyproject.toml
 requirements.txt
 .github/workflows/check.yml
 .github/workflows/publish.yml
 aiokdb/__init__.py
 aiokdb/cli.py
 aiokdb/client.py
```

### Comparing `aiokdb-0.1.1/pyproject.toml` & `aiokdb-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/test/test_atoms.py` & `aiokdb-0.1.2/test/test_atoms.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest
 
 from aiokdb import (
     AttrEnum,
     TypeEnum,
     b9,
+    cv,
     d9,
     ka,
     kb,
     kc,
     kg,
     kh,
     ki,
@@ -330,7 +331,45 @@
     k2 = kk(ks("function"), kj(17), ks("XBT"), kb(False))
     assert b9(k) == b9(k2)
 
 
 def test_equals() -> None:
     assert kj(34) == kj(34)
     assert kj(34) != kj(35)
+
+
+def test_table_uuid_str_column() -> None:
+    # x:([envelope_id:"G"$("2d948578-e9d6-79a2-8207-9df7a71f0b3b";"409031f3-b19c-6770-ee84-6e9369c98697")]payload:("abc";"xy");time:2024.05.14D23:13:19.044908000)
+    # envelope_id                         | payload time
+    # ------------------------------------| -------------------------------------
+    # 2d948578-e9d6-79a2-8207-9df7a71f0b3b| "abc"   2024.05.14D23:13:19.044908000
+    # 409031f3-b19c-6770-ee84-6e9369c98697| "xy"    2024.05.14D23:13:19.044908000
+    # -8!x
+    exp = h2b(
+        "0x0100000093000000636200630b0001000000656e76656c6f70655f6964000000010000000200020000002d948578e9d679a282079df7a71f0b3b409031f3b19c6770ee846e9369c986976200630b00020000007061796c6f61640074696d65000000020000000000020000000a00030000006162630a000200000078790c0002000000e013dc291431ac0ae013dc291431ac0a"
+    )
+
+    # keyed table
+    # dictionary with tables for keys and values
+    key_hdr = ktn(TypeEnum.KS).appendS("envelope_id")
+    key_val = ktn(TypeEnum.K)
+    key_val.kK().append(ktn(TypeEnum.UU))
+
+    val_hdr = ktn(TypeEnum.KS).appendS("payload", "time")
+    val_val = ktn(TypeEnum.K)
+    val_val.kK().append(ktn(TypeEnum.K))
+    val_val.kK().append(ktn(TypeEnum.KP))
+    kt = xd(xt(xd(key_hdr, key_val)), xt(xd(val_hdr, val_val)))
+
+    # add items
+    kt.kkey()["envelope_id"].kU().append(
+        uuid.UUID("2d948578-e9d6-79a2-8207-9df7a71f0b3b")
+    )
+    kt.kvalue()["payload"].kK().append(cv("abc"))
+    kt.kvalue()["time"].kJ().append(769043599044908000)
+
+    kt.kkey()["envelope_id"].kU().append(
+        uuid.UUID("409031f3-b19c-6770-ee84-6e9369c98697")
+    )
+    kt.kvalue()["payload"].kK().append(cv("xy"))
+    kt.kvalue()["time"].kJ().append(769043599044908000)
+    assert b9(kt).hex() == exp.hex()
```

### Comparing `aiokdb-0.1.1/test/test_client_server.py` & `aiokdb-0.1.2/test/test_client_server.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/test/test_format.py` & `aiokdb-0.1.2/test/test_format.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/test/test_rpc.py` & `aiokdb-0.1.2/test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `aiokdb-0.1.1/test/test_serialization_examples.py` & `aiokdb-0.1.2/test/test_serialization_examples.py`

 * *Files identical despite different names*

