# Comparing `tmp/mediajson-2.2.1.tar.gz` & `tmp/mediajson-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediajson-2.2.1.tar", last modified: Tue Nov 14 16:10:36 2023, max compression
+gzip compressed data, was "mediajson-2.3.0.tar", last modified: Wed May 15 14:38:41 2024, max compression
```

## Comparing `mediajson-2.2.1.tar` & `mediajson-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 16:10:36.835361 mediajson-2.2.1/
--rw-r--r--   0 root         (0) root         (0)      557 2023-11-14 16:09:21.000000 mediajson-2.2.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       90 2023-11-14 16:09:21.000000 mediajson-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      602 2023-11-14 16:09:21.000000 mediajson-2.2.1/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      560 2023-11-14 16:10:36.835361 mediajson-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2647 2023-11-14 16:09:21.000000 mediajson-2.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 16:10:36.831361 mediajson-2.2.1/mediajson/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-11-14 16:09:21.000000 mediajson-2.2.1/mediajson/__init__.py
--rw-r--r--   0 root         (0) root         (0)       98 2023-11-14 16:10:29.000000 mediajson-2.2.1/mediajson/_version.py
--rw-r--r--   0 root         (0) root         (0)     3576 2023-11-14 16:09:21.000000 mediajson-2.2.1/mediajson/decode.py
--rw-r--r--   0 root         (0) root         (0)     3567 2023-11-14 16:09:21.000000 mediajson-2.2.1/mediajson/encode.py
--rw-r--r--   0 root         (0) root         (0)     1151 2023-11-14 16:09:21.000000 mediajson-2.2.1/mediajson/immutable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-14 16:09:21.000000 mediajson-2.2.1/mediajson/py.typed
--rw-r--r--   0 root         (0) root         (0)     3644 2023-11-14 16:09:21.000000 mediajson-2.2.1/mediajson/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 16:10:36.831361 mediajson-2.2.1/mediajson.egg-info/
--rw-r--r--   0 root         (0) root         (0)      560 2023-11-14 16:10:36.000000 mediajson-2.2.1/mediajson.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2023-11-14 16:10:36.000000 mediajson-2.2.1/mediajson.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-14 16:10:36.000000 mediajson-2.2.1/mediajson.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-11-14 16:10:36.000000 mediajson-2.2.1/mediajson.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-11-14 16:10:36.000000 mediajson-2.2.1/mediajson.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-14 16:10:36.835361 mediajson-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1545 2023-11-14 16:09:21.000000 mediajson-2.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-14 16:10:36.835361 mediajson-2.2.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-14 16:09:21.000000 mediajson-2.2.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-11-14 16:09:21.000000 mediajson-2.2.1/tests/test_decode.py
--rw-r--r--   0 root         (0) root         (0)     4980 2023-11-14 16:09:21.000000 mediajson-2.2.1/tests/test_encode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:38:41.022322 mediajson-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)      557 2024-05-15 14:36:56.000000 mediajson-2.3.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-15 14:36:56.000000 mediajson-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      602 2024-05-15 14:36:56.000000 mediajson-2.3.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      560 2024-05-15 14:38:41.022322 mediajson-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-05-15 14:36:56.000000 mediajson-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:38:41.018322 mediajson-2.3.0/mediajson/
+-rw-r--r--   0 root         (0) root         (0)     1414 2024-05-15 14:36:56.000000 mediajson-2.3.0/mediajson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       98 2024-05-15 14:38:32.000000 mediajson-2.3.0/mediajson/_version.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2024-05-15 14:36:56.000000 mediajson-2.3.0/mediajson/decode.py
+-rw-r--r--   0 root         (0) root         (0)     3567 2024-05-15 14:36:56.000000 mediajson-2.3.0/mediajson/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-05-15 14:36:56.000000 mediajson-2.3.0/mediajson/immutable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 14:36:56.000000 mediajson-2.3.0/mediajson/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-15 14:36:56.000000 mediajson-2.3.0/mediajson/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:38:41.022322 mediajson-2.3.0/mediajson.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      560 2024-05-15 14:38:41.000000 mediajson-2.3.0/mediajson.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-15 14:38:41.000000 mediajson-2.3.0/mediajson.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 14:38:41.000000 mediajson-2.3.0/mediajson.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-15 14:38:41.000000 mediajson-2.3.0/mediajson.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-15 14:38:41.000000 mediajson-2.3.0/mediajson.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 14:38:41.022322 mediajson-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-15 14:36:56.000000 mediajson-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:38:41.022322 mediajson-2.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 14:36:56.000000 mediajson-2.3.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4169 2024-05-15 14:36:56.000000 mediajson-2.3.0/tests/test_decode.py
+-rw-r--r--   0 root         (0) root         (0)     4980 2024-05-15 14:36:56.000000 mediajson-2.3.0/tests/test_encode.py
```

### Comparing `mediajson-2.2.1/LICENSE.md` & `mediajson-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mediajson-2.2.1/NOTICE.md` & `mediajson-2.3.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `mediajson-2.2.1/PKG-INFO` & `mediajson-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediajson
-Version: 2.2.1
+Version: 2.3.0
 Summary: A JSON serialiser and parser for python that supports extensions convenient for our media grain formats
 Home-page: https://github.com/bbc/rd-apmm-python-lib-mediajson
 Author: BBC R&D
 Author-email: cloudfit-opensource@rd.bbc.co.uk
 License: Apache 2
 Requires-Python: >=3.10.0
 License-File: LICENSE.md
```

### Comparing `mediajson-2.2.1/README.md` & `mediajson-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mediajson-2.2.1/mediajson/__init__.py` & `mediajson-2.3.0/mediajson/__init__.py`

 * *Files identical despite different names*

### Comparing `mediajson-2.2.1/mediajson/decode.py` & `mediajson-2.3.0/mediajson/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     return json.loads(*_args, **kwargs)
 
 
 def decode_value(o: JSONSerialisable) -> MediaJSONSerialisable:
     if isinstance(o, dict):
         if len(o.keys()) == 2 and "numerator" in o and "denominator" in o:
             return Fraction(o['numerator'], o['denominator'])
+        elif len(o.keys()) == 1 and "numerator" in o:
+            return Fraction(o['numerator'], 1)
         else:
             res = {}
             for key in o:
                 res[key] = decode_value(o[key])
             return res
     elif isinstance(o, list):
         return [decode_value(v) for v in o]
```

### Comparing `mediajson-2.2.1/mediajson/encode.py` & `mediajson-2.3.0/mediajson/encode.py`

 * *Files identical despite different names*

### Comparing `mediajson-2.2.1/mediajson/immutable.py` & `mediajson-2.3.0/mediajson/immutable.py`

 * *Files identical despite different names*

### Comparing `mediajson-2.2.1/mediajson/typing.py` & `mediajson-2.3.0/mediajson/typing.py`

 * *Files identical despite different names*

### Comparing `mediajson-2.2.1/mediajson.egg-info/PKG-INFO` & `mediajson-2.3.0/mediajson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediajson
-Version: 2.2.1
+Version: 2.3.0
 Summary: A JSON serialiser and parser for python that supports extensions convenient for our media grain formats
 Home-page: https://github.com/bbc/rd-apmm-python-lib-mediajson
 Author: BBC R&D
 Author-email: cloudfit-opensource@rd.bbc.co.uk
 License: Apache 2
 Requires-Python: >=3.10.0
 License-File: LICENSE.md
```

### Comparing `mediajson-2.2.1/setup.py` & `mediajson-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mediajson-2.2.1/tests/test_decode.py` & `mediajson-2.3.0/tests/test_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "baz": ["boop", "beep"],
     "boggle": {"cat": u"\u732b",
                "kitten": u"\u5b50\u732b"},
     "numeric": 25,
     "boolean": True,
     "decimal": 0.44,
     "uuid": UUID("b8b4a34f-3293-11e8-89c0-acde48001122"),
-    "rational": Fraction(30000, 1001),
+    "rationals": [Fraction(30000, 1001), Fraction(50, 1)],
     "timestamps": [Timestamp.from_sec_nsec("417798915:0"), Timestamp.from_sec_nsec("-417798915:0")],
     "timeranges": [TimeRange(Timestamp(417798915, 0), Timestamp(417798916, 999), TimeRange.INCLUSIVE),
                    TimeRange(Timestamp(417798915, 0), Timestamp(417798916, 999), TimeRange.EXCLUSIVE),
                    TimeRange(Timestamp(417798915, 0), Timestamp(417798916, 999), TimeRange.INCLUDE_START),
                    TimeRange(Timestamp(417798915, 0), Timestamp(417798916, 999), TimeRange.INCLUDE_END),
                    TimeRange.never(),
                    TimeRange.eternity(),
@@ -59,15 +59,15 @@
                    TimeRange(Timestamp(417798916, 999, -1), Timestamp(417798915, 0), TimeRange.INCLUSIVE),
                    TimeRange.from_start(Timestamp(417798916, 999, -1), TimeRange.INCLUSIVE),
                    TimeRange.from_end(Timestamp(417798916, 999, -1), TimeRange.INCLUSIVE)]
 }
 
 MEDIAJSON_STRING = '{"foo": "bar", "baz": ["boop", "beep"], "boggle": {"cat": "\\u732b", "kitten": "\\u5b50\\u732b"}, '\
     '"numeric": 25, "boolean": true, "decimal": 0.44, "uuid": "b8b4a34f-3293-11e8-89c0-acde48001122", '\
-    '"rational": {"numerator": 30000, "denominator": 1001},'\
+    '"rationals": [{"numerator": 30000, "denominator": 1001}, {"numerator": 50}], '\
     '"timestamps": ["417798915:0", "-417798915:0"],'\
     '"timeranges": ["[417798915:0_417798916:999]", "(417798915:0_417798916:999)", "[417798915:0_417798916:999)",'\
     '"(417798915:0_417798916:999]", "()", "_", "[417798915:0_", "(417798915:0_", "_417798915:0]", "_417798915:0)",'\
     '"[-417798916:999_-417798915:0]", "[-417798916:999_417798915:0]", "[-417798916:999_", "_-417798916:999]"]}'
 
 
 class TestJSONDecode(unittest.TestCase):
```

### Comparing `mediajson-2.2.1/tests/test_encode.py` & `mediajson-2.3.0/tests/test_encode.py`

 * *Files identical despite different names*

