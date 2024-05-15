# Comparing `tmp/splitio_client-9.6.2.tar.gz` & `tmp/splitio_client-9.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splitio_client-9.6.2.tar", last modified: Fri Apr  5 19:57:31 2024, max compression
+gzip compressed data, was "dist/splitio_client-9.7.0.tar", last modified: Wed May 15 18:04:56 2024, max compression
```

## Comparing `splitio_client-9.6.2.tar` & `splitio_client-9.7.0.tar`

### file list

```diff
@@ -1,134 +1,174 @@
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2024-04-05 19:57:31.000000 splitio_client-9.6.2/PKG-INFO
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5240 2024-04-05 19:55:06.000000 splitio_client-9.6.2/README.md
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2024-04-05 19:57:31.000000 splitio_client-9.6.2/setup.cfg
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1738 2024-04-05 19:55:06.000000 splitio_client-9.6.2/setup.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/api/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2430 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/auth.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5170 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4015 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/commons.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2917 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/events.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5179 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2873 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2829 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/splits.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4063 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/api/telemetry.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/client/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    24159 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5405 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/config.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    29723 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/factory.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20321 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/input_validator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/key.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/listener.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/localhost.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3497 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/client/util.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/engine/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/engine/cache/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/cache/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/cache/lru.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7143 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/evaluator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/filters.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/engine/hashfns/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/hashfns/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/hashfns/legacy.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/hashfns/murmur3py.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/engine/impressions/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2928 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7354 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/adapters.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/strategies.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3049 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/impressions/unique_keys_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/splitters.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    13487 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/engine/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/exceptions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/factories.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/key.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/models/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/datatypes.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/events.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/models/grammar/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4099 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/condition.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/base.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/keys.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/misc.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/numeric.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/sets.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/matchers/string.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/grammar/partitions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/notification.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7964 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/splits.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    36838 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2037 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/models/token.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/push/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9110 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    15365 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/parser.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3241 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/processor.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/segmentworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/splitsse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5601 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/splitworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/sse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/push/status_tracker.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/recorder/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/recorder/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/recorder/recorder.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/storage/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8718 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/storage/adapters/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/adapters/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/adapters/cache_trait.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    19144 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/adapters/redis.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/adapters/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    26459 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/inmemmory.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    33160 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/pluggable.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    28191 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/storage/redis.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/sync/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/event.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/impression.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12506 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/segment.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21424 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/split.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    23444 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3254 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2961 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/unique_keys.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/sync/util.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/tasks/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/events_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/impressions_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/segment_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/split_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/telemetry_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/unique_keys_sync.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/tasks/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6142 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/util/asynctask.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/tasks/util/workerpool.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/backoff.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/decorators.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2457 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/storage_helper.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/threadutil.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/util/time.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       22 2024-04-05 19:55:06.000000 splitio_client-9.6.2/splitio/version.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/PKG-INFO
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3259 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/SOURCES.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/dependency_links.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      311 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/requires.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        8 2024-04-05 19:57:31.000000 splitio_client-9.6.2/splitio_client.egg-info/top_level.txt
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      564 2024-05-15 16:06:01.000000 splitio_client-9.7.0/LICENSE.txt
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      732 2024-05-15 18:04:56.000000 splitio_client-9.7.0/PKG-INFO
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5242 2024-05-15 16:48:35.000000 splitio_client-9.7.0/README.md
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      419 2024-05-15 18:04:56.000000 splitio_client-9.7.0/setup.cfg
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1671 2024-05-15 16:48:35.000000 splitio_client-9.7.0/setup.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      122 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/__init__.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/api/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      422 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/api/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2486 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/api/auth.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5170 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/api/client.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4326 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/api/commons.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2917 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/api/events.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5179 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/api/impressions.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2873 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/api/segments.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2829 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/api/splits.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4063 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/api/telemetry.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/client/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/client/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    24159 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/client/client.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5405 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/client/config.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    29723 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/client/factory.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    20321 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/client/input_validator.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      534 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/client/key.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2117 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/client/listener.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1329 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/client/localhost.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3497 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/client/manager.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1533 2023-01-10 16:34:16.000000 splitio_client-9.7.0/splitio/client/util.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/engine/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/engine/__init__.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/engine/cache/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/engine/cache/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3926 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/engine/cache/lru.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     7143 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/engine/evaluator.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2097 2022-11-29 19:27:27.000000 splitio_client-9.7.0/splitio/engine/filters.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/engine/hashfns/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1315 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/engine/hashfns/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      725 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/engine/hashfns/legacy.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5711 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/engine/hashfns/murmur3py.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/engine/impressions/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2928 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/engine/impressions/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     7354 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/engine/impressions/adapters.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2373 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/engine/impressions/impressions.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5310 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/engine/impressions/manager.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3460 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/engine/impressions/strategies.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3049 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/engine/impressions/unique_keys_tracker.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1941 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/engine/splitters.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    13487 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/engine/telemetry.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      195 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/exceptions.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)       85 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/factories.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      109 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/impressions.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)       72 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/key.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/models/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      217 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/models/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1483 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/datatypes.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      352 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/events.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/models/grammar/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/grammar/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4152 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/models/grammar/condition.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3683 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3836 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/base.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2811 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/keys.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3190 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/misc.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     8680 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/numeric.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     9351 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/semver.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     6520 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/sets.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     8613 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/string.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/utils/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/utils/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5293 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/models/grammar/matchers/utils/utils.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1494 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/grammar/partitions.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1296 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/impressions.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     6054 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/notification.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2123 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/models/segments.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     9076 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/models/splits.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    36838 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/models/telemetry.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2037 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/models/token.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/push/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/push/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     9110 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/push/manager.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    15365 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/push/parser.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3241 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/push/processor.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2155 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/push/segmentworker.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5297 2024-05-07 19:38:44.000000 splitio_client-9.7.0/splitio/push/splitsse.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5601 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/push/splitworker.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4587 2024-05-07 19:38:44.000000 splitio_client-9.7.0/splitio/push/sse.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     8494 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/push/status_tracker.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/recorder/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/recorder/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     6537 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/recorder/recorder.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)       21 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/spec.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/storage/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     8718 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/storage/__init__.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/storage/adapters/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/storage/adapters/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     6613 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/storage/adapters/cache_trait.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    19144 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/storage/adapters/redis.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3456 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/storage/adapters/util.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    26459 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/storage/inmemmory.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    33161 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/storage/pluggable.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    28198 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/storage/redis.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/sync/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/sync/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2164 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/sync/event.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3324 2022-11-29 19:27:27.000000 splitio_client-9.7.0/splitio/sync/impression.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     7248 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/sync/manager.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    12528 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/sync/segment.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    21424 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/sync/split.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    23444 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/sync/synchronizer.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3254 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/sync/telemetry.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2961 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/sync/unique_keys.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2768 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/sync/util.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/tasks/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      698 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/tasks/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1432 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/tasks/events_sync.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2523 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/tasks/impressions_sync.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1011 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/tasks/segment_sync.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1094 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/tasks/split_sync.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1402 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/tasks/telemetry_sync.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2597 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/tasks/unique_keys_sync.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/tasks/util/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/tasks/util/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     6142 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/tasks/util/asynctask.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4820 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/tasks/util/workerpool.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio/util/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/util/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      956 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/util/backoff.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      293 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/util/decorators.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2457 2024-05-15 16:06:01.000000 splitio_client-9.7.0/splitio/util/storage_helper.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1512 2022-05-26 22:38:21.000000 splitio_client-9.7.0/splitio/util/threadutil.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      634 2023-01-30 20:34:47.000000 splitio_client-9.7.0/splitio/util/time.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)       22 2024-05-15 16:48:35.000000 splitio_client-9.7.0/splitio/version.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio_client.egg-info/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      732 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio_client.egg-info/PKG-INFO
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4324 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        1 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      245 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio_client.egg-info/requires.txt
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        8 2024-05-15 18:04:56.000000 splitio_client-9.7.0/splitio_client.egg-info/top_level.txt
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/tests/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/tests/__init__.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/tests/helpers/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)      220 2022-05-26 22:38:21.000000 splitio_client-9.7.0/tests/helpers/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     8872 2023-01-30 20:34:47.000000 splitio_client-9.7.0/tests/helpers/mockserver.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/tests/integration/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     8319 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/integration/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    78469 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/integration/test_client_e2e.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    11839 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/integration/test_redis_integration.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    64386 2024-05-15 16:48:35.000000 splitio_client-9.7.0/tests/integration/test_streaming_e2e.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/tests/push/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/tests/push/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    12859 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/push/test_manager.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4181 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/push/test_parser.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2500 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/push/test_processor.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1764 2024-05-09 15:22:46.000000 splitio_client-9.7.0/tests/push/test_segment_worker.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    14156 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/push/test_split_worker.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4332 2024-05-09 15:22:55.000000 splitio_client-9.7.0/tests/push/test_splitsse.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     4038 2024-05-09 15:22:59.000000 splitio_client-9.7.0/tests/push/test_sse.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    12475 2023-01-30 20:34:47.000000 splitio_client-9.7.0/tests/push/test_status_tracker.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/tests/recorder/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/tests/recorder/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     3903 2023-01-30 20:34:47.000000 splitio_client-9.7.0/tests/recorder/test_recorder.py
+drwxr-xr-x   0 matiasmelograno   (503) staff       (20)        0 2024-05-15 18:04:56.000000 splitio_client-9.7.0/tests/sync/
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)        0 2022-05-26 22:38:21.000000 splitio_client-9.7.0/tests/sync/__init__.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2074 2022-05-26 22:38:21.000000 splitio_client-9.7.0/tests/sync/test_events_synchronizer.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     1420 2022-11-29 19:27:27.000000 splitio_client-9.7.0/tests/sync/test_impressions_count_synchronizer.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2259 2022-05-26 22:38:21.000000 splitio_client-9.7.0/tests/sync/test_impressions_synchronizer.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     5424 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/sync/test_manager.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    16555 2024-05-15 16:48:35.000000 splitio_client-9.7.0/tests/sync/test_segments_synchronizer.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    27392 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/sync/test_splits_synchronizer.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)    20115 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/sync/test_synchronizer.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     8088 2024-05-15 16:06:01.000000 splitio_client-9.7.0/tests/sync/test_telemetry.py
+-rw-r--r--   0 matiasmelograno   (503) staff       (20)     2869 2022-11-29 19:27:27.000000 splitio_client-9.7.0/tests/sync/test_unique_keys_sync.py
```

### Comparing `splitio_client-9.6.2/PKG-INFO` & `splitio_client-9.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: splitio_client
-Version: 9.6.2
+Version: 9.7.0
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.6.2
+Download-URL: https://github.com/splitio/python-client/tarball/9.7.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `splitio_client-9.6.2/README.md` & `splitio_client-9.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ## Overview
 This SDK is designed to work with Split, the platform for controlled rollouts, which serves features to your users via a Split feature flag to manage your complete customer experience.
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/splitsoftware.svg?style=social&label=Follow&maxAge=1529000)](https://twitter.com/intent/follow?screen_name=splitsoftware)
 
 ## Compatibility
-This SDK is compatible with **Python 3 and higher**.
+This SDK is compatible with **Python 3.7 and higher**.
 
 ## Getting started
 Below is a simple example that describes the instantiation and most basic usage of our SDK:
 
 Run `pip install splitio_client`
```

### Comparing `splitio_client-9.6.2/setup.py` & `splitio_client-9.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 # !/usr/bin/env python
 
 from os import path
 from setuptools import setup, find_packages
 
 TESTS_REQUIRES = [
     'flake8',
-    'pytest==7.0.1',
-    'pytest-mock==3.12.0',
-    'coverage==6.2',
+    'pytest==7.1.0',
+    'pytest-mock==3.11.1',
+    'coverage==7.2.7',
     'pytest-cov',
-    'importlib-metadata==4.2',
-    'tomli==1.2.3',
-    'iniconfig==1.1.1',
-    'attrs==22.1.0'
+    'importlib-metadata==6.7',
+    'tomli',
+    'iniconfig',
+    'attrs'
 ]
 
 INSTALL_REQUIRES = [
-    'requests>=2.9.1',
-    'pyyaml>=5.4',
+    'requests',
+    'pyyaml',
     'docopt>=0.6.2',
-    'enum34;python_version<"3.4"',
     'bloom-filter2>=2.0.0'
 ]
 
 with open(path.join(path.abspath(path.dirname(__file__)), 'splitio', 'version.py')) as f:
     exec(f.read())  # pylint: disable=exec-used
 
 setup(
```

### Comparing `splitio_client-9.6.2/splitio/api/auth.py` & `splitio_client-9.7.0/splitio/api/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Auth API module."""
 
 import logging
 import json
 
 from splitio.api import APIException
 from splitio.api.commons import headers_from_metadata, record_telemetry
+from splitio.spec import SPEC_VERSION
 from splitio.util.time import get_current_epoch_time_ms
 from splitio.api.client import HttpClientException
 from splitio.models.token import from_raw
 from splitio.models.telemetry import HTTPExceptionsAndLatencies
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -39,15 +40,15 @@
         :return: Json representation of an authentication.
         :rtype: splitio.models.token.Token
         """
         start = get_current_epoch_time_ms()
         try:
             response = self._client.get(
                 'auth',
-                '/v2/auth',
+                '/v2/auth?s=' + SPEC_VERSION,
                 self._sdk_key,
                 extra_headers=self._metadata,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.TOKEN, self._telemetry_runtime_producer)
             if 200 <= response.status_code < 300:
                 payload = json.loads(response.body)
                 return from_raw(payload)
```

### Comparing `splitio_client-9.6.2/splitio/api/client.py` & `splitio_client-9.7.0/splitio/api/client.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/api/commons.py` & `splitio_client-9.7.0/splitio/api/commons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Commons module."""
 from splitio.util.time import get_current_epoch_time_ms
+from splitio.spec import SPEC_VERSION
 
 _CACHE_CONTROL = 'Cache-Control'
 _CACHE_CONTROL_NO_CACHE = 'no-cache'
 
-
 def headers_from_metadata(sdk_metadata, client_key=None):
     """
     Generate a dict with headers required by data-recording API endpoints.
 
     :param sdk_metadata: SDK Metadata object, generated at sdk initialization time.
     :type sdk_metadata: splitio.client.util.SdkMetadata
 
@@ -53,15 +53,15 @@
         telemetry_runtime_producer.record_successful_sync(metric_name, get_current_epoch_time_ms())
         return
     telemetry_runtime_producer.record_sync_error(metric_name, status_code)
 
 class FetchOptions(object):
     """Fetch Options object."""
 
-    def __init__(self, cache_control_headers=False, change_number=None, sets=None):
+    def __init__(self, cache_control_headers=False, change_number=None, sets=None, spec=SPEC_VERSION):
         """
         Class constructor.
 
         :param cache_control_headers: Flag for Cache-Control header
         :type cache_control_headers: bool
 
         :param change_number: ChangeNumber to use for bypassing CDN in request.
@@ -69,14 +69,15 @@
 
         :param sets: list of flag sets
         :type sets: list
         """
         self._cache_control_headers = cache_control_headers
         self._change_number = change_number
         self._sets = sets
+        self._spec = spec
 
     @property
     def cache_control_headers(self):
         """Return cache control headers."""
         return self._cache_control_headers
 
     @property
@@ -85,22 +86,29 @@
         return self._change_number
 
     @property
     def sets(self):
         """Return sets."""
         return self._sets
 
+    @property
+    def spec(self):
+        """Return sets."""
+        return self._spec
+
     def __eq__(self, other):
         """Match between other options."""
         if self._cache_control_headers != other._cache_control_headers:
             return False
         if self._change_number != other._change_number:
             return False
         if self._sets != other._sets:
             return False
+        if self._spec != other._spec:
+            return False
         return True
 
 
 def build_fetch(change_number, fetch_options, metadata):
     """
     Build fetch with new flags if that is the case.
 
@@ -112,18 +120,19 @@
 
     :param metadata: Metadata Headers.
     :type metadata: dict
 
     :return: Objects for fetch
     :rtype: dict, dict
     """
-    query = {'since': change_number}
+    query = {'s': fetch_options.spec} if fetch_options.spec is not None else {}
+    query['since'] = change_number
     extra_headers = metadata
     if fetch_options is None:
         return query, extra_headers
     if fetch_options.cache_control_headers:
         extra_headers[_CACHE_CONTROL] = _CACHE_CONTROL_NO_CACHE
-    if fetch_options.change_number is not None:
-        query['till'] = fetch_options.change_number
     if fetch_options.sets is not None:
         query['sets'] = fetch_options.sets
+    if fetch_options.change_number is not None:
+        query['till'] = fetch_options.change_number
     return query, extra_headers
```

### Comparing `splitio_client-9.6.2/splitio/api/events.py` & `splitio_client-9.7.0/splitio/api/events.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/api/impressions.py` & `splitio_client-9.7.0/splitio/api/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/api/segments.py` & `splitio_client-9.7.0/splitio/api/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/api/splits.py` & `splitio_client-9.7.0/splitio/api/splits.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/api/telemetry.py` & `splitio_client-9.7.0/splitio/api/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/client.py` & `splitio_client-9.7.0/splitio/client/client.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/config.py` & `splitio_client-9.7.0/splitio/client/config.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/factory.py` & `splitio_client-9.7.0/splitio/client/factory.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/input_validator.py` & `splitio_client-9.7.0/splitio/client/input_validator.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/key.py` & `splitio_client-9.7.0/splitio/client/key.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/listener.py` & `splitio_client-9.7.0/splitio/client/listener.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/localhost.py` & `splitio_client-9.7.0/splitio/client/localhost.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/manager.py` & `splitio_client-9.7.0/splitio/client/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/client/util.py` & `splitio_client-9.7.0/splitio/client/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/cache/lru.py` & `splitio_client-9.7.0/splitio/engine/cache/lru.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/evaluator.py` & `splitio_client-9.7.0/splitio/engine/evaluator.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/filters.py` & `splitio_client-9.7.0/splitio/engine/filters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/hashfns/__init__.py` & `splitio_client-9.7.0/splitio/engine/hashfns/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/hashfns/legacy.py` & `splitio_client-9.7.0/splitio/engine/hashfns/legacy.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/hashfns/murmur3py.py` & `splitio_client-9.7.0/splitio/engine/hashfns/murmur3py.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/impressions/__init__.py` & `splitio_client-9.7.0/splitio/engine/impressions/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/impressions/adapters.py` & `splitio_client-9.7.0/splitio/engine/impressions/adapters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/impressions/impressions.py` & `splitio_client-9.7.0/splitio/engine/impressions/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/impressions/manager.py` & `splitio_client-9.7.0/splitio/engine/impressions/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/impressions/strategies.py` & `splitio_client-9.7.0/splitio/engine/impressions/strategies.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/impressions/unique_keys_tracker.py` & `splitio_client-9.7.0/splitio/engine/impressions/unique_keys_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/splitters.py` & `splitio_client-9.7.0/splitio/engine/splitters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/engine/telemetry.py` & `splitio_client-9.7.0/splitio/engine/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/datatypes.py` & `splitio_client-9.7.0/splitio/models/datatypes.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/grammar/condition.py` & `splitio_client-9.7.0/splitio/models/grammar/condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Split conditions module."""
 
 from enum import Enum
 
+from splitio.models import MatcherNotFoundException
 from splitio.models.grammar import matchers
 from splitio.models.grammar import partitions
 
 _MATCHER_COMBINERS = {
     'AND': lambda ms, k, a, c: all(m.evaluate(k, a, c) for m in ms)
 }
 
@@ -120,13 +121,14 @@
     """
     parsed_partitions = [
         partitions.from_raw(raw_partition)
         for raw_partition in raw_condition['partitions']
     ]
 
     matcher_objects = [matchers.from_raw(x) for x in raw_condition['matcherGroup']['matchers']]
+
     combiner = _MATCHER_COMBINERS[raw_condition['matcherGroup']['combiner']]
     label = raw_condition.get('label')
 
     condition_type = ConditionType(raw_condition.get('conditionType', ConditionType.WHITELIST))
 
     return Condition(matcher_objects, combiner, parsed_partitions, label, condition_type)
```

### Comparing `splitio_client-9.6.2/splitio/models/grammar/matchers/__init__.py` & `splitio_client-9.7.0/splitio/models/grammar/matchers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Matchers entrypoint module."""
+from splitio.models import MatcherNotFoundException
 from splitio.models.grammar.matchers.keys import AllKeysMatcher, UserDefinedSegmentMatcher
 from splitio.models.grammar.matchers.numeric import BetweenMatcher, EqualToMatcher, \
     GreaterThanOrEqualMatcher, LessThanOrEqualMatcher
 from splitio.models.grammar.matchers.sets import ContainsAllOfSetMatcher, \
     ContainsAnyOfSetMatcher, EqualToSetMatcher, PartOfSetMatcher
 from splitio.models.grammar.matchers.string import ContainsStringMatcher, \
     EndsWithMatcher, RegexMatcher, StartsWithMatcher, WhitelistMatcher
 from splitio.models.grammar.matchers.misc import BooleanMatcher, DependencyMatcher
+from splitio.models.grammar.matchers.semver import EqualToSemverMatcher, GreaterThanOrEqualToSemverMatcher, LessThanOrEqualToSemverMatcher, \
+        BetweenSemverMatcher, InListSemverMatcher
 
 
 MATCHER_TYPE_ALL_KEYS = 'ALL_KEYS'
 MATCHER_TYPE_IN_SEGMENT = 'IN_SEGMENT'
 MATCHER_TYPE_WHITELIST = 'WHITELIST'
 MATCHER_TYPE_EQUAL_TO = 'EQUAL_TO'
 MATCHER_TYPE_GREATER_THAN_OR_EQUAL_TO = 'GREATER_THAN_OR_EQUAL_TO'
@@ -22,14 +25,19 @@
 MATCHER_TYPE_CONTAINS_ANY_OF_SET = 'CONTAINS_ANY_OF_SET'
 MATCHER_TYPE_STARTS_WITH = 'STARTS_WITH'
 MATCHER_TYPE_ENDS_WITH = 'ENDS_WITH'
 MATCHER_TYPE_CONTAINS_STRING = 'CONTAINS_STRING'
 MATCHER_TYPE_IN_SPLIT_TREATMENT = 'IN_SPLIT_TREATMENT'
 MATCHER_TYPE_EQUAL_TO_BOOLEAN = 'EQUAL_TO_BOOLEAN'
 MATCHER_TYPE_MATCHES_STRING = 'MATCHES_STRING'
+MATCHER_TYPE_EQUAL_TO_SEMVER = 'EQUAL_TO_SEMVER'
+MATCHER_GREATER_THAN_OR_EQUAL_TO_SEMVER = 'GREATER_THAN_OR_EQUAL_TO_SEMVER'
+MATCHER_LESS_THAN_OR_EQUAL_TO_SEMVER = 'LESS_THAN_OR_EQUAL_TO_SEMVER'
+MATCHER_BETWEEN_SEMVER = 'BETWEEN_SEMVER'
+MATCHER_INLIST_SEMVER = 'IN_LIST_SEMVER'
 
 
 _MATCHER_BUILDERS = {
     MATCHER_TYPE_ALL_KEYS: AllKeysMatcher,
     MATCHER_TYPE_IN_SEGMENT: UserDefinedSegmentMatcher,
     MATCHER_TYPE_WHITELIST: WhitelistMatcher,
     MATCHER_TYPE_EQUAL_TO: EqualToMatcher,
@@ -41,27 +49,31 @@
     MATCHER_TYPE_CONTAINS_ALL_OF_SET: ContainsAllOfSetMatcher,
     MATCHER_TYPE_CONTAINS_ANY_OF_SET: ContainsAnyOfSetMatcher,
     MATCHER_TYPE_STARTS_WITH: StartsWithMatcher,
     MATCHER_TYPE_ENDS_WITH: EndsWithMatcher,
     MATCHER_TYPE_CONTAINS_STRING: ContainsStringMatcher,
     MATCHER_TYPE_IN_SPLIT_TREATMENT: DependencyMatcher,
     MATCHER_TYPE_EQUAL_TO_BOOLEAN: BooleanMatcher,
-    MATCHER_TYPE_MATCHES_STRING: RegexMatcher
+    MATCHER_TYPE_MATCHES_STRING: RegexMatcher,
+    MATCHER_TYPE_EQUAL_TO_SEMVER: EqualToSemverMatcher,
+    MATCHER_GREATER_THAN_OR_EQUAL_TO_SEMVER: GreaterThanOrEqualToSemverMatcher,
+    MATCHER_LESS_THAN_OR_EQUAL_TO_SEMVER: LessThanOrEqualToSemverMatcher,
+    MATCHER_BETWEEN_SEMVER: BetweenSemverMatcher,
+    MATCHER_INLIST_SEMVER: InListSemverMatcher
 }
 
-
 def from_raw(raw_matcher):
     """
     Parse a condition from a JSON portion of splitChanges.
 
     :param raw_matcher: JSON object extracted from a condition's matcher array.
     :type raw_matcher: dict
 
     :return: A concrete Matcher object.
     :rtype: Matcher
     """
     matcher_type = raw_matcher['matcherType']
     try:
         builder = _MATCHER_BUILDERS[matcher_type]
     except KeyError:
-        raise ValueError('Invalid matcher type %s' % matcher_type)
+        raise MatcherNotFoundException('Invalid matcher type %s' % matcher_type)
     return builder(raw_matcher)
```

### Comparing `splitio_client-9.6.2/splitio/models/grammar/matchers/base.py` & `splitio_client-9.7.0/splitio/models/grammar/matchers/base.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/grammar/matchers/keys.py` & `splitio_client-9.7.0/splitio/models/grammar/matchers/keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/grammar/matchers/misc.py` & `splitio_client-9.7.0/splitio/models/grammar/matchers/misc.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/grammar/matchers/numeric.py` & `splitio_client-9.7.0/splitio/models/grammar/matchers/numeric.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/grammar/matchers/sets.py` & `splitio_client-9.7.0/splitio/models/grammar/matchers/sets.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/grammar/matchers/string.py` & `splitio_client-9.7.0/splitio/models/grammar/matchers/string.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/grammar/partitions.py` & `splitio_client-9.7.0/splitio/models/grammar/partitions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/impressions.py` & `splitio_client-9.7.0/splitio/models/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/notification.py` & `splitio_client-9.7.0/splitio/models/notification.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/segments.py` & `splitio_client-9.7.0/splitio/models/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/splits.py` & `splitio_client-9.7.0/splitio/models/splits.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,50 @@
 """Splits module."""
 from enum import Enum
 from collections import namedtuple
+import logging
 
+from splitio.models import MatcherNotFoundException
 from splitio.models.grammar import condition
 
+_LOGGER = logging.getLogger(__name__)
 
 SplitView = namedtuple(
     'SplitView',
     ['name', 'traffic_type', 'killed', 'treatments', 'change_number', 'configs', 'default_treatment', 'sets']
 )
 
+_DEFAULT_CONDITIONS_TEMPLATE =   {
+    "conditionType": "ROLLOUT",
+    "matcherGroup": {
+        "combiner": "AND",
+        "matchers": [
+        {
+            "keySelector": None,
+            "matcherType": "ALL_KEYS",
+            "negate": False,
+            "userDefinedSegmentMatcherData": None,
+            "whitelistMatcherData": None,
+            "unaryNumericMatcherData": None,
+            "betweenMatcherData": None,
+            "dependencyMatcherData": None,
+            "booleanMatcherData": None,
+            "stringMatcherData": None
+        }]
+    },
+    "partitions": [
+        {
+        "treatment": "control",
+        "size": 100
+        }
+    ],
+    "label": "targeting rule type unsupported by sdk"
+}
+
+
 
 class Status(Enum):
     """Split status."""
 
     ACTIVE = "ACTIVE"
     ARCHIVED = "ARCHIVED"
 
@@ -234,22 +265,28 @@
 
     :param raw_split: JSON object extracted from a splitChange's split array (splitChanges response)
     :type raw_split: dict
 
     :return: A parsed Split object capable of performing evaluations.
     :rtype: Split
     """
+    try:
+        conditions = [condition.from_raw(c) for c in raw_split['conditions']]
+    except MatcherNotFoundException as e:
+        _LOGGER.error(str(e))
+        _LOGGER.debug("Using default conditions template for feature flag: %s", raw_split['name'])
+        conditions = [condition.from_raw(_DEFAULT_CONDITIONS_TEMPLATE)]
     return Split(
         raw_split['name'],
         raw_split['seed'],
         raw_split['killed'],
         raw_split['defaultTreatment'],
         raw_split['trafficTypeName'],
         raw_split['status'],
         raw_split['changeNumber'],
-        [condition.from_raw(c) for c in raw_split['conditions']],
+        conditions,
         raw_split.get('algo'),
         traffic_allocation=raw_split.get('trafficAllocation'),
         traffic_allocation_seed=raw_split.get('trafficAllocationSeed'),
         configurations=raw_split.get('configurations'),
         sets=set(raw_split.get('sets')) if raw_split.get('sets') is not None else []
     )
```

### Comparing `splitio_client-9.6.2/splitio/models/telemetry.py` & `splitio_client-9.7.0/splitio/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/models/token.py` & `splitio_client-9.7.0/splitio/models/token.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/push/manager.py` & `splitio_client-9.7.0/splitio/push/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/push/parser.py` & `splitio_client-9.7.0/splitio/push/parser.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/push/processor.py` & `splitio_client-9.7.0/splitio/push/processor.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/push/segmentworker.py` & `splitio_client-9.7.0/splitio/push/segmentworker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/push/splitsse.py` & `splitio_client-9.7.0/splitio/push/splitsse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/push/splitworker.py` & `splitio_client-9.7.0/splitio/push/splitworker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/push/sse.py` & `splitio_client-9.7.0/splitio/push/sse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/push/status_tracker.py` & `splitio_client-9.7.0/splitio/push/status_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/recorder/recorder.py` & `splitio_client-9.7.0/splitio/recorder/recorder.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/storage/__init__.py` & `splitio_client-9.7.0/splitio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/storage/adapters/cache_trait.py` & `splitio_client-9.7.0/splitio/storage/adapters/cache_trait.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/storage/adapters/redis.py` & `splitio_client-9.7.0/splitio/storage/adapters/redis.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/storage/adapters/util.py` & `splitio_client-9.7.0/splitio/storage/adapters/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/storage/inmemmory.py` & `splitio_client-9.7.0/splitio/storage/inmemmory.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/storage/pluggable.py` & `splitio_client-9.7.0/splitio/storage/pluggable.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
         :rtype: bool
         """
         try:
             return self._pluggable_adapter.item_contains(self._prefix.format(segment_name=segment_name), key)
         except Exception:
             _LOGGER.error('Error checking segment key')
             _LOGGER.debug('Error: ', exc_info=True)
-            return None
+            return False
 
     def get_segment_keys_count(self):
         """
         Get count of all keys in segments.
 
         :return: keys count
         :rtype: int
```

### Comparing `splitio_client-9.6.2/splitio/storage/redis.py` & `splitio_client-9.7.0/splitio/storage/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,19 +384,19 @@
 
         :return: True if the segment contains the key. False otherwise.
         :rtype: bool
         """
         try:
             res = self._redis.sismember(self._get_key(segment_name), key)
             _LOGGER.debug("Checking Segment [%s] contain key [%s] in redis: %s" % (segment_name, key, res))
-            return res
+            return bool(res)
         except RedisAdapterException:
             _LOGGER.error('Error testing members in segment stored in redis')
             _LOGGER.debug('Error: ', exc_info=True)
-            return None
+            return False
 
     def get_segments_count(self):
         """
         Return segment count.
 
         :return: 0
         :rtype: int
```

### Comparing `splitio_client-9.6.2/splitio/sync/event.py` & `splitio_client-9.7.0/splitio/sync/event.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/sync/impression.py` & `splitio_client-9.7.0/splitio/sync/impression.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/sync/manager.py` & `splitio_client-9.7.0/splitio/sync/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/sync/segment.py` & `splitio_client-9.7.0/splitio/sync/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,21 +140,21 @@
 
         :param till: ChangeNumber received.
         :type till: int
 
         :return: True if no error occurs. False otherwise.
         :rtype: bool
         """
-        fetch_options = FetchOptions(True)  # Set Cache-Control to no-cache
+        fetch_options = FetchOptions(True, spec=None)  # Set Cache-Control to no-cache
         successful_sync, remaining_attempts, change_number = self._attempt_segment_sync(segment_name, fetch_options, till)
         attempts = _ON_DEMAND_FETCH_BACKOFF_MAX_RETRIES - remaining_attempts
         if successful_sync:  # succedeed sync
             _LOGGER.debug('Refresh completed in %d attempts.', attempts)
             return True
-        with_cdn_bypass = FetchOptions(True, change_number)  # Set flag for bypassing CDN
+        with_cdn_bypass = FetchOptions(True, change_number, spec=None)  # Set flag for bypassing CDN
         without_cdn_successful_sync, remaining_attempts, change_number = self._attempt_segment_sync(segment_name, with_cdn_bypass, till)
         without_cdn_attempts = _ON_DEMAND_FETCH_BACKOFF_MAX_RETRIES - remaining_attempts
         if without_cdn_successful_sync:
             _LOGGER.debug('Refresh completed bypassing the CDN in %d attempts.',
                           without_cdn_attempts)
             return True
         _LOGGER.debug('No changes fetched after %d attempts with CDN bypassed.',
```

### Comparing `splitio_client-9.6.2/splitio/sync/split.py` & `splitio_client-9.7.0/splitio/sync/split.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/sync/synchronizer.py` & `splitio_client-9.7.0/splitio/sync/synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/sync/telemetry.py` & `splitio_client-9.7.0/splitio/sync/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/sync/unique_keys.py` & `splitio_client-9.7.0/splitio/sync/unique_keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/sync/util.py` & `splitio_client-9.7.0/splitio/sync/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/__init__.py` & `splitio_client-9.7.0/splitio/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/events_sync.py` & `splitio_client-9.7.0/splitio/tasks/events_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/impressions_sync.py` & `splitio_client-9.7.0/splitio/tasks/impressions_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/segment_sync.py` & `splitio_client-9.7.0/splitio/tasks/segment_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/split_sync.py` & `splitio_client-9.7.0/splitio/tasks/split_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/telemetry_sync.py` & `splitio_client-9.7.0/splitio/tasks/telemetry_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/unique_keys_sync.py` & `splitio_client-9.7.0/splitio/tasks/unique_keys_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/util/asynctask.py` & `splitio_client-9.7.0/splitio/tasks/util/asynctask.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/tasks/util/workerpool.py` & `splitio_client-9.7.0/splitio/tasks/util/workerpool.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/util/backoff.py` & `splitio_client-9.7.0/splitio/util/backoff.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/util/storage_helper.py` & `splitio_client-9.7.0/splitio/util/storage_helper.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/util/threadutil.py` & `splitio_client-9.7.0/splitio/util/threadutil.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio/util/time.py` & `splitio_client-9.7.0/splitio/util/time.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.6.2/splitio_client.egg-info/PKG-INFO` & `splitio_client-9.7.0/splitio_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: splitio-client
-Version: 9.6.2
+Version: 9.7.0
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.6.2
+Download-URL: https://github.com/splitio/python-client/tarball/9.7.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `splitio_client-9.6.2/splitio_client.egg-info/SOURCES.txt` & `splitio_client-9.7.0/splitio_client.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 splitio/__init__.py
 splitio/exceptions.py
 splitio/factories.py
 splitio/impressions.py
 splitio/key.py
+splitio/spec.py
 splitio/version.py
 splitio/api/__init__.py
 splitio/api/auth.py
 splitio/api/client.py
 splitio/api/commons.py
 splitio/api/events.py
 splitio/api/impressions.py
@@ -55,16 +57,19 @@
 splitio/models/grammar/condition.py
 splitio/models/grammar/partitions.py
 splitio/models/grammar/matchers/__init__.py
 splitio/models/grammar/matchers/base.py
 splitio/models/grammar/matchers/keys.py
 splitio/models/grammar/matchers/misc.py
 splitio/models/grammar/matchers/numeric.py
+splitio/models/grammar/matchers/semver.py
 splitio/models/grammar/matchers/sets.py
 splitio/models/grammar/matchers/string.py
+splitio/models/grammar/matchers/utils/__init__.py
+splitio/models/grammar/matchers/utils/utils.py
 splitio/push/__init__.py
 splitio/push/manager.py
 splitio/push/parser.py
 splitio/push/processor.py
 splitio/push/segmentworker.py
 splitio/push/splitsse.py
 splitio/push/splitworker.py
@@ -106,8 +111,36 @@
 splitio/util/storage_helper.py
 splitio/util/threadutil.py
 splitio/util/time.py
 splitio_client.egg-info/PKG-INFO
 splitio_client.egg-info/SOURCES.txt
 splitio_client.egg-info/dependency_links.txt
 splitio_client.egg-info/requires.txt
-splitio_client.egg-info/top_level.txt
+splitio_client.egg-info/top_level.txt
+tests/__init__.py
+tests/helpers/__init__.py
+tests/helpers/mockserver.py
+tests/integration/__init__.py
+tests/integration/test_client_e2e.py
+tests/integration/test_redis_integration.py
+tests/integration/test_streaming_e2e.py
+tests/push/__init__.py
+tests/push/test_manager.py
+tests/push/test_parser.py
+tests/push/test_processor.py
+tests/push/test_segment_worker.py
+tests/push/test_split_worker.py
+tests/push/test_splitsse.py
+tests/push/test_sse.py
+tests/push/test_status_tracker.py
+tests/recorder/__init__.py
+tests/recorder/test_recorder.py
+tests/sync/__init__.py
+tests/sync/test_events_synchronizer.py
+tests/sync/test_impressions_count_synchronizer.py
+tests/sync/test_impressions_synchronizer.py
+tests/sync/test_manager.py
+tests/sync/test_segments_synchronizer.py
+tests/sync/test_splits_synchronizer.py
+tests/sync/test_synchronizer.py
+tests/sync/test_telemetry.py
+tests/sync/test_unique_keys_sync.py
```

