# Comparing `tmp/jito_searcher_client-0.1.3.tar.gz` & `tmp/jito_searcher_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jito_searcher_client-0.1.3.tar", max compression
+gzip compressed data, was "jito_searcher_client-0.1.4.tar", max compression
```

## Comparing `jito_searcher_client-0.1.3.tar` & `jito_searcher_client-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1971 2024-03-26 15:14:33.396208 jito_searcher_client-0.1.3/README.md
--rw-r--r--   0        0        0      239 2024-03-26 15:14:33.396830 jito_searcher_client-0.1.3/jito_searcher_client/__init__.py
--rw-r--r--   0        0        0     6275 2024-03-26 15:14:33.397014 jito_searcher_client-0.1.3/jito_searcher_client/async_searcher.py
--rw-r--r--   0        0        0      847 2024-03-26 15:14:33.397126 jito_searcher_client-0.1.3/jito_searcher_client/convert.py
--rw-r--r--   0        0        0      127 2024-03-26 15:14:33.397297 jito_searcher_client-0.1.3/jito_searcher_client/generated/__init__.py
--rw-r--r--   0        0        0     3109 2024-03-26 15:14:33.397415 jito_searcher_client-0.1.3/jito_searcher_client/generated/auth_pb2.py
--rw-r--r--   0        0        0     6712 2024-03-26 15:14:33.397594 jito_searcher_client-0.1.3/jito_searcher_client/generated/auth_pb2.pyi
--rw-r--r--   0        0        0     5981 2024-03-26 15:14:33.397779 jito_searcher_client-0.1.3/jito_searcher_client/generated/auth_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2024-03-26 15:14:33.397881 jito_searcher_client-0.1.3/jito_searcher_client/generated/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0     4755 2024-03-26 15:14:33.398072 jito_searcher_client-0.1.3/jito_searcher_client/generated/block_engine_pb2.py
--rw-r--r--   0        0        0     9066 2024-03-26 15:14:33.398321 jito_searcher_client-0.1.3/jito_searcher_client/generated/block_engine_pb2.pyi
--rw-r--r--   0        0        0    13185 2024-03-26 15:14:33.398607 jito_searcher_client-0.1.3/jito_searcher_client/generated/block_engine_pb2_grpc.py
--rw-r--r--   0        0        0     5837 2024-03-26 15:14:33.398795 jito_searcher_client-0.1.3/jito_searcher_client/generated/block_engine_pb2_grpc.pyi
--rw-r--r--   0        0        0     1304 2024-03-26 15:14:33.398935 jito_searcher_client-0.1.3/jito_searcher_client/generated/block_pb2.py
--rw-r--r--   0        0        0     2142 2024-03-26 15:14:33.399089 jito_searcher_client-0.1.3/jito_searcher_client/generated/block_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-26 15:14:33.399195 jito_searcher_client-0.1.3/jito_searcher_client/generated/block_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-03-26 15:14:33.399295 jito_searcher_client-0.1.3/jito_searcher_client/generated/block_pb2_grpc.pyi
--rw-r--r--   0        0        0     3204 2024-03-26 15:14:33.399408 jito_searcher_client-0.1.3/jito_searcher_client/generated/bundle_pb2.py
--rw-r--r--   0        0        0     9999 2024-03-26 15:14:33.399639 jito_searcher_client-0.1.3/jito_searcher_client/generated/bundle_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-26 15:14:33.399747 jito_searcher_client-0.1.3/jito_searcher_client/generated/bundle_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-03-26 15:14:33.399851 jito_searcher_client-0.1.3/jito_searcher_client/generated/bundle_pb2_grpc.pyi
--rw-r--r--   0        0        0     1744 2024-03-26 15:14:33.399982 jito_searcher_client-0.1.3/jito_searcher_client/generated/packet_pb2.py
--rw-r--r--   0        0        0     3677 2024-03-26 15:14:33.400094 jito_searcher_client-0.1.3/jito_searcher_client/generated/packet_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-26 15:14:33.400205 jito_searcher_client-0.1.3/jito_searcher_client/generated/packet_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-03-26 15:14:33.400302 jito_searcher_client-0.1.3/jito_searcher_client/generated/packet_pb2_grpc.pyi
--rw-r--r--   0        0        0     2083 2024-03-26 15:14:33.400427 jito_searcher_client-0.1.3/jito_searcher_client/generated/relayer_pb2.py
--rw-r--r--   0        0        0     2883 2024-03-26 15:14:33.400562 jito_searcher_client-0.1.3/jito_searcher_client/generated/relayer_pb2.pyi
--rw-r--r--   0        0        0     5002 2024-03-26 15:14:33.400732 jito_searcher_client-0.1.3/jito_searcher_client/generated/relayer_pb2_grpc.py
--rw-r--r--   0        0        0     2396 2024-03-26 15:14:33.400837 jito_searcher_client-0.1.3/jito_searcher_client/generated/relayer_pb2_grpc.pyi
--rw-r--r--   0        0        0     5369 2024-03-26 15:14:33.401042 jito_searcher_client-0.1.3/jito_searcher_client/generated/searcher_pb2.py
--rw-r--r--   0        0        0    10723 2024-03-26 15:14:33.401262 jito_searcher_client-0.1.3/jito_searcher_client/generated/searcher_pb2.pyi
--rw-r--r--   0        0        0    12743 2024-03-26 15:14:33.401551 jito_searcher_client-0.1.3/jito_searcher_client/generated/searcher_pb2_grpc.py
--rw-r--r--   0        0        0     4518 2024-03-26 15:14:33.401730 jito_searcher_client-0.1.3/jito_searcher_client/generated/searcher_pb2_grpc.pyi
--rw-r--r--   0        0        0     1359 2024-03-26 15:14:33.401857 jito_searcher_client-0.1.3/jito_searcher_client/generated/shared_pb2.py
--rw-r--r--   0        0        0     1868 2024-03-26 15:14:33.401975 jito_searcher_client-0.1.3/jito_searcher_client/generated/shared_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-26 15:14:33.402099 jito_searcher_client-0.1.3/jito_searcher_client/generated/shared_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-03-26 15:14:33.402206 jito_searcher_client-0.1.3/jito_searcher_client/generated/shared_pb2_grpc.pyi
--rw-r--r--   0        0        0     1412 2024-03-26 15:14:33.402366 jito_searcher_client-0.1.3/jito_searcher_client/generated/shredstream_pb2.py
--rw-r--r--   0        0        0     2114 2024-03-26 15:14:33.402492 jito_searcher_client-0.1.3/jito_searcher_client/generated/shredstream_pb2.pyi
--rw-r--r--   0        0        0     2491 2024-03-26 15:14:33.402608 jito_searcher_client-0.1.3/jito_searcher_client/generated/shredstream_pb2_grpc.py
--rw-r--r--   0        0        0      815 2024-03-26 15:14:33.402727 jito_searcher_client-0.1.3/jito_searcher_client/generated/shredstream_pb2_grpc.pyi
--rw-r--r--   0        0        0     5964 2024-03-26 15:14:33.402906 jito_searcher_client-0.1.3/jito_searcher_client/searcher.py
--rw-r--r--   0        0        0      191 2024-03-26 15:14:33.402999 jito_searcher_client-0.1.3/jito_searcher_client/token.py
--rw-r--r--   0        0        0      733 2024-03-26 15:23:42.011728 jito_searcher_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2551 1970-01-01 00:00:00.000000 jito_searcher_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1971 2024-03-26 15:14:33.396208 jito_searcher_client-0.1.4/README.md
+-rw-r--r--   0        0        0      239 2024-03-26 15:14:33.396830 jito_searcher_client-0.1.4/jito_searcher_client/__init__.py
+-rw-r--r--   0        0        0     6275 2024-03-26 15:14:33.397014 jito_searcher_client-0.1.4/jito_searcher_client/async_searcher.py
+-rw-r--r--   0        0        0      847 2024-03-26 15:14:33.397126 jito_searcher_client-0.1.4/jito_searcher_client/convert.py
+-rw-r--r--   0        0        0      127 2024-03-26 15:14:33.397297 jito_searcher_client-0.1.4/jito_searcher_client/generated/__init__.py
+-rw-r--r--   0        0        0     3109 2024-03-26 15:14:33.397415 jito_searcher_client-0.1.4/jito_searcher_client/generated/auth_pb2.py
+-rw-r--r--   0        0        0     6712 2024-03-26 15:14:33.397594 jito_searcher_client-0.1.4/jito_searcher_client/generated/auth_pb2.pyi
+-rw-r--r--   0        0        0     5981 2024-03-26 15:14:33.397779 jito_searcher_client-0.1.4/jito_searcher_client/generated/auth_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2024-03-26 15:14:33.397881 jito_searcher_client-0.1.4/jito_searcher_client/generated/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4755 2024-03-26 15:14:33.398072 jito_searcher_client-0.1.4/jito_searcher_client/generated/block_engine_pb2.py
+-rw-r--r--   0        0        0     9066 2024-03-26 15:14:33.398321 jito_searcher_client-0.1.4/jito_searcher_client/generated/block_engine_pb2.pyi
+-rw-r--r--   0        0        0    13185 2024-03-26 15:14:33.398607 jito_searcher_client-0.1.4/jito_searcher_client/generated/block_engine_pb2_grpc.py
+-rw-r--r--   0        0        0     5837 2024-03-26 15:14:33.398795 jito_searcher_client-0.1.4/jito_searcher_client/generated/block_engine_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1304 2024-03-26 15:14:33.398935 jito_searcher_client-0.1.4/jito_searcher_client/generated/block_pb2.py
+-rw-r--r--   0        0        0     2142 2024-03-26 15:14:33.399089 jito_searcher_client-0.1.4/jito_searcher_client/generated/block_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-03-26 15:14:33.399195 jito_searcher_client-0.1.4/jito_searcher_client/generated/block_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-03-26 15:14:33.399295 jito_searcher_client-0.1.4/jito_searcher_client/generated/block_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3204 2024-03-26 15:14:33.399408 jito_searcher_client-0.1.4/jito_searcher_client/generated/bundle_pb2.py
+-rw-r--r--   0        0        0     9999 2024-03-26 15:14:33.399639 jito_searcher_client-0.1.4/jito_searcher_client/generated/bundle_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-03-26 15:14:33.399747 jito_searcher_client-0.1.4/jito_searcher_client/generated/bundle_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-03-26 15:14:33.399851 jito_searcher_client-0.1.4/jito_searcher_client/generated/bundle_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1744 2024-03-26 15:14:33.399982 jito_searcher_client-0.1.4/jito_searcher_client/generated/packet_pb2.py
+-rw-r--r--   0        0        0     3677 2024-03-26 15:14:33.400094 jito_searcher_client-0.1.4/jito_searcher_client/generated/packet_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-03-26 15:14:33.400205 jito_searcher_client-0.1.4/jito_searcher_client/generated/packet_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-03-26 15:14:33.400302 jito_searcher_client-0.1.4/jito_searcher_client/generated/packet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2083 2024-03-26 15:14:33.400427 jito_searcher_client-0.1.4/jito_searcher_client/generated/relayer_pb2.py
+-rw-r--r--   0        0        0     2883 2024-03-26 15:14:33.400562 jito_searcher_client-0.1.4/jito_searcher_client/generated/relayer_pb2.pyi
+-rw-r--r--   0        0        0     5002 2024-03-26 15:14:33.400732 jito_searcher_client-0.1.4/jito_searcher_client/generated/relayer_pb2_grpc.py
+-rw-r--r--   0        0        0     2396 2024-03-26 15:14:33.400837 jito_searcher_client-0.1.4/jito_searcher_client/generated/relayer_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5369 2024-03-26 15:14:33.401042 jito_searcher_client-0.1.4/jito_searcher_client/generated/searcher_pb2.py
+-rw-r--r--   0        0        0    10723 2024-03-26 15:14:33.401262 jito_searcher_client-0.1.4/jito_searcher_client/generated/searcher_pb2.pyi
+-rw-r--r--   0        0        0    12743 2024-03-26 15:14:33.401551 jito_searcher_client-0.1.4/jito_searcher_client/generated/searcher_pb2_grpc.py
+-rw-r--r--   0        0        0     4518 2024-03-26 15:14:33.401730 jito_searcher_client-0.1.4/jito_searcher_client/generated/searcher_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1359 2024-03-26 15:14:33.401857 jito_searcher_client-0.1.4/jito_searcher_client/generated/shared_pb2.py
+-rw-r--r--   0        0        0     1868 2024-03-26 15:14:33.401975 jito_searcher_client-0.1.4/jito_searcher_client/generated/shared_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-03-26 15:14:33.402099 jito_searcher_client-0.1.4/jito_searcher_client/generated/shared_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-03-26 15:14:33.402206 jito_searcher_client-0.1.4/jito_searcher_client/generated/shared_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1412 2024-03-26 15:14:33.402366 jito_searcher_client-0.1.4/jito_searcher_client/generated/shredstream_pb2.py
+-rw-r--r--   0        0        0     2114 2024-03-26 15:14:33.402492 jito_searcher_client-0.1.4/jito_searcher_client/generated/shredstream_pb2.pyi
+-rw-r--r--   0        0        0     2491 2024-03-26 15:14:33.402608 jito_searcher_client-0.1.4/jito_searcher_client/generated/shredstream_pb2_grpc.py
+-rw-r--r--   0        0        0      815 2024-03-26 15:14:33.402727 jito_searcher_client-0.1.4/jito_searcher_client/generated/shredstream_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5964 2024-03-26 15:14:33.402906 jito_searcher_client-0.1.4/jito_searcher_client/searcher.py
+-rw-r--r--   0        0        0      191 2024-03-26 15:14:33.402999 jito_searcher_client-0.1.4/jito_searcher_client/token.py
+-rw-r--r--   0        0        0      733 2024-05-15 14:14:10.743818 jito_searcher_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2551 1970-01-01 00:00:00.000000 jito_searcher_client-0.1.4/PKG-INFO
```

### Comparing `jito_searcher_client-0.1.3/README.md` & `jito_searcher_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/async_searcher.py` & `jito_searcher_client-0.1.4/jito_searcher_client/async_searcher.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/convert.py` & `jito_searcher_client-0.1.4/jito_searcher_client/convert.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/auth_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/auth_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/auth_pb2_grpc.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/auth_pb2_grpc.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/auth_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/block_engine_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/block_engine_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/block_engine_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/block_engine_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/block_engine_pb2_grpc.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/block_engine_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/block_engine_pb2_grpc.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/block_engine_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/block_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/block_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/block_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/bundle_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/bundle_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/packet_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/packet_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/packet_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/packet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/relayer_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/relayer_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/relayer_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/relayer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/relayer_pb2_grpc.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/relayer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/relayer_pb2_grpc.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/relayer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/searcher_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/searcher_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/searcher_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/searcher_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/searcher_pb2_grpc.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/searcher_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/searcher_pb2_grpc.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/searcher_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/shared_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/shared_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/shredstream_pb2.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/shredstream_pb2.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/shredstream_pb2.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/shredstream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/shredstream_pb2_grpc.py` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/shredstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/generated/shredstream_pb2_grpc.pyi` & `jito_searcher_client-0.1.4/jito_searcher_client/generated/shredstream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/jito_searcher_client/searcher.py` & `jito_searcher_client-0.1.4/jito_searcher_client/searcher.py`

 * *Files identical despite different names*

### Comparing `jito_searcher_client-0.1.3/pyproject.toml` & `jito_searcher_client-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "jito_searcher_client"
-version = "0.1.3"
+version = "0.1.4"
 description = "Jito Labs Python Searcher Client"
 authors = ["Jito Labs <support@jito.wtf>"]
 readme = "README.md"
 packages = [{ include = "jito_searcher_client" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 grpcio = "^1.62.1"
 protobuf = "^4.25.3"
 click = "^8.1.3"
-solana = "0.30.1"
+solana = "0.34.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-grpc-plugin]
 proto_path = "../mev-protos"
```

### Comparing `jito_searcher_client-0.1.3/PKG-INFO` & `jito_searcher_client-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: jito_searcher_client
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jito Labs Python Searcher Client
 Author: Jito Labs
 Author-email: support@jito.wtf
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: grpcio (>=1.62.1,<2.0.0)
 Requires-Dist: protobuf (>=4.25.3,<5.0.0)
-Requires-Dist: solana (==0.30.1)
+Requires-Dist: solana (==0.34.0)
 Description-Content-Type: text/markdown
 
 # About
 This library contains tooling to interact with Jito Lab's Block Engine as a searcher.
 
 # Downloading
 ```bash
```

