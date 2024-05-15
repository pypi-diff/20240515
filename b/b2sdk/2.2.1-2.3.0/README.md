# Comparing `tmp/b2sdk-2.2.1.tar.gz` & `tmp/b2sdk-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sdk-2.2.1.tar", last modified: Thu May  9 11:12:15 2024, max compression
+gzip compressed data, was "b2sdk-2.3.0.tar", last modified: Wed May 15 12:37:05 2024, max compression
```

## Comparing `b2sdk-2.2.1.tar` & `b2sdk-2.3.0.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0    11963 2024-05-09 11:12:02.112265 b2sdk-2.2.1/LICENSE
--rw-r--r--   0        0        0     2219 2024-05-09 11:12:02.112265 b2sdk-2.2.1/README.md
-lrwxr-xr-x   0        0        0        0 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0      422 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/__init__.py
--rw-r--r--   0        0        0      319 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/__main__.py
--rw-r--r--   0        0        0      443 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/__init__.py
--rw-r--r--   0        0        0      414 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/account_info/__init__.py
--rw-r--r--   0        0        0    12688 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/account_info/abstract.py
--rw-r--r--   0        0        0     1381 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/account_info/exception.py
--rw-r--r--   0        0        0     4400 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/account_info/in_memory.py
--rw-r--r--   0        0        0    24095 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/account_info/sqlite_account_info.py
--rw-r--r--   0        0        0     4349 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/account_info/stub.py
--rw-r--r--   0        0        0     3534 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/account_info/upload_url_pool.py
--rw-r--r--   0        0        0    26244 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/api.py
--rw-r--r--   0        0        0     1748 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/api_config.py
--rw-r--r--   0        0        0     5835 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/application_key.py
--rw-r--r--   0        0        0    21710 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/b2http.py
--rw-r--r--   0        0        0     2316 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/bounded_queue_executor.py
--rw-r--r--   0        0        0    80634 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/bucket.py
--rw-r--r--   0        0        0     3746 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/cache.py
--rw-r--r--   0        0        0      340 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/encryption/__init__.py
--rw-r--r--   0        0        0    12661 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/encryption/setting.py
--rw-r--r--   0        0        0     1433 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/encryption/types.py
--rw-r--r--   0        0        0    20991 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/exception.py
--rw-r--r--   0        0        0    13765 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/file_lock.py
--rw-r--r--   0        0        0    23877 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/file_version.py
--rw-r--r--   0        0        0     1997 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/filter.py
--rw-r--r--   0        0        0     1555 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/http_constants.py
--rw-r--r--   0        0        0      863 2024-05-09 11:12:02.112265 b2sdk-2.2.1/b2sdk/_internal/included_sources.py
--rw-r--r--   0        0        0      340 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/large_file/__init__.py
--rw-r--r--   0        0        0     1496 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/large_file/part.py
--rw-r--r--   0        0        0     4777 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/large_file/services.py
--rw-r--r--   0        0        0     2923 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/large_file/unfinished_large_file.py
--rw-r--r--   0        0        0     7131 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/progress.py
--rw-r--r--   0        0        0    39883 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/raw_api.py
--rw-r--r--   0        0        0    80006 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/raw_simulator.py
--rw-r--r--   0        0        0      341 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/replication/__init__.py
--rw-r--r--   0        0        0     8707 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/replication/monitoring.py
--rw-r--r--   0        0        0     7331 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/replication/setting.py
--rw-r--r--   0        0        0    13198 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/replication/setup.py
--rw-r--r--   0        0        0      710 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/replication/types.py
--rw-r--r--   0        0        0    10141 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/requests/LICENSE
--rw-r--r--   0        0        0      289 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/requests/NOTICE
--rw-r--r--   0        0        0      232 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/requests/README.md
--rw-r--r--   0        0        0     3275 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/requests/__init__.py
--rw-r--r--   0        0        0      868 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/requests/included_source_meta.py
--rw-r--r--   0        0        0      334 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/scan/__init__.py
--rw-r--r--   0        0        0     2880 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/scan/exception.py
--rw-r--r--   0        0        0    15885 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/scan/folder.py
--rw-r--r--   0        0        0     2021 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/scan/folder_parser.py
--rw-r--r--   0        0        0     2724 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/scan/path.py
--rw-r--r--   0        0        0     9060 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/scan/policies.py
--rw-r--r--   0        0        0     6879 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/scan/report.py
--rw-r--r--   0        0        0     3935 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/scan/scan.py
--rw-r--r--   0        0        0    21244 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/session.py
--rw-r--r--   0        0        0      615 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/stream/__init__.py
--rw-r--r--   0        0        0      531 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/stream/base.py
--rw-r--r--   0        0        0     5273 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/stream/chained.py
--rw-r--r--   0        0        0     2389 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/stream/hashing.py
--rw-r--r--   0        0        0     3100 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/stream/progress.py
--rw-r--r--   0        0        0     2597 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/stream/range.py
--rw-r--r--   0        0        0     2278 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/stream/wrapper.py
--rw-r--r--   0        0        0      334 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/sync/__init__.py
--rw-r--r--   0        0        0    18071 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/sync/action.py
--rw-r--r--   0        0        0     3901 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/sync/encryption_provider.py
--rw-r--r--   0        0        0      422 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/sync/exception.py
--rw-r--r--   0        0        0    18364 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/sync/policy.py
--rw-r--r--   0        0        0     4378 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/sync/policy_manager.py
--rw-r--r--   0        0        0     6351 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/sync/report.py
--rw-r--r--   0        0        0    14535 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/sync/sync.py
--rw-r--r--   0        0        0      620 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/__init__.py
--rw-r--r--   0        0        0      345 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/__init__.py
--rw-r--r--   0        0        0    14793 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/emerger.py
--rw-r--r--   0        0        0      556 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/exception.py
--rw-r--r--   0        0        0    29077 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/executor.py
--rw-r--r--   0        0        0      353 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/planner/__init__.py
--rw-r--r--   0        0        0     5456 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/planner/part_definition.py
--rw-r--r--   0        0        0    32575 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/planner/planner.py
--rw-r--r--   0        0        0     3582 2024-05-09 11:12:02.116265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py
--rw-r--r--   0        0        0     8394 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/unbound_write_intent.py
--rw-r--r--   0        0        0     3229 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/write_intent.py
--rw-r--r--   0        0        0      346 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/__init__.py
--rw-r--r--   0        0        0     4399 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/download_manager.py
--rw-r--r--   0        0        0    10032 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloaded_file.py
--rw-r--r--   0        0        0      357 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/__init__.py
--rw-r--r--   0        0        0     5098 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/abstract.py
--rw-r--r--   0        0        0    18422 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/parallel.py
--rw-r--r--   0        0        0     3702 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/simple.py
--rw-r--r--   0        0        0     3114 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py
--rw-r--r--   0        0        0      347 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/__init__.py
--rw-r--r--   0        0        0    10338 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/copy_manager.py
--rw-r--r--   0        0        0     3118 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/copy_source.py
--rw-r--r--   0        0        0     2114 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/large_file_upload_state.py
--rw-r--r--   0        0        0     1804 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/outbound_source.py
--rw-r--r--   0        0        0     1625 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/progress_reporter.py
--rw-r--r--   0        0        0     9583 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/upload_manager.py
--rw-r--r--   0        0        0    13100 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/upload_source.py
--rw-r--r--   0        0        0      560 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/transfer/transfer_manager.py
--rw-r--r--   0        0        0    14906 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1561 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/utils/docs.py
--rw-r--r--   0        0        0     1659 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/utils/escape.py
--rw-r--r--   0        0        0      948 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/utils/filesystem.py
--rw-r--r--   0        0        0     1186 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/utils/http_date.py
--rw-r--r--   0        0        0     1660 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/utils/range_.py
--rw-r--r--   0        0        0     3546 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/utils/thread_pool.py
--rw-r--r--   0        0        0      561 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/utils/typing.py
--rw-r--r--   0        0        0     7160 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_internal/version_utils.py
--rw-r--r--   0        0        0      551 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_pyinstaller/__init__.py
--rw-r--r--   0        0        0      417 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_pyinstaller/hook-b2sdk.py
--rw-r--r--   0        0        0    12542 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_v3/__init__.py
--rw-r--r--   0        0        0     7083 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/_v3/exception.py
--rw-r--r--   0        0        0      705 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v0/__init__.py
--rw-r--r--   0        0        0     2035 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v0/account_info.py
--rw-r--r--   0        0        0      999 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v0/api.py
--rw-r--r--   0        0        0     1078 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v0/bucket.py
--rw-r--r--   0        0        0      969 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v0/exception.py
--rw-r--r--   0        0        0     7245 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v0/sync.py
--rw-r--r--   0        0        0     1351 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/__init__.py
--rw-r--r--   0        0        0     5908 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/account_info.py
--rw-r--r--   0        0        0     8348 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/api.py
--rw-r--r--   0        0        0     1927 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/b2http.py
--rw-r--r--   0        0        0    13668 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/bucket.py
--rw-r--r--   0        0        0      530 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/cache.py
--rw-r--r--   0        0        0     6787 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/download_dest.py
--rw-r--r--   0        0        0     1580 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/exception.py
--rw-r--r--   0        0        0     2218 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/file_metadata.py
--rw-r--r--   0        0        0     7019 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/file_version.py
--rw-r--r--   0        0        0      334 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/replication/__init__.py
--rw-r--r--   0        0        0     1148 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/replication/monitoring.py
--rw-r--r--   0        0        0     2596 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/session.py
--rw-r--r--   0        0        0      505 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/__init__.py
--rw-r--r--   0        0        0     3869 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/encryption_provider.py
--rw-r--r--   0        0        0     3849 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/file.py
--rw-r--r--   0        0        0     2816 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/file_to_path_translator.py
--rw-r--r--   0        0        0     2318 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/folder.py
--rw-r--r--   0        0        0      738 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/folder_parser.py
--rw-r--r--   0        0        0      846 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/report.py
--rw-r--r--   0        0        0     6929 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/scan_policies.py
--rw-r--r--   0        0        0     5387 2024-05-09 11:12:02.120265 b2sdk-2.2.1/b2sdk/v1/sync/sync.py
--rw-r--r--   0        0        0     1356 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/__init__.py
--rw-r--r--   0        0        0      454 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/_compat.py
--rw-r--r--   0        0        0      494 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/account_info.py
--rw-r--r--   0        0        0     2235 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/api.py
--rw-r--r--   0        0        0      804 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/b2http.py
--rw-r--r--   0        0        0     3086 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/bucket.py
--rw-r--r--   0        0        0      803 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/exception.py
--rw-r--r--   0        0        0     2902 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/file_version.py
--rw-r--r--   0        0        0     1339 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/large_file.py
--rw-r--r--   0        0        0     2751 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/raw_api.py
--rw-r--r--   0        0        0     3704 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/raw_simulator.py
--rw-r--r--   0        0        0     1523 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/session.py
--rw-r--r--   0        0        0      369 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/sync.py
--rw-r--r--   0        0        0      584 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/transfer.py
--rw-r--r--   0        0        0     1033 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/utils.py
--rw-r--r--   0        0        0     1612 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/v2/version_utils.py
--rw-r--r--   0        0        0      767 2024-05-09 11:12:02.124265 b2sdk-2.2.1/b2sdk/version.py
--rw-r--r--   0        0        0     4436 2024-05-09 11:12:15.044209 b2sdk-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 b2sdk-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11963 2024-05-15 12:36:52.332543 b2sdk-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2219 2024-05-15 12:36:52.332543 b2sdk-2.3.0/README.md
+lrwxr-xr-x   0        0        0        0 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0      422 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/__init__.py
+-rw-r--r--   0        0        0      319 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/__main__.py
+-rw-r--r--   0        0        0      443 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/__init__.py
+-rw-r--r--   0        0        0      414 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/account_info/__init__.py
+-rw-r--r--   0        0        0    12688 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/account_info/abstract.py
+-rw-r--r--   0        0        0     1381 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/account_info/exception.py
+-rw-r--r--   0        0        0     4400 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/account_info/in_memory.py
+-rw-r--r--   0        0        0    24095 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/account_info/sqlite_account_info.py
+-rw-r--r--   0        0        0     4349 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/account_info/stub.py
+-rw-r--r--   0        0        0     3534 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/account_info/upload_url_pool.py
+-rw-r--r--   0        0        0    26244 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/api.py
+-rw-r--r--   0        0        0     1748 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/api_config.py
+-rw-r--r--   0        0        0     5835 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/application_key.py
+-rw-r--r--   0        0        0    21710 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/b2http.py
+-rw-r--r--   0        0        0     2316 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/bounded_queue_executor.py
+-rw-r--r--   0        0        0    81452 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/bucket.py
+-rw-r--r--   0        0        0     3746 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/cache.py
+-rw-r--r--   0        0        0      340 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/encryption/__init__.py
+-rw-r--r--   0        0        0    12661 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/encryption/setting.py
+-rw-r--r--   0        0        0     1433 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/encryption/types.py
+-rw-r--r--   0        0        0    20991 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/exception.py
+-rw-r--r--   0        0        0    13765 2024-05-15 12:36:52.332543 b2sdk-2.3.0/b2sdk/_internal/file_lock.py
+-rw-r--r--   0        0        0    23877 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/file_version.py
+-rw-r--r--   0        0        0     1997 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/filter.py
+-rw-r--r--   0        0        0     1555 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/http_constants.py
+-rw-r--r--   0        0        0      863 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/included_sources.py
+-rw-r--r--   0        0        0      340 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/large_file/__init__.py
+-rw-r--r--   0        0        0     1496 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/large_file/part.py
+-rw-r--r--   0        0        0     4777 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/large_file/services.py
+-rw-r--r--   0        0        0     2923 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/large_file/unfinished_large_file.py
+-rw-r--r--   0        0        0     7131 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/progress.py
+-rw-r--r--   0        0        0    39883 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/raw_api.py
+-rw-r--r--   0        0        0    80006 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/raw_simulator.py
+-rw-r--r--   0        0        0      341 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/replication/__init__.py
+-rw-r--r--   0        0        0     8707 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/replication/monitoring.py
+-rw-r--r--   0        0        0     7331 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/replication/setting.py
+-rw-r--r--   0        0        0    13198 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/replication/setup.py
+-rw-r--r--   0        0        0      710 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/replication/types.py
+-rw-r--r--   0        0        0    10141 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/requests/LICENSE
+-rw-r--r--   0        0        0      289 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/requests/NOTICE
+-rw-r--r--   0        0        0      232 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/requests/README.md
+-rw-r--r--   0        0        0     3275 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/requests/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/requests/included_source_meta.py
+-rw-r--r--   0        0        0      334 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/scan/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/scan/exception.py
+-rw-r--r--   0        0        0    15885 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/scan/folder.py
+-rw-r--r--   0        0        0     2021 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/scan/folder_parser.py
+-rw-r--r--   0        0        0     2724 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/scan/path.py
+-rw-r--r--   0        0        0     9060 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/scan/policies.py
+-rw-r--r--   0        0        0     6879 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/scan/report.py
+-rw-r--r--   0        0        0     3935 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/scan/scan.py
+-rw-r--r--   0        0        0    21244 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/session.py
+-rw-r--r--   0        0        0      615 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/stream/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/stream/base.py
+-rw-r--r--   0        0        0     5273 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/stream/chained.py
+-rw-r--r--   0        0        0     2389 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/stream/hashing.py
+-rw-r--r--   0        0        0     3100 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/stream/progress.py
+-rw-r--r--   0        0        0     2597 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/stream/range.py
+-rw-r--r--   0        0        0     2278 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/stream/wrapper.py
+-rw-r--r--   0        0        0      334 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/sync/__init__.py
+-rw-r--r--   0        0        0    18071 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/sync/action.py
+-rw-r--r--   0        0        0     3901 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/sync/encryption_provider.py
+-rw-r--r--   0        0        0      422 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/sync/exception.py
+-rw-r--r--   0        0        0    18364 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/sync/policy.py
+-rw-r--r--   0        0        0     4378 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/sync/policy_manager.py
+-rw-r--r--   0        0        0     6351 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/sync/report.py
+-rw-r--r--   0        0        0    14535 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/sync/sync.py
+-rw-r--r--   0        0        0      620 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/transfer/__init__.py
+-rw-r--r--   0        0        0      345 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/__init__.py
+-rw-r--r--   0        0        0    14793 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/emerger.py
+-rw-r--r--   0        0        0      556 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/exception.py
+-rw-r--r--   0        0        0    29077 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/executor.py
+-rw-r--r--   0        0        0      353 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/planner/__init__.py
+-rw-r--r--   0        0        0     5456 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py
+-rw-r--r--   0        0        0    32575 2024-05-15 12:36:52.336543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/planner/planner.py
+-rw-r--r--   0        0        0     3582 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py
+-rw-r--r--   0        0        0     8394 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py
+-rw-r--r--   0        0        0     3229 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/write_intent.py
+-rw-r--r--   0        0        0      346 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/__init__.py
+-rw-r--r--   0        0        0     4399 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/download_manager.py
+-rw-r--r--   0        0        0    10032 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloaded_file.py
+-rw-r--r--   0        0        0      357 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/__init__.py
+-rw-r--r--   0        0        0     5098 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py
+-rw-r--r--   0        0        0    18422 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py
+-rw-r--r--   0        0        0     3702 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/simple.py
+-rw-r--r--   0        0        0     3114 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py
+-rw-r--r--   0        0        0      347 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/__init__.py
+-rw-r--r--   0        0        0    10338 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/copy_manager.py
+-rw-r--r--   0        0        0     3118 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/copy_source.py
+-rw-r--r--   0        0        0     2114 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py
+-rw-r--r--   0        0        0     1804 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/outbound_source.py
+-rw-r--r--   0        0        0     1625 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/progress_reporter.py
+-rw-r--r--   0        0        0     9583 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/upload_manager.py
+-rw-r--r--   0        0        0    13100 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/upload_source.py
+-rw-r--r--   0        0        0      560 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/transfer/transfer_manager.py
+-rw-r--r--   0        0        0    14906 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1561 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/utils/docs.py
+-rw-r--r--   0        0        0     1659 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/utils/escape.py
+-rw-r--r--   0        0        0      948 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0     1186 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/utils/http_date.py
+-rw-r--r--   0        0        0     1660 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/utils/range_.py
+-rw-r--r--   0        0        0     3546 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/utils/thread_pool.py
+-rw-r--r--   0        0        0      561 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/utils/typing.py
+-rw-r--r--   0        0        0     7160 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_internal/version_utils.py
+-rw-r--r--   0        0        0      551 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_pyinstaller/__init__.py
+-rw-r--r--   0        0        0      417 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_pyinstaller/hook-b2sdk.py
+-rw-r--r--   0        0        0    12542 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_v3/__init__.py
+-rw-r--r--   0        0        0     7083 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/_v3/exception.py
+-rw-r--r--   0        0        0      705 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v0/__init__.py
+-rw-r--r--   0        0        0     2035 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v0/account_info.py
+-rw-r--r--   0        0        0      999 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v0/api.py
+-rw-r--r--   0        0        0     1078 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v0/bucket.py
+-rw-r--r--   0        0        0      969 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v0/exception.py
+-rw-r--r--   0        0        0     7245 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v0/sync.py
+-rw-r--r--   0        0        0     1351 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/__init__.py
+-rw-r--r--   0        0        0     5908 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/account_info.py
+-rw-r--r--   0        0        0     8348 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/api.py
+-rw-r--r--   0        0        0     1927 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/b2http.py
+-rw-r--r--   0        0        0    13668 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/bucket.py
+-rw-r--r--   0        0        0      530 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/cache.py
+-rw-r--r--   0        0        0     6787 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/download_dest.py
+-rw-r--r--   0        0        0     1580 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/exception.py
+-rw-r--r--   0        0        0     2218 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/file_metadata.py
+-rw-r--r--   0        0        0     7019 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/file_version.py
+-rw-r--r--   0        0        0      334 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/replication/__init__.py
+-rw-r--r--   0        0        0     1148 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/replication/monitoring.py
+-rw-r--r--   0        0        0     2596 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/session.py
+-rw-r--r--   0        0        0      505 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/sync/__init__.py
+-rw-r--r--   0        0        0     3869 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/sync/encryption_provider.py
+-rw-r--r--   0        0        0     3849 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/sync/file.py
+-rw-r--r--   0        0        0     2816 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/sync/file_to_path_translator.py
+-rw-r--r--   0        0        0     2318 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/sync/folder.py
+-rw-r--r--   0        0        0      738 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/sync/folder_parser.py
+-rw-r--r--   0        0        0      846 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/sync/report.py
+-rw-r--r--   0        0        0     6929 2024-05-15 12:36:52.340543 b2sdk-2.3.0/b2sdk/v1/sync/scan_policies.py
+-rw-r--r--   0        0        0     5387 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v1/sync/sync.py
+-rw-r--r--   0        0        0     1356 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/__init__.py
+-rw-r--r--   0        0        0      454 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/_compat.py
+-rw-r--r--   0        0        0      494 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/account_info.py
+-rw-r--r--   0        0        0     2235 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/api.py
+-rw-r--r--   0        0        0      804 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/b2http.py
+-rw-r--r--   0        0        0     6249 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/bucket.py
+-rw-r--r--   0        0        0      803 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/exception.py
+-rw-r--r--   0        0        0     2902 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/file_version.py
+-rw-r--r--   0        0        0     1339 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/large_file.py
+-rw-r--r--   0        0        0     2751 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/raw_api.py
+-rw-r--r--   0        0        0     3704 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/raw_simulator.py
+-rw-r--r--   0        0        0     1523 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/session.py
+-rw-r--r--   0        0        0      369 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/sync.py
+-rw-r--r--   0        0        0      584 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/transfer.py
+-rw-r--r--   0        0        0     1033 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/utils.py
+-rw-r--r--   0        0        0     1612 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/v2/version_utils.py
+-rw-r--r--   0        0        0      767 2024-05-15 12:36:52.344543 b2sdk-2.3.0/b2sdk/version.py
+-rw-r--r--   0        0        0     4436 2024-05-15 12:37:05.840790 b2sdk-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 b2sdk-2.3.0/PKG-INFO
```

### Comparing `b2sdk-2.2.1/LICENSE` & `b2sdk-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/README.md` & `b2sdk-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/account_info/abstract.py` & `b2sdk-2.3.0/b2sdk/_internal/account_info/abstract.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/account_info/exception.py` & `b2sdk-2.3.0/b2sdk/_internal/account_info/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/account_info/in_memory.py` & `b2sdk-2.3.0/b2sdk/_internal/account_info/in_memory.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/account_info/sqlite_account_info.py` & `b2sdk-2.3.0/b2sdk/_internal/account_info/sqlite_account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/account_info/stub.py` & `b2sdk-2.3.0/b2sdk/_internal/account_info/stub.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/account_info/upload_url_pool.py` & `b2sdk-2.3.0/b2sdk/_internal/account_info/upload_url_pool.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/api.py` & `b2sdk-2.3.0/b2sdk/_internal/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/api_config.py` & `b2sdk-2.3.0/b2sdk/_internal/api_config.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/application_key.py` & `b2sdk-2.3.0/b2sdk/_internal/application_key.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/b2http.py` & `b2sdk-2.3.0/b2sdk/_internal/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/bounded_queue_executor.py` & `b2sdk-2.3.0/b2sdk/_internal/bounded_queue_executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/bucket.py` & `b2sdk-2.3.0/b2sdk/_internal/bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 from __future__ import annotations
 
 import datetime as dt
 import fnmatch
+import itertools
 import logging
 import pathlib
 from contextlib import suppress
 from typing import Iterable, Sequence
 
 from .encryption.setting import EncryptionSetting, EncryptionSettingFactory
 from .encryption.types import EncryptionMode
@@ -330,15 +331,15 @@
         :param int start_part_number: the first part number to return.  defaults to the first part.
         :param int batch_size: the number of parts to fetch at a time from the server
         """
         return self.api.list_parts(file_id, start_part_number, batch_size)
 
     def list_file_versions(
         self, file_name: str, fetch_count: int | None = LIST_FILE_NAMES_MAX_LIMIT
-    ):
+    ) -> Iterable[FileVersion]:
         """
         Lists all of the versions for a single file.
 
         :param file_name: the name of the file to list.
         :param fetch_count: how many entries to list per API call or ``None`` to use the default. Acceptable values: 1 - 10000
         :rtype: generator[b2sdk.v2.FileVersion]
         """
@@ -362,34 +363,36 @@
             start_file_name = response['nextFileName']
             start_file_id = response['nextFileId']
             if start_file_name is None:
                 return
 
     def ls(
         self,
-        folder_to_list: str = '',
+        path: str = '',
         latest_only: bool = True,
         recursive: bool = False,
         fetch_count: int | None = LIST_FILE_NAMES_MAX_LIMIT,
         with_wildcard: bool = False,
         filters: Sequence[Filter] = (),
-    ):
+    ) -> Iterable[tuple[FileVersion, str]]:
         """
         Pretend that folders exist and yields the information about the files in a folder.
 
         B2 has a flat namespace for the files in a bucket, but there is a convention
         of using "/" as if there were folders.  This method searches through the
         flat namespace to find the files and "folders" that live within a given
         folder.
 
         When the `recursive` flag is set, lists all of the files in the given
         folder, and all of its sub-folders.
 
-        :param folder_to_list: the name of the folder to list; must not start with "/".
-                               Empty string means top-level folder
+        :param path: Path to list.
+                     To reduce the number of API calls, if path points to a folder, it should end with "/".
+                     Must not start with "/".
+                     Empty string means top-level folder.
         :param latest_only: when ``False`` returns info about all versions of a file,
                             when ``True``, just returns info about the most recent versions
         :param recursive: if ``True``, list folders recursively
         :param fetch_count: how many entries to list per API call or ``None`` to use the default. Acceptable values: 1 - 10000
         :param with_wildcard: Accepts "*", "?", "[]" and "[!]" in folder_to_list, similarly to what shell does.
                               As of 1.19.0 it can only be enabled when recursive is also enabled.
                               Also, in this mode, folder_to_list is considered to be a filename or a pattern.
@@ -400,14 +403,28 @@
         .. note::
             In case of `recursive=True`, folder_name is not returned.
         """
         # Ensure that recursive is enabled when with_wildcard is enabled.
         if with_wildcard and not recursive:
             raise ValueError('with_wildcard requires recursive to be turned on as well')
 
+        # check if path points to an object instead of a folder
+        if path and not with_wildcard and not path.endswith('/'):
+            file_versions = self.list_file_versions(path, 1 if latest_only else fetch_count)
+            if latest_only:
+                file_versions = itertools.islice(file_versions, 1)
+            path_pointed_to_file = False
+            for file_version in file_versions:
+                path_pointed_to_file = True
+                if not latest_only or file_version.action == 'upload':
+                    yield file_version, None
+            if path_pointed_to_file:
+                return
+
+        folder_to_list = path
         # Every file returned must have a name that starts with the
         # folder name and a "/".
         prefix = folder_to_list
         # In case of wildcards, we don't assume that this is folder that we're searching through.
         # It could be an exact file, e.g. 'a/b.txt' that we're trying to locate.
         if prefix != '' and not prefix.endswith('/') and not with_wildcard:
             prefix += '/'
```

### Comparing `b2sdk-2.2.1/b2sdk/_internal/cache.py` & `b2sdk-2.3.0/b2sdk/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/encryption/setting.py` & `b2sdk-2.3.0/b2sdk/_internal/encryption/setting.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/encryption/types.py` & `b2sdk-2.3.0/b2sdk/_internal/encryption/types.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/exception.py` & `b2sdk-2.3.0/b2sdk/_internal/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/file_lock.py` & `b2sdk-2.3.0/b2sdk/_internal/file_lock.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/file_version.py` & `b2sdk-2.3.0/b2sdk/_internal/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/filter.py` & `b2sdk-2.3.0/b2sdk/_internal/filter.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/http_constants.py` & `b2sdk-2.3.0/b2sdk/_internal/http_constants.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/included_sources.py` & `b2sdk-2.3.0/b2sdk/_internal/included_sources.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/large_file/part.py` & `b2sdk-2.3.0/b2sdk/_internal/large_file/part.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/large_file/services.py` & `b2sdk-2.3.0/b2sdk/_internal/large_file/services.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/large_file/unfinished_large_file.py` & `b2sdk-2.3.0/b2sdk/_internal/large_file/unfinished_large_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/progress.py` & `b2sdk-2.3.0/b2sdk/_internal/progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/raw_api.py` & `b2sdk-2.3.0/b2sdk/_internal/raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/raw_simulator.py` & `b2sdk-2.3.0/b2sdk/_internal/raw_simulator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/replication/monitoring.py` & `b2sdk-2.3.0/b2sdk/_internal/replication/monitoring.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/replication/setting.py` & `b2sdk-2.3.0/b2sdk/_internal/replication/setting.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/replication/setup.py` & `b2sdk-2.3.0/b2sdk/_internal/replication/setup.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/replication/types.py` & `b2sdk-2.3.0/b2sdk/_internal/replication/types.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/requests/LICENSE` & `b2sdk-2.3.0/b2sdk/_internal/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/requests/__init__.py` & `b2sdk-2.3.0/b2sdk/_internal/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/requests/included_source_meta.py` & `b2sdk-2.3.0/b2sdk/_internal/requests/included_source_meta.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/scan/exception.py` & `b2sdk-2.3.0/b2sdk/_internal/scan/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/scan/folder.py` & `b2sdk-2.3.0/b2sdk/_internal/scan/folder.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/scan/folder_parser.py` & `b2sdk-2.3.0/b2sdk/_internal/scan/folder_parser.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/scan/path.py` & `b2sdk-2.3.0/b2sdk/_internal/scan/path.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/scan/policies.py` & `b2sdk-2.3.0/b2sdk/_internal/scan/policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/scan/report.py` & `b2sdk-2.3.0/b2sdk/_internal/scan/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/scan/scan.py` & `b2sdk-2.3.0/b2sdk/_internal/scan/scan.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/session.py` & `b2sdk-2.3.0/b2sdk/_internal/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/stream/__init__.py` & `b2sdk-2.3.0/b2sdk/_internal/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/stream/base.py` & `b2sdk-2.3.0/b2sdk/_internal/stream/base.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/stream/chained.py` & `b2sdk-2.3.0/b2sdk/_internal/stream/chained.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/stream/hashing.py` & `b2sdk-2.3.0/b2sdk/_internal/stream/hashing.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/stream/progress.py` & `b2sdk-2.3.0/b2sdk/_internal/stream/progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/stream/range.py` & `b2sdk-2.3.0/b2sdk/_internal/stream/range.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/stream/wrapper.py` & `b2sdk-2.3.0/b2sdk/_internal/stream/wrapper.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/sync/action.py` & `b2sdk-2.3.0/b2sdk/_internal/sync/action.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/sync/encryption_provider.py` & `b2sdk-2.3.0/b2sdk/_internal/sync/encryption_provider.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/sync/policy.py` & `b2sdk-2.3.0/b2sdk/_internal/sync/policy.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/sync/policy_manager.py` & `b2sdk-2.3.0/b2sdk/_internal/sync/policy_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/sync/report.py` & `b2sdk-2.3.0/b2sdk/_internal/sync/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/sync/sync.py` & `b2sdk-2.3.0/b2sdk/_internal/sync/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/__init__.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/emerger.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/emerger.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/exception.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/executor.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/planner/part_definition.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/planner/planner.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/planner/planner.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/unbound_write_intent.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/emerge/write_intent.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/emerge/write_intent.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/download_manager.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/download_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloaded_file.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloaded_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/abstract.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/parallel.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/simple.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/simple.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/copy_manager.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/copy_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/copy_source.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/copy_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/large_file_upload_state.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/outbound_source.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/outbound_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/progress_reporter.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/upload_manager.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/upload_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/outbound/upload_source.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/outbound/upload_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/transfer/transfer_manager.py` & `b2sdk-2.3.0/b2sdk/_internal/transfer/transfer_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/utils/__init__.py` & `b2sdk-2.3.0/b2sdk/_internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/utils/docs.py` & `b2sdk-2.3.0/b2sdk/_internal/utils/docs.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/utils/escape.py` & `b2sdk-2.3.0/b2sdk/_internal/utils/escape.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/utils/filesystem.py` & `b2sdk-2.3.0/b2sdk/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/utils/http_date.py` & `b2sdk-2.3.0/b2sdk/_internal/utils/http_date.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/utils/range_.py` & `b2sdk-2.3.0/b2sdk/_internal/utils/range_.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/utils/thread_pool.py` & `b2sdk-2.3.0/b2sdk/_internal/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/utils/typing.py` & `b2sdk-2.3.0/b2sdk/_internal/utils/typing.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_internal/version_utils.py` & `b2sdk-2.3.0/b2sdk/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_pyinstaller/__init__.py` & `b2sdk-2.3.0/b2sdk/_pyinstaller/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_v3/__init__.py` & `b2sdk-2.3.0/b2sdk/_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/_v3/exception.py` & `b2sdk-2.3.0/b2sdk/_v3/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v0/__init__.py` & `b2sdk-2.3.0/b2sdk/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v0/account_info.py` & `b2sdk-2.3.0/b2sdk/v0/account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v0/api.py` & `b2sdk-2.3.0/b2sdk/v0/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v0/bucket.py` & `b2sdk-2.3.0/b2sdk/v0/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v0/exception.py` & `b2sdk-2.3.0/b2sdk/v0/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v0/sync.py` & `b2sdk-2.3.0/b2sdk/v0/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/__init__.py` & `b2sdk-2.3.0/b2sdk/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/account_info.py` & `b2sdk-2.3.0/b2sdk/v1/account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/api.py` & `b2sdk-2.3.0/b2sdk/v1/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/b2http.py` & `b2sdk-2.3.0/b2sdk/v1/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/bucket.py` & `b2sdk-2.3.0/b2sdk/v1/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/cache.py` & `b2sdk-2.3.0/b2sdk/v1/cache.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/download_dest.py` & `b2sdk-2.3.0/b2sdk/v1/download_dest.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/exception.py` & `b2sdk-2.3.0/b2sdk/v1/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/file_metadata.py` & `b2sdk-2.3.0/b2sdk/v1/file_metadata.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/file_version.py` & `b2sdk-2.3.0/b2sdk/v1/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/replication/monitoring.py` & `b2sdk-2.3.0/b2sdk/v1/replication/monitoring.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/session.py` & `b2sdk-2.3.0/b2sdk/v1/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/sync/encryption_provider.py` & `b2sdk-2.3.0/b2sdk/v1/sync/encryption_provider.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/sync/file.py` & `b2sdk-2.3.0/b2sdk/v1/sync/file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/sync/file_to_path_translator.py` & `b2sdk-2.3.0/b2sdk/v1/sync/file_to_path_translator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/sync/folder.py` & `b2sdk-2.3.0/b2sdk/v1/sync/folder.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/sync/folder_parser.py` & `b2sdk-2.3.0/b2sdk/v1/sync/folder_parser.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/sync/report.py` & `b2sdk-2.3.0/b2sdk/v1/sync/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/sync/scan_policies.py` & `b2sdk-2.3.0/b2sdk/v1/sync/scan_policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v1/sync/sync.py` & `b2sdk-2.3.0/b2sdk/v1/sync/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/__init__.py` & `b2sdk-2.3.0/b2sdk/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/api.py` & `b2sdk-2.3.0/b2sdk/v2/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/b2http.py` & `b2sdk-2.3.0/b2sdk/v2/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/exception.py` & `b2sdk-2.3.0/b2sdk/v2/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/file_version.py` & `b2sdk-2.3.0/b2sdk/v2/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/large_file.py` & `b2sdk-2.3.0/b2sdk/v2/large_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/raw_api.py` & `b2sdk-2.3.0/b2sdk/v2/raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/raw_simulator.py` & `b2sdk-2.3.0/b2sdk/v2/raw_simulator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/session.py` & `b2sdk-2.3.0/b2sdk/v2/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/transfer.py` & `b2sdk-2.3.0/b2sdk/v2/transfer.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/utils.py` & `b2sdk-2.3.0/b2sdk/v2/utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/v2/version_utils.py` & `b2sdk-2.3.0/b2sdk/v2/version_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/b2sdk/version.py` & `b2sdk-2.3.0/b2sdk/version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.2.1/pyproject.toml` & `b2sdk-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "2.2.1"
+version = "2.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Backblaze/b2-sdk-python"
```

### Comparing `b2sdk-2.2.1/PKG-INFO` & `b2sdk-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2sdk
-Version: 2.2.1
+Version: 2.3.0
 Summary: Backblaze B2 SDK
 Keywords: backblaze,b2,cloud,storage
 Author-Email: Backblaze Inc <support@backblaze.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

