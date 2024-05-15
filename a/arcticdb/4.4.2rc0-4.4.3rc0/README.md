# Comparing `tmp/arcticdb-4.4.2rc0-cp39-cp39-win_amd64.whl.zip` & `tmp/arcticdb-4.4.3rc0-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,95 +1,81 @@
-Zip file size: 6301276 bytes, number of entries: 93
--rw-rw-rw-  2.0 fat 20562432 b- defN 24-May-04 13:59 arcticdb_ext.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      302 b- defN 24-May-04 13:33 arcticc/__init__.py
--rw-rw-rw-  2.0 fat     1508 b- defN 24-May-04 13:33 arcticc/pb2/__init__.py
--rw-rw-rw-  2.0 fat      749 b- defN 24-May-04 13:33 arcticdb/__init__.py
--rw-rw-rw-  2.0 fat      447 b- defN 24-May-04 13:33 arcticdb/_msgpack_compat.py
--rw-rw-rw-  2.0 fat    15472 b- defN 24-May-04 13:33 arcticdb/arctic.py
--rw-rw-rw-  2.0 fat     8619 b- defN 24-May-04 13:33 arcticdb/config.py
--rw-rw-rw-  2.0 fat      429 b- defN 24-May-04 13:33 arcticdb/encoding_version.py
--rw-rw-rw-  2.0 fat     1146 b- defN 24-May-04 13:33 arcticdb/exceptions.py
--rw-rw-rw-  2.0 fat     9158 b- defN 24-May-04 13:33 arcticdb/flattener.py
--rw-rw-rw-  2.0 fat     1897 b- defN 24-May-04 13:33 arcticdb/log.py
--rw-rw-rw-  2.0 fat    10733 b- defN 24-May-04 13:33 arcticdb/options.py
--rw-rw-rw-  2.0 fat      519 b- defN 24-May-04 13:33 arcticdb/preconditions.py
--rw-rw-rw-  2.0 fat     2006 b- defN 24-May-04 13:33 arcticdb/supported_types.py
--rw-rw-rw-  2.0 fat     3150 b- defN 24-May-04 13:33 arcticdb/tools.py
--rw-rw-rw-  2.0 fat      284 b- defN 24-May-04 13:33 arcticdb/adapters/__init__.py
--rw-rw-rw-  2.0 fat     4064 b- defN 24-May-04 13:33 arcticdb/adapters/arctic_library_adapter.py
--rw-rw-rw-  2.0 fat     5488 b- defN 24-May-04 13:33 arcticdb/adapters/azure_library_adapter.py
--rw-rw-rw-  2.0 fat     1906 b- defN 24-May-04 13:33 arcticdb/adapters/in_memory_library_adapter.py
--rw-rw-rw-  2.0 fat     5974 b- defN 24-May-04 13:33 arcticdb/adapters/lmdb_library_adapter.py
--rw-rw-rw-  2.0 fat     2763 b- defN 24-May-04 13:33 arcticdb/adapters/mongo_library_adapter.py
--rw-rw-rw-  2.0 fat     3599 b- defN 24-May-04 13:33 arcticdb/adapters/prefixing_library_adapter_decorator.py
--rw-rw-rw-  2.0 fat     8436 b- defN 24-May-04 13:33 arcticdb/adapters/s3_library_adapter.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 13:33 arcticdb/authorization/__init__.py
--rw-rw-rw-  2.0 fat      969 b- defN 24-May-04 13:33 arcticdb/authorization/permissions.py
--rw-rw-rw-  2.0 fat     4669 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/azure_storage_pb2.py
--rw-rw-rw-  2.0 fat     8935 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/config_pb2.py
--rw-rw-rw-  2.0 fat    98342 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/descriptors_pb2.py
--rw-rw-rw-  2.0 fat    31651 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/encoding_pb2.py
--rw-rw-rw-  2.0 fat     1561 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/in_memory_storage_pb2.py
--rw-rw-rw-  2.0 fat     5111 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/lmdb_storage_pb2.py
--rw-rw-rw-  2.0 fat    24224 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/logger_pb2.py
--rw-rw-rw-  2.0 fat     6142 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/mapped_file_storage_pb2.py
--rw-rw-rw-  2.0 fat     3409 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/mongo_storage_pb2.py
--rw-rw-rw-  2.0 fat     6878 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/nfs_backed_storage_pb2.py
--rw-rw-rw-  2.0 fat     1974 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/rocksdb_storage_pb2.py
--rw-rw-rw-  2.0 fat     7204 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/s3_storage_pb2.py
--rw-rw-rw-  2.0 fat    68704 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/storage_pb2.py
--rw-rw-rw-  2.0 fat    12621 b- defN 24-May-04 13:39 arcticdb/proto/3/arcticc/pb2/utils_pb2.py
--rw-rw-rw-  2.0 fat     1393 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/azure_storage_pb2.py
--rw-rw-rw-  2.0 fat     2518 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/config_pb2.py
--rw-rw-rw-  2.0 fat    16112 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/descriptors_pb2.py
--rw-rw-rw-  2.0 fat     5654 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/encoding_pb2.py
--rw-rw-rw-  2.0 fat     1070 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/in_memory_storage_pb2.py
--rw-rw-rw-  2.0 fat     1524 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/lmdb_storage_pb2.py
--rw-rw-rw-  2.0 fat     4478 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/logger_pb2.py
--rw-rw-rw-  2.0 fat     1739 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/mapped_file_storage_pb2.py
--rw-rw-rw-  2.0 fat     1352 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/mongo_storage_pb2.py
--rw-rw-rw-  2.0 fat     1593 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/nfs_backed_storage_pb2.py
--rw-rw-rw-  2.0 fat     1102 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/rocksdb_storage_pb2.py
--rw-rw-rw-  2.0 fat     1627 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/s3_storage_pb2.py
--rw-rw-rw-  2.0 fat    10801 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/storage_pb2.py
--rw-rw-rw-  2.0 fat     2482 b- defN 24-May-04 13:39 arcticdb/proto/4/arcticc/pb2/utils_pb2.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 13:33 arcticdb/scripts/__init__.py
--rw-rw-rw-  2.0 fat     3213 b- defN 24-May-04 13:33 arcticdb/scripts/update_storage.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 13:33 arcticdb/storage_fixtures/__init__.py
--rw-rw-rw-  2.0 fat     8162 b- defN 24-May-04 13:33 arcticdb/storage_fixtures/api.py
--rw-rw-rw-  2.0 fat     7402 b- defN 24-May-04 13:33 arcticdb/storage_fixtures/azure.py
--rw-rw-rw-  2.0 fat     1522 b- defN 24-May-04 13:33 arcticdb/storage_fixtures/in_memory.py
--rw-rw-rw-  2.0 fat     3881 b- defN 24-May-04 13:33 arcticdb/storage_fixtures/lmdb.py
--rw-rw-rw-  2.0 fat     6940 b- defN 24-May-04 13:33 arcticdb/storage_fixtures/mongo.py
--rw-rw-rw-  2.0 fat    14090 b- defN 24-May-04 13:33 arcticdb/storage_fixtures/s3.py
--rw-rw-rw-  2.0 fat     5622 b- defN 24-May-04 13:33 arcticdb/storage_fixtures/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 13:33 arcticdb/toolbox/__init__.py
--rw-rw-rw-  2.0 fat     5848 b- defN 24-May-04 13:33 arcticdb/toolbox/library_tool.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 13:33 arcticdb/util/__init__.py
--rw-rw-rw-  2.0 fat      599 b- defN 24-May-04 13:33 arcticdb/util/_versions.py
--rw-rw-rw-  2.0 fat     2705 b- defN 24-May-04 13:33 arcticdb/util/errors.py
--rw-rw-rw-  2.0 fat     9483 b- defN 24-May-04 13:33 arcticdb/util/hypothesis.py
--rw-rw-rw-  2.0 fat     6079 b- defN 24-May-04 13:33 arcticdb/util/tasks.py
--rw-rw-rw-  2.0 fat    17439 b- defN 24-May-04 13:33 arcticdb/util/test.py
--rw-rw-rw-  2.0 fat      131 b- defN 24-May-04 13:33 arcticdb/version_store/__init__.py
--rw-rw-rw-  2.0 fat     7812 b- defN 24-May-04 13:33 arcticdb/version_store/_common.py
--rw-rw-rw-  2.0 fat     4193 b- defN 24-May-04 13:33 arcticdb/version_store/_custom_normalizers.py
--rw-rw-rw-  2.0 fat    60214 b- defN 24-May-04 13:33 arcticdb/version_store/_normalization.py
--rw-rw-rw-  2.0 fat   123018 b- defN 24-May-04 13:33 arcticdb/version_store/_store.py
--rw-rw-rw-  2.0 fat    12208 b- defN 24-May-04 13:33 arcticdb/version_store/helper.py
--rw-rw-rw-  2.0 fat    72824 b- defN 24-May-04 13:33 arcticdb/version_store/library.py
--rw-rw-rw-  2.0 fat    29412 b- defN 24-May-04 13:33 arcticdb/version_store/processing.py
--rw-rw-rw-  2.0 fat      603 b- defN 24-May-04 13:33 arcticdb/version_store/read_result.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-04 13:33 benchmarks/__init__.py
--rw-rw-rw-  2.0 fat    12321 b- defN 24-May-04 13:33 benchmarks/basic_functions.py
--rw-rw-rw-  2.0 fat     2843 b- defN 24-May-04 13:33 benchmarks/common.py
--rw-rw-rw-  2.0 fat     1583 b- defN 24-May-04 13:33 benchmarks/list_functions.py
--rw-rw-rw-  2.0 fat     4786 b- defN 24-May-04 13:33 benchmarks/local_query_builder.py
--rw-rw-rw-  2.0 fat     3359 b- defN 24-May-04 13:33 benchmarks/persistent_query_builder.py
--rw-rw-rw-  2.0 fat     4851 b- defN 24-May-04 13:59 arcticdb-4.4.2rc0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     9943 b- defN 24-May-04 13:59 arcticdb-4.4.2rc0.dist-info/METADATA
--rw-rw-rw-  2.0 fat    19083 b- defN 24-May-04 13:59 arcticdb-4.4.2rc0.dist-info/NOTICE.txt
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-04 13:59 arcticdb-4.4.2rc0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       81 b- defN 24-May-04 13:59 arcticdb-4.4.2rc0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       41 b- defN 24-May-04 13:59 arcticdb-4.4.2rc0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     8600 b- defN 24-May-04 13:59 arcticdb-4.4.2rc0.dist-info/RECORD
-93 files, 21457911 bytes uncompressed, 6287460 bytes compressed:  70.7%
+Zip file size: 6287531 bytes, number of entries: 79
+-rw-rw-rw-  2.0 fat 20719616 b- defN 24-May-15 15:19 arcticdb_ext.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      302 b- defN 24-May-15 14:54 arcticc/__init__.py
+-rw-rw-rw-  2.0 fat     1508 b- defN 24-May-15 14:54 arcticc/pb2/__init__.py
+-rw-rw-rw-  2.0 fat      749 b- defN 24-May-15 14:54 arcticdb/__init__.py
+-rw-rw-rw-  2.0 fat      447 b- defN 24-May-15 14:54 arcticdb/_msgpack_compat.py
+-rw-rw-rw-  2.0 fat    15472 b- defN 24-May-15 14:54 arcticdb/arctic.py
+-rw-rw-rw-  2.0 fat     8619 b- defN 24-May-15 14:54 arcticdb/config.py
+-rw-rw-rw-  2.0 fat      429 b- defN 24-May-15 14:54 arcticdb/encoding_version.py
+-rw-rw-rw-  2.0 fat     1146 b- defN 24-May-15 14:54 arcticdb/exceptions.py
+-rw-rw-rw-  2.0 fat     9158 b- defN 24-May-15 14:54 arcticdb/flattener.py
+-rw-rw-rw-  2.0 fat     1897 b- defN 24-May-15 14:54 arcticdb/log.py
+-rw-rw-rw-  2.0 fat    10733 b- defN 24-May-15 14:54 arcticdb/options.py
+-rw-rw-rw-  2.0 fat      519 b- defN 24-May-15 14:54 arcticdb/preconditions.py
+-rw-rw-rw-  2.0 fat     2006 b- defN 24-May-15 14:54 arcticdb/supported_types.py
+-rw-rw-rw-  2.0 fat     3150 b- defN 24-May-15 14:54 arcticdb/tools.py
+-rw-rw-rw-  2.0 fat      284 b- defN 24-May-15 14:54 arcticdb/adapters/__init__.py
+-rw-rw-rw-  2.0 fat     4064 b- defN 24-May-15 14:54 arcticdb/adapters/arctic_library_adapter.py
+-rw-rw-rw-  2.0 fat     5488 b- defN 24-May-15 14:54 arcticdb/adapters/azure_library_adapter.py
+-rw-rw-rw-  2.0 fat     1906 b- defN 24-May-15 14:54 arcticdb/adapters/in_memory_library_adapter.py
+-rw-rw-rw-  2.0 fat     5974 b- defN 24-May-15 14:54 arcticdb/adapters/lmdb_library_adapter.py
+-rw-rw-rw-  2.0 fat     2763 b- defN 24-May-15 14:54 arcticdb/adapters/mongo_library_adapter.py
+-rw-rw-rw-  2.0 fat     3599 b- defN 24-May-15 14:54 arcticdb/adapters/prefixing_library_adapter_decorator.py
+-rw-rw-rw-  2.0 fat     8436 b- defN 24-May-15 14:54 arcticdb/adapters/s3_library_adapter.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-15 14:54 arcticdb/authorization/__init__.py
+-rw-rw-rw-  2.0 fat      969 b- defN 24-May-15 14:54 arcticdb/authorization/permissions.py
+-rw-rw-rw-  2.0 fat     1393 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/azure_storage_pb2.py
+-rw-rw-rw-  2.0 fat     2518 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/config_pb2.py
+-rw-rw-rw-  2.0 fat    16112 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/descriptors_pb2.py
+-rw-rw-rw-  2.0 fat     5654 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/encoding_pb2.py
+-rw-rw-rw-  2.0 fat     1070 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/in_memory_storage_pb2.py
+-rw-rw-rw-  2.0 fat     1524 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/lmdb_storage_pb2.py
+-rw-rw-rw-  2.0 fat     4478 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/logger_pb2.py
+-rw-rw-rw-  2.0 fat     1739 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/mapped_file_storage_pb2.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/mongo_storage_pb2.py
+-rw-rw-rw-  2.0 fat     1593 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/nfs_backed_storage_pb2.py
+-rw-rw-rw-  2.0 fat     1102 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/rocksdb_storage_pb2.py
+-rw-rw-rw-  2.0 fat     1627 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/s3_storage_pb2.py
+-rw-rw-rw-  2.0 fat    10801 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/storage_pb2.py
+-rw-rw-rw-  2.0 fat     2482 b- defN 24-May-15 14:58 arcticdb/proto/4/arcticc/pb2/utils_pb2.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-15 14:54 arcticdb/scripts/__init__.py
+-rw-rw-rw-  2.0 fat     3213 b- defN 24-May-15 14:54 arcticdb/scripts/update_storage.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-15 14:54 arcticdb/storage_fixtures/__init__.py
+-rw-rw-rw-  2.0 fat     8162 b- defN 24-May-15 14:54 arcticdb/storage_fixtures/api.py
+-rw-rw-rw-  2.0 fat     7402 b- defN 24-May-15 14:54 arcticdb/storage_fixtures/azure.py
+-rw-rw-rw-  2.0 fat     1522 b- defN 24-May-15 14:54 arcticdb/storage_fixtures/in_memory.py
+-rw-rw-rw-  2.0 fat     3881 b- defN 24-May-15 14:54 arcticdb/storage_fixtures/lmdb.py
+-rw-rw-rw-  2.0 fat     6940 b- defN 24-May-15 14:54 arcticdb/storage_fixtures/mongo.py
+-rw-rw-rw-  2.0 fat    14090 b- defN 24-May-15 14:54 arcticdb/storage_fixtures/s3.py
+-rw-rw-rw-  2.0 fat     5622 b- defN 24-May-15 14:54 arcticdb/storage_fixtures/utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-15 14:54 arcticdb/toolbox/__init__.py
+-rw-rw-rw-  2.0 fat     5848 b- defN 24-May-15 14:54 arcticdb/toolbox/library_tool.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-15 14:54 arcticdb/util/__init__.py
+-rw-rw-rw-  2.0 fat      599 b- defN 24-May-15 14:54 arcticdb/util/_versions.py
+-rw-rw-rw-  2.0 fat     2705 b- defN 24-May-15 14:54 arcticdb/util/errors.py
+-rw-rw-rw-  2.0 fat     9483 b- defN 24-May-15 14:54 arcticdb/util/hypothesis.py
+-rw-rw-rw-  2.0 fat     6079 b- defN 24-May-15 14:54 arcticdb/util/tasks.py
+-rw-rw-rw-  2.0 fat    17439 b- defN 24-May-15 14:54 arcticdb/util/test.py
+-rw-rw-rw-  2.0 fat      131 b- defN 24-May-15 14:54 arcticdb/version_store/__init__.py
+-rw-rw-rw-  2.0 fat     7812 b- defN 24-May-15 14:54 arcticdb/version_store/_common.py
+-rw-rw-rw-  2.0 fat     4193 b- defN 24-May-15 14:54 arcticdb/version_store/_custom_normalizers.py
+-rw-rw-rw-  2.0 fat    60214 b- defN 24-May-15 14:54 arcticdb/version_store/_normalization.py
+-rw-rw-rw-  2.0 fat   123018 b- defN 24-May-15 14:54 arcticdb/version_store/_store.py
+-rw-rw-rw-  2.0 fat    12208 b- defN 24-May-15 14:54 arcticdb/version_store/helper.py
+-rw-rw-rw-  2.0 fat    72824 b- defN 24-May-15 14:54 arcticdb/version_store/library.py
+-rw-rw-rw-  2.0 fat    29412 b- defN 24-May-15 14:54 arcticdb/version_store/processing.py
+-rw-rw-rw-  2.0 fat      603 b- defN 24-May-15 14:54 arcticdb/version_store/read_result.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-15 14:54 benchmarks/__init__.py
+-rw-rw-rw-  2.0 fat    12321 b- defN 24-May-15 14:54 benchmarks/basic_functions.py
+-rw-rw-rw-  2.0 fat     2843 b- defN 24-May-15 14:54 benchmarks/common.py
+-rw-rw-rw-  2.0 fat     1583 b- defN 24-May-15 14:54 benchmarks/list_functions.py
+-rw-rw-rw-  2.0 fat     4786 b- defN 24-May-15 14:54 benchmarks/local_query_builder.py
+-rw-rw-rw-  2.0 fat     3359 b- defN 24-May-15 14:54 benchmarks/persistent_query_builder.py
+-rw-rw-rw-  2.0 fat     4851 b- defN 24-May-15 15:19 arcticdb-4.4.3rc0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     9943 b- defN 24-May-15 15:19 arcticdb-4.4.3rc0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat    19083 b- defN 24-May-15 15:19 arcticdb-4.4.3rc0.dist-info/NOTICE.txt
+-rw-rw-rw-  2.0 fat      102 b- defN 24-May-15 15:19 arcticdb-4.4.3rc0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       81 b- defN 24-May-15 15:19 arcticdb-4.4.3rc0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       41 b- defN 24-May-15 15:19 arcticdb-4.4.3rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     7134 b- defN 24-May-15 15:19 arcticdb-4.4.3rc0.dist-info/RECORD
+79 files, 21332206 bytes uncompressed, 6276105 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: arcticdb_ext.cp39-win_amd64.pyd
+Filename: arcticdb_ext.cp311-win_amd64.pyd
 Comment: 
 
 Filename: arcticc/__init__.py
 Comment: 
 
 Filename: arcticc/pb2/__init__.py
 Comment: 
@@ -69,56 +69,14 @@
 
 Filename: arcticdb/authorization/__init__.py
 Comment: 
 
 Filename: arcticdb/authorization/permissions.py
 Comment: 
 
-Filename: arcticdb/proto/3/arcticc/pb2/azure_storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/config_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/descriptors_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/encoding_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/in_memory_storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/lmdb_storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/logger_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/mapped_file_storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/mongo_storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/nfs_backed_storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/rocksdb_storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/s3_storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/storage_pb2.py
-Comment: 
-
-Filename: arcticdb/proto/3/arcticc/pb2/utils_pb2.py
-Comment: 
-
 Filename: arcticdb/proto/4/arcticc/pb2/azure_storage_pb2.py
 Comment: 
 
 Filename: arcticdb/proto/4/arcticc/pb2/config_pb2.py
 Comment: 
 
 Filename: arcticdb/proto/4/arcticc/pb2/descriptors_pb2.py
@@ -252,29 +210,29 @@
 
 Filename: benchmarks/local_query_builder.py
 Comment: 
 
 Filename: benchmarks/persistent_query_builder.py
 Comment: 
 
-Filename: arcticdb-4.4.2rc0.dist-info/LICENSE.txt
+Filename: arcticdb-4.4.3rc0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: arcticdb-4.4.2rc0.dist-info/METADATA
+Filename: arcticdb-4.4.3rc0.dist-info/METADATA
 Comment: 
 
-Filename: arcticdb-4.4.2rc0.dist-info/NOTICE.txt
+Filename: arcticdb-4.4.3rc0.dist-info/NOTICE.txt
 Comment: 
 
-Filename: arcticdb-4.4.2rc0.dist-info/WHEEL
+Filename: arcticdb-4.4.3rc0.dist-info/WHEEL
 Comment: 
 
-Filename: arcticdb-4.4.2rc0.dist-info/entry_points.txt
+Filename: arcticdb-4.4.3rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: arcticdb-4.4.2rc0.dist-info/top_level.txt
+Filename: arcticdb-4.4.3rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: arcticdb-4.4.2rc0.dist-info/RECORD
+Filename: arcticdb-4.4.3rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## arcticdb/__init__.py

```diff
@@ -11,8 +11,8 @@
 from arcticdb_ext.version_store import DataError, VersionRequestType
 from arcticdb_ext.exceptions import ErrorCode, ErrorCategory
 from arcticdb.version_store.library import WritePayload, ReadInfoRequest, ReadRequest
 from arcticdb.version_store.library import StagedDataFinalizeMethod, WriteMetadataPayload
 
 set_config_from_env_vars(_os.environ)
 
-__version__ = "4.4.2rc0"
+__version__ = "4.4.3rc0"
```

## Comparing `arcticdb-4.4.2rc0.dist-info/LICENSE.txt` & `arcticdb-4.4.3rc0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `arcticdb-4.4.2rc0.dist-info/METADATA` & `arcticdb-4.4.3rc0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcticdb
-Version: 4.4.2rc0
+Version: 4.4.3rc0
 Summary: ArcticDB DataFrame Database
 Home-page: https://github.com/man-group/arcticdb
 Author: Man Alpha Technology
 Author-email: arcticdb@man.com
 License: Business Source License 1.1 (See LICENSE.txt)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arcticdb Version: 4.4.2rc0 Summary: ArcticDB
+Metadata-Version: 2.1 Name: arcticdb Version: 4.4.3rc0 Summary: ArcticDB
 DataFrame Database Home-page: https://github.com/man-group/arcticdb Author: Man
 Alpha Technology Author-email: arcticdb@man.com License: Business Source
 License 1.1 (See LICENSE.txt) Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
 Microsoft :: Windows Classifier: Topic :: Database Classifier: Topic ::
 Database :: Database Engines/Servers Description-Content-Type: text/markdown
 License-File: LICENSE.txt License-File: NOTICE.txt Requires-Dist: numpy
```

## Comparing `arcticdb-4.4.2rc0.dist-info/NOTICE.txt` & `arcticdb-4.4.3rc0.dist-info/NOTICE.txt`

 * *Files identical despite different names*

## Comparing `arcticdb-4.4.2rc0.dist-info/RECORD` & `arcticdb-4.4.3rc0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-arcticdb_ext.cp39-win_amd64.pyd,sha256=f_3xx-8F4fjIJ8MP27ov_ZqM17b6uwKKYUjdLDyBxps,20562432
+arcticdb_ext.cp311-win_amd64.pyd,sha256=BHET197iykJz9weRyzmDdkCgo6_yOkZQgmzv1o9_rcI,20719616
 arcticc/__init__.py,sha256=TgMgqqJDwst6cvC4-whG_3DQOzyry3fRe8HxvE_jrPM,302
 arcticc/pb2/__init__.py,sha256=GpuYw9AtQz-EGOqyKjeyjdc0l9yZV0RUtbkW49U5i-4,1508
-arcticdb/__init__.py,sha256=EChxf5wU6fLtUr7d6cyPbXwQBPL-AxNaGClG8uJ8bsg,749
+arcticdb/__init__.py,sha256=AwjmWJCQwqIp9WyI3BrBY1HU5zgexPeA3rjqSHhxki0,749
 arcticdb/_msgpack_compat.py,sha256=i_3HluY89KVSXFnxC-UjcdK0zNsIcSBLmY3YpKFeLl8,447
 arcticdb/arctic.py,sha256=bI70pcMbGcfqG0-YIgftMAgJdCiA2d6hMZZrYeDRtA0,15472
 arcticdb/config.py,sha256=NOp3kk2ToD48TAhTPj94a98fiLqK91DGCDsO-8JjlOI,8619
 arcticdb/encoding_version.py,sha256=vRHz5oyP06Wa_NFDxDBHrQaHMHx8QWN3RMAqenVgeS4,429
 arcticdb/exceptions.py,sha256=SEk8eBUqMNaP18oRXUddhZF585eguY6zEs43ZwAl5C8,1146
 arcticdb/flattener.py,sha256=2zfEcOHbbwiPn5wOy7UmiR8u53-MmQcS_2UBT3Gzlo8,9158
 arcticdb/log.py,sha256=zRbg8u9EwfZ-QSspK1ub5YwYwUi1ruZc08-WDPonMv4,1897
@@ -19,28 +19,14 @@
 arcticdb/adapters/in_memory_library_adapter.py,sha256=p_DiFcYorTzNddXvcgqxEeq0Ip_7eycVZObrXDuYPVI,1906
 arcticdb/adapters/lmdb_library_adapter.py,sha256=C0Z4pg4T1ahsFlPRErGoAh-Roi7VzNyITZyMnPscdmc,5974
 arcticdb/adapters/mongo_library_adapter.py,sha256=MMfNS2bVA4TfJ0DXSF-l520oxi3X2TPC6BXnusdfdMk,2763
 arcticdb/adapters/prefixing_library_adapter_decorator.py,sha256=gh6BoNTD_kqneb7W7w-CdemDychq3Vn36VE32RVEp5o,3599
 arcticdb/adapters/s3_library_adapter.py,sha256=FWErc5KkkYFpKmGmoSjTGKtLkM0kzI6J1lRSzMtBxEo,8436
 arcticdb/authorization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 arcticdb/authorization/permissions.py,sha256=3E91GMrL6xSEKloOWdIGdaKrHfHoqhkSEqJwjJZJ3HQ,969
-arcticdb/proto/3/arcticc/pb2/azure_storage_pb2.py,sha256=v7LhaW518oPZKNiRmcnTEmn7zqO7CD-QQ5n-914GsEE,4669
-arcticdb/proto/3/arcticc/pb2/config_pb2.py,sha256=W1pb3T1ArzmExVkjgF3xWn5WMWL5l9fR7rR0unnKhxE,8935
-arcticdb/proto/3/arcticc/pb2/descriptors_pb2.py,sha256=IDAF6pQqb2ZyeThlX0ngsahGteBEZXKY6vfNPjupegE,98342
-arcticdb/proto/3/arcticc/pb2/encoding_pb2.py,sha256=qT9YxRLKuFdjw0GPKtUEUhw8uDfGL2ve8A2ZZk-LlA4,31651
-arcticdb/proto/3/arcticc/pb2/in_memory_storage_pb2.py,sha256=GMLd0-psYcHfHauhM43-9y0leeRLw7RnxHYyD2dpk4o,1561
-arcticdb/proto/3/arcticc/pb2/lmdb_storage_pb2.py,sha256=nPGOr0k4IentCSviXMfG4CEl2KGrfYqaOnfkZOw1GnQ,5111
-arcticdb/proto/3/arcticc/pb2/logger_pb2.py,sha256=N2KLqqE3Q1mLPVMW6IDbJ72eTxIJEH-BHvAVNOOLg4I,24224
-arcticdb/proto/3/arcticc/pb2/mapped_file_storage_pb2.py,sha256=mwIq_FIjw4ystjXLUydrwB5oin1zbEq2RIdiSOnoykg,6142
-arcticdb/proto/3/arcticc/pb2/mongo_storage_pb2.py,sha256=u9iJy3eF_bGtDqsO5d7zQF3k9psxmRYfHsGL6XGauo0,3409
-arcticdb/proto/3/arcticc/pb2/nfs_backed_storage_pb2.py,sha256=1ZnNdkR-Zbg_2GsDOPPDWObbZdFO7xOousPky27WTyU,6878
-arcticdb/proto/3/arcticc/pb2/rocksdb_storage_pb2.py,sha256=T5z7n8AV_R_j8c1ziWjKDQPLsnpQYHXxo-LlV8QwgHg,1974
-arcticdb/proto/3/arcticc/pb2/s3_storage_pb2.py,sha256=YS73swFG8CxArfbJmgScysiWOU83unRjYi8-YeujzOs,7204
-arcticdb/proto/3/arcticc/pb2/storage_pb2.py,sha256=1sVVq22ZjmKDwFnS7DryklsSPQRn6X6psabtOxDI7lE,68704
-arcticdb/proto/3/arcticc/pb2/utils_pb2.py,sha256=VVissg-IkyLhDcT8v2Axy2OcMp704bxqqI-oYCQKECo,12621
 arcticdb/proto/4/arcticc/pb2/azure_storage_pb2.py,sha256=uzCn33ZttMy_f75sp-qOMLhUX-iJuVXky8BGihhlq1s,1393
 arcticdb/proto/4/arcticc/pb2/config_pb2.py,sha256=_9is6zvURPHt1fjB95lH1SYXt05PCeGqXvY6xfsmicA,2518
 arcticdb/proto/4/arcticc/pb2/descriptors_pb2.py,sha256=OYVQ3VNJBX8d4f0r6Sb5EasT1ZRzeC8cKlCOSFjpcHk,16112
 arcticdb/proto/4/arcticc/pb2/encoding_pb2.py,sha256=JNXlrXagsQkHWOqynIzvbKP0YKdrLU9-PZx50sEBMNQ,5654
 arcticdb/proto/4/arcticc/pb2/in_memory_storage_pb2.py,sha256=dssuEpbS80VS6xWUG8thiDdmFvbmEz01eaAmGkbP7cw,1070
 arcticdb/proto/4/arcticc/pb2/lmdb_storage_pb2.py,sha256=GFGzZVKO_Q5u0OheX2zLO5UZMpOSobs2vH_wfkYwpn8,1524
 arcticdb/proto/4/arcticc/pb2/logger_pb2.py,sha256=RRYIdSSvWS-vblKslp8pgeePefIXE2WOo7UMjskCMNc,4478
@@ -80,14 +66,14 @@
 arcticdb/version_store/read_result.py,sha256=5HhAJ0Wh01f111qA5XvWqOXABO-2H0jZ78kx-iiQzOk,603
 benchmarks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 benchmarks/basic_functions.py,sha256=yv-9lhJLgI8oX9rVq7cDd-h9qP1J0alt90DPvXSYn5g,12321
 benchmarks/common.py,sha256=Ei73yefIWGc4XR77vb4VJAwPX-cShT9Zssrz7FHHlIU,2843
 benchmarks/list_functions.py,sha256=S1Zgk7W2srbCebYkXADni5pucJz-1JzXUVQHVXMqJ1A,1583
 benchmarks/local_query_builder.py,sha256=zd6EAWrjv02CVAq4blE6UtAXQv8pCmilRhJjT38Kch4,4786
 benchmarks/persistent_query_builder.py,sha256=1ZPaCZ6cEBphJOrbCvUukc63iJmBAsPOI9QOLsyM5XM,3359
-arcticdb-4.4.2rc0.dist-info/LICENSE.txt,sha256=ruvCXWZm0cgyb-XAEjFcfdJkJ_nGbv9gsYNeps514Ys,4851
-arcticdb-4.4.2rc0.dist-info/METADATA,sha256=h21VWZilrAshzssrKLlzVkpDJvTO_dXcUXR35gbtbQA,9943
-arcticdb-4.4.2rc0.dist-info/NOTICE.txt,sha256=b2JkaWSaLTBu5IAbhydxaW5-03nXcYi_kjQIHhLwDEg,19083
-arcticdb-4.4.2rc0.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-arcticdb-4.4.2rc0.dist-info/entry_points.txt,sha256=kjWBBV4t6WBbf7wZZeKFZA8HRSDvYL870_GUURC8xUs,81
-arcticdb-4.4.2rc0.dist-info/top_level.txt,sha256=MCkYLYcLX-7nafd0NWXRDSfbk1ej8dYre7YXYbfYt6c,41
-arcticdb-4.4.2rc0.dist-info/RECORD,,
+arcticdb-4.4.3rc0.dist-info/LICENSE.txt,sha256=ruvCXWZm0cgyb-XAEjFcfdJkJ_nGbv9gsYNeps514Ys,4851
+arcticdb-4.4.3rc0.dist-info/METADATA,sha256=O_Z0Xy7cEUn9EdnMyTocwpPD_ngjyYHlCvGFYJc_RGs,9943
+arcticdb-4.4.3rc0.dist-info/NOTICE.txt,sha256=b2JkaWSaLTBu5IAbhydxaW5-03nXcYi_kjQIHhLwDEg,19083
+arcticdb-4.4.3rc0.dist-info/WHEEL,sha256=wklNeoByNLhdCl-oEQTdaHIeDl4q9zaQVqAlPxUEgLU,102
+arcticdb-4.4.3rc0.dist-info/entry_points.txt,sha256=kjWBBV4t6WBbf7wZZeKFZA8HRSDvYL870_GUURC8xUs,81
+arcticdb-4.4.3rc0.dist-info/top_level.txt,sha256=MCkYLYcLX-7nafd0NWXRDSfbk1ej8dYre7YXYbfYt6c,41
+arcticdb-4.4.3rc0.dist-info/RECORD,,
```

