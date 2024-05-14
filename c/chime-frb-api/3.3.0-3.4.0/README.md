# Comparing `tmp/chime_frb_api-3.3.0.tar.gz` & `tmp/chime_frb_api-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chime_frb_api-3.3.0.tar", max compression
+gzip compressed data, was "chime_frb_api-3.4.0.tar", max compression
```

## Comparing `chime_frb_api-3.3.0.tar` & `chime_frb_api-3.4.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
--rw-r--r--   0        0        0     1080 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/LICENSE
--rw-r--r--   0        0        0     1386 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/README.md
--rw-r--r--   0        0        0      277 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/__init__.py
--rw-r--r--   0        0        0        0 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/backends/__init__.py
--rw-r--r--   0        0        0      352 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/backends/bucket.py
--rw-r--r--   0        0        0      392 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/backends/distributor.py
--rw-r--r--   0        0        0     1932 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/backends/frb_master.py
--rw-r--r--   0        0        0      784 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/cli.py
--rw-r--r--   0        0        0      368 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/configs/__init__.py
--rw-r--r--   0        0        0      136 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/configs/test_workflow.yaml
--rw-r--r--   0        0        0     1185 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/configs/workflow.yaml
--rw-r--r--   0        0        0       48 2023-10-24 19:43:45.099926 chime_frb_api-3.3.0/chime_frb_api/core/__init__.py
--rw-r--r--   0        0        0    18785 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/core/core.py
--rw-r--r--   0        0        0      289 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/core/exceptions.py
--rw-r--r--   0        0        0      144 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/core/json_type.py
--rw-r--r--   0        0        0     2569 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/core/logger.py
--rw-r--r--   0        0        0      265 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/__init__.py
--rw-r--r--   0        0        0     4193 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/bucket.py
--rw-r--r--   0        0        0     8750 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/buckets.py
--rw-r--r--   0        0        0     4548 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/calibration.py
--rw-r--r--   0        0        0      570 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/candidates.py
--rw-r--r--   0        0        0      810 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/catalog.py
--rw-r--r--   0        0        0     4839 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/distributor.py
--rw-r--r--   0        0        0    11808 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/events.py
--rw-r--r--   0        0        0     5521 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/metrics.py
--rw-r--r--   0        0        0     2013 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/mimic.py
--rw-r--r--   0        0        0     4000 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/parameters.py
--rw-r--r--   0        0        0     4947 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/results.py
--rw-r--r--   0        0        0     1875 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/sources.py
--rw-r--r--   0        0        0    11581 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/swarm.py
--rw-r--r--   0        0        0    12551 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/tns.py
--rw-r--r--   0        0        0     1879 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/verification.py
--rw-r--r--   0        0        0    12214 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/voe.py
--rw-r--r--   0        0        0     4234 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/modules/voe_subscribers.py
--rw-r--r--   0        0        0        0 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/stations/__init__.py
--rw-r--r--   0        0        0       22 2023-10-24 19:43:45.103926 chime_frb_api-3.3.0/chime_frb_api/stations/aro.py
--rw-r--r--   0        0        0      706 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/stations/drao.py
--rw-r--r--   0        0        0       22 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/stations/gbo.py
--rw-r--r--   0        0        0     2876 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/docker-compose.yml
--rw-r--r--   0        0        0    10182 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_archive.py
--rw-r--r--   0        0        0     3423 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_audit_daemon.py
--rw-r--r--   0        0        0     1830 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_bucket.py
--rw-r--r--   0        0        0     4507 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_buckets.py
--rw-r--r--   0        0        0     1764 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_calibration.py
--rw-r--r--   0        0        0      262 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_candidates.py
--rw-r--r--   0        0        0      610 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_catalog.py
--rw-r--r--   0        0        0     3413 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_core.py
--rw-r--r--   0        0        0     2066 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_distributor.py
--rw-r--r--   0        0        0     6891 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_events.py
--rw-r--r--   0        0        0     3335 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_metrics.py
--rw-r--r--   0        0        0      960 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_mimic.py
--rw-r--r--   0        0        0      849 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_parameters.py
--rw-r--r--   0        0        0     2134 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_results.py
--rw-r--r--   0        0        0      384 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_sources.py
--rw-r--r--   0        0        0      256 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_stations.py
--rw-r--r--   0        0        0     1454 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_swarm.py
--rw-r--r--   0        0        0     7035 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_tns.py
--rw-r--r--   0        0        0     5367 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_transfer_daemon.py
--rw-r--r--   0        0        0      467 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_verification.py
--rw-r--r--   0        0        0     8503 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_voe.py
--rw-r--r--   0        0        0     2780 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_voe_subscribers.py
--rw-r--r--   0        0        0     5167 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_work.py
--rw-r--r--   0        0        0     1208 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_work_http_operations.py
--rw-r--r--   0        0        0     8292 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/utils/__init__.py
--rw-r--r--   0        0        0     2642 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/utils/copy.py
--rw-r--r--   0        0        0      859 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/utils/github.py
--rw-r--r--   0        0        0     1263 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/utils/loki.py
--rw-r--r--   0        0        0     2642 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/utils/move.py
--rw-r--r--   0        0        0       76 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/__init__.py
--rw-r--r--   0        0        0        0 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/cli/__init__.py
--rw-r--r--   0        0        0     3899 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/cli/buckets.py
--rw-r--r--   0        0        0     5680 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/cli/pipelines.py
--rw-r--r--   0        0        0    10559 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/cli/run.py
--rw-r--r--   0        0        0      789 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/cli/sample.py
--rw-r--r--   0        0        0      787 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/cli/sample.yaml
--rw-r--r--   0        0        0        0 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/daemons/__init__.py
--rw-r--r--   0        0        0      980 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/daemons/audit.py
--rw-r--r--   0        0        0     6787 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/daemons/transfer.py
--rw-r--r--   0        0        0       32 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/__init__.py
--rw-r--r--   0        0        0     5753 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/archive.py
--rw-r--r--   0        0        0       33 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/attempt.py
--rw-r--r--   0        0        0      523 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/container.py
--rw-r--r--   0        0        0     4323 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/execute.py
--rw-r--r--   0        0        0     1818 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/validate.py
--rwxr-xr-x   0        0        0      408 2023-10-24 19:43:45.107926 chime_frb_api-3.3.0/chime_frb_api/workflow/runner.py
--rw-r--r--   0        0        0    18365 2023-10-24 19:43:45.111926 chime_frb_api-3.3.0/chime_frb_api/workflow/work.py
--rw-r--r--   0        0        0     1842 2023-10-24 19:43:45.127926 chime_frb_api-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 chime_frb_api-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/LICENSE
+-rw-r--r--   0        0        0     1386 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/README.md
+-rw-r--r--   0        0        0      277 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/backends/__init__.py
+-rw-r--r--   0        0        0      352 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/backends/bucket.py
+-rw-r--r--   0        0        0      392 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/backends/distributor.py
+-rw-r--r--   0        0        0     1932 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/backends/frb_master.py
+-rw-r--r--   0        0        0      784 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/cli.py
+-rw-r--r--   0        0        0      368 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/configs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/configs/test_workflow.yaml
+-rw-r--r--   0        0        0     1185 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/configs/workflow.yaml
+-rw-r--r--   0        0        0       48 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/core/__init__.py
+-rw-r--r--   0        0        0    18785 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/core/core.py
+-rw-r--r--   0        0        0      289 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/core/exceptions.py
+-rw-r--r--   0        0        0      144 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/core/json_type.py
+-rw-r--r--   0        0        0     2569 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/core/logger.py
+-rw-r--r--   0        0        0      265 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/__init__.py
+-rw-r--r--   0        0        0     4193 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/bucket.py
+-rw-r--r--   0        0        0     8750 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/buckets.py
+-rw-r--r--   0        0        0     4548 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/calibration.py
+-rw-r--r--   0        0        0      570 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/candidates.py
+-rw-r--r--   0        0        0      810 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/catalog.py
+-rw-r--r--   0        0        0     4839 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/distributor.py
+-rw-r--r--   0        0        0    11803 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/events.py
+-rw-r--r--   0        0        0     5521 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/metrics.py
+-rw-r--r--   0        0        0     2013 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/mimic.py
+-rw-r--r--   0        0        0     4000 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/parameters.py
+-rw-r--r--   0        0        0    10259 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/results.py
+-rw-r--r--   0        0        0     1875 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/sources.py
+-rw-r--r--   0        0        0    11581 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/swarm.py
+-rw-r--r--   0        0        0    12551 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/tns.py
+-rw-r--r--   0        0        0     1879 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/verification.py
+-rw-r--r--   0        0        0    12214 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/voe.py
+-rw-r--r--   0        0        0     4234 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/modules/voe_subscribers.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/stations/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/stations/aro.py
+-rw-r--r--   0        0        0      706 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/stations/drao.py
+-rw-r--r--   0        0        0       22 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/stations/gbo.py
+-rw-r--r--   0        0        0     2876 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/docker-compose.yml
+-rw-r--r--   0        0        0    10182 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_archive.py
+-rw-r--r--   0        0        0     3423 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_audit_daemon.py
+-rw-r--r--   0        0        0     1830 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_bucket.py
+-rw-r--r--   0        0        0     4507 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_buckets.py
+-rw-r--r--   0        0        0     1764 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_calibration.py
+-rw-r--r--   0        0        0      262 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_candidates.py
+-rw-r--r--   0        0        0      610 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_catalog.py
+-rw-r--r--   0        0        0     3413 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_core.py
+-rw-r--r--   0        0        0     2066 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_distributor.py
+-rw-r--r--   0        0        0     6891 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_events.py
+-rw-r--r--   0        0        0     3335 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_metrics.py
+-rw-r--r--   0        0        0      960 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_mimic.py
+-rw-r--r--   0        0        0      849 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_parameters.py
+-rw-r--r--   0        0        0     5930 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_results.py
+-rw-r--r--   0        0        0      384 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_sources.py
+-rw-r--r--   0        0        0      256 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_stations.py
+-rw-r--r--   0        0        0     1454 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_swarm.py
+-rw-r--r--   0        0        0     7035 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_tns.py
+-rw-r--r--   0        0        0     5367 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_transfer_daemon.py
+-rw-r--r--   0        0        0      467 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_verification.py
+-rw-r--r--   0        0        0     8503 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_voe.py
+-rw-r--r--   0        0        0     2780 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_voe_subscribers.py
+-rw-r--r--   0        0        0     5167 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_work.py
+-rw-r--r--   0        0        0     1208 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_work_http_operations.py
+-rw-r--r--   0        0        0     8292 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/utils/__init__.py
+-rw-r--r--   0        0        0     2642 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/utils/copy.py
+-rw-r--r--   0        0        0      859 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/utils/github.py
+-rw-r--r--   0        0        0     1263 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/utils/loki.py
+-rw-r--r--   0        0        0     3706 2024-05-14 22:03:18.954264 chime_frb_api-3.4.0/chime_frb_api/utils/migrate.py
+-rw-r--r--   0        0        0     2642 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/utils/move.py
+-rw-r--r--   0        0        0       76 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/cli/__init__.py
+-rw-r--r--   0        0        0     3899 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/cli/buckets.py
+-rw-r--r--   0        0        0     5680 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/cli/pipelines.py
+-rw-r--r--   0        0        0    10559 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/cli/run.py
+-rw-r--r--   0        0        0      789 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/cli/sample.py
+-rw-r--r--   0        0        0      787 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/cli/sample.yaml
+-rw-r--r--   0        0        0        0 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/daemons/__init__.py
+-rw-r--r--   0        0        0      980 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/daemons/audit.py
+-rw-r--r--   0        0        0     6787 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/daemons/transfer.py
+-rw-r--r--   0        0        0       32 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/__init__.py
+-rw-r--r--   0        0        0     5753 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/archive.py
+-rw-r--r--   0        0        0       33 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/attempt.py
+-rw-r--r--   0        0        0      523 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/container.py
+-rw-r--r--   0        0        0     4323 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/execute.py
+-rw-r--r--   0        0        0     1818 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/validate.py
+-rwxr-xr-x   0        0        0      408 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/runner.py
+-rw-r--r--   0        0        0    18365 2024-05-14 22:03:18.958264 chime_frb_api-3.4.0/chime_frb_api/workflow/work.py
+-rw-r--r--   0        0        0     1842 2024-05-14 22:03:18.970265 chime_frb_api-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 chime_frb_api-3.4.0/PKG-INFO
```

### Comparing `chime_frb_api-3.3.0/LICENSE` & `chime_frb_api-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/README.md` & `chime_frb_api-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/backends/frb_master.py` & `chime_frb_api-3.4.0/chime_frb_api/backends/frb_master.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/cli.py` & `chime_frb_api-3.4.0/chime_frb_api/cli.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/configs/workflow.yaml` & `chime_frb_api-3.4.0/chime_frb_api/configs/workflow.yaml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/core/core.py` & `chime_frb_api-3.4.0/chime_frb_api/core/core.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/core/logger.py` & `chime_frb_api-3.4.0/chime_frb_api/core/logger.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/bucket.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/bucket.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/buckets.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/calibration.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/calibration.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/candidates.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/candidates.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/catalog.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/catalog.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/distributor.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/distributor.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/events.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,28 +150,28 @@
             dict
         """
         if full_header:
             return self.API.get(f"/v1/events/full-header/{event_number}")
         else:
             return self.API.get(f"/v1/events/{event_number}")
 
-    def get_events(self, event_numbers: List[int], full_header: bool = False) -> List[dict]:
+    def get_events(self, event_numbers: List[int], full_header: bool = False) -> dict:
         """Get CHIME/FRB Events Information.
 
         Args:
             event_numbers: list of CHIME/FRB Event Number
             full_header: Get the full event from L4, default is False
 
         Returns:
             List[dict]
         """
         event_data = {}
         url_prefix = "/v1/events/full-header/" if full_header else "/v1/events/"
         for event_number in event_numbers:
-            event_data[event_number]= self.API.get(f"{url_prefix}{event_number}")
+            event_data[event_number] = self.API.get(f"{url_prefix}{event_number}")
         return event_data
 
     def get_all_events(self) -> list:
         """Get all CHIME/FRB Events from Events Database.
 
         Args:
             None
```

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/metrics.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/metrics.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/mimic.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/mimic.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/parameters.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/parameters.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/sources.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/sources.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/swarm.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/swarm.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/tns.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/tns.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/verification.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/verification.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/voe.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/voe.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/modules/voe_subscribers.py` & `chime_frb_api-3.4.0/chime_frb_api/modules/voe_subscribers.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/stations/drao.py` & `chime_frb_api-3.4.0/chime_frb_api/stations/drao.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/docker-compose.yml` & `chime_frb_api-3.4.0/chime_frb_api/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_archive.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_audit_daemon.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_audit_daemon.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_bucket.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_buckets.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_calibration.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_catalog.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_core.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_distributor.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_distributor.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_events.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_metrics.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_mimic.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_mimic.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_parameters.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_swarm.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_swarm.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_tns.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_tns.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_transfer_daemon.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_transfer_daemon.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_voe.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_voe.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_voe_subscribers.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_voe_subscribers.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_work.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_work.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_work_http_operations.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_work_http_operations.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/tests/test_workflow.py` & `chime_frb_api-3.4.0/chime_frb_api/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/utils/copy.py` & `chime_frb_api-3.4.0/chime_frb_api/utils/copy.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/utils/github.py` & `chime_frb_api-3.4.0/chime_frb_api/utils/github.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/utils/loki.py` & `chime_frb_api-3.4.0/chime_frb_api/utils/loki.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/utils/move.py` & `chime_frb_api-3.4.0/chime_frb_api/utils/move.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/cli/buckets.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/cli/buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/cli/pipelines.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/cli/run.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/cli/run.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/cli/sample.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/cli/sample.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/cli/sample.yaml` & `chime_frb_api-3.4.0/chime_frb_api/workflow/cli/sample.yaml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/daemons/audit.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/daemons/audit.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/daemons/transfer.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/daemons/transfer.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/archive.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/archive.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/container.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/container.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/execute.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/execute.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/lifecycle/validate.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/lifecycle/validate.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/chime_frb_api/workflow/work.py` & `chime_frb_api-3.4.0/chime_frb_api/workflow/work.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.3.0/pyproject.toml` & `chime_frb_api-3.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chime-frb-api"
-version = "3.3.0"
+version = "3.4.0"
 description = "CHIME/FRB API"
 authors = ["Shiny Brar <charanjotbrar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CHIMEFRB/frb-api"
 documentation = "https://github.com/CHIMEFRB/frb-api"
 classifiers = [
```

### Comparing `chime_frb_api-3.3.0/PKG-INFO` & `chime_frb_api-3.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chime-frb-api
-Version: 3.3.0
+Version: 3.4.0
 Summary: CHIME/FRB API
 Home-page: https://github.com/CHIMEFRB/frb-api
 License: MIT
 Author: Shiny Brar
 Author-email: charanjotbrar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: click (>=7)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: mkdocs-material (>=8) ; extra == "docs"
```

