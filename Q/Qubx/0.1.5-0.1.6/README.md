# Comparing `tmp/qubx-0.1.5.tar.gz` & `tmp/qubx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubx-0.1.5.tar", max compression
+gzip compressed data, was "qubx-0.1.6.tar", max compression
```

## Comparing `qubx-0.1.5.tar` & `qubx-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.5/README.md
--rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.5/build.py
--rw-r--r--   0        0        0     1378 2024-05-12 17:27:41.499398 qubx-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/__init__.py
--rw-r--r--   0        0        0     1875 2024-05-12 17:27:41.499398 qubx-0.1.5/src/qubx/_nb_magic.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/core/__init__.py
--rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.5/src/qubx/core/account.py
--rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/core/basics.py
--rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/core/helpers.py
--rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/core/loggers.py
--rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/core/lookups.py
--rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/core/series.pxd
--rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/core/series.pyx
--rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/core/strategy.py
--rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/core/utils.pyx
--rw-r--r--   0        0        0    19648 2024-05-08 18:11:34.565668 qubx-0.1.5/src/qubx/data/readers.py
--rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/impl/ccxt_connector.py
--rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/impl/ccxt_customizations.py
--rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/impl/ccxt_trading.py
--rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/impl/ccxt_utils.py
--rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/math/__init__.py
--rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/math/stats.py
--rw-r--r--   0        0        0      175 2024-05-12 17:27:41.499398 qubx-0.1.5/src/qubx/pandaz/__init__.py
--rw-r--r--   0        0        0    85271 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/pandaz/ta.py
--rw-r--r--   0        0        0    19109 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/pandaz/utils.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/ta/__init__.py
--rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/ta/indicators.pyx
--rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/trackers/__init__.py
--rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/trackers/rebalancers.py
--rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.5/src/qubx/utils/__init__.py
--rw-r--r--   0        0        0    12076 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/utils/_pyxreloader.py
--rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.5/src/qubx/utils/charting/mpl_helpers.py
--rw-r--r--   0        0        0    10993 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/utils/marketdata/binance.py
--rw-r--r--   0        0        0     9831 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/utils/misc.py
--rw-r--r--   0        0        0     9306 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/utils/runner.py
--rw-r--r--   0        0        0     4884 2024-05-07 13:17:10.569607 qubx-0.1.5/src/qubx/utils/time.py
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 qubx-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.6/README.md
+-rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.6/build.py
+-rw-r--r--   0        0        0     1555 2024-05-14 18:46:30.086224 qubx-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.6/src/qubx/__init__.py
+-rw-r--r--   0        0        0     1875 2024-05-12 17:27:41.499398 qubx-0.1.6/src/qubx/_nb_magic.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.6/src/qubx/core/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.6/src/qubx/core/account.py
+-rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.6/src/qubx/core/basics.py
+-rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.6/src/qubx/core/helpers.py
+-rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.6/src/qubx/core/loggers.py
+-rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.6/src/qubx/core/lookups.py
+-rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.6/src/qubx/core/series.pxd
+-rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.6/src/qubx/core/series.pyx
+-rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.6/src/qubx/core/strategy.py
+-rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.6/src/qubx/core/utils.pyx
+-rw-r--r--   0        0        0    21310 2024-05-14 18:44:12.292214 qubx-0.1.6/src/qubx/data/readers.py
+-rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.6/src/qubx/impl/ccxt_connector.py
+-rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.6/src/qubx/impl/ccxt_customizations.py
+-rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.6/src/qubx/impl/ccxt_trading.py
+-rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.6/src/qubx/impl/ccxt_utils.py
+-rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.6/src/qubx/math/__init__.py
+-rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.6/src/qubx/math/stats.py
+-rw-r--r--   0        0        0      175 2024-05-12 17:27:41.499398 qubx-0.1.6/src/qubx/pandaz/__init__.py
+-rw-r--r--   0        0        0    85271 2024-05-12 17:27:41.503398 qubx-0.1.6/src/qubx/pandaz/ta.py
+-rw-r--r--   0        0        0    19109 2024-05-12 17:27:41.503398 qubx-0.1.6/src/qubx/pandaz/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.6/src/qubx/ta/__init__.py
+-rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.6/src/qubx/ta/indicators.pyx
+-rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.6/src/qubx/trackers/__init__.py
+-rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.6/src/qubx/trackers/rebalancers.py
+-rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.6/src/qubx/utils/__init__.py
+-rw-r--r--   0        0        0    12017 2024-05-14 18:44:12.292214 qubx-0.1.6/src/qubx/utils/_pyxreloader.py
+-rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.6/src/qubx/utils/charting/mpl_helpers.py
+-rw-r--r--   0        0        0    10993 2024-05-12 17:27:41.503398 qubx-0.1.6/src/qubx/utils/marketdata/binance.py
+-rw-r--r--   0        0        0     9831 2024-05-12 17:27:41.503398 qubx-0.1.6/src/qubx/utils/misc.py
+-rw-r--r--   0        0        0     9306 2024-05-12 17:27:41.503398 qubx-0.1.6/src/qubx/utils/runner.py
+-rw-r--r--   0        0        0     4911 2024-05-14 18:44:12.292214 qubx-0.1.6/src/qubx/utils/time.py
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 qubx-0.1.6/PKG-INFO
```

### Comparing `qubx-0.1.5/README.md` & `qubx-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/build.py` & `qubx-0.1.6/build.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/pyproject.toml` & `qubx-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Qubx"
-version = "0.1.5"
+version = "0.1.6"
 description = "Qubx - quantitative trading framework"
 authors = ["Dmitry Marienko <dmitry@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "qubx", from = "src" },
 ]
 repository = "https://github.com/dmarienko/Qubx"
@@ -29,14 +29,23 @@
 python-binance = "^1.0.19"
 pyarrow = "^15.0.0"
 scipy = "^1.12.0"
 cython = "3.0.8"
 ccxt = "^4.2.68"
 croniter = "^2.0.5"
 psycopg = "^3.1.18"
+pandas = "^2.2.2"
+statsmodels = "^0.14.2"
+matplotlib = "^3.8.4"
+numba = "^0.59.1"
+scikit-learn = "^1.4.2"
+plotly = "^5.22.0"
+psycopg-binary = "^3.1.19"
+psycopg-pool = "^3.2.2"
+
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 pytest = "^7.1.3"
 
 #[project.optional-dependencies]
 #numba = "^0.57.1"
```

### Comparing `qubx-0.1.5/src/qubx/__init__.py` & `qubx-0.1.6/src/qubx/__init__.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/_nb_magic.py` & `qubx-0.1.6/src/qubx/_nb_magic.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/account.py` & `qubx-0.1.6/src/qubx/core/account.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/basics.py` & `qubx-0.1.6/src/qubx/core/basics.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/helpers.py` & `qubx-0.1.6/src/qubx/core/helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/loggers.py` & `qubx-0.1.6/src/qubx/core/loggers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/lookups.py` & `qubx-0.1.6/src/qubx/core/lookups.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/series.pxd` & `qubx-0.1.6/src/qubx/core/series.pxd`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/series.pyx` & `qubx-0.1.6/src/qubx/core/series.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/strategy.py` & `qubx-0.1.6/src/qubx/core/strategy.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/core/utils.pyx` & `qubx-0.1.6/src/qubx/core/utils.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/data/readers.py` & `qubx-0.1.6/src/qubx/data/readers.py`

 * *Files 8% similar despite different names*

```diff
@@ -461,53 +461,103 @@
 
     @_retry
     def read(self, data_id: str, start: str|None=None, stop: str|None=None, 
              transform: DataTransformer = DataTransformer(),
              chunksize=0,  # TODO: use self._cursor.fetchmany in this case !!!!
              timeframe: str='1m') -> Any:
         start, end = handle_start_stop(start, stop)
-        w0 = f"timestamp >= '{start}'" if start else ''
-        w1 = f"timestamp <= '{end}'" if end else ''
-        where = f'where {w0} and {w1}' if (w0 and w1) else f"where {(w0 or w1)}"
+        _req = self._prepare_data_sql(data_id, start, end, timeframe)
+
+        self._cursor.execute(_req) # type: ignore
+        records = self._cursor.fetchall() # TODO: for chunksize > 0 use fetchmany etc
+
+        names = [d.name for d in self._cursor.description] # type: ignore
+        transform.start_transform(data_id, names)
+
+        transform.process_data(records)
+        return transform.collect()
 
+    def _prepare_data_sql(self, data_id: str, start: str|None, end: str|None, resample: str) -> str:
         # just a temp hack - actually we need to discuss symbology etc
         symbol = data_id#.split('.')[-1]
 
-        self._cursor.execute(
-            f"""
+        w0 = f"timestamp >= '{start}'" if start else ''
+        w1 = f"timestamp <= '{end}'" if end else ''
+        where = f'where {w0} and {w1}' if (w0 and w1) else f"where {(w0 or w1)}"
+
+        return f"""
                 select timestamp, 
                 first(open) as open, 
                 max(high) as high,
                 min(low) as low,
                 last(close) as close,
                 sum(volume) as volume,
                 sum(quote_volume) as quote_volume,
                 sum(count) as count,
                 sum(taker_buy_volume) as taker_buy_volume,
                 sum(taker_buy_quote_volume) as taker_buy_quote_volume
                 from "{symbol.upper()}" {where}
-                SAMPLE by {timeframe};
-            """ # type: ignore
-        )
-        records = self._cursor.fetchall() # TODO: for chunksize > 0 use fetchmany etc
-        names = [d.name for d in self._cursor.description]
+                SAMPLE by {resample};
+            """ 
 
-        transform.start_transform(data_id, names)
-        
-        # d = np.array(records)
-        transform.process_data(records)
-        return transform.collect()
+    def _prepare_names_sql(self) -> str:
+        return "select table_name from tables()"
 
     @_retry
     def get_names(self) -> List[str] :
-        self._cursor.execute("select table_name from tables()")
+        self._cursor.execute(self._prepare_names_sql()) # type: ignore
         records = self._cursor.fetchall()
         return [r[0] for r in records]
 
     def __del__(self):
         for c in (self._cursor, self._connection):
             try:
                 logger.info("Closing connection")
                 c.close()
             except:
                 pass
 
+
+class SnapshotsBuilder(DataTransformer):
+    """
+    Snapshots assembler from OB updates
+    """
+    def __init__(self, 
+                 levels: int=-1,     # how many levels restore, 1 - TOB, -1 - all
+                 as_frame=False      # result is dataframe
+    ):
+        self.buffer = []
+        self.levels = levels
+        self.as_frame = as_frame
+
+    def start_transform(self, name: str, column_names: List[str]):
+        # initialize buffer / series etc
+        # let's keep restored snapshots into some buffer etc
+        self.buffer = []
+
+        # do additional init stuff here
+
+    def process_data(self, rows_data:List[List]) -> Any:
+        for r in rows_data:
+            # restore snapshots and put into buffer or series
+            pass
+
+    def collect(self) -> Any:
+        # - may be convert it to pandas DataFrame ?
+        if self.as_frame:
+            return pd.DataFrame.from_records(self.buffer) # or custom transform
+
+        # - or just returns as plain list
+        return self.buffer
+
+
+class QuestDBOrderBookConnector(QuestDBConnector):
+    """
+    Example of custom OrderBook data connector 
+    """
+
+    def _prepare_data_sql(self, data_id: str, start: str|None, end: str|None, resample: str|None) -> str:
+        raise NotImplemented("TODO")
+
+    def _prepare_names_sql(self) -> str:
+        # return "select table_name from tables() where ..."
+        raise NotImplemented("TODO")
```

### Comparing `qubx-0.1.5/src/qubx/impl/ccxt_connector.py` & `qubx-0.1.6/src/qubx/impl/ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/impl/ccxt_customizations.py` & `qubx-0.1.6/src/qubx/impl/ccxt_customizations.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/impl/ccxt_trading.py` & `qubx-0.1.6/src/qubx/impl/ccxt_trading.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/impl/ccxt_utils.py` & `qubx-0.1.6/src/qubx/impl/ccxt_utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/math/stats.py` & `qubx-0.1.6/src/qubx/math/stats.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/pandaz/ta.py` & `qubx-0.1.6/src/qubx/pandaz/ta.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/pandaz/utils.py` & `qubx-0.1.6/src/qubx/pandaz/utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/ta/indicators.pyx` & `qubx-0.1.6/src/qubx/ta/indicators.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/trackers/rebalancers.py` & `qubx-0.1.6/src/qubx/trackers/rebalancers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/utils/_pyxreloader.py` & `qubx-0.1.6/src/qubx/utils/_pyxreloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 
 import importlib, glob, os, sys
 from importlib.abc import MetaPathFinder
 from importlib.util import spec_from_file_location
 from importlib.machinery import ExtensionFileLoader, SourceFileLoader
 from typing import List
 
-# - disable warn about deprecation of imp module: after dev stage _pyxreloader will be removed
-import warnings
-warnings.filterwarnings("ignore", category=DeprecationWarning)
-import imp
 
 PYX_EXT = ".pyx"
 PYXDEP_EXT = ".pyxdep"
 PYXBLD_EXT = ".pyxbld"
 
 
 def handle_dependencies(pyxfilename):
@@ -45,14 +41,18 @@
             if newer(file, pyxfilename):
                 print("Rebuilding %s because of %s", pyxfilename, file)
                 filetime = os.path.getmtime(file)
                 os.utime(pyxfilename, (filetime, filetime))
 
 
 def handle_special_build(modname, pyxfilename):
+    try:
+        import imp
+    except:
+        return None, None
     special_build = os.path.splitext(pyxfilename)[0] + PYXBLD_EXT
     ext = None
     setup_args={}
     if os.path.exists(special_build):
         # globls = {}
         # locs = {}
         # execfile(special_build, globls, locs)
@@ -132,14 +132,18 @@
                 print("Couldn't remove %s", path)
 
     return so_path
 
 
 def load_module(name, pyxfilename, pyxbuild_dir=None, is_package=False, build_inplace=False, language_level=None, so_path=None):
     try:
+        import imp
+    except:
+        return None
+    try:
         if so_path is None:
             if is_package:
                 module_name = name + '.__init__'
             else:
                 module_name = name
             so_path = build_module(module_name, pyxfilename, pyxbuild_dir, inplace=build_inplace, language_level=language_level)
         mod = imp.load_dynamic(name, so_path)
```

### Comparing `qubx-0.1.5/src/qubx/utils/charting/mpl_helpers.py` & `qubx-0.1.6/src/qubx/utils/charting/mpl_helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/utils/marketdata/binance.py` & `qubx-0.1.6/src/qubx/utils/marketdata/binance.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/utils/misc.py` & `qubx-0.1.6/src/qubx/utils/misc.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/utils/runner.py` & `qubx-0.1.6/src/qubx/utils/runner.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.5/src/qubx/utils/time.py` & `qubx-0.1.6/src/qubx/utils/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import List, Optional, Union
+from typing import List, Optional, Tuple, Union
 import numpy as np
 import re
 
 import pandas as pd
 
 UNIX_T0 = np.datetime64('1970-01-01T00:00:00')
 
@@ -111,15 +111,15 @@
     values = np.array(sorted([(x if isinstance(x, np.timedelta64) else int(1e9 * x.total_seconds())) for x in np.abs(np.diff(times_index))]))
     diff = np.concatenate(([1], np.diff(values)))
     idx = np.concatenate((np.where(diff)[0], [len(values)]))
     freqs = dict(zip(values[idx[:-1]], np.diff(idx)))
     return np.timedelta64(max(freqs, key=freqs.get))
 
 
-def handle_start_stop(s: Optional[str], e: Optional[str], convert=str) -> tuple:
+def handle_start_stop(s: Optional[str], e: Optional[str], convert=str) -> Tuple[str|None, str|None]:
     """
     Process start/stop times
 
         handle_start_stop('2020-01-01', '2020-02-01') # 2020-01-01, 2020-02-01
         handle_start_stop('2020-02-01', '2020-01-01') # 2020-01-01, 2020-02-01
         handle_start_stop('2020-01-01', '1w')         # 2020-01-01, 2020-01-01 + 1week
         handle_start_stop('1w', '2020-01-01')         # 2020-01-01 - 1week, '2020-01-01'
```

### Comparing `qubx-0.1.5/PKG-INFO` & `qubx-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: Qubx
-Version: 0.1.5
+Version: 0.1.6
 Summary: Qubx - quantitative trading framework
 Home-page: https://github.com/dmarienko/Qubx
 Author: Dmitry Marienko
 Author-email: dmitry@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ccxt (>=4.2.68,<5.0.0)
 Requires-Dist: croniter (>=2.0.5,<3.0.0)
 Requires-Dist: cython (==3.0.8)
 Requires-Dist: importlib-metadata
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: ntplib (>=0.4.0,<0.5.0)
+Requires-Dist: numba (>=0.59.1,<0.60.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: plotly (>=5.22.0,<6.0.0)
 Requires-Dist: psycopg (>=3.1.18,<4.0.0)
+Requires-Dist: psycopg-binary (>=3.1.19,<4.0.0)
+Requires-Dist: psycopg-pool (>=3.2.2,<4.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pymongo (>=4.6.1,<5.0.0)
 Requires-Dist: pytest[lazyfixture] (>=7.2.0,<8.0.0)
 Requires-Dist: python-binance (>=1.0.19,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: stackprinter (>=0.2.10,<0.3.0)
+Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/dmarienko/Qubx
 Description-Content-Type: text/markdown
 
 # Qubx
 
 ## Next generation of Qube quantitative backtesting framework (QUBX)
```

