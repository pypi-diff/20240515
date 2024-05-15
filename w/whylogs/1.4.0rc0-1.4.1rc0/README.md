# Comparing `tmp/whylogs-1.4.0rc0.tar.gz` & `tmp/whylogs-1.4.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.4.0rc0.tar", max compression
+gzip compressed data, was "whylogs-1.4.1rc0.tar", max compression
```

## Comparing `whylogs-1.4.0rc0.tar` & `whylogs-1.4.1rc0.tar`

### file list

```diff
@@ -1,252 +1,250 @@
--rw-r--r--   0        0        0     3166 2024-04-26 21:02:29.946175 whylogs-1.4.0rc0/DESCRIPTION.md
--rw-r--r--   0        0        0     6650 2024-04-27 00:02:55.944051 whylogs-1.4.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1801 2024-04-26 21:02:30.063493 whylogs-1.4.0rc0/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2024-04-26 21:02:30.063708 whylogs-1.4.0rc0/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2024-04-26 21:02:30.063845 whylogs-1.4.0rc0/whylogs/api/annotations.py
--rw-r--r--   0        0        0      168 2024-04-26 21:02:30.064133 whylogs-1.4.0rc0/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2024-04-26 21:02:30.064351 whylogs-1.4.0rc0/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2024-04-26 21:02:30.064518 whylogs-1.4.0rc0/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0    12819 2024-04-26 21:02:57.083873 whylogs-1.4.0rc0/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0      101 2024-04-26 21:02:30.066009 whylogs-1.4.0rc0/whylogs/api/logger/events/__init__.py
--rw-r--r--   0        0        0     5621 2024-04-26 21:02:30.066189 whylogs-1.4.0rc0/whylogs/api/logger/events/event.py
--rw-r--r--   0        0        0      750 2024-04-26 21:02:30.066765 whylogs-1.4.0rc0/whylogs/api/logger/events/file_name.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.067049 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/__init__.py
--rw-r--r--   0        0        0     7953 2024-04-26 21:02:30.068170 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/actor.py
--rw-r--r--   0        0        0     2614 2024-04-26 21:02:30.068350 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py
--rw-r--r--   0        0        0     1607 2024-04-26 21:02:30.068507 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
--rw-r--r--   0        0        0     1557 2024-04-26 21:02:30.068753 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/future_util.py
--rw-r--r--   0        0        0     1282 2024-04-26 21:02:30.068996 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/list_util.py
--rw-r--r--   0        0        0     1638 2024-04-26 21:02:30.069153 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
--rw-r--r--   0        0        0     5181 2024-04-26 21:02:30.069309 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py
--rw-r--r--   0        0        0      281 2024-04-26 21:02:30.069434 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
--rw-r--r--   0        0        0     5476 2024-04-26 21:02:30.069598 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py
--rw-r--r--   0        0        0    18881 2024-04-26 21:02:57.084243 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
--rw-r--r--   0        0        0     9034 2024-04-26 21:02:30.074524 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
--rw-r--r--   0        0        0      486 2024-04-26 21:02:30.074679 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/signal_util.py
--rw-r--r--   0        0        0      641 2024-04-26 21:02:30.075590 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/string_util.py
--rw-r--r--   0        0        0     3010 2024-04-26 21:02:30.076218 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
--rw-r--r--   0        0        0    18936 2024-04-26 21:02:30.076557 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
--rw-r--r--   0        0        0     4225 2024-04-26 21:02:30.076782 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/time_util.py
--rw-r--r--   0        0        0     5777 2024-04-26 21:02:30.077041 whylogs-1.4.0rc0/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    22351 2024-04-26 21:02:57.084889 whylogs-1.4.0rc0/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9549 2024-04-26 21:02:30.077787 whylogs-1.4.0rc0/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2024-04-26 21:02:30.078010 whylogs-1.4.0rc0/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     7090 2024-04-26 21:02:30.079019 whylogs-1.4.0rc0/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2024-04-26 21:02:30.079308 whylogs-1.4.0rc0/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2024-04-26 21:02:30.079668 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6178 2024-04-26 21:02:30.079867 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7673 2024-04-26 21:02:30.080008 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2024-04-26 21:02:30.080255 whylogs-1.4.0rc0/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2024-04-26 21:02:30.080389 whylogs-1.4.0rc0/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2024-04-26 21:02:30.080528 whylogs-1.4.0rc0/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2024-04-26 21:02:30.081205 whylogs-1.4.0rc0/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2024-04-26 21:02:30.081559 whylogs-1.4.0rc0/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2024-04-26 21:02:30.081764 whylogs-1.4.0rc0/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2024-04-26 21:02:30.082376 whylogs-1.4.0rc0/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2024-04-26 21:02:30.082644 whylogs-1.4.0rc0/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2024-04-26 21:02:30.083354 whylogs-1.4.0rc0/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2024-04-26 21:02:30.083784 whylogs-1.4.0rc0/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2024-04-26 21:02:30.084259 whylogs-1.4.0rc0/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0    18270 2024-04-26 21:02:30.084747 whylogs-1.4.0rc0/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      354 2024-04-26 21:02:30.084948 whylogs-1.4.0rc0/whylogs/api/whylabs/session/lazy.py
--rw-r--r--   0        0        0      442 2024-04-26 21:02:30.085192 whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3893 2024-04-26 21:02:30.085442 whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0     2823 2024-04-26 21:02:30.085705 whylogs-1.4.0rc0/whylogs/api/whylabs/session/prompts.py
--rw-r--r--   0        0        0    13613 2024-04-26 21:02:30.086301 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session.py
--rw-r--r--   0        0        0     6940 2024-04-26 21:02:30.086995 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0     5142 2024-04-26 21:02:30.087545 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      278 2024-04-26 21:02:30.087706 whylogs-1.4.0rc0/whylogs/api/whylabs/session/why_init.py
--rw-r--r--   0        0        0     6581 2024-04-26 21:02:30.087863 whylogs-1.4.0rc0/whylogs/api/whylabs/session/whylabs_client_cache.py
--rw-r--r--   0        0        0     6622 2024-04-26 21:18:13.863456 whylogs-1.4.0rc0/whylogs/api/writer/#whylabs_batch_writer.py#
--rw-r--r--   0        0        0      152 2024-04-26 21:02:57.085198 whylogs-1.4.0rc0/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     3498 2024-04-26 21:02:57.085563 whylogs-1.4.0rc0/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     2300 2024-04-26 21:02:57.085930 whylogs-1.4.0rc0/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2421 2024-04-26 21:02:57.086194 whylogs-1.4.0rc0/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0        0 2024-04-27 00:05:16.106073 whylogs-1.4.0rc0/whylogs/api/writer/richard@richards-MacBook-Pro.26122
--rw-r--r--   0        0        0     4021 2024-04-26 21:02:57.086609 whylogs-1.4.0rc0/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    11074 2024-04-26 22:54:01.723581 whylogs-1.4.0rc0/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0    10110 2024-04-26 21:02:57.087536 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_base.py
--rw-r--r--   0        0        0     6633 2024-04-26 21:16:43.382854 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_batch_writer.py
--rw-r--r--   0        0        0    38861 2024-04-26 21:02:57.088060 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_client.py
--rw-r--r--   0        0        0     4167 2024-04-26 21:02:57.088290 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_estimation_result_writer.py
--rw-r--r--   0        0        0     6678 2024-04-26 21:18:33.755656 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_reference_writer.py
--rw-r--r--   0        0        0     6755 2024-04-26 22:35:16.271359 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_transaction_writer.py
--rw-r--r--   0        0        0     5433 2024-04-26 21:02:57.089133 whylogs-1.4.0rc0/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.089202 whylogs-1.4.0rc0/whylogs/context/__init__.py
--rw-r--r--   0        0        0      302 2024-04-26 21:02:30.089357 whylogs-1.4.0rc0/whylogs/context/environ.py
--rw-r--r--   0        0        0      516 2024-04-26 21:02:30.090077 whylogs-1.4.0rc0/whylogs/context/version.py
--rw-r--r--   0        0        0     1090 2024-04-26 21:02:30.090383 whylogs-1.4.0rc0/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3575 2024-04-26 21:02:30.090535 whylogs-1.4.0rc0/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2024-04-26 21:02:30.090670 whylogs-1.4.0rc0/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2024-04-26 21:02:30.090879 whylogs-1.4.0rc0/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2024-04-26 21:02:30.091165 whylogs-1.4.0rc0/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2024-04-26 21:02:30.091993 whylogs-1.4.0rc0/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2024-04-26 21:02:30.092239 whylogs-1.4.0rc0/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2024-04-26 21:02:30.092453 whylogs-1.4.0rc0/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2024-04-26 21:02:30.092612 whylogs-1.4.0rc0/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2024-04-26 21:02:30.092764 whylogs-1.4.0rc0/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2024-04-26 21:02:30.092928 whylogs-1.4.0rc0/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2024-04-26 21:02:30.093167 whylogs-1.4.0rc0/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2024-04-26 21:02:30.093863 whylogs-1.4.0rc0/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30661 2024-04-26 21:02:30.094241 whylogs-1.4.0rc0/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11321 2024-04-26 21:02:57.089842 whylogs-1.4.0rc0/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4230 2024-04-26 21:02:30.095454 whylogs-1.4.0rc0/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2024-04-26 21:02:30.096077 whylogs-1.4.0rc0/whylogs/core/errors.py
--rw-r--r--   0        0        0     1400 2024-04-26 21:02:57.090158 whylogs-1.4.0rc0/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2024-04-26 21:02:30.096562 whylogs-1.4.0rc0/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     2987 2024-04-26 21:02:30.096782 whylogs-1.4.0rc0/whylogs/core/metadata.py
--rw-r--r--   0        0        0     1740 2024-04-26 21:02:30.096939 whylogs-1.4.0rc0/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2024-04-26 21:02:30.097220 whylogs-1.4.0rc0/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2024-04-26 21:02:30.097456 whylogs-1.4.0rc0/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2024-04-26 21:02:30.097696 whylogs-1.4.0rc0/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2024-04-26 21:02:30.098380 whylogs-1.4.0rc0/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0    10678 2024-04-26 21:02:30.098841 whylogs-1.4.0rc0/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2024-04-26 21:02:30.099685 whylogs-1.4.0rc0/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2024-04-26 21:02:30.099997 whylogs-1.4.0rc0/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2024-04-26 21:02:30.100234 whylogs-1.4.0rc0/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2024-04-26 21:02:30.101104 whylogs-1.4.0rc0/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2024-04-26 21:02:30.101553 whylogs-1.4.0rc0/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2024-04-26 21:02:30.101832 whylogs-1.4.0rc0/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2024-04-26 21:02:30.102576 whylogs-1.4.0rc0/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2024-04-26 21:02:30.102850 whylogs-1.4.0rc0/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2024-04-26 21:02:30.103687 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0    10663 2024-04-26 21:02:30.104196 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2024-04-26 21:02:30.104467 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2024-04-26 21:02:30.104746 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2024-04-26 21:02:30.105006 whylogs-1.4.0rc0/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14608 2024-04-26 21:02:30.105755 whylogs-1.4.0rc0/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2024-04-26 21:02:30.105951 whylogs-1.4.0rc0/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2024-04-26 21:02:30.106363 whylogs-1.4.0rc0/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2024-04-26 21:02:30.106838 whylogs-1.4.0rc0/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2024-04-26 23:53:13.202845 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2024-04-26 23:53:12.021184 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2024-04-26 23:53:12.023238 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2024-04-26 23:53:12.027712 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2024-04-26 23:53:13.448691 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2024-04-26 23:53:12.032451 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2024-04-26 23:53:11.785488 whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2024-04-26 23:53:11.788864 whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2024-04-26 21:02:30.107160 whylogs-1.4.0rc0/whylogs/core/relations.py
--rw-r--r--   0        0        0    11357 2024-04-26 21:02:30.107626 whylogs-1.4.0rc0/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10754 2024-04-26 21:02:30.107983 whylogs-1.4.0rc0/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2024-04-26 21:02:30.108593 whylogs-1.4.0rc0/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2024-04-26 21:02:30.108833 whylogs-1.4.0rc0/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2024-04-26 21:02:30.109060 whylogs-1.4.0rc0/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2118 2024-04-26 21:02:30.109644 whylogs-1.4.0rc0/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2024-04-26 21:02:30.110010 whylogs-1.4.0rc0/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2024-04-26 21:02:30.110216 whylogs-1.4.0rc0/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2024-04-26 21:02:30.110377 whylogs-1.4.0rc0/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2024-04-26 21:02:30.110574 whylogs-1.4.0rc0/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     2004 2024-04-26 21:02:30.110740 whylogs-1.4.0rc0/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      281 2024-04-26 21:02:30.110948 whylogs-1.4.0rc0/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4823 2024-04-26 21:02:30.111113 whylogs-1.4.0rc0/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1329 2024-04-26 21:02:30.111610 whylogs-1.4.0rc0/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2024-04-26 21:02:30.111979 whylogs-1.4.0rc0/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2024-04-26 21:02:30.112333 whylogs-1.4.0rc0/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    18600 2024-04-26 21:02:57.090538 whylogs-1.4.0rc0/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     9474 2024-04-26 21:02:57.091117 whylogs-1.4.0rc0/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2024-04-26 21:02:30.113593 whylogs-1.4.0rc0/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2024-04-26 21:02:30.113832 whylogs-1.4.0rc0/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2024-04-26 21:02:30.114504 whylogs-1.4.0rc0/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.114862 whylogs-1.4.0rc0/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2024-04-26 21:02:30.115167 whylogs-1.4.0rc0/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2024-04-26 21:02:30.116132 whylogs-1.4.0rc0/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2024-04-26 21:02:30.116732 whylogs-1.4.0rc0/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2024-04-26 21:02:30.117401 whylogs-1.4.0rc0/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2024-04-26 21:02:30.117969 whylogs-1.4.0rc0/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2024-04-26 21:02:30.118208 whylogs-1.4.0rc0/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2024-04-26 21:02:30.118700 whylogs-1.4.0rc0/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.118942 whylogs-1.4.0rc0/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.119221 whylogs-1.4.0rc0/whylogs/experimental/api/__init__.py
--rw-r--r--   0        0        0    15177 2024-04-26 21:02:30.119905 whylogs-1.4.0rc0/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2024-04-26 21:02:30.120168 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2024-04-26 21:02:30.120422 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2024-04-26 21:02:30.120686 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2024-04-26 21:02:30.120930 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2024-04-26 21:02:30.121140 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2024-04-26 21:02:30.121327 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2024-04-26 21:02:30.121539 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2024-04-26 21:02:30.122243 whylogs-1.4.0rc0/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    19154 2024-04-26 21:02:30.122535 whylogs-1.4.0rc0/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0      299 2024-04-26 21:02:30.122823 whylogs-1.4.0rc0/whylogs/experimental/core/validators/__init__.py
--rw-r--r--   0        0        0     1218 2024-04-26 21:02:30.122974 whylogs-1.4.0rc0/whylogs/experimental/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1698 2024-04-26 21:02:30.123128 whylogs-1.4.0rc0/whylogs/experimental/core/validators/validator.py
--rw-r--r--   0        0        0     8861 2024-04-26 21:02:30.123654 whylogs-1.4.0rc0/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2024-04-26 21:02:30.123862 whylogs-1.4.0rc0/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2024-04-26 21:02:30.124080 whylogs-1.4.0rc0/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.124365 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-26 21:02:57.091490 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2024-04-26 21:02:30.126148 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2024-04-26 21:02:30.128009 whylogs-1.4.0rc0/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    11126 2024-04-26 21:02:30.128727 whylogs-1.4.0rc0/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2024-04-26 21:02:30.129427 whylogs-1.4.0rc0/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15564 2024-04-26 21:02:30.130625 whylogs-1.4.0rc0/whylogs/migration/converters.py
--rw-r--r--   0        0        0     7662 2024-04-26 21:02:30.130849 whylogs-1.4.0rc0/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2024-04-26 21:02:30.131116 whylogs-1.4.0rc0/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2024-04-26 21:02:30.131338 whylogs-1.4.0rc0/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.131523 whylogs-1.4.0rc0/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    22069 2024-04-26 21:02:30.132305 whylogs-1.4.0rc0/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2024-04-26 21:02:30.132487 whylogs-1.4.0rc0/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.132653 whylogs-1.4.0rc0/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2024-04-26 21:02:30.132892 whylogs-1.4.0rc0/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2024-04-26 21:02:30.133697 whylogs-1.4.0rc0/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2024-04-26 21:02:30.133973 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2024-04-26 21:02:30.134163 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2171 2024-04-26 21:02:57.091852 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2024-04-26 21:02:30.135017 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2024-04-26 21:02:30.135259 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2024-04-26 21:02:30.135605 whylogs-1.4.0rc0/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2024-04-26 21:02:30.135825 whylogs-1.4.0rc0/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2024-04-26 21:02:30.136368 whylogs-1.4.0rc0/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2024-04-26 21:02:30.136699 whylogs-1.4.0rc0/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2024-04-26 21:02:30.137324 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2024-04-26 21:02:30.137795 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2024-04-26 21:02:30.163153 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2024-04-26 21:02:30.163664 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2024-04-26 21:02:30.164714 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2024-04-26 21:02:30.165330 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2024-04-26 21:02:30.165793 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2024-04-26 21:02:30.166103 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2024-04-26 21:02:30.166288 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2024-04-26 21:02:30.166714 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2024-04-26 21:02:30.167040 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2024-04-26 21:02:30.167237 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2024-04-26 21:02:30.167700 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2024-04-26 21:02:30.168007 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2024-04-26 21:02:30.168227 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2024-04-26 21:02:30.168656 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2024-04-26 21:02:30.169371 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2024-04-26 21:02:30.169558 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2024-04-26 21:02:30.170475 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2024-04-26 21:02:30.170829 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2024-04-26 21:02:30.171479 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2024-04-26 21:02:30.171957 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2024-04-26 21:02:30.172659 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2024-04-26 21:02:30.173258 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2024-04-26 21:02:30.173506 whylogs-1.4.0rc0/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2024-04-26 21:02:30.173841 whylogs-1.4.0rc0/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2024-04-26 21:02:30.174623 whylogs-1.4.0rc0/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2024-04-26 21:02:30.175451 whylogs-1.4.0rc0/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2024-04-26 21:02:30.175796 whylogs-1.4.0rc0/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2024-04-26 21:02:30.176016 whylogs-1.4.0rc0/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2024-04-26 21:02:30.176733 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2024-04-26 21:02:30.177157 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2024-04-26 21:02:30.177379 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2024-04-26 21:02:30.177724 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2024-04-26 21:02:30.178049 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2024-04-26 21:02:30.178223 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2024-04-26 21:02:30.178408 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2024-04-26 21:02:30.179832 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2024-04-26 21:02:30.180443 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2024-04-26 21:02:30.180710 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2024-04-26 21:02:30.180899 whylogs-1.4.0rc0/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    22429 2024-04-26 21:02:30.181067 whylogs-1.4.0rc0/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2024-04-26 21:02:30.181325 whylogs-1.4.0rc0/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2024-04-26 21:02:30.181455 whylogs-1.4.0rc0/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2024-04-26 21:02:30.182816 whylogs-1.4.0rc0/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2024-04-26 21:02:30.182997 whylogs-1.4.0rc0/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2024-04-26 21:02:30.186179 whylogs-1.4.0rc0/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1128 2024-04-26 21:02:30.186828 whylogs-1.4.0rc0/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2024-04-26 21:02:30.193627 whylogs-1.4.0rc0/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2024-04-26 21:02:30.193953 whylogs-1.4.0rc0/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     7007 1970-01-01 00:00:00.000000 whylogs-1.4.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     3166 2024-05-13 20:41:30.719503 whylogs-1.4.1rc0/DESCRIPTION.md
+-rw-r--r--   0        0        0     6650 2024-05-15 03:01:34.485133 whylogs-1.4.1rc0/pyproject.toml
+-rw-r--r--   0        0        0     1801 2024-05-13 20:41:30.907000 whylogs-1.4.1rc0/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2024-05-13 20:41:30.907352 whylogs-1.4.1rc0/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-13 20:41:30.907525 whylogs-1.4.1rc0/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      168 2024-05-13 20:41:30.907751 whylogs-1.4.1rc0/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2024-05-13 20:41:30.907985 whylogs-1.4.1rc0/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2024-05-13 20:41:30.908136 whylogs-1.4.1rc0/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0    12819 2024-05-13 20:41:30.908467 whylogs-1.4.1rc0/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-13 20:41:30.908686 whylogs-1.4.1rc0/whylogs/api/logger/events/__init__.py
+-rw-r--r--   0        0        0     5621 2024-05-13 20:41:30.908950 whylogs-1.4.1rc0/whylogs/api/logger/events/event.py
+-rw-r--r--   0        0        0      750 2024-05-13 20:41:30.909958 whylogs-1.4.1rc0/whylogs/api/logger/events/file_name.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.910300 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/__init__.py
+-rw-r--r--   0        0        0     7953 2024-05-13 20:41:30.910669 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/actor.py
+-rw-r--r--   0        0        0     2614 2024-05-13 20:41:30.910850 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py
+-rw-r--r--   0        0        0     1607 2024-05-13 20:41:30.911008 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
+-rw-r--r--   0        0        0     1557 2024-05-13 20:41:30.911170 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/future_util.py
+-rw-r--r--   0        0        0     1282 2024-05-13 20:41:30.911337 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/list_util.py
+-rw-r--r--   0        0        0     1638 2024-05-13 20:41:30.911582 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
+-rw-r--r--   0        0        0     5181 2024-05-13 20:41:30.911910 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py
+-rw-r--r--   0        0        0      281 2024-05-13 20:41:30.912206 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
+-rw-r--r--   0        0        0     5476 2024-05-13 20:41:30.912493 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py
+-rw-r--r--   0        0        0    18881 2024-05-13 20:41:30.912846 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
+-rw-r--r--   0        0        0     9034 2024-05-13 20:41:30.913261 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
+-rw-r--r--   0        0        0      486 2024-05-13 20:41:30.913499 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/signal_util.py
+-rw-r--r--   0        0        0      641 2024-05-13 20:41:30.913745 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/string_util.py
+-rw-r--r--   0        0        0     3010 2024-05-13 20:41:30.913978 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
+-rw-r--r--   0        0        0    18936 2024-05-13 20:41:30.914261 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
+-rw-r--r--   0        0        0     4225 2024-05-13 20:41:30.914591 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/time_util.py
+-rw-r--r--   0        0        0     5777 2024-05-13 20:41:30.914912 whylogs-1.4.1rc0/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    22400 2024-05-15 02:30:21.369918 whylogs-1.4.1rc0/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9549 2024-05-13 20:41:30.915622 whylogs-1.4.1rc0/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2024-05-13 20:41:30.915893 whylogs-1.4.1rc0/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     7090 2024-05-13 20:41:30.916267 whylogs-1.4.1rc0/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2024-05-13 20:41:30.916520 whylogs-1.4.1rc0/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2024-05-13 20:41:30.917022 whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6178 2024-05-13 20:41:30.917370 whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7673 2024-05-13 20:41:30.917928 whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2024-05-13 20:41:30.918356 whylogs-1.4.1rc0/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2024-05-13 20:41:30.918577 whylogs-1.4.1rc0/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2024-05-13 20:41:30.918825 whylogs-1.4.1rc0/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2024-05-13 20:41:30.919109 whylogs-1.4.1rc0/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2024-05-13 20:41:30.919586 whylogs-1.4.1rc0/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2024-05-13 20:41:30.919946 whylogs-1.4.1rc0/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2024-05-13 20:41:30.920220 whylogs-1.4.1rc0/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2024-05-13 20:41:30.920477 whylogs-1.4.1rc0/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2024-05-13 20:41:30.920840 whylogs-1.4.1rc0/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2024-05-13 20:41:30.921341 whylogs-1.4.1rc0/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2024-05-13 20:41:30.921727 whylogs-1.4.1rc0/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0    18270 2024-05-13 20:41:30.922239 whylogs-1.4.1rc0/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      354 2024-05-13 20:41:30.922431 whylogs-1.4.1rc0/whylogs/api/whylabs/session/lazy.py
+-rw-r--r--   0        0        0      442 2024-05-13 20:41:30.922716 whylogs-1.4.1rc0/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3893 2024-05-13 20:41:30.922952 whylogs-1.4.1rc0/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0     2823 2024-05-13 20:41:30.923189 whylogs-1.4.1rc0/whylogs/api/whylabs/session/prompts.py
+-rw-r--r--   0        0        0    13613 2024-05-13 20:41:30.923686 whylogs-1.4.1rc0/whylogs/api/whylabs/session/session.py
+-rw-r--r--   0        0        0     6940 2024-05-13 20:41:30.923985 whylogs-1.4.1rc0/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0     5142 2024-05-13 20:41:30.924237 whylogs-1.4.1rc0/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      278 2024-05-13 20:41:30.924455 whylogs-1.4.1rc0/whylogs/api/whylabs/session/why_init.py
+-rw-r--r--   0        0        0     6581 2024-05-13 20:41:30.924726 whylogs-1.4.1rc0/whylogs/api/whylabs/session/whylabs_client_cache.py
+-rw-r--r--   0        0        0      152 2024-05-13 20:41:30.925032 whylogs-1.4.1rc0/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     3498 2024-05-13 20:41:30.925288 whylogs-1.4.1rc0/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     2300 2024-05-13 20:41:30.925512 whylogs-1.4.1rc0/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2421 2024-05-13 20:41:30.925673 whylogs-1.4.1rc0/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     4021 2024-05-13 20:41:30.925836 whylogs-1.4.1rc0/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    11074 2024-05-13 20:41:30.926073 whylogs-1.4.1rc0/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0    10271 2024-05-13 20:41:30.926311 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_base.py
+-rw-r--r--   0        0        0     6668 2024-05-13 20:41:30.926551 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_batch_writer.py
+-rw-r--r--   0        0        0    39735 2024-05-13 20:41:30.926792 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_client.py
+-rw-r--r--   0        0        0     4167 2024-05-13 20:41:30.927025 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_estimation_result_writer.py
+-rw-r--r--   0        0        0     6713 2024-05-13 20:41:30.927310 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_reference_writer.py
+-rw-r--r--   0        0        0     6789 2024-05-13 20:41:30.927510 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_transaction_writer.py
+-rw-r--r--   0        0        0     5433 2024-05-13 20:41:30.927736 whylogs-1.4.1rc0/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.927915 whylogs-1.4.1rc0/whylogs/context/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-13 20:41:30.928076 whylogs-1.4.1rc0/whylogs/context/environ.py
+-rw-r--r--   0        0        0      516 2024-05-13 20:41:30.928216 whylogs-1.4.1rc0/whylogs/context/version.py
+-rw-r--r--   0        0        0     1090 2024-05-13 20:41:30.928921 whylogs-1.4.1rc0/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3575 2024-05-13 20:41:30.929096 whylogs-1.4.1rc0/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2024-05-13 20:41:30.929270 whylogs-1.4.1rc0/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2024-05-13 20:41:30.929429 whylogs-1.4.1rc0/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2024-05-13 20:41:30.929662 whylogs-1.4.1rc0/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2024-05-13 20:41:30.929899 whylogs-1.4.1rc0/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-13 20:41:30.930056 whylogs-1.4.1rc0/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2024-05-13 20:41:30.930215 whylogs-1.4.1rc0/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2024-05-13 20:41:30.931005 whylogs-1.4.1rc0/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2024-05-13 20:41:30.931353 whylogs-1.4.1rc0/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2024-05-13 20:41:30.931575 whylogs-1.4.1rc0/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2024-05-13 20:41:30.931751 whylogs-1.4.1rc0/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2024-05-13 20:41:30.931922 whylogs-1.4.1rc0/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30661 2024-05-13 20:41:30.932293 whylogs-1.4.1rc0/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11321 2024-05-13 20:41:30.932713 whylogs-1.4.1rc0/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4230 2024-05-13 20:41:30.933105 whylogs-1.4.1rc0/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2024-05-13 20:41:30.933342 whylogs-1.4.1rc0/whylogs/core/errors.py
+-rw-r--r--   0        0        0     1453 2024-05-15 02:30:21.370599 whylogs-1.4.1rc0/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2024-05-13 20:41:30.933808 whylogs-1.4.1rc0/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     2987 2024-05-13 20:41:30.934024 whylogs-1.4.1rc0/whylogs/core/metadata.py
+-rw-r--r--   0        0        0     1740 2024-05-13 20:41:30.934222 whylogs-1.4.1rc0/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2024-05-13 20:41:30.934991 whylogs-1.4.1rc0/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2024-05-13 20:41:30.935290 whylogs-1.4.1rc0/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2024-05-13 20:41:30.935564 whylogs-1.4.1rc0/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2024-05-13 20:41:30.935923 whylogs-1.4.1rc0/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0    10678 2024-05-13 20:41:30.936222 whylogs-1.4.1rc0/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2024-05-13 20:41:30.936404 whylogs-1.4.1rc0/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2024-05-13 20:41:30.936738 whylogs-1.4.1rc0/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2024-05-13 20:41:30.936912 whylogs-1.4.1rc0/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2024-05-13 20:41:30.937166 whylogs-1.4.1rc0/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2024-05-13 20:41:30.937492 whylogs-1.4.1rc0/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2024-05-13 20:41:30.937745 whylogs-1.4.1rc0/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2024-05-13 20:41:30.938071 whylogs-1.4.1rc0/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2024-05-13 20:41:30.938345 whylogs-1.4.1rc0/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2024-05-13 20:41:30.938605 whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0    10663 2024-05-13 20:41:30.938862 whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2024-05-13 20:41:30.939106 whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2024-05-13 20:41:30.939268 whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2024-05-13 20:41:30.939524 whylogs-1.4.1rc0/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14608 2024-05-13 20:41:30.939849 whylogs-1.4.1rc0/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2024-05-13 20:41:30.940059 whylogs-1.4.1rc0/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2024-05-13 20:41:30.940367 whylogs-1.4.1rc0/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2024-05-13 20:41:30.940631 whylogs-1.4.1rc0/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2024-05-15 03:02:34.632043 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2024-05-15 03:02:33.305842 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2024-05-15 03:02:33.307701 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2024-05-15 03:02:33.310293 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2024-05-15 03:02:34.877348 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2024-05-15 03:02:33.315543 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2024-05-15 03:02:33.030760 whylogs-1.4.1rc0/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2024-05-15 03:02:33.036140 whylogs-1.4.1rc0/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2024-05-13 20:41:30.940879 whylogs-1.4.1rc0/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11357 2024-05-13 20:41:30.941200 whylogs-1.4.1rc0/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10754 2024-05-13 20:41:30.941456 whylogs-1.4.1rc0/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2024-05-13 20:41:30.941607 whylogs-1.4.1rc0/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2024-05-13 20:41:30.941773 whylogs-1.4.1rc0/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2024-05-13 20:41:30.941963 whylogs-1.4.1rc0/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2118 2024-05-13 20:41:30.942176 whylogs-1.4.1rc0/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2024-05-13 20:41:30.942405 whylogs-1.4.1rc0/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2024-05-13 20:41:30.942560 whylogs-1.4.1rc0/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2024-05-13 20:41:30.942700 whylogs-1.4.1rc0/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2024-05-13 20:41:30.942853 whylogs-1.4.1rc0/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     2004 2024-05-13 20:41:30.943026 whylogs-1.4.1rc0/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      281 2024-05-13 20:41:30.943287 whylogs-1.4.1rc0/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4823 2024-05-13 20:41:30.943558 whylogs-1.4.1rc0/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1329 2024-05-13 20:41:30.943778 whylogs-1.4.1rc0/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2024-05-13 20:41:30.944297 whylogs-1.4.1rc0/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2024-05-13 20:41:30.944676 whylogs-1.4.1rc0/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    18600 2024-05-13 20:41:30.945021 whylogs-1.4.1rc0/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     9474 2024-05-13 20:41:30.945420 whylogs-1.4.1rc0/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2024-05-13 20:41:30.945789 whylogs-1.4.1rc0/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2024-05-13 20:41:30.946183 whylogs-1.4.1rc0/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2024-05-13 20:41:30.946534 whylogs-1.4.1rc0/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.946810 whylogs-1.4.1rc0/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2024-05-13 20:41:30.947195 whylogs-1.4.1rc0/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2024-05-13 20:41:30.947472 whylogs-1.4.1rc0/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2024-05-13 20:41:30.948164 whylogs-1.4.1rc0/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2024-05-13 20:41:30.949324 whylogs-1.4.1rc0/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2024-05-13 20:41:30.950641 whylogs-1.4.1rc0/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2024-05-13 20:41:30.950920 whylogs-1.4.1rc0/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2024-05-13 20:41:30.951685 whylogs-1.4.1rc0/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.952010 whylogs-1.4.1rc0/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.952250 whylogs-1.4.1rc0/whylogs/experimental/api/__init__.py
+-rw-r--r--   0        0        0    16453 2024-05-13 20:41:30.952578 whylogs-1.4.1rc0/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2024-05-13 20:41:30.952889 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2024-05-13 20:41:30.953055 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2024-05-13 20:41:30.953221 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2024-05-13 20:41:30.953384 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2024-05-13 20:41:30.953622 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2024-05-13 20:41:30.954215 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2024-05-13 20:41:30.954467 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2024-05-13 20:41:30.955051 whylogs-1.4.1rc0/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    19154 2024-05-13 20:41:30.955300 whylogs-1.4.1rc0/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0      299 2024-05-13 20:41:30.955597 whylogs-1.4.1rc0/whylogs/experimental/core/validators/__init__.py
+-rw-r--r--   0        0        0     1218 2024-05-13 20:41:30.955843 whylogs-1.4.1rc0/whylogs/experimental/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1698 2024-05-13 20:41:30.956083 whylogs-1.4.1rc0/whylogs/experimental/core/validators/validator.py
+-rw-r--r--   0        0        0     8861 2024-05-13 20:41:30.956579 whylogs-1.4.1rc0/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2024-05-13 20:41:30.956884 whylogs-1.4.1rc0/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2024-05-13 20:41:30.957168 whylogs-1.4.1rc0/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.957460 whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1369 2024-05-15 02:30:21.371374 whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2024-05-13 20:41:30.958548 whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2024-05-13 20:41:30.959073 whylogs-1.4.1rc0/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    11126 2024-05-13 20:41:30.959737 whylogs-1.4.1rc0/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2024-05-13 20:41:30.960137 whylogs-1.4.1rc0/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15564 2024-05-13 20:41:30.960577 whylogs-1.4.1rc0/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     7662 2024-05-13 20:41:30.960903 whylogs-1.4.1rc0/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2024-05-13 20:41:30.961302 whylogs-1.4.1rc0/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2024-05-13 20:41:30.961582 whylogs-1.4.1rc0/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.961990 whylogs-1.4.1rc0/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    22069 2024-05-13 20:41:30.962393 whylogs-1.4.1rc0/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2024-05-13 20:41:30.962713 whylogs-1.4.1rc0/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.962986 whylogs-1.4.1rc0/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2024-05-13 20:41:30.963500 whylogs-1.4.1rc0/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:41:30.963787 whylogs-1.4.1rc0/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2024-05-13 20:41:30.964141 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2024-05-13 20:41:30.964338 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2221 2024-05-15 02:30:21.372269 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2024-05-13 20:41:30.965593 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2024-05-13 20:41:30.965806 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2024-05-13 20:41:30.966035 whylogs-1.4.1rc0/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2024-05-13 20:41:30.966197 whylogs-1.4.1rc0/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2024-05-13 20:41:30.966896 whylogs-1.4.1rc0/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2024-05-13 20:41:30.967298 whylogs-1.4.1rc0/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2024-05-13 20:41:30.968459 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2024-05-13 20:41:30.969346 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2024-05-13 20:41:30.970143 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2024-05-13 20:41:30.971247 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2024-05-13 20:41:30.971901 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2024-05-13 20:41:30.972211 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2024-05-13 20:41:30.973349 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2024-05-13 20:41:30.973892 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2024-05-13 20:41:30.975202 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2024-05-13 20:41:30.976031 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2024-05-13 20:41:30.977239 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2024-05-13 20:41:30.977969 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2024-05-13 20:41:30.978839 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2024-05-13 20:41:30.979722 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2024-05-13 20:41:30.980137 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2024-05-13 20:41:30.980848 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2024-05-13 20:41:30.981667 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2024-05-13 20:41:30.981990 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2024-05-13 20:41:30.982756 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2024-05-13 20:41:30.983725 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2024-05-13 20:41:30.984109 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2024-05-13 20:41:30.984873 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2024-05-13 20:41:30.985612 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2024-05-13 20:41:30.985962 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2024-05-13 20:41:30.986354 whylogs-1.4.1rc0/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2024-05-13 20:41:30.986744 whylogs-1.4.1rc0/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2024-05-13 20:41:30.988999 whylogs-1.4.1rc0/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2024-05-13 20:41:30.989496 whylogs-1.4.1rc0/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2024-05-13 20:41:30.990082 whylogs-1.4.1rc0/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2024-05-13 20:41:30.990502 whylogs-1.4.1rc0/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2024-05-13 20:41:30.991128 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2024-05-13 20:41:30.991614 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2024-05-13 20:41:30.992038 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2024-05-13 20:41:30.992470 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2024-05-13 20:41:30.992839 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2024-05-13 20:41:30.993104 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2024-05-13 20:41:30.993447 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2024-05-13 20:41:30.995992 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2024-05-13 20:41:30.997043 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2024-05-13 20:41:30.998284 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2024-05-13 20:41:30.998658 whylogs-1.4.1rc0/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    22429 2024-05-13 20:41:30.998983 whylogs-1.4.1rc0/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2024-05-13 20:41:30.999513 whylogs-1.4.1rc0/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2024-05-13 20:41:30.999780 whylogs-1.4.1rc0/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2024-05-13 20:41:31.000214 whylogs-1.4.1rc0/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2024-05-13 20:41:31.000477 whylogs-1.4.1rc0/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2024-05-13 20:41:31.000760 whylogs-1.4.1rc0/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1128 2024-05-13 20:41:31.000999 whylogs-1.4.1rc0/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2024-05-13 20:41:31.001387 whylogs-1.4.1rc0/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2024-05-13 20:41:31.001651 whylogs-1.4.1rc0/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     7007 1970-01-01 00:00:00.000000 whylogs-1.4.1rc0/PKG-INFO
```

### Comparing `whylogs-1.4.0rc0/DESCRIPTION.md` & `whylogs-1.4.1rc0/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/pyproject.toml` & `whylogs-1.4.1rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.4.0-rc0"
+version = "1.4.1-rc0"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
```

### Comparing `whylogs-1.4.0rc0/whylogs/__init__.py` & `whylogs-1.4.1rc0/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/annotations.py` & `whylogs-1.4.1rc0/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/fugue/profiler.py` & `whylogs-1.4.1rc0/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/fugue/registry.py` & `whylogs-1.4.1rc0/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/__init__.py` & `whylogs-1.4.1rc0/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/events/event.py` & `whylogs-1.4.1rc0/whylogs/api/logger/events/event.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/events/file_name.py` & `whylogs-1.4.1rc0/whylogs/api/logger/events/file_name.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/actor.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/future_util.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/future_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/list_util.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/list_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/string_util.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/string_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/time_util.py` & `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/time_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/logger.py` & `whylogs-1.4.1rc0/whylogs/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/result_set.py` & `whylogs-1.4.1rc0/whylogs/api/logger/result_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from logging import getLogger
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from whylabs_client.model.segment_tag import SegmentTag
 
 from whylogs.api.reader import Reader, Readers
-from whylogs.api.writer.writer import Writable
+from whylogs.api.writer.writer import Writable, WriterWrapper
 from whylogs.core import DatasetProfile, DatasetProfileView, Segment
 from whylogs.core.metrics.metrics import Metric
 from whylogs.core.model_performance_metrics import ModelPerformanceMetrics
 from whylogs.core.segmentation_partition import SegmentationPartition
 from whylogs.core.utils import ensure_timezone
 from whylogs.core.view.dataset_profile_view import _MODEL_PERFORMANCE
 from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
@@ -571,7 +571,10 @@
             merged_metrics = _merge_metrics(self.dataset_metrics, other.dataset_metrics)
             merged_partitions = _merge_partitions(lhs_partitions, rhs_partitions)
             properties = _accumulate_properties(self._dataset_properties, other.dataset_properties)
 
             return SegmentedResultSet(merged_segments, merged_partitions, metrics=merged_metrics, properties=properties)
         else:
             raise ValueError(f"Cannot merge incompatible SegmentedResultSet and {type(other)}")
+
+
+ResultSetWriter = WriterWrapper
```

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/rolling.py` & `whylogs-1.4.1rc0/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/segment_cache.py` & `whylogs-1.4.1rc0/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/segment_processing.py` & `whylogs-1.4.1rc0/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/logger/transient.py` & `whylogs-1.4.1rc0/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/reader/local.py` & `whylogs-1.4.1rc0/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/reader/reader.py` & `whylogs-1.4.1rc0/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/reader/s3.py` & `whylogs-1.4.1rc0/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/store/local_store.py` & `whylogs-1.4.1rc0/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/store/profile_store.py` & `whylogs-1.4.1rc0/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/store/query.py` & `whylogs-1.4.1rc0/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/store/sqlite_store.py` & `whylogs-1.4.1rc0/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/usage_stats/__init__.py` & `whylogs-1.4.1rc0/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/whylabs/session/config.py` & `whylogs-1.4.1rc0/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.4.1rc0/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/whylabs/session/prompts.py` & `whylogs-1.4.1rc0/whylogs/api/whylabs/session/prompts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session.py` & `whylogs-1.4.1rc0/whylogs/api/whylabs/session/session.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.4.1rc0/whylogs/api/whylabs/session/session_manager.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.4.1rc0/whylogs/api/whylabs/session/session_types.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/whylabs/session/whylabs_client_cache.py` & `whylogs-1.4.1rc0/whylogs/api/whylabs/session/whylabs_client_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/#whylabs_batch_writer.py#` & `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_batch_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,17 +131,19 @@
         return self._upload_view(view, profile_id, upload_url, dataset_timestamp_epoch, **kwargs)
 
     @deprecated_alias(profile="file")
     def write(
         self, file: Writable, dest: Optional[str] = None, **kwargs: Any
     ) -> Tuple[bool, Union[str, List[Tuple[bool, str]]]]:
         self._whylabs_client = self._whylabs_client.option(**kwargs)  # type: ignore
+        self._custom_tagging(file)
 
         if isinstance(file, SegmentedResultSet):
-            if kwargs.get("zip"):  # TODO: force zip if the number of segemtns is large
+            # TODO: force zip if the number of segemtns is large
+            if kwargs.get("zip"):
                 return self._write_segmented_result_set_zip(file, **kwargs)
             else:
                 return self._write_segmented_result_set(file, **kwargs)
 
         # file represents a single profile/segment, extract a view of it
         view = self._get_view_of_writable(file)
         return self._write_view(view, **kwargs)
```

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/gcs.py` & `whylogs-1.4.1rc0/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/local.py` & `whylogs-1.4.1rc0/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/mlflow.py` & `whylogs-1.4.1rc0/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/s3.py` & `whylogs-1.4.1rc0/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/whylabs.py` & `whylogs-1.4.1rc0/whylogs/api/writer/whylabs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_base.py` & `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tempfile
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import requests  # type: ignore
 from whylabs_client import ApiClient
 from whylabs_client.model.segment_tag import SegmentTag
 
-from whylogs.api.logger.result_set import ProfileResultSet, ViewResultSet
+from whylogs.api.logger.result_set import ProfileResultSet, ResultSet, ViewResultSet
 from whylogs.api.whylabs.session.session_manager import default_init
 from whylogs.api.writer.whylabs_client import WhyLabsClient
 from whylogs.api.writer.writer import Writable, Writer
 from whylogs.core import DatasetProfileView
 from whylogs.core.dataset_profile import DatasetProfile
 from whylogs.core.errors import BadConfigError
 from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
@@ -173,24 +173,27 @@
             logger.error(
                 f"Profiles should have timestamps greater than 0, but found a timestamp of {stamp}"
                 f" and current timestamp is {utc_now.timestamp()}, this is likely an error."
             )
 
         return int(stamp * 1000)
 
+    def _custom_tagging(
+        self,
+        view: Union[DatasetProfile, DatasetProfileView, SegmentedDatasetProfileView, ResultSet],
+    ) -> None:
+        self._whylabs_client._tag_custom_perf_metrics(view)
+        self._whylabs_client._tag_custom_output_metrics(view)
+
     def _prepare_view_for_upload(
         self,
         view: Union[DatasetProfileView, SegmentedDatasetProfileView],
     ) -> Union[DatasetProfileView, SegmentedDatasetProfileView]:
         view_is_a_segment = isinstance(view, SegmentedDatasetProfileView)
-        self._whylabs_client._tag_custom_perf_metrics(view)
-        self._whylabs_client._tag_custom_output_metrics(view)
-
         flags = FeatureFlags(_check_whylabs_condition_count_uncompound())
-
         if _uncompound_metric_feature_flag():
             if view_is_a_segment:
                 updated_profile_view = _uncompound_dataset_profile(view.profile_view, flags)
                 view = SegmentedDatasetProfileView(
                     profile_view=updated_profile_view, segment=view._segment, partition=view._partition
                 )
```

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_batch_writer.py` & `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_reference_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import logging
 import tempfile
 from typing import Any, List, Optional, Tuple, Union
 from zipfile import ZipFile
 
 from whylabs_client import ApiClient
 
@@ -14,17 +13,17 @@
 from whylogs.core import DatasetProfileView
 from whylogs.core.utils import deprecated_alias
 from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
 
 logger = logging.getLogger(__name__)
 
 
-class WhyLabsBatchWriter(WhyLabsWriterBase):
+class WhyLabsReferenceWriter(WhyLabsWriterBase):
     f"""
-    A WhyLogs writer to upload batch profiles onto the WhyLabs platform.
+    A WhyLogs writer to upload reference profiles onto the WhyLabs platform.
 
     >**IMPORTANT**: In order to correctly send your profiles over, make sure you have
     the following environment variables set: `[WHYLABS_ORG_ID, WHYLABS_API_KEY, WHYLABS_DEFAULT_DATASET_ID]`. You
     can also follow the authentication instructions for the why.init() method at {INIT_DOCS}.
     It is highly recommended you don't persist credentials in code!
 
     You shouldn't have to supply these parameters to the writer in practice. You should depend on why.init() to resolve
@@ -71,47 +70,46 @@
 
     def _write_segmented_result_set(self, file: SegmentedResultSet, **kwargs: Any) -> Tuple[bool, str]:
         views = file.get_writables()
         if not views:
             logger.warning("Attempt to write a result set with no writables, nothing written!")
             return True, ""
 
-        utc_now = datetime.datetime.now(datetime.timezone.utc)
-        messages: List[str] = list()
+        whylabs_tags = file.get_whylabs_tags()
+        dataset_timestamp_epoch = self._get_dataset_epoch(views[-1])  # original writer used timestamp of last segment
         and_status: bool = True
-        logger.debug(f"About to write {len(views)} files:")
-        # TODO: special handling of large number of files, handle throttling
-        for view in views:
-            dataset_timestamp_epoch = self._get_dataset_epoch(view, utc_now)
-            profile_id, upload_url = self._whylabs_client.get_upload_url_batch(dataset_timestamp_epoch)  # type: ignore
-            bool_status, message = self._upload_view(view, profile_id, upload_url, dataset_timestamp_epoch)
-            messages.append(message)
+        profile_id, upload_urls = self._whylabs_client._get_upload_urls_segmented_reference(  # type: ignore
+            whylabs_tags, dataset_timestamp_epoch, self._reference_profile_name
+        )
+        for view, url in zip(views, upload_urls):
+            bool_status, message = self._upload_view(view, profile_id, url, dataset_timestamp_epoch)
             and_status = and_status and bool_status
 
-        logger.debug(f"Completed writing {len(views)} files!")
-        return and_status, ("; ".join(messages) if and_status else "Failed to upload all segments")
+        return and_status, (message if and_status else "Failed to upload all segments")
 
     # TODO: Sadly, we can't use Writer::_create_zip() because we have to fiddle with the
     # views before serializing them. We could add a Writable fiddling call-back argument
     # to _create_zip(), but this isn't too bad...
     def _write_segmented_result_set_zip(self, file: SegmentedResultSet, **kwargs: Any) -> Tuple[bool, str]:
         views = file.get_writables()
         if not views:
             logger.warning("Attempt to write a result set with no writables, nothing written!")
             return True, ""
 
-        utc_now = datetime.datetime.now(datetime.timezone.utc)
-        dataset_timestamp_epoch = self._get_dataset_epoch(views[0], utc_now)
-        profile_id, upload_url = self._whylabs_client.get_upload_url_batch_zip(dataset_timestamp_epoch)  # type: ignore
+        whylabs_tags = file.get_whylabs_tags()
+        dataset_timestamp_epoch = self._get_dataset_epoch(views[-1])  # original writer used timestamp of last segment
+        profile_id, upload_url = self._whylabs_client._get_upload_url_segmented_reference_zip(  # type: ignore
+            whylabs_tags, dataset_timestamp_epoch, self._reference_profile_name
+        )
         with tempfile.NamedTemporaryFile(suffix=".zip") as tmp_file:
             with ZipFile(tmp_file, "w", allowZip64=True) as zip_file:
                 for view in views:
                     view = self._prepare_view_for_upload(view)
                     with tempfile.NamedTemporaryFile() as view_file:
-                        view.write(file=view_file)
+                        view.write(file=view_file)  # TODO: error checking
                         view_file.flush()
                         view_file.seek(0)
                         zip_file.write(view_file.name, view_file.name.split("/")[-1])
 
             tmp_file.flush()
             tmp_file.seek(0)
             return self._whylabs_client.do_upload(  # type: ignore
@@ -123,26 +121,29 @@
 
     def _write_view(
         self,
         view: Union[DatasetProfileView, SegmentedDatasetProfileView],
         **kwargs: Any,
     ) -> Tuple[bool, str]:
         dataset_timestamp_epoch = self._get_dataset_epoch(view)
-        profile_id, upload_url = self._whylabs_client.get_upload_url_batch(dataset_timestamp_epoch)  # type: ignore
+        profile_id, upload_url = self._whylabs_client.get_upload_url_unsegmented_reference(  # type: ignore
+            dataset_timestamp_epoch, self._reference_profile_name
+        )
         return self._upload_view(view, profile_id, upload_url, dataset_timestamp_epoch, **kwargs)
 
     @deprecated_alias(profile="file")
     def write(
         self, file: Writable, dest: Optional[str] = None, **kwargs: Any
     ) -> Tuple[bool, Union[str, List[Tuple[bool, str]]]]:
+        self.option(**kwargs)
         self._whylabs_client = self._whylabs_client.option(**kwargs)  # type: ignore
+        self._custom_tagging(file)
 
         if isinstance(file, SegmentedResultSet):
-            # TODO: force zip if the number of segemtns is large
-            if kwargs.get("zip"):
+            if kwargs.get("zip"):  # TODO: force zip if the number of segemtns is large
                 return self._write_segmented_result_set_zip(file, **kwargs)
             else:
                 return self._write_segmented_result_set(file, **kwargs)
 
         # file represents a single profile/segment, extract a view of it
         view = self._get_view_of_writable(file)
         return self._write_view(view, **kwargs)
```

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_client.py` & `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import pprint
-from typing import IO, Any, Dict, List, Optional, Tuple, Union
+from typing import IO, Any, Dict, List, Optional, Set, Tuple, Union
 from urllib.parse import urlparse
 
 import requests  # type: ignore
 from urllib3 import PoolManager, ProxyManager
 from whylabs_client import ApiClient, Configuration  # type: ignore
 from whylabs_client.api.dataset_profile_api import DatasetProfileApi  # type: ignore
 from whylabs_client.api.feature_weights_api import FeatureWeightsApi  # type: ignore
@@ -28,23 +28,24 @@
 from whylabs_client.model.segment import Segment  # type: ignore
 from whylabs_client.model.segment_tag import SegmentTag  # type: ignore
 from whylabs_client.model.transaction_commit_request import TransactionCommitRequest
 from whylabs_client.model.transaction_log_request import TransactionLogRequest
 from whylabs_client.model.transaction_start_request import TransactionStartRequest
 from whylabs_client.rest import ForbiddenException  # type: ignore
 
+from whylogs.api.logger.result_set import ResultSet, SegmentedResultSet
 from whylogs.api.whylabs.session.session_manager import INIT_DOCS, default_init
 from whylogs.api.whylabs.session.whylabs_client_cache import (
     ClientCacheConfig,
     EnvironmentKeyRefresher,
     KeyRefresher,
     WhylabsClientCache,
 )
 from whylogs.context.environ import read_bool_env_var
-from whylogs.core import DatasetProfileView
+from whylogs.core import DatasetProfile, DatasetProfileView
 from whylogs.core.feature_weights import FeatureWeights
 from whylogs.core.utils.utils import get_auth_headers
 from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
 
 FIVE_MINUTES_IN_SECONDS = 60 * 5
 DAY_IN_SECONDS = 60 * 60 * 24
 FIVE_YEARS_IN_SECONDS = DAY_IN_SECONDS * 365 * 5
@@ -78,14 +79,36 @@
     "top_rank": ("integral", "continuous"),
     "average_precision_k_": ("fractional", "continuous"),
     "norm_dis_cumul_gain_k_": ("fractional", "continuous"),
     "sum_gain_k_": ("fractional", "continuous"),
 }
 
 
+def _get_column_names(x: Union[DatasetProfile, DatasetProfileView, SegmentedDatasetProfileView, ResultSet]) -> Set[str]:
+    if isinstance(x, DatasetProfile):
+        return _get_column_names(x.view())
+    elif isinstance(x, DatasetProfileView):
+        return set(x.get_columns().keys())
+    elif isinstance(x, SegmentedDatasetProfileView):
+        return _get_column_names(x._profile_view)
+    elif isinstance(x, SegmentedResultSet):
+        maps = x._segments.values()
+        if not maps:
+            return set()
+        segments = list(maps)[0].values()
+        if not segments:
+            return set()
+        segment = list(segments)[0]
+        view = segment if isinstance(segment, DatasetProfileView) else segment.view()
+        return _get_column_names(view)
+
+    assert isinstance(x, ResultSet)
+    return _get_column_names(x.view())
+
+
 class TransactionAbortedException(Exception):
     pass
 
 
 class WhyLabsClient:
     f"""
     An interface for interacting with the WhyLabs platform.
@@ -464,35 +487,37 @@
                 f"Failed to set column outputs {self._org_id}/{self._dataset_id} for column name: ("
                 f"{column_name}) "
                 f"{self.whylabs_api_endpoint}"
                 f" with API token ID: {self.key_id}"
             )
             raise e
 
-    def _tag_custom_output_metrics(self, view: Union[DatasetProfileView, SegmentedDatasetProfileView]):
-        if isinstance(view, DatasetProfileView):
-            column_names = view.get_columns().keys()
-            for column_name in column_names:
-                for perf_col in KNOWN_CUSTOM_OUTPUT_METRICS:
-                    if column_name.startswith(perf_col):
-                        data_type = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][0]
-                        discreteness = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][1]
-                        column_schema: ColumnSchema = ColumnSchema(
-                            classifier="output", data_type=data_type, discreteness=discreteness  # type: ignore
-                        )
-                        self._set_column_schema(column_name, column_schema=column_schema)
-
-    def _tag_custom_perf_metrics(self, view: Union[DatasetProfileView, SegmentedDatasetProfileView]):
-        if isinstance(view, DatasetProfileView):
-            column_names = view.get_columns().keys()
-            for column_name in column_names:
-                for perf_col in KNOWN_CUSTOM_PERFORMANCE_METRICS:
-                    if column_name.startswith(perf_col):
-                        metric = KNOWN_CUSTOM_PERFORMANCE_METRICS[perf_col]
-                        self.tag_custom_performance_column(column_name, default_metric=metric)
+    def _tag_custom_output_metrics(
+        self, view: Union[DatasetProfile, DatasetProfileView, SegmentedDatasetProfileView, ResultSet]
+    ) -> None:
+        column_names = _get_column_names(view)
+        for column_name in column_names:
+            for perf_col in KNOWN_CUSTOM_OUTPUT_METRICS:
+                if column_name.startswith(perf_col):
+                    data_type = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][0]
+                    discreteness = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][1]
+                    column_schema: ColumnSchema = ColumnSchema(
+                        classifier="output", data_type=data_type, discreteness=discreteness  # type: ignore
+                    )
+                    self._set_column_schema(column_name, column_schema=column_schema)
+
+    def _tag_custom_perf_metrics(
+        self, view: Union[DatasetProfile, DatasetProfileView, SegmentedDatasetProfileView, ResultSet]
+    ) -> None:
+        column_names = _get_column_names(view)
+        for column_name in column_names:
+            for perf_col in KNOWN_CUSTOM_PERFORMANCE_METRICS:
+                if column_name.startswith(perf_col):
+                    metric = KNOWN_CUSTOM_PERFORMANCE_METRICS[perf_col]
+                    self.tag_custom_performance_column(column_name, default_metric=metric)
 
     def _do_get_feature_weights(self):
         """Get latest version for the feature weights for the specified dataset
 
         Returns
         -------
             Response of the GET request, with segmentWeights and metadata.
```

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_estimation_result_writer.py` & `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_estimation_result_writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_transaction_writer.py` & `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_transaction_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             return False, f"Transaction {self.transaction_id} was aborted"
 
         transaction_id = kwargs.get("transaction_id") or self.transaction_id
         if not transaction_id:
             raise ValueError("Missing transaction id")
 
         self._whylabs_client = self._whylabs_client.option(**kwargs)  # type: ignore
-
+        self._custom_tagging(file)
         if isinstance(file, SegmentedResultSet):
             return self._write_segmented_result_set(file, **kwargs)
 
         # file represents a single profile/segment, extract a view of it
         view = self._get_view_of_writable(file)
         return self._write_view(view, **kwargs)
```

### Comparing `whylogs-1.4.0rc0/whylogs/api/writer/writer.py` & `whylogs-1.4.1rc0/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/context/version.py` & `whylogs-1.4.1rc0/whylogs/context/version.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/__init__.py` & `whylogs-1.4.1rc0/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/column_profile.py` & `whylogs-1.4.1rc0/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/configs.py` & `whylogs-1.4.1rc0/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.4.1rc0/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/dataset_profile.py` & `whylogs-1.4.1rc0/whylogs/core/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/datatypes.py` & `whylogs-1.4.1rc0/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/errors.py` & `whylogs-1.4.1rc0/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/feature_weights.py` & `whylogs-1.4.1rc0/whylogs/core/feature_weights.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from whylogs.api.writer.writer import Writable
+from whylogs.api.writer.writer import Writable, WriterWrapper
 from whylogs.core import Segment
 
 
 class FeatureWeights(Writable):
     def __init__(self, weights: Dict[str, float], segment: Optional[Segment] = None, metadata: Optional[Dict] = None):
         """Feature Weights
 
@@ -32,7 +32,10 @@
         raise ValueError("I'm not a real Writable")
 
     def to_json(self) -> str:
         return json.dumps({"segment": self.segment, "weights": self.weights})
 
     def to_dict(self) -> Dict[str, Union[Optional[Segment], Optional[float]]]:
         return {"segment": self.segment, "weights": self.weights}
+
+
+FeatureWeightWriter = WriterWrapper
```

### Comparing `whylogs-1.4.0rc0/whylogs/core/input_resolver.py` & `whylogs-1.4.1rc0/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metadata.py` & `whylogs-1.4.1rc0/whylogs/core/metadata.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metric_getters.py` & `whylogs-1.4.1rc0/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/__init__.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/aggregators.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/column_metrics.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/compound_metric.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/decorators.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/deserializers.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/maths.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/metric_components.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/metrics.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/multimetric.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/serializers.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/metrics/unicode_range.py` & `whylogs-1.4.1rc0/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/predicate_parser.py` & `whylogs-1.4.1rc0/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/preprocessing.py` & `whylogs-1.4.1rc0/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.4.1rc0/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.4.1rc0/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/relations.py` & `whylogs-1.4.1rc0/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/resolvers.py` & `whylogs-1.4.1rc0/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/schema.py` & `whylogs-1.4.1rc0/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/segmentation_partition.py` & `whylogs-1.4.1rc0/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/specialized_resolvers.py` & `whylogs-1.4.1rc0/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/stubs.py` & `whylogs-1.4.1rc0/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.4.1rc0/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/utils/stats_calculations.py` & `whylogs-1.4.1rc0/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/utils/utils.py` & `whylogs-1.4.1rc0/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/validators/condition_validator.py` & `whylogs-1.4.1rc0/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/validators/validator.py` & `whylogs-1.4.1rc0/whylogs/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/view/column_profile_view.py` & `whylogs-1.4.1rc0/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.4.1rc0/whylogs/core/view/dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.4.1rc0/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/base.py` & `whylogs-1.4.1rc0/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/configs.py` & `whylogs-1.4.1rc0/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.4.1rc0/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/descr/employee.rst` & `whylogs-1.4.1rc0/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/descr/weather.rst` & `whylogs-1.4.1rc0/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/ecommerce.py` & `whylogs-1.4.1rc0/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/employee.py` & `whylogs-1.4.1rc0/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/utils.py` & `whylogs-1.4.1rc0/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/datasets/weather.py` & `whylogs-1.4.1rc0/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/api/logger/__init__.py` & `whylogs-1.4.1rc0/whylogs/experimental/api/logger/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import math
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Set, Tuple, Union
 
 from whylogs.api.logger import log
-from whylogs.api.logger.result_set import ViewResultSet
+from whylogs.api.logger.result_set import SegmentedResultSet, ViewResultSet
 from whylogs.core import DatasetSchema
 from whylogs.core.stubs import np, pd
 
 diagnostic_logger = logging.getLogger(__name__)
 
 
 def _convert_to_int_if_bool(data: pd.core.frame.DataFrame, *columns: str) -> pd.core.frame.DataFrame:
@@ -131,14 +131,34 @@
     return averages
 
 
 def _all_strings(data: pd.Series) -> bool:
     return all([all([isinstance(y, str) for y in x]) for x in data])
 
 
+def _get_segment_columns(schema: DatasetSchema, data: pd.DataFrame) -> List[str]:
+    columns: Set[str] = set()
+    for partition_name, partition in schema.segments.items():
+        if partition.filter:
+            raise ValueError("Filters are not supported for segmented ranking metrics")  # Filters are deprecated
+        if partition.mapper:
+            columns = columns.union(set(partition.mapper.col_names))
+
+    return list(columns)
+
+
+def _drop_non_output_columns(result: SegmentedResultSet, keep_columns: Set[str]) -> SegmentedResultSet:
+    for partition in result._segments.values():
+        for segment in partition.values():
+            for column in {column for column in segment._columns.keys() if column not in keep_columns}:
+                segment._columns.pop(column)
+
+    return result
+
+
 def log_batch_ranking_metrics(
     data: pd.core.frame.DataFrame,
     prediction_column: Optional[str] = None,
     target_column: Optional[str] = None,
     score_column: Optional[str] = None,
     k: Optional[int] = None,
     schema: Union[DatasetSchema, None] = None,
@@ -326,22 +346,29 @@
         formatted_data, target_column, prediction_column, convert_non_numeric=convert_non_numeric, k=k  # type: ignore
     )
 
     output_data["norm_dis_cumul_gain" + ("_k_" + str(k) if k else "")] = formatted_data.apply(
         row_wise_functions.calculate_row_ndcg, args=(k,), axis=1
     )
     output_data[f"sum_gain_k_{k}"] = formatted_data.apply(row_wise_functions.sum_gains, args=(k,), axis=1)
-    hit_ratio = formatted_data["count_at_k"].apply(lambda x: bool(x)).sum() / len(formatted_data)
     mrr = (1 / formatted_data["top_rank"]).replace([np.inf, np.nan], 0)
     output_data["reciprocal_rank"] = mrr
+
+    if schema and schema.segments:
+        original_columns = set(data.columns)
+        for column in set(formatted_data.columns):
+            if column not in original_columns:
+                formatted_data = formatted_data.drop(column, axis=1)
+
+        if log_full_data:
+            return log(pandas=pd.concat([formatted_data, output_data], axis=1), schema=schema)
+        else:
+            segment_columns = _get_segment_columns(schema, formatted_data)
+            segmentable_data = formatted_data[segment_columns]
+            result = log(pandas=pd.concat([segmentable_data, output_data], axis=1), schema=schema)
+            result = _drop_non_output_columns(result, set(output_data.columns))
+            return result
+
     result = log(pandas=output_data, schema=schema)
-    result = result.merge(
-        log(
-            row={
-                "accuracy" + ("_k_" + str(k) if k else ""): hit_ratio,
-            },
-            schema=schema,
-        )
-    )
     if log_full_data:
         result = result.merge(log(pandas=data, schema=schema))
     return result
```

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.4.1rc0/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/core/udf_schema.py` & `whylogs-1.4.1rc0/whylogs/experimental/core/udf_schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/core/validators/condition_validator.py` & `whylogs-1.4.1rc0/whylogs/experimental/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/core/validators/validator.py` & `whylogs-1.4.1rc0/whylogs/experimental/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.4.1rc0/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.4.1rc0/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.4.1rc0/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from logging import getLogger
 from typing import Any, List, Optional, Tuple, Union
 
-from whylogs.api.writer import Writable
+from whylogs.api.writer import Writable, WriterWrapper
 
 logger = getLogger(__name__)
 
 
 class EstimationResult(Writable):
     """
     The result of a performance estimation.
@@ -31,7 +31,10 @@
         raise ValueError("I'm not a real Writable")
 
     def _get_default_path(self) -> str:
         raise ValueError("I'm not a real Writable")
 
     def write(self, path: Optional[str] = None, **kwargs: Any) -> Tuple[bool, Union[str, List[str]]]:
         raise ValueError("I'm not a real Writable")
+
+
+EstimationResultWriter = WriterWrapper  # only works with WhylabsWriter
```

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.4.1rc0/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/extras/image_metric.py` & `whylogs-1.4.1rc0/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/migration/converters.py` & `whylogs-1.4.1rc0/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/migration/uncompound.py` & `whylogs-1.4.1rc0/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.4.1rc0/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/drift/configs.py` & `whylogs-1.4.1rc0/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/enums/enums.py` & `whylogs-1.4.1rc0/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.4.1rc0/whylogs/viz/extensions/reports/html_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from abc import ABC, abstractmethod
 from typing import Any, List, Optional, Tuple, Union
 
 from IPython.core.display import HTML  # type: ignore
 
 from whylogs import DatasetProfileView
-from whylogs.api.writer.writer import Writable
+from whylogs.api.writer.writer import Writable, WriterWrapper
 from whylogs.viz.enums.enums import PageSpec
 
 
 class HTMLReport(Writable, ABC):
     def __init__(
         self,
         ref_view: Optional[DatasetProfileView] = None,
@@ -64,7 +64,10 @@
             return True, file.name
 
     def option(self):
         return self
 
     def _get_default_filename(self) -> str:
         return "html_reports/ProfileReport.html"
+
+
+HTMLReportWriter = WriterWrapper
```

### Comparing `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.4.1rc0/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.4.1rc0/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.4.1rc0/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.4.1rc0/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.4.1rc0/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.4.1rc0/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/js/d3.min.js` & `whylogs-1.4.1rc0/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/js/handlebars.js` & `whylogs-1.4.1rc0/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.4.1rc0/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.4.1rc0/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/html/templates/index.html` & `whylogs-1.4.1rc0/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.4.1rc0/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.4.1rc0/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.4.1rc0/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.4.1rc0/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.4.1rc0/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.4.1rc0/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.4.1rc0/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.4.1rc0/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0rc0/PKG-INFO` & `whylogs-1.4.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.4.0rc0
+Version: 1.4.1rc0
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

