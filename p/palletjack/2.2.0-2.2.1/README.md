# Comparing `tmp/palletjack-2.2.0.tar.gz` & `tmp/palletjack-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palletjack-2.2.0.tar", last modified: Wed May  8 15:35:39 2024, max compression
+gzip compressed data, was "palletjack-2.2.1.tar", last modified: Wed May 15 14:07:34 2024, max compression
```

## Comparing `palletjack-2.2.0.tar` & `palletjack-2.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:39.140204 palletjack-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 15:29:22.000000 palletjack-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-08 15:35:39.136204 palletjack-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-08 15:29:22.000000 palletjack-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:39.136204 palletjack-2.2.0/palletjack/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/cpalletjack.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    28644 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/palletjack.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/palletjack.h
--rw-r--r--   0 runner    (1001) docker     (127)  1757552 2024-05-08 15:35:37.000000 palletjack-2.2.0/palletjack/palletjack_cython.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/palletjack_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   216223 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/parquet_types_palletjack.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    86184 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/parquet_types_palletjack.h
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/windows_fixup.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:39.136204 palletjack-2.2.0/palletjack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:35:37.000000 palletjack-2.2.0/palletjack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 15:29:22.000000 palletjack-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:35:39.140204 palletjack-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-08 15:29:22.000000 palletjack-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:39.136204 palletjack-2.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-05-08 15:29:22.000000 palletjack-2.2.0/test/test_palletjack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-08 15:29:22.000000 palletjack-2.2.0/test/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:07:34.631770 palletjack-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 14:06:58.000000 palletjack-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-15 14:07:34.631770 palletjack-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-15 14:06:58.000000 palletjack-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:07:34.631770 palletjack-2.2.1/palletjack/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 14:06:58.000000 palletjack-2.2.1/palletjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-15 14:06:58.000000 palletjack-2.2.1/palletjack/cpalletjack.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    28517 2024-05-15 14:06:58.000000 palletjack-2.2.1/palletjack/palletjack.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-15 14:06:58.000000 palletjack-2.2.1/palletjack/palletjack.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1757552 2024-05-15 14:07:33.000000 palletjack-2.2.1/palletjack/palletjack_cython.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-15 14:06:58.000000 palletjack-2.2.1/palletjack/palletjack_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   216223 2024-05-15 14:06:58.000000 palletjack-2.2.1/palletjack/parquet_types_palletjack.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    86184 2024-05-15 14:06:58.000000 palletjack-2.2.1/palletjack/parquet_types_palletjack.h
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 14:06:58.000000 palletjack-2.2.1/palletjack/windows_fixup.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:07:34.631770 palletjack-2.2.1/palletjack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-15 14:07:34.000000 palletjack-2.2.1/palletjack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-15 14:07:34.000000 palletjack-2.2.1/palletjack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:07:34.000000 palletjack-2.2.1/palletjack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:07:33.000000 palletjack-2.2.1/palletjack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 14:07:34.000000 palletjack-2.2.1/palletjack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 14:07:34.000000 palletjack-2.2.1/palletjack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 14:06:58.000000 palletjack-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:07:34.631770 palletjack-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-15 14:06:58.000000 palletjack-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:07:34.631770 palletjack-2.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-05-15 14:06:58.000000 palletjack-2.2.1/test/test_palletjack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-15 14:06:58.000000 palletjack-2.2.1/test/test_readme.py
```

### Comparing `palletjack-2.2.0/LICENSE` & `palletjack-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/PKG-INFO` & `palletjack-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palletjack
-Version: 2.2.0
+Version: 2.2.1
 Summary: Faster parquet metadata reading
 Author-email: Marcin Krystianc <marcin.krystianc@gmail.com>
 Project-URL: Homepage, https://github.com/marcin-krystianc/PalletJack
 Project-URL: Issues, https://github.com/marcin-krystianc/PalletJack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `palletjack-2.2.0/README.md` & `palletjack-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/palletjack/cpalletjack.pxd` & `palletjack-2.2.1/palletjack/cpalletjack.pxd`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/palletjack/palletjack.cc` & `palletjack-2.2.1/palletjack/palletjack.cc`

 * *Files 2% similar despite different names*

```diff
@@ -83,34 +83,30 @@
 constexpr int32_t kDefaultThriftStringSizeLimit = 100 * 1000 * 1000;
 constexpr int32_t kDefaultThriftContainerSizeLimit = 1000 * 1000;
 
 using ThriftBuffer = apache::thrift::transport::TMemoryBuffer;
 
 std::shared_ptr<ThriftBuffer> CreateReadOnlyMemoryBuffer(uint8_t *buf, uint32_t len)
 {
-#if PARQUET_THRIFT_VERSION_MAJOR > 0 || PARQUET_THRIFT_VERSION_MINOR >= 14
     auto conf = std::make_shared<apache::thrift::TConfiguration>();
     conf->setMaxMessageSize(std::numeric_limits<int>::max());
     return std::make_shared<ThriftBuffer>(buf, len, ThriftBuffer::OBSERVE, conf);
-#else
-    return std::make_shared<ThriftBuffer>(buf, len);
-#endif
 }
 
-template <class T>
 void DeserializeUnencryptedMessage(const uint8_t *buf, uint32_t *len,
-                                   T *deserialized_msg)
+                                   palletjack::parquet::FileMetaData *deserialized_msg)
 {
     // Deserialize msg bytes into c++ thrift msg using memory transport.
     auto tmem_transport = CreateReadOnlyMemoryBuffer(const_cast<uint8_t *>(buf), *len);
     apache::thrift::protocol::TCompactProtocolFactoryT<ThriftBuffer> tproto_factory;
     // Protect against CPU and memory bombs
     tproto_factory.setStringSizeLimit(kDefaultThriftStringSizeLimit);
     tproto_factory.setContainerSizeLimit(kDefaultThriftContainerSizeLimit);
     auto tproto = tproto_factory.getProtocol(tmem_transport);
+
     try
     {
         deserialized_msg->read(tproto.get());
     }
     catch (std::exception &e)
     {
         std::stringstream ss;
```

### Comparing `palletjack-2.2.0/palletjack/palletjack.h` & `palletjack-2.2.1/palletjack/palletjack.h`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/palletjack/palletjack_cython.cpp` & `palletjack-2.2.1/palletjack/palletjack_cython.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/numpy/core/include/numpy/halffloat.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/api.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/array/concatenate.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/builder.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/c/abi.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/c/bridge.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack_abi.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/compute/api.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/compute/cast.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/compute/expression.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/config.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/csv/api.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/extension/fixed_shape_tensor.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/extension_type.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/io/api.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/ipc/api.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/json/options.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/json/reader.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/api.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/arrow_to_pandas.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/async.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/benchmark.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/common.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/csv.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/extension_type.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/gdb.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/inference.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/init.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/ipc.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/platform.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/pyarrow.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/udf.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/result.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/byte_size.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/cancel.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/compression.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/decimal.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/future.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/io_util.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/iterator.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/key_value_metadata.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/thread_pool.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/value_parsing.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/api/reader.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/api/schema.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/api/writer.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/reader.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/schema.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/writer.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/encryption/encryption.h",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/properties.h"
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/numpy/core/include/numpy/halffloat.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/api.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/array/concatenate.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/builder.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/c/abi.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/c/bridge.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack_abi.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/compute/api.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/compute/cast.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/compute/expression.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/config.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/csv/api.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/extension/fixed_shape_tensor.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/extension_type.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/io/api.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/ipc/api.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/json/options.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/json/reader.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/api.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/arrow_to_pandas.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/async.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/benchmark.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/common.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/csv.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/extension_type.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/gdb.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/inference.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/init.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/ipc.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/platform.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/pyarrow.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/python/udf.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/result.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/byte_size.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/cancel.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/compression.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/decimal.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/future.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/io_util.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/iterator.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/key_value_metadata.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/thread_pool.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/arrow/util/value_parsing.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/parquet/api/reader.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/parquet/api/schema.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/parquet/api/writer.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/reader.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/schema.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/writer.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/parquet/encryption/encryption.h",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include/parquet/properties.h"
         ],
         "extra_compile_args": [
             "-std=c++17"
         ],
         "include_dirs": [
             ".",
             "/home/runner/work/PalletJack/PalletJack/python/vcpkg_installed/include",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow/include",
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "libraries": [
             "arrow",
             "parquet",
             "thrift"
         ],
         "library_dirs": [
             "/home/runner/work/PalletJack/PalletJack/python/vcpkg_installed/lib",
-            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow"
+            "/tmp/build-env-1y_lfa13/lib/python3.10/site-packages/pyarrow"
         ],
         "name": "palletjack.palletjack_cython",
         "sources": [
             "palletjack/palletjack_cython.pyx",
             "palletjack/palletjack.cc",
             "palletjack/parquet_types_palletjack.cpp"
         ]
```

### Comparing `palletjack-2.2.0/palletjack/palletjack_cython.pyx` & `palletjack-2.2.1/palletjack/palletjack_cython.pyx`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/palletjack/parquet_types_palletjack.cpp` & `palletjack-2.2.1/palletjack/parquet_types_palletjack.cpp`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/palletjack/parquet_types_palletjack.h` & `palletjack-2.2.1/palletjack/parquet_types_palletjack.h`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/palletjack.egg-info/PKG-INFO` & `palletjack-2.2.1/palletjack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palletjack
-Version: 2.2.0
+Version: 2.2.1
 Summary: Faster parquet metadata reading
 Author-email: Marcin Krystianc <marcin.krystianc@gmail.com>
 Project-URL: Homepage, https://github.com/marcin-krystianc/PalletJack
 Project-URL: Issues, https://github.com/marcin-krystianc/PalletJack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `palletjack-2.2.0/palletjack.egg-info/SOURCES.txt` & `palletjack-2.2.1/palletjack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/pyproject.toml` & `palletjack-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "thrift",
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "palletjack"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
   { name="Marcin Krystianc", email="marcin.krystianc@gmail.com" },
 ]
 description = "Faster parquet metadata reading"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `palletjack-2.2.0/setup.py` & `palletjack-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/test/test_palletjack.py` & `palletjack-2.2.1/test/test_palletjack.py`

 * *Files identical despite different names*

### Comparing `palletjack-2.2.0/test/test_readme.py` & `palletjack-2.2.1/test/test_readme.py`

 * *Files identical despite different names*

