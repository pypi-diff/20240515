# Comparing `tmp/neptune-2.0.0a2.tar.gz` & `tmp/neptune-2.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune-2.0.0a2.tar", max compression
+gzip compressed data, was "neptune-2.0.0a3.tar", max compression
```

## Comparing `neptune-2.0.0a2.tar` & `neptune-2.0.0a3.tar`

### file list

```diff
@@ -1,283 +1,284 @@
--rw-r--r--   0        0        0    45352 2024-04-17 12:47:35.378597 neptune-2.0.0a2/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-17 12:47:35.378597 neptune-2.0.0a2/LICENSE
--rw-r--r--   0        0        0    12786 2024-04-17 12:47:35.378597 neptune-2.0.0a2/README.md
--rw-r--r--   0        0        0    10932 2024-04-17 12:47:47.738600 neptune-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     3596 2024-04-17 12:47:35.378597 neptune-2.0.0a2/src/neptune/__init__.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.378597 neptune-2.0.0a2/src/neptune/api/__init__.py
--rw-r--r--   0        0        0     1936 2024-04-17 12:47:35.378597 neptune-2.0.0a2/src/neptune/api/fetching_series_values.py
--rw-r--r--   0        0        0     2768 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/field_visitor.py
--rw-r--r--   0        0        0    22709 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/models.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/__init__.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/__init__.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/__init__.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/__init__.py
--rw-r--r--   0        0        0     1590 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py
--rw-r--r--   0        0        0     1642 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi
--rw-r--r--   0        0        0     6126 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py
--rw-r--r--   0        0        0    17492 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi
--rw-r--r--   0        0        0     1669 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.py
--rw-r--r--   0        0        0     1955 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.pyi
--rw-r--r--   0        0        0      990 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/requests_utils.py
--rw-r--r--   0        0        0     7771 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/searching_entries.py
--rw-r--r--   0        0        0     1218 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3146 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2105 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     2215 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     2446 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2397 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2665 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2139 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     3425 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4585 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     2094 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4515 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2899 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6193 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3762 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2809 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2057 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0     3184 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5391 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/collect.py
--rw-r--r--   0        0        0     5220 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/commands.py
--rw-r--r--   0        0        0    10813 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/containers.py
--rw-r--r--   0        0        0     1511 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3854 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/status.py
--rw-r--r--   0        0        0     5537 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5167 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/utils.py
--rw-r--r--   0        0        0     1087 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/constants.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/__init__.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/abstract.py
--rw-r--r--   0        0        0     2172 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/metadata_file.py
--rw-r--r--   0        0        0     1237 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/operation_storage.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/queue/__init__.py
--rw-r--r--   0        0        0     8848 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/queue/disk_queue.py
--rw-r--r--   0        0        0     3610 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/queue/json_file_splitter.py
--rw-r--r--   0        0        0     2229 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/core/components/queue/log_file.py
--rw-r--r--   0        0        0     1766 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/core/components/queue/sync_offset_file.py
--rw-r--r--   0        0        0     2596 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/envs.py
--rw-r--r--   0        0        0    42022 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/exceptions.py
--rw-r--r--   0        0        0    33497 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      775 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0      796 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      784 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      781 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      790 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      795 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/mosaicml/__init__.py
--rw-r--r--   0        0        0      784 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0     3633 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/pandas/__init__.py
--rw-r--r--   0        0        0      787 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3026 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0      787 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0      814 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      784 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      787 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0      799 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/tensorboard/__init__.py
--rw-r--r--   0        0        0      814 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0      812 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0      864 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      787 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4879 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     5141 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2377 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     5735 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     9567 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     6714 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    18056 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    46935 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     9603 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    33084 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     2894 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     5898 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3948 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5005 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13843 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1642 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5658 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0    15994 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1517 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1134 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      947 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2349 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0      859 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/envs.py
--rw-r--r--   0        0        0    15028 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0     1725 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/extensions.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3216 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/constants.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1560 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2031 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1772 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1756 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2488 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     5122 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3496 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1681 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      949 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2323 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2512 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/system/system_monitor.py
--rw-r--r--   0        0        0      933 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0     1137 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1854 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0     4784 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/oauth.py
--rw-r--r--   0        0        0    17298 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    13129 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     3073 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     3936 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py
--rw-r--r--   0        0        0     3070 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     6886 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/operation_logger.py
--rw-r--r--   0        0        0     1422 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1146 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     3361 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     2443 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/utils.py
--rw-r--r--   0        0        0     3724 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      886 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/patches/__init__.py
--rw-r--r--   0        0        0     2731 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/patches/bravado.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/__init__.py
--rw-r--r--   0        0        0     2883 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/background_job.py
--rw-r--r--   0        0        0     1663 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/signals.py
--rw-r--r--   0        0        0     4899 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/signals_processor.py
--rw-r--r--   0        0        0     1789 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/utils.py
--rw-r--r--   0        0        0      776 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/state.py
--rw-r--r--   0        0        0     1130 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/storage/__init__.py
--rw-r--r--   0        0        0     3227 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/storage/datastream.py
--rw-r--r--   0        0        0     7330 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/storage/storage_utils.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     1999 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     3066 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     5581 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4586 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     2484 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0      799 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/types/utils.py
--rw-r--r--   0        0        0     5311 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     2409 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2116 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     5746 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/disk_utilization.py
--rw-r--r--   0        0        0     2300 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     6158 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0     2490 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/git_info.py
--rw-r--r--   0        0        0      849 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0    10577 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1152 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/iso_dates.py
--rw-r--r--   0        0        0     1288 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     1657 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     2972 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1065 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0      726 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/patterns.py
--rw-r--r--   0        0        0     2187 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1168 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/requirement_check.py
--rw-r--r--   0        0        0     1566 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1143 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1345 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2266 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     2001 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2450 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     7575 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/utils.py
--rw-r--r--   0        0        0     4442 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0     3284 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/warnings.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3591 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2638 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0     5210 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1231 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0     4795 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    44742 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2021 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      923 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/__init__.py
--rw-r--r--   0        0        0     2031 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/abstract.py
--rw-r--r--   0        0        0    15915 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/model.py
--rw-r--r--   0        0        0    13820 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/model_version.py
--rw-r--r--   0        0        0    26780 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/neptune_object.py
--rw-r--r--   0        0        0    19245 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/project.py
--rw-r--r--   0        0        0    26549 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/run.py
--rw-r--r--   0        0        0     1576 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/structure_version.py
--rw-r--r--   0        0        0     4043 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/utils.py
--rw-r--r--   0        0        0     5783 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/table.py
--rw-r--r--   0        0        0     1071 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    12157 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1753 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2473 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     3854 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0     3089 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/typing.py
--rw-r--r--   0        0        0     4310 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     1431 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/version.py
--rw-r--r--   0        0        0    16599 1970-01-01 00:00:00.000000 neptune-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0    45667 2024-04-19 09:57:49.020855 neptune-2.0.0a3/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-19 09:57:49.020855 neptune-2.0.0a3/LICENSE
+-rw-r--r--   0        0        0    12786 2024-04-19 09:57:49.020855 neptune-2.0.0a3/README.md
+-rw-r--r--   0        0        0    10913 2024-04-19 09:57:58.188943 neptune-2.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3596 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/__init__.py
+-rw-r--r--   0        0        0     1936 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/fetching_series_values.py
+-rw-r--r--   0        0        0     2768 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/field_visitor.py
+-rw-r--r--   0        0        0    25839 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/models.py
+-rw-r--r--   0        0        0     1591 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/pagination.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/__init__.py
+-rw-r--r--   0        0        0     1590 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py
+-rw-r--r--   0        0        0     1642 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi
+-rw-r--r--   0        0        0     6126 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py
+-rw-r--r--   0        0        0    17492 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi
+-rw-r--r--   0        0        0     1669 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.py
+-rw-r--r--   0        0        0     1955 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.pyi
+-rw-r--r--   0        0        0      990 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/requests_utils.py
+-rw-r--r--   0        0        0     7771 2024-04-19 09:57:49.020855 neptune-2.0.0a3/src/neptune/api/searching_entries.py
+-rw-r--r--   0        0        0     1218 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3146 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2105 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     2215 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     2446 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2397 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2665 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2139 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     3425 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4585 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     2094 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4547 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2899 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6193 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3762 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2809 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2057 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0     3184 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5391 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/collect.py
+-rw-r--r--   0        0        0     5220 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0    10813 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/containers.py
+-rw-r--r--   0        0        0     1511 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3854 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     5537 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5167 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0     1087 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/constants.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/abstract.py
+-rw-r--r--   0        0        0     2172 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/metadata_file.py
+-rw-r--r--   0        0        0     1237 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/operation_storage.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/queue/__init__.py
+-rw-r--r--   0        0        0     8848 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/queue/disk_queue.py
+-rw-r--r--   0        0        0     3610 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/queue/json_file_splitter.py
+-rw-r--r--   0        0        0     2229 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/queue/log_file.py
+-rw-r--r--   0        0        0     1766 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/core/components/queue/sync_offset_file.py
+-rw-r--r--   0        0        0     2596 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/envs.py
+-rw-r--r--   0        0        0    42022 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    33564 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      775 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-19 09:57:49.024855 neptune-2.0.0a3/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      795 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/mosaicml/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0     3633 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/pandas/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3026 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0      787 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/tensorboard/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      787 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4879 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     5141 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2377 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     5735 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     9567 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     6714 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    18056 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    49007 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0    10295 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    33992 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     2894 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     6656 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3948 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5005 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13843 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1642 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5658 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0    15994 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1517 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1134 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      947 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2349 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0      859 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/envs.py
+-rw-r--r--   0        0        0    15028 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0     1725 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/extensions.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3216 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/constants.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1560 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2031 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1772 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1756 2024-04-19 09:57:49.028855 neptune-2.0.0a3/src/neptune/internal/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2488 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     5122 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3496 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1681 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      949 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2323 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2512 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0      933 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0     1137 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1854 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0     4784 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/oauth.py
+-rw-r--r--   0        0        0    17298 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    13129 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     3073 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     3936 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py
+-rw-r--r--   0        0        0     3070 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     6886 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/operation_logger.py
+-rw-r--r--   0        0        0     1422 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1146 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     3361 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     2443 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_processors/utils.py
+-rw-r--r--   0        0        0     3724 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      886 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/patches/bravado.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/signals_processing/__init__.py
+-rw-r--r--   0        0        0     2883 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/signals_processing/background_job.py
+-rw-r--r--   0        0        0     1663 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/signals_processing/signals.py
+-rw-r--r--   0        0        0     4899 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/signals_processing/signals_processor.py
+-rw-r--r--   0        0        0     1789 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/signals_processing/utils.py
+-rw-r--r--   0        0        0      776 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/state.py
+-rw-r--r--   0        0        0     1130 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/storage/__init__.py
+-rw-r--r--   0        0        0     3227 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/storage/datastream.py
+-rw-r--r--   0        0        0     7330 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/storage/storage_utils.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     1999 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     3066 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     5581 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4586 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     2484 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0      799 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/types/utils.py
+-rw-r--r--   0        0        0     5311 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     2409 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2116 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     5746 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/disk_utilization.py
+-rw-r--r--   0        0        0     2300 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     6158 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0     2490 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/git_info.py
+-rw-r--r--   0        0        0      849 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0    10577 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1152 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/iso_dates.py
+-rw-r--r--   0        0        0     1288 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     1657 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     2972 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1065 2024-04-19 09:57:49.032855 neptune-2.0.0a3/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0      726 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/patterns.py
+-rw-r--r--   0        0        0     2187 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1168 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/requirement_check.py
+-rw-r--r--   0        0        0     1566 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1143 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1345 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2266 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     2001 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2450 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     7575 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/utils/utils.py
+-rw-r--r--   0        0        0     4442 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0     3284 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/warnings.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3591 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2638 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0     5210 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1231 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0     4795 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    44742 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2021 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      923 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/abstract.py
+-rw-r--r--   0        0        0    15915 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/model.py
+-rw-r--r--   0        0        0    13820 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/model_version.py
+-rw-r--r--   0        0        0    26780 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/neptune_object.py
+-rw-r--r--   0        0        0    19245 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/project.py
+-rw-r--r--   0        0        0    26549 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/run.py
+-rw-r--r--   0        0        0     1576 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/structure_version.py
+-rw-r--r--   0        0        0     4043 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/objects/utils.py
+-rw-r--r--   0        0        0     5783 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/table.py
+-rw-r--r--   0        0        0     1071 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    12157 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1753 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2473 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     3854 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2024-04-19 09:57:49.036855 neptune-2.0.0a3/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2024-04-19 09:57:49.040855 neptune-2.0.0a3/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2024-04-19 09:57:49.040855 neptune-2.0.0a3/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0     3089 2024-04-19 09:57:49.040855 neptune-2.0.0a3/src/neptune/typing.py
+-rw-r--r--   0        0        0     4310 2024-04-19 09:57:49.040855 neptune-2.0.0a3/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:57:49.040855 neptune-2.0.0a3/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2024-04-19 09:57:49.040855 neptune-2.0.0a3/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2024-04-19 09:57:49.040855 neptune-2.0.0a3/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     1431 2024-04-19 09:57:49.040855 neptune-2.0.0a3/src/neptune/version.py
+-rw-r--r--   0        0        0    16567 1970-01-01 00:00:00.000000 neptune-2.0.0a3/PKG-INFO
```

### Comparing `neptune-2.0.0a2/CHANGELOG.md` & `neptune-2.0.0a3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,26 @@
 - Disabled `neptune command-line tool` ([#1718](https://github.com/neptune-ai/neptune-client/pull/1718))
 - Disabled deleting fields in `Handler` ([#1729](https://github.com/neptune-ai/neptune-client/pull/1729))
 - Removed `AbstractNeptuneObject` ([#1725](https://github.com/neptune-ai/neptune-client/pull/1725))
 - Disabled artifact-related methods in `Handler` ([#1734](https://github.com/neptune-ai/neptune-client/pull/1734))
 - Removed `boto3` from requirements ([#1743](https://github.com/neptune-ai/neptune-client/pull/1743))
 - Disabled `StringSet` `remove` and `clear` methods ([#1732](https://github.com/neptune-ai/neptune-client/pull/1732))
 - Disable `fetch_last` and `download_last` ([#1731](https://github.com/neptune-ai/neptune-client/pull/1731))
+- Removed `pillow` from requirements ([#1745](https://github.com/neptune-ai/neptune-client/pull/1745))
 - Disabled file related functionality ([#1726](https://github.com/neptune-ai/neptune-client/pull/1726))
+- Disabled file logging ([#1733](https://github.com/neptune-ai/neptune-client/pull/1733))
 
 ### Changes
 - Stop sending `X-Neptune-LegacyClient` header ([#1715](https://github.com/neptune-ai/neptune-client/pull/1715))
 - Use `tqdm.auto` ([#1717](https://github.com/neptune-ai/neptune-client/pull/1717))
 - Fields DTO conversion reworked ([#1722](https://github.com/neptune-ai/neptune-client/pull/1722))
 - Added support for Protocol Buffers ([#1728](https://github.com/neptune-ai/neptune-client/pull/1728))
 - Series values DTO conversion reworked with protocol buffer support ([#1738](https://github.com/neptune-ai/neptune-client/pull/1738))
 - Series values fetching reworked with protocol buffer support ([#1744](https://github.com/neptune-ai/neptune-client/pull/1744))
+- Added support for enhanced field definitions querying ([#1751](https://github.com/neptune-ai/neptune-client/pull/1751))
 
 ### Fixes
 - Fixed `tqdm.notebook` import only in Notebook environment ([#1716](https://github.com/neptune-ai/neptune-client/pull/1716))
 - Added `setuptools` to dependencies for `python >= 3.12` ([#1721](https://github.com/neptune-ai/neptune-client/pull/1721))
 - Fixed compatibility checks with pre-release versions ([#1730](https://github.com/neptune-ai/neptune-client/pull/1730))
 - Added `Accept` and `Accept-Encoding` headers to protocol buffer requests ([#1736](https://github.com/neptune-ai/neptune-client/pull/1736))
 - Fixed default params for getAttributesWithPathsFilter ([#1740](https://github.com/neptune-ai/neptune-client/pull/1740))
```

### Comparing `neptune-2.0.0a2/LICENSE` & `neptune-2.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/README.md` & `neptune-2.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/pyproject.toml` & `neptune-2.0.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 requests-oauthlib = ">=1.0.0"
 websocket-client = ">=0.35.0, !=1.0.0"
 urllib3 = "*"
 swagger-spec-validator = ">=2.7.4"
 protobuf = "^4.0.0"
 
 # Built-in integrations
-Pillow = ">=1.1.6"
 GitPython = ">=2.0.8"
 psutil = "*"
 pandas = "*"
 
 # Additional integrations
 kedro-neptune = { version = "*", optional = true, python = ">=3.9,<3.12" }
 neptune-detectron2 = { version = "*", optional = true, python = ">=3.7"}
@@ -86,15 +85,15 @@
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune"
 readme = "README.md"
-version = "2.0.0-alpha.2"
+version = "2.0.0-alpha.3"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune-2.0.0a2/src/neptune/__init__.py` & `neptune-2.0.0a3/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/__init__.py` & `neptune-2.0.0a3/src/neptune/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/fetching_series_values.py` & `neptune-2.0.0a3/src/neptune/api/fetching_series_values.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/field_visitor.py` & `neptune-2.0.0a3/src/neptune/api/field_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/models.py` & `neptune-2.0.0a3/src/neptune/api/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     "ArtifactField",
     "FieldDefinition",
     "FloatSeriesValues",
     "FloatPointValue",
     "StringSeriesValues",
     "StringPointValue",
     "ImageSeriesValues",
+    "QueryFieldDefinitionsResult",
+    "NextPage",
+    "QueryFieldsResult",
 )
 
 import abc
 import re
 from dataclasses import dataclass
 from dataclasses import field as dataclass_field
 from datetime import (
@@ -598,14 +601,113 @@
         return LeaderboardEntriesSearchResult(
             entries=[LeaderboardEntry.from_proto(entry) for entry in data.entries],
             matching_item_count=data.matching_item_count,
         )
 
 
 @dataclass
+class NextPage:
+    limit: Optional[int]
+    next_page_token: Optional[str]
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> NextPage:
+        return NextPage(limit=data.get("limit"), next_page_token=data.get("nextPageToken"))
+
+    @staticmethod
+    def from_model(model: Any) -> NextPage:
+        return NextPage(limit=model.limit, next_page_token=model.nextPageToken)
+
+    @staticmethod
+    def from_proto(data: Any) -> NextPage:
+        raise NotImplementedError()
+
+    def to_dto(self) -> Dict[str, Any]:
+        return {
+            "limit": self.limit,
+            "nextPageToken": self.next_page_token,
+        }
+
+
+@dataclass
+class QueryFieldsExperimentResult:
+    object_id: str
+    object_key: str
+    fields: List[Field]
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> QueryFieldsExperimentResult:
+        return QueryFieldsExperimentResult(
+            object_id=data["experimentId"],
+            object_key=data["experimentShortId"],
+            fields=[Field.from_dict(field) for field in data["attributes"]],
+        )
+
+    @staticmethod
+    def from_model(model: Any) -> QueryFieldsExperimentResult:
+        return QueryFieldsExperimentResult(
+            object_id=model.experimentId,
+            object_key=model.experimentShortId,
+            fields=[Field.from_model(field) for field in model.attributes],
+        )
+
+    @staticmethod
+    def from_proto(data: Any) -> QueryFieldsExperimentResult:
+        raise NotImplementedError()
+
+
+@dataclass
+class QueryFieldsResult:
+    entries: List[QueryFieldsExperimentResult]
+    next_page: NextPage
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> QueryFieldsResult:
+        return QueryFieldsResult(
+            entries=[QueryFieldsExperimentResult.from_dict(entry) for entry in data["entries"]],
+            next_page=NextPage.from_dict(data["nextPage"]),
+        )
+
+    @staticmethod
+    def from_model(model: Any) -> QueryFieldsResult:
+        return QueryFieldsResult(
+            entries=[QueryFieldsExperimentResult.from_model(entry) for entry in model.entries],
+            next_page=NextPage.from_model(model.nextPage),
+        )
+
+    @staticmethod
+    def from_proto(data: Any) -> QueryFieldsResult:
+        raise NotImplementedError()
+
+
+@dataclass
+class QueryFieldDefinitionsResult:
+    entries: List[FieldDefinition]
+    next_page: NextPage
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> QueryFieldDefinitionsResult:
+        return QueryFieldDefinitionsResult(
+            entries=[FieldDefinition.from_dict(entry) for entry in data["entries"]],
+            next_page=NextPage.from_dict(data["nextPage"]),
+        )
+
+    @staticmethod
+    def from_model(model: Any) -> QueryFieldDefinitionsResult:
+        return QueryFieldDefinitionsResult(
+            entries=[FieldDefinition.from_model(entry) for entry in model.entries],
+            next_page=NextPage.from_model(model.nextPage),
+        )
+
+    @staticmethod
+    def from_proto(data: Any) -> QueryFieldDefinitionsResult:
+        raise NotImplementedError()
+
+
+@dataclass
 class FieldDefinition:
     path: str
     type: FieldType
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> FieldDefinition:
         return FieldDefinition(path=data["name"], type=FieldType(data["type"]))
```

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/__init__.py` & `neptune-2.0.0a3/src/neptune/api/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/__init__.py` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/__init__.py` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/__init__.py` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.py` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.pyi` & `neptune-2.0.0a3/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/requests_utils.py` & `neptune-2.0.0a3/src/neptune/api/requests_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/api/searching_entries.py` & `neptune-2.0.0a3/src/neptune/api/searching_entries.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/__init__.py` & `neptune-2.0.0a3/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/__init__.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/artifact.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/atom.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/boolean.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/copiable_atom.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/datetime.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/file.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/float.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/git_ref.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/integer.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/notebook_ref.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/run_state.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/atoms/string.py` & `neptune-2.0.0a3/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/attribute.py` & `neptune-2.0.0a3/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/constants.py` & `neptune-2.0.0a3/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/file_set.py` & `neptune-2.0.0a3/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/namespace.py` & `neptune-2.0.0a3/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/series/__init__.py` & `neptune-2.0.0a3/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/series/fetchable_series.py` & `neptune-2.0.0a3/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/series/file_series.py` & `neptune-2.0.0a3/src/neptune/attributes/series/file_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,14 @@
 import pathlib
 from typing import (
     Iterable,
     List,
     Optional,
 )
 
-from PIL import (
-    Image,
-    UnidentifiedImageError,
-)
-
 from neptune.attributes.series.series import Series
 from neptune.exceptions import (
     FileNotFound,
     NeptuneUnsupportedFunctionalityException,
     OperationNotSupported,
 )
 from neptune.internal.operation import (
@@ -80,14 +75,19 @@
             if not os.path.exists(file.path):
                 raise FileNotFound(file.path)
             with open(file.path, "rb") as image_file:
                 file_content = File.from_stream(image_file).content
         else:
             file_content = file.content
 
+        from PIL import (
+            Image,
+            UnidentifiedImageError,
+        )
+
         try:
             with Image.open(io.BytesIO(file_content)):
                 ...
         except UnidentifiedImageError:
             raise OperationNotSupported(
                 "FileSeries supports only image files for now. Other file types will be implemented in future."
             )
```

### Comparing `neptune-2.0.0a2/src/neptune/attributes/series/float_series.py` & `neptune-2.0.0a3/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/series/series.py` & `neptune-2.0.0a3/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/series/string_series.py` & `neptune-2.0.0a3/src/neptune/attributes/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/sets/__init__.py` & `neptune-2.0.0a3/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/sets/set.py` & `neptune-2.0.0a3/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/sets/string_set.py` & `neptune-2.0.0a3/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/attributes/utils.py` & `neptune-2.0.0a3/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/__init__.py` & `neptune-2.0.0a3/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/__main__.py` & `neptune-2.0.0a3/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/clear.py` & `neptune-2.0.0a3/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/collect.py` & `neptune-2.0.0a3/src/neptune/cli/collect.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/commands.py` & `neptune-2.0.0a3/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/containers.py` & `neptune-2.0.0a3/src/neptune/cli/containers.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/path_option.py` & `neptune-2.0.0a3/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/status.py` & `neptune-2.0.0a3/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/sync.py` & `neptune-2.0.0a3/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/cli/utils.py` & `neptune-2.0.0a3/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/constants.py` & `neptune-2.0.0a3/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/__init__.py` & `neptune-2.0.0a3/src/neptune/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/__init__.py` & `neptune-2.0.0a3/src/neptune/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/abstract.py` & `neptune-2.0.0a3/src/neptune/core/components/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/metadata_file.py` & `neptune-2.0.0a3/src/neptune/core/components/metadata_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/operation_storage.py` & `neptune-2.0.0a3/src/neptune/core/components/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/queue/__init__.py` & `neptune-2.0.0a3/src/neptune/core/components/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/queue/disk_queue.py` & `neptune-2.0.0a3/src/neptune/core/components/queue/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/queue/json_file_splitter.py` & `neptune-2.0.0a3/src/neptune/core/components/queue/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/queue/log_file.py` & `neptune-2.0.0a3/src/neptune/core/components/queue/log_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/core/components/queue/sync_offset_file.py` & `neptune-2.0.0a3/src/neptune/core/components/queue/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/envs.py` & `neptune-2.0.0a3/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/exceptions.py` & `neptune-2.0.0a3/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/handler.py` & `neptune-2.0.0a3/src/neptune/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,14 +331,15 @@
                     first_value = value
 
                 if is_float(first_value):
                     attr = FloatSeries(self._container, parse_path(self._path))
                 elif is_string(first_value):
                     attr = StringSeries(self._container, parse_path(self._path))
                 elif FileVal.is_convertable(first_value):
+                    raise NeptuneUnsupportedFunctionalityException
                     attr = FileSeries(self._container, parse_path(self._path))
                 elif is_float_like(first_value):
                     attr = FloatSeries(self._container, parse_path(self._path))
                 elif from_stringify_value:
                     if is_collection(value):
                         value = list(map(str, value))
                     else:
```

### Comparing `neptune-2.0.0a2/src/neptune/integrations/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/aws/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/detectron2/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/fastai/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/kedro/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/lightgbm/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/mosaicml/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/mosaicml/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/optuna/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/pandas/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/prophet/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/python_logger.py` & `neptune-2.0.0a3/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/pytorch/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/sacred/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/sklearn/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/tensorboard/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/transformers/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/utils.py` & `neptune-2.0.0a3/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/integrations/xgboost/__init__.py` & `neptune-2.0.0a3/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/artifacts/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/local.py` & `neptune-2.0.0a3/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/s3.py` & `neptune-2.0.0a3/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/artifacts/file_hasher.py` & `neptune-2.0.0a3/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune-2.0.0a3/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/artifacts/types.py` & `neptune-2.0.0a3/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/artifacts/utils.py` & `neptune-2.0.0a3/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/api_model.py` & `neptune-2.0.0a3/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/factory.py` & `neptune-2.0.0a3/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune-2.0.0a3/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/hosted_client.py` & `neptune-2.0.0a3/src/neptune/internal/backends/hosted_client.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/hosted_file_operations.py` & `neptune-2.0.0a3/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune-2.0.0a3/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,17 @@
     FileField,
     FloatField,
     FloatSeriesField,
     FloatSeriesValues,
     ImageSeriesValues,
     IntField,
     LeaderboardEntry,
+    NextPage,
+    QueryFieldDefinitionsResult,
+    QueryFieldsResult,
     StringField,
     StringSeriesField,
     StringSeriesValues,
     StringSetField,
 )
 from neptune.api.proto.neptune_pb.api.model.attributes_pb2 import ProtoAttributesSearchResultDTO
 from neptune.api.proto.neptune_pb.api.model.leaderboard_entries_pb2 import ProtoAttributesDTO
@@ -1022,14 +1025,39 @@
                     .result
                 )
                 return FloatSeriesValues.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
+    def query_fields_within_project(
+        self,
+        project_id: QualifiedName,
+        field_names_filter: Optional[List[str]] = None,
+        experiment_ids_filter: Optional[List[str]] = None,
+        next_page: Optional[NextPage] = None,
+    ) -> QueryFieldsResult:
+        pagination = {"nextPage": next_page.to_dto()} if next_page else {}
+        params = {
+            "projectIdentifier": project_id,
+            "query": {
+                **pagination,
+                "attributeNamesFilter": field_names_filter,
+                "experimentIdsFilter": experiment_ids_filter,
+            },
+            **DEFAULT_REQUEST_KWARGS,
+        }
+
+        try:
+            result = self.leaderboard_client.api.queryAttributesWithinProject(**params).response().result
+            return QueryFieldsResult.from_model(result)
+        except HTTPNotFound:
+            raise ProjectNotFound(project_id=project_id)
+
+    @with_api_exceptions_handler
     def fetch_atom_attribute_values(
         self, container_id: str, container_type: ContainerType, path: List[str]
     ) -> List[Tuple[str, FieldType, Any]]:
         params = {
             "experimentId": container_id,
         }
         try:
@@ -1139,14 +1167,44 @@
         workspace: str,
         project_name: str,
         sys_id: str,
     ) -> str:
         base_url = self.get_display_address()
         return f"{base_url}/{workspace}/{project_name}/m/{model_id}/v/{sys_id}"
 
+    def query_fields_definitions_within_project(
+        self,
+        project_id: QualifiedName,
+        field_name_regex: Optional[str] = None,
+        experiment_ids_filter: Optional[List[str]] = None,
+        next_page: Optional[NextPage] = None,
+    ) -> QueryFieldDefinitionsResult:
+        pagination = {"nextPage": next_page.to_dto()} if next_page else {}
+        params = {
+            "projectIdentifier": project_id,
+            "query": {
+                **pagination,
+                "experimentIdsFilter": experiment_ids_filter,
+                "attributeNameRegex": field_name_regex,
+            },
+        }
+
+        try:
+            data = (
+                self.leaderboard_client.api.queryAttributeDefinitionsWithinProject(
+                    **params,
+                    **DEFAULT_REQUEST_KWARGS,
+                )
+                .response()
+                .result
+            )
+            return QueryFieldDefinitionsResult.from_model(data)
+        except HTTPNotFound:
+            raise ProjectNotFound(project_id=project_id)
+
     def get_fields_definitions(
         self,
         container_id: str,
         container_type: ContainerType,
         use_proto: Optional[bool] = None,
     ) -> List[FieldDefinition]:
         use_proto = use_proto if use_proto is not None else self.use_proto
```

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/neptune_backend.py` & `neptune-2.0.0a3/src/neptune/internal/backends/neptune_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     FileField,
     FloatField,
     FloatSeriesField,
     FloatSeriesValues,
     ImageSeriesValues,
     IntField,
     LeaderboardEntry,
+    NextPage,
+    QueryFieldDefinitionsResult,
+    QueryFieldsResult,
     StringField,
     StringSeriesField,
     StringSeriesValues,
     StringSetField,
 )
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.internal.artifacts.types import ArtifactFileData
@@ -330,7 +333,25 @@
         use_proto: Optional[bool] = None,
     ) -> Generator[LeaderboardEntry, None, None]:
         pass
 
     @abc.abstractmethod
     def list_fileset_files(self, attribute: List[str], container_id: str, path: str) -> List[FileEntry]:
         pass
+
+    @abc.abstractmethod
+    def query_fields_definitions_within_project(
+        self,
+        project_id: QualifiedName,
+        field_name_regex: Optional[str] = None,
+        experiment_ids_filter: Optional[List[str]] = None,
+        next_page: Optional[NextPage] = None,
+    ) -> QueryFieldDefinitionsResult: ...
+
+    @abc.abstractmethod
+    def query_fields_within_project(
+        self,
+        project_id: QualifiedName,
+        field_names_filter: Optional[List[str]] = None,
+        experiment_ids_filter: Optional[List[str]] = None,
+        next_page: Optional[NextPage] = None,
+    ) -> QueryFieldsResult: ...
```

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune-2.0.0a3/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
     FloatField,
     FloatPointValue,
     FloatSeriesField,
     FloatSeriesValues,
     ImageSeriesValues,
     IntField,
     LeaderboardEntry,
+    NextPage,
+    QueryFieldDefinitionsResult,
+    QueryFieldsResult,
     StringField,
     StringPointValue,
     StringSeriesField,
     StringSeriesValues,
     StringSetField,
 )
 from neptune.core.components.operation_storage import OperationStorage
@@ -799,7 +802,31 @@
             )
         ]
 
     def get_fields_with_paths_filter(
         self, container_id: str, container_type: ContainerType, paths: List[str], use_proto: Optional[bool] = None
     ) -> List[Field]:
         return []
+
+    def query_fields_definitions_within_project(
+        self,
+        project_id: QualifiedName,
+        field_name_regex: Optional[str] = None,
+        experiment_ids_filter: Optional[List[str]] = None,
+        next_page: Optional[NextPage] = None,
+    ) -> QueryFieldDefinitionsResult:
+        return QueryFieldDefinitionsResult(
+            entries=[],
+            next_page=NextPage(next_page_token=None, limit=0),
+        )
+
+    def query_fields_within_project(
+        self,
+        project_id: QualifiedName,
+        field_names_filter: Optional[List[str]] = None,
+        experiment_ids_filter: Optional[List[str]] = None,
+        next_page: Optional[NextPage] = None,
+    ) -> QueryFieldsResult:
+        return QueryFieldsResult(
+            entries=[],
+            next_page=NextPage(next_page_token=None, limit=0),
+        )
```

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/nql.py` & `neptune-2.0.0a3/src/neptune/internal/backends/nql.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune-2.0.0a3/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,25 +32,31 @@
     FileField,
     FloatField,
     FloatSeriesField,
     FloatSeriesValues,
     ImageSeriesValues,
     IntField,
     LeaderboardEntry,
+    NextPage,
+    QueryFieldDefinitionsResult,
+    QueryFieldsResult,
     StringField,
     StringSeriesField,
     StringSeriesValues,
     StringSetField,
 )
 from neptune.exceptions import NeptuneOfflineModeFetchException
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.backends.neptune_backend_mock import NeptuneBackendMock
 from neptune.internal.backends.nql import NQLQuery
 from neptune.internal.container_type import ContainerType
-from neptune.internal.id_formats import UniqueId
+from neptune.internal.id_formats import (
+    QualifiedName,
+    UniqueId,
+)
 from neptune.typing import ProgressBarType
 
 
 class OfflineNeptuneBackend(NeptuneBackendMock):
     WORKSPACE_NAME = "offline"
 
     def get_attributes(self, container_id: str, container_type: ContainerType) -> List[FieldDefinition]:
@@ -166,7 +172,25 @@
         limit: Optional[int] = None,
         sort_by: str = "sys/creation_time",
         ascending: bool = False,
         progress_bar: Optional[ProgressBarType] = None,
         use_proto: Optional[bool] = None,
     ) -> Generator[LeaderboardEntry, None, None]:
         raise NeptuneOfflineModeFetchException
+
+    def query_fields_definitions_within_project(
+        self,
+        project_id: QualifiedName,
+        field_name_regex: Optional[str] = None,
+        experiment_ids_filter: Optional[List[str]] = None,
+        next_page: Optional[NextPage] = None,
+    ) -> QueryFieldDefinitionsResult:
+        raise NeptuneOfflineModeFetchException
+
+    def query_fields_within_project(
+        self,
+        project_id: QualifiedName,
+        field_names_filter: Optional[List[str]] = None,
+        experiment_ids_filter: Optional[List[str]] = None,
+        next_page: Optional[NextPage] = None,
+    ) -> QueryFieldsResult:
+        raise NeptuneOfflineModeFetchException
```

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune-2.0.0a3/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune-2.0.0a3/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/operations_preprocessor.py` & `neptune-2.0.0a3/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/project_name_lookup.py` & `neptune-2.0.0a3/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune-2.0.0a3/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backends/utils.py` & `neptune-2.0.0a3/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/backgroud_job_list.py` & `neptune-2.0.0a3/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/background_job.py` & `neptune-2.0.0a3/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/constants.py` & `neptune-2.0.0a3/src/neptune/internal/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/container_structure.py` & `neptune-2.0.0a3/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/container_type.py` & `neptune-2.0.0a3/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/credentials.py` & `neptune-2.0.0a3/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/envs.py` & `neptune-2.0.0a3/src/neptune/internal/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/exceptions.py` & `neptune-2.0.0a3/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/extensions.py` & `neptune-2.0.0a3/src/neptune/internal/extensions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/cgroup_monitor.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/constants.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/cpu.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge_factory.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge_mode.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gpu.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/memory.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gpu/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metric.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metrics_container.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metrics_factory.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_report.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_reporter.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/metric_service.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/metric_service_factory.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/resources/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/resources/system_resource_info.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/resources/system_resource_info_factory.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/system/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/hardware/system/system_monitor.py` & `neptune-2.0.0a3/src/neptune/internal/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/id_formats.py` & `neptune-2.0.0a3/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/init/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/init/parameters.py` & `neptune-2.0.0a3/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/notebooks/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/notebooks/comm.py` & `neptune-2.0.0a3/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/notebooks/notebooks.py` & `neptune-2.0.0a3/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/oauth.py` & `neptune-2.0.0a3/src/neptune/internal/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation.py` & `neptune-2.0.0a3/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/factory.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/operation_logger.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/operation_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/operation_processor.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_processors/utils.py` & `neptune-2.0.0a3/src/neptune/internal/operation_processors/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/operation_visitor.py` & `neptune-2.0.0a3/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/patches/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/patches/bravado.py` & `neptune-2.0.0a3/src/neptune/internal/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/signals_processing/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/signals_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/signals_processing/background_job.py` & `neptune-2.0.0a3/src/neptune/internal/signals_processing/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/signals_processing/signals.py` & `neptune-2.0.0a3/src/neptune/internal/signals_processing/signals.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/signals_processing/signals_processor.py` & `neptune-2.0.0a3/src/neptune/internal/signals_processing/signals_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/signals_processing/utils.py` & `neptune-2.0.0a3/src/neptune/internal/signals_processing/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/state.py` & `neptune-2.0.0a3/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/storage/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/storage/datastream.py` & `neptune-2.0.0a3/src/neptune/internal/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/storage/storage_utils.py` & `neptune-2.0.0a3/src/neptune/internal/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/streams/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/streams/std_capture_background_job.py` & `neptune-2.0.0a3/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune-2.0.0a3/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/threading/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/threading/daemon.py` & `neptune-2.0.0a3/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/types/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/types/file_types.py` & `neptune-2.0.0a3/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/types/stringify_value.py` & `neptune-2.0.0a3/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/types/utils.py` & `neptune-2.0.0a3/src/neptune/internal/types/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/dependency_tracking.py` & `neptune-2.0.0a3/src/neptune/internal/utils/dependency_tracking.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/deprecation.py` & `neptune-2.0.0a3/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/disk_utilization.py` & `neptune-2.0.0a3/src/neptune/internal/utils/disk_utilization.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune-2.0.0a3/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/git.py` & `neptune-2.0.0a3/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/git_info.py` & `neptune-2.0.0a3/src/neptune/internal/utils/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/hashing.py` & `neptune-2.0.0a3/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/images.py` & `neptune-2.0.0a3/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/iso_dates.py` & `neptune-2.0.0a3/src/neptune/internal/utils/iso_dates.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/iteration.py` & `neptune-2.0.0a3/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/limits.py` & `neptune-2.0.0a3/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/logger.py` & `neptune-2.0.0a3/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/paths.py` & `neptune-2.0.0a3/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/patterns.py` & `neptune-2.0.0a3/src/neptune/internal/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/ping_background_job.py` & `neptune-2.0.0a3/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/process_killer.py` & `neptune-2.0.0a3/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/requirement_check.py` & `neptune-2.0.0a3/src/neptune/internal/utils/requirement_check.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/run_state.py` & `neptune-2.0.0a3/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/runningmode.py` & `neptune-2.0.0a3/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/s3.py` & `neptune-2.0.0a3/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/source_code.py` & `neptune-2.0.0a3/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/traceback_job.py` & `neptune-2.0.0a3/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune-2.0.0a3/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/utils/utils.py` & `neptune-2.0.0a3/src/neptune/internal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/value_to_attribute_visitor.py` & `neptune-2.0.0a3/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/warnings.py` & `neptune-2.0.0a3/src/neptune/internal/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/websockets/__init__.py` & `neptune-2.0.0a3/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/websockets/reconnecting_websocket.py` & `neptune-2.0.0a3/src/neptune/internal/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/websockets/websocket_client_adapter.py` & `neptune-2.0.0a3/src/neptune/internal/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune-2.0.0a3/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/internal/websockets/websockets_factory.py` & `neptune-2.0.0a3/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/management/__init__.py` & `neptune-2.0.0a3/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/management/exceptions.py` & `neptune-2.0.0a3/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/management/internal/__init__.py` & `neptune-2.0.0a3/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/management/internal/api.py` & `neptune-2.0.0a3/src/neptune/management/internal/api.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/management/internal/dto.py` & `neptune-2.0.0a3/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/management/internal/types.py` & `neptune-2.0.0a3/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/management/internal/utils.py` & `neptune-2.0.0a3/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/__init__.py` & `neptune-2.0.0a3/src/neptune/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/abstract.py` & `neptune-2.0.0a3/src/neptune/objects/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/model.py` & `neptune-2.0.0a3/src/neptune/objects/model.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/model_version.py` & `neptune-2.0.0a3/src/neptune/objects/model_version.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/neptune_object.py` & `neptune-2.0.0a3/src/neptune/objects/neptune_object.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/project.py` & `neptune-2.0.0a3/src/neptune/objects/project.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/run.py` & `neptune-2.0.0a3/src/neptune/objects/run.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/structure_version.py` & `neptune-2.0.0a3/src/neptune/objects/structure_version.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/objects/utils.py` & `neptune-2.0.0a3/src/neptune/objects/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/table.py` & `neptune-2.0.0a3/src/neptune/table.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/__init__.py` & `neptune-2.0.0a3/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/__init__.py` & `neptune-2.0.0a3/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/artifact.py` & `neptune-2.0.0a3/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/atom.py` & `neptune-2.0.0a3/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/boolean.py` & `neptune-2.0.0a3/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/datetime.py` & `neptune-2.0.0a3/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/file.py` & `neptune-2.0.0a3/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/float.py` & `neptune-2.0.0a3/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/git_ref.py` & `neptune-2.0.0a3/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/integer.py` & `neptune-2.0.0a3/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/atoms/string.py` & `neptune-2.0.0a3/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/file_set.py` & `neptune-2.0.0a3/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/mode.py` & `neptune-2.0.0a3/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/model_version_stage.py` & `neptune-2.0.0a3/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/namespace.py` & `neptune-2.0.0a3/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/series/__init__.py` & `neptune-2.0.0a3/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/series/file_series.py` & `neptune-2.0.0a3/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/series/float_series.py` & `neptune-2.0.0a3/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/series/series.py` & `neptune-2.0.0a3/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/series/series_value.py` & `neptune-2.0.0a3/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/series/string_series.py` & `neptune-2.0.0a3/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/sets/__init__.py` & `neptune-2.0.0a3/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/sets/set.py` & `neptune-2.0.0a3/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/sets/string_set.py` & `neptune-2.0.0a3/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/type_casting.py` & `neptune-2.0.0a3/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/value.py` & `neptune-2.0.0a3/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/value_copy.py` & `neptune-2.0.0a3/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/types/value_visitor.py` & `neptune-2.0.0a3/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/typing.py` & `neptune-2.0.0a3/src/neptune/typing.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/utils.py` & `neptune-2.0.0a3/src/neptune/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/vendor/lib_programname.py` & `neptune-2.0.0a3/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/vendor/pynvml.py` & `neptune-2.0.0a3/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/src/neptune/version.py` & `neptune-2.0.0a3/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a2/PKG-INFO` & `neptune-2.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -45,15 +45,14 @@
 Provides-Extra: sklearn
 Provides-Extra: tensorboard
 Provides-Extra: tensorflow-keras
 Provides-Extra: transformers
 Provides-Extra: xgboost
 Provides-Extra: zenml
 Requires-Dist: GitPython (>=2.0.8)
-Requires-Dist: Pillow (>=1.1.6)
 Requires-Dist: PyJWT
 Requires-Dist: bravado (>=11.0.0,<12.0.0)
 Requires-Dist: click (>=7.0)
 Requires-Dist: importlib-metadata ; python_version < "3.8"
 Requires-Dist: kedro-neptune ; (python_version >= "3.9" and python_version < "3.12") and (extra == "kedro")
 Requires-Dist: mosaicml ; extra == "mosaicml"
 Requires-Dist: neptune-airflow ; extra == "airflow"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neptune Version: 2.0.0a2 Summary: Neptune Client
+Metadata-Version: 2.1 Name: neptune Version: 2.0.0a3 Summary: Neptune Client
 Home-page: https://neptune.ai/ License: Apache-2.0 Keywords: MLOps,ML
 Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store Author:
 neptune.ai Author-email: contact@neptune.ai Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
@@ -18,29 +18,29 @@
 Development :: Libraries :: Python Modules Provides-Extra: airflow Provides-
 Extra: aws Provides-Extra: detectron2 Provides-Extra: experimental Provides-
 Extra: fastai Provides-Extra: kedro Provides-Extra: lightgbm Provides-Extra:
 mlflow Provides-Extra: mosaicml Provides-Extra: optuna Provides-Extra: prophet
 Provides-Extra: pytorch Provides-Extra: pytorch-lightning Provides-Extra:
 sacred Provides-Extra: sklearn Provides-Extra: tensorboard Provides-Extra:
 tensorflow-keras Provides-Extra: transformers Provides-Extra: xgboost Provides-
-Extra: zenml Requires-Dist: GitPython (>=2.0.8) Requires-Dist: Pillow (>=1.1.6)
-Requires-Dist: PyJWT Requires-Dist: bravado (>=11.0.0,<12.0.0) Requires-Dist:
-click (>=7.0) Requires-Dist: importlib-metadata ; python_version < "3.8"
-Requires-Dist: kedro-neptune ; (python_version >= "3.9" and python_version <
-"3.12") and (extra == "kedro") Requires-Dist: mosaicml ; extra == "mosaicml"
-Requires-Dist: neptune-airflow ; extra == "airflow" Requires-Dist: neptune-aws
-; extra == "aws" Requires-Dist: neptune-detectron2 ; (python_version >= "3.7")
-and (extra == "detectron2") Requires-Dist: neptune-fastai ; extra == "fastai"
-Requires-Dist: neptune-lightgbm ; extra == "lightgbm" Requires-Dist: neptune-
-mlflow ; extra == "mlflow" Requires-Dist: neptune-optuna ; extra == "optuna"
-Requires-Dist: neptune-prophet ; extra == "prophet" Requires-Dist: neptune-
-pytorch ; extra == "pytorch" Requires-Dist: neptune-sacred ; extra == "sacred"
-Requires-Dist: neptune-sklearn ; extra == "sklearn" Requires-Dist: neptune-
-tensorboard ; extra == "tensorboard" Requires-Dist: neptune-tensorflow-keras ;
-extra == "tensorflow-keras" Requires-Dist: neptune-xgboost ; extra == "xgboost"
+Extra: zenml Requires-Dist: GitPython (>=2.0.8) Requires-Dist: PyJWT Requires-
+Dist: bravado (>=11.0.0,<12.0.0) Requires-Dist: click (>=7.0) Requires-Dist:
+importlib-metadata ; python_version < "3.8" Requires-Dist: kedro-neptune ;
+(python_version >= "3.9" and python_version < "3.12") and (extra == "kedro")
+Requires-Dist: mosaicml ; extra == "mosaicml" Requires-Dist: neptune-airflow ;
+extra == "airflow" Requires-Dist: neptune-aws ; extra == "aws" Requires-Dist:
+neptune-detectron2 ; (python_version >= "3.7") and (extra == "detectron2")
+Requires-Dist: neptune-fastai ; extra == "fastai" Requires-Dist: neptune-
+lightgbm ; extra == "lightgbm" Requires-Dist: neptune-mlflow ; extra ==
+"mlflow" Requires-Dist: neptune-optuna ; extra == "optuna" Requires-Dist:
+neptune-prophet ; extra == "prophet" Requires-Dist: neptune-pytorch ; extra ==
+"pytorch" Requires-Dist: neptune-sacred ; extra == "sacred" Requires-Dist:
+neptune-sklearn ; extra == "sklearn" Requires-Dist: neptune-tensorboard ; extra
+== "tensorboard" Requires-Dist: neptune-tensorflow-keras ; extra ==
+"tensorflow-keras" Requires-Dist: neptune-xgboost ; extra == "xgboost"
 Requires-Dist: oauthlib (>=2.1.0) Requires-Dist: packaging Requires-Dist:
 pandas Requires-Dist: protobuf (>=4.0.0,<5.0.0) Requires-Dist: psutil Requires-
 Dist: pytorch-lightning ; extra == "pytorch-lightning" Requires-Dist: requests
 (>=2.20.0) Requires-Dist: requests-oauthlib (>=1.0.0) Requires-Dist: setuptools
 ; python_version >= "3.12" Requires-Dist: swagger-spec-validator (>=2.7.4)
 Requires-Dist: transformers ; extra == "transformers" Requires-Dist: typing-
 extensions (>=3.10.0) Requires-Dist: urllib3 Requires-Dist: websocket-client
```

