# Comparing `tmp/peeweext-1.2.7-py3-none-any.whl.zip` & `tmp/peeweext-1.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10636 bytes, number of entries: 13
--rw-r--r--  2.0 unx       22 b- defN 24-May-11 07:30 peeweext/__init__.py
--rw-r--r--  2.0 unx     1663 b- defN 24-May-11 07:30 peeweext/fields.py
--rw-r--r--  2.0 unx     1795 b- defN 24-May-11 07:30 peeweext/flask.py
--rw-r--r--  2.0 unx     3739 b- defN 24-May-11 07:30 peeweext/mixins.py
--rw-r--r--  2.0 unx     5089 b- defN 24-May-11 07:30 peeweext/model.py
--rw-r--r--  2.0 unx      551 b- defN 24-May-11 07:30 peeweext/otel.py
--rw-r--r--  2.0 unx     2517 b- defN 24-May-11 07:30 peeweext/sea.py
--rw-r--r--  2.0 unx     5859 b- defN 24-May-11 07:30 peeweext/validation.py
--rw-r--r--  2.0 unx     1064 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     1733 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      986 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/RECORD
-13 files, 25119 bytes uncompressed, 9012 bytes compressed:  64.1%
+Zip file size: 10789 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       22 b- defN 24-May-15 10:05 peeweext/__init__.py
+-rw-r--r--  2.0 unx     1663 b- defN 24-May-15 10:05 peeweext/fields.py
+-rw-r--r--  2.0 unx     1795 b- defN 24-May-15 10:05 peeweext/flask.py
+-rw-r--r--  2.0 unx     3739 b- defN 24-May-15 10:05 peeweext/mixins.py
+-rw-r--r--  2.0 unx     5089 b- defN 24-May-15 10:05 peeweext/model.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-15 10:05 peeweext/otel.py
+-rw-r--r--  2.0 unx     2517 b- defN 24-May-15 10:05 peeweext/sea.py
+-rw-r--r--  2.0 unx     5859 b- defN 24-May-15 10:05 peeweext/validation.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-15 10:05 peeweext-1.2.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1786 b- defN 24-May-15 10:05 peeweext-1.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 10:05 peeweext-1.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-15 10:05 peeweext-1.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      987 b- defN 24-May-15 10:05 peeweext-1.2.8.dist-info/RECORD
+13 files, 25752 bytes uncompressed, 9165 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: peeweext/sea.py
 Comment: 
 
 Filename: peeweext/validation.py
 Comment: 
 
-Filename: peeweext-1.2.7.dist-info/LICENSE
+Filename: peeweext-1.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: peeweext-1.2.7.dist-info/METADATA
+Filename: peeweext-1.2.8.dist-info/METADATA
 Comment: 
 
-Filename: peeweext-1.2.7.dist-info/WHEEL
+Filename: peeweext-1.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: peeweext-1.2.7.dist-info/top_level.txt
+Filename: peeweext-1.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: peeweext-1.2.7.dist-info/RECORD
+Filename: peeweext-1.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## peeweext/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.2.7'
+__version__ = '1.2.8'
```

## peeweext/otel.py

```diff
@@ -1,20 +1,46 @@
+from enum import Enum
 from opentelemetry import trace
-from opentelemetry.instrumentation.mysqlclient import MySQLClientInstrumentor
+
+mysql_connector = None
+
+
+class MySQLConnector(Enum):
+    mysqldb = 0
+    pymysql = 1
+
+
+try:
+    import MySQLdb
+    from opentelemetry.instrumentation.mysqlclient import MySQLClientInstrumentor
+
+    mysql_connector = MySQLConnector.mysqldb
+except ImportError:
+    try:
+        import pymysql
+        from opentelemetry.instrumentation.pymysql import PyMySQLInstrumentor
+
+        mysql_connector = MySQLConnector.pymysql
+    except ImportError:
+        pass
 
 
 def sync_once(func):
     def wrapper(*args, **kwargs):
         if not wrapper._done:
             wrapper._done = True
             return func(*args, **kwargs)
 
     wrapper._done = False
     return wrapper
 
 
 @sync_once
 def otel_instrument(app=None):
-    if app is None or app.config.get_namespace("OTEL_").get("enable", False):
-        MySQLClientInstrumentor().instrument(
-            tracer_provider=trace.get_tracer_provider()
-        )
+    if app is not None and not app.config.get_namespace("OTEL_").get("enable", False):
+        return
+
+    tp = trace.get_tracer_provider()
+    if mysql_connector == MySQLConnector.mysqldb:
+        MySQLClientInstrumentor().instrument(tracer_provider=tp)
+    elif mysql_connector == MySQLConnector.pymysql:
+        PyMySQLInstrumentor().instrument(tracer_provider=tp)
```

## Comparing `peeweext-1.2.7.dist-info/LICENSE` & `peeweext-1.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `peeweext-1.2.7.dist-info/METADATA` & `peeweext-1.2.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeweext
-Version: 1.2.7
+Version: 1.2.8
 Summary: peewee extension
 Home-page: https://github.com/shanbay/peeweext
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: MIT
 Keywords: peewee,orm
 Classifier: Development Status :: 1 - Planning
@@ -20,15 +20,16 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 License-File: LICENSE
 Requires-Dist: peewee
 Requires-Dist: pendulum >=2.0.0
 Requires-Dist: blinker
-Requires-Dist: opentelemetry.instrumentation.mysqlclient
+Requires-Dist: opentelemetry-instrumentation-pymysql
+Requires-Dist: opentelemetry-instrumentation-mysqlclient
 
 # [Home Page](https://shanbay.github.io/peeweext/)
 
 [![](https://img.shields.io/travis/shanbay/peeweext.svg?style=flat-square)](https://travis-ci.org/shanbay/peeweext)
 [![Maintainability](https://api.codeclimate.com/v1/badges/774db211d37720bb2599/maintainability)](https://codeclimate.com/github/shanbay/peeweext/maintainability)
 [![Coverage Status](https://coveralls.io/repos/github/shanbay/peeweext/badge.svg?branch=master)](https://coveralls.io/github/shanbay/peeweext?branch=master)
 [![](https://img.shields.io/pypi/v/peeweext.svg)](https://github.com/shanbay/peeweext)
```

## Comparing `peeweext-1.2.7.dist-info/RECORD` & `peeweext-1.2.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-peeweext/__init__.py,sha256=ZPIeIspmBptDYG5CCWeXrMEitl5VFLx13DZa9qaB4EA,22
+peeweext/__init__.py,sha256=qGbXFEJiAOnWJQBRuZoZtO2VVVauuuZtAP1iQd2Gnq4,22
 peeweext/fields.py,sha256=kUN0yssg3ywkt9bRqsoixQxGhqwsSU_1AlZXRLmBQ7I,1663
 peeweext/flask.py,sha256=pRW1Afu1d6dDVxTR6i2UuhzZWAwQFK9JKtLBGGJemw8,1795
 peeweext/mixins.py,sha256=14y5GxdIb30FYeDO6BsL_y6lBFVEZL-Wc5eQVoVllvg,3739
 peeweext/model.py,sha256=Lh1s2oGnXBke2jus8oi23MxdcSHbvulWxzWKOQw7G_M,5089
-peeweext/otel.py,sha256=nQYTSXZmQgjvyNcKh84wtCtfJm5ow1mL3vjuM0zrFAE,551
+peeweext/otel.py,sha256=B3EVrCZcgSrbE6LE8Gtwa4AmnrcHBdRY7SO0YAPQRuA,1130
 peeweext/sea.py,sha256=E14gkIKAASub4nQcZlLpYWaZUyJVa_u4e2BVTW7-rCs,2517
 peeweext/validation.py,sha256=d-4CwGLLkCfowLNhDg911VNIihWEJUfZhbAkMmD3Fho,5859
-peeweext-1.2.7.dist-info/LICENSE,sha256=wTusV_NaHPTpuXq6lIajiiZ3QcQDkn3X7GzWHK6BMrg,1064
-peeweext-1.2.7.dist-info/METADATA,sha256=GcgwPzxDPguI6fa8Kkz1e_5hXcK7PgJR5hImtephaFQ,1733
-peeweext-1.2.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-peeweext-1.2.7.dist-info/top_level.txt,sha256=ZLpM6VFIxRFWqwerKPyOKLC-3cwyewx92t70T91tQUc,9
-peeweext-1.2.7.dist-info/RECORD,,
+peeweext-1.2.8.dist-info/LICENSE,sha256=wTusV_NaHPTpuXq6lIajiiZ3QcQDkn3X7GzWHK6BMrg,1064
+peeweext-1.2.8.dist-info/METADATA,sha256=1-1KZMCth603aKqb2t54xnk0gItB713OHdna3TUrdLo,1786
+peeweext-1.2.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+peeweext-1.2.8.dist-info/top_level.txt,sha256=ZLpM6VFIxRFWqwerKPyOKLC-3cwyewx92t70T91tQUc,9
+peeweext-1.2.8.dist-info/RECORD,,
```

