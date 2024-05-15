# Comparing `tmp/fractal_server-2.0.4.tar.gz` & `tmp/fractal_server-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-2.0.4.tar", max compression
+gzip compressed data, was "fractal_server-2.0.5.tar", max compression
```

## Comparing `fractal_server-2.0.4.tar` & `fractal_server-2.0.5.tar`

### file list

```diff
@@ -1,169 +1,168 @@
--rw-r--r--   0        0        0     1576 2024-05-06 12:52:10.654958 fractal_server-2.0.4/LICENSE
--rw-r--r--   0        0        0     2486 2024-05-06 12:52:10.654958 fractal_server-2.0.4/README.md
--rw-r--r--   0        0        0       22 2024-05-06 12:52:10.658958 fractal_server-2.0.4/fractal_server/__init__.py
--rw-r--r--   0        0        0     4958 2024-05-06 12:52:10.658958 fractal_server-2.0.4/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2024-05-06 12:52:10.658958 fractal_server-2.0.4/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.658958 fractal_server-2.0.4/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     4042 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      267 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0      567 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     3378 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/security.py
--rw-r--r--   0        0        0      458 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/__init__.py
--rw-r--r--   0        0        0     2017 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/dataset.py
--rw-r--r--   0        0        0     3304 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/job.py
--rw-r--r--   0        0        0      859 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/project.py
--rw-r--r--   0        0        0     1095 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/state.py
--rw-r--r--   0        0        0     2782 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/task.py
--rw-r--r--   0        0        0     3950 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/workflow.py
--rw-r--r--   0        0        0      473 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/__init__.py
--rw-r--r--   0        0        0      588 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/collection_state.py
--rw-r--r--   0        0        0     1455 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/dataset.py
--rw-r--r--   0        0        0     1535 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/job.py
--rw-r--r--   0        0        0      817 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/project.py
--rw-r--r--   0        0        0     3257 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/task.py
--rw-r--r--   0        0        0     1069 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/workflow.py
--rw-r--r--   0        0        0     1532 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/workflowtask.py
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/admin/__init__.py
--rw-r--r--   0        0        0    13996 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/admin/v1.py
--rw-r--r--   0        0        0     9830 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/admin/v2.py
--rw-r--r--   0        0        0      315 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/__init__.py
--rw-r--r--   0        0        0      958 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/__init__.py
--rw-r--r--   0        0        0    11973 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/_aux_functions.py
--rw-r--r--   0        0        0    16923 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/dataset.py
--rw-r--r--   0        0        0     5436 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/job.py
--rw-r--r--   0        0        0    15799 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/project.py
--rw-r--r--   0        0        0     6129 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/task.py
--rw-r--r--   0        0        0     8882 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/task_collection.py
--rw-r--r--   0        0        0    10942 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/workflow.py
--rw-r--r--   0        0        0     5582 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/workflowtask.py
--rw-r--r--   0        0        0     1487 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/__init__.py
--rw-r--r--   0        0        0    14301 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/_aux_functions.py
--rw-r--r--   0        0        0     8248 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/dataset.py
--rw-r--r--   0        0        0     7894 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/images.py
--rw-r--r--   0        0        0     5325 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/job.py
--rw-r--r--   0        0        0     5594 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/project.py
--rw-r--r--   0        0        0     6394 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/status.py
--rw-r--r--   0        0        0     6940 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/submit.py
--rw-r--r--   0        0        0     7130 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/task.py
--rw-r--r--   0        0        0     8988 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/task_collection.py
--rw-r--r--   0        0        0     1628 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/task_legacy.py
--rw-r--r--   0        0        0    11863 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/workflow.py
--rw-r--r--   0        0        0     8802 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/workflowtask.py
--rw-r--r--   0        0        0     4885 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/auth.py
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/aux/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/aux/_job.py
--rw-r--r--   0        0        0      675 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/aux/_runner.py
--rw-r--r--   0        0        0       16 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0      829 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/async_wrap.py
--rw-r--r--   0        0        0      119 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/components.py
--rw-r--r--   0        0        0     4159 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/__init__.py
--rw-r--r--   0        0        0       65 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/__init__.py
--rw-r--r--   0        0        0     8841 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_batching.py
--rw-r--r--   0        0        0     1908 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
--rw-r--r--   0        0        0     4421 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    15552 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_slurm_config.py
--rw-r--r--   0        0        0     5123 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    44655 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/executor.py
--rw-r--r--   0        0        0     5852 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/remote.py
--rw-r--r--   0        0        0      206 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/filenames.py
--rw-r--r--   0        0        0     1254 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/set_start_and_last_task_index.py
--rw-r--r--   0        0        0     3180 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/task_files.py
--rw-r--r--   0        0        0    13620 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/v1/__init__.py
--rw-r--r--   0        0        0    21246 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/v1/_common.py
--rw-r--r--   0        0        0     6839 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/v1/_local/__init__.py
--rw-r--r--   0        0        0     3147 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_local/_local_config.py
--rw-r--r--   0        0        0     1493 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_local/executor.py
--rw-r--r--   0        0        0    10853 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/__init__.py
--rw-r--r--   0        0        0     2738 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     5977 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0     3294 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/common.py
--rw-r--r--   0        0        0     4684 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/handle_failed_job.py
--rw-r--r--   0        0        0    12500 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/__init__.py
--rw-r--r--   0        0        0     5881 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_local/__init__.py
--rw-r--r--   0        0        0     3630 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_local/_local_config.py
--rw-r--r--   0        0        0     1614 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_local/executor.py
--rw-r--r--   0        0        0     4409 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/__init__.py
--rw-r--r--   0        0        0     2793 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     6726 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0      639 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/deduplicate_list.py
--rw-r--r--   0        0        0     5415 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/handle_failed_job.py
--rw-r--r--   0        0        0     1281 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/merge_outputs.py
--rw-r--r--   0        0        0    14160 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/runner.py
--rw-r--r--   0        0        0    11067 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/runner_functions.py
--rw-r--r--   0        0        0     3710 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/runner_functions_low_level.py
--rw-r--r--   0        0        0     1866 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/task_interface.py
--rw-r--r--   0        0        0      912 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/v1_compat.py
--rw-r--r--   0        0        0       40 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/__init__.py
--rw-r--r--   0        0        0     3461 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/_validators.py
--rw-r--r--   0        0        0      692 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/state.py
--rw-r--r--   0        0        0     3113 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/user.py
--rw-r--r--   0        0        0     1809 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/__init__.py
--rw-r--r--   0        0        0     4302 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/applyworkflow.py
--rw-r--r--   0        0        0     3444 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/dataset.py
--rw-r--r--   0        0        0     1274 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/dumps.py
--rw-r--r--   0        0        0     3829 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/manifest.py
--rw-r--r--   0        0        0     1218 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/project.py
--rw-r--r--   0        0        0     3704 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/task.py
--rw-r--r--   0        0        0     3057 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/task_collection.py
--rw-r--r--   0        0        0     4618 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/workflow.py
--rw-r--r--   0        0        0     1852 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/__init__.py
--rw-r--r--   0        0        0     2599 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/dataset.py
--rw-r--r--   0        0        0     2063 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/dumps.py
--rw-r--r--   0        0        0     3250 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/job.py
--rw-r--r--   0        0        0     6243 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/manifest.py
--rw-r--r--   0        0        0      736 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/project.py
--rw-r--r--   0        0        0      332 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/status.py
--rw-r--r--   0        0        0     4672 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/task.py
--rw-r--r--   0        0        0     3171 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/task_collection.py
--rw-r--r--   0        0        0     1827 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/workflow.py
--rw-r--r--   0        0        0     6552 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/workflowtask.py
--rw-r--r--   0        0        0    11203 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0    15048 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/config.py
--rw-r--r--   0        0        0     2918 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/data_migrations/2_0_3.py
--rw-r--r--   0        0        0      398 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/data_migrations/README.md
--rw-r--r--   0        0        0      196 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/images/__init__.py
--rw-r--r--   0        0        0     4167 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/images/models.py
--rw-r--r--   0        0        0     2209 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/images/tools.py
--rw-r--r--   0        0        0     4178 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/logger.py
--rw-r--r--   0        0        0     3381 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/main.py
--rw-r--r--   0        0        0       59 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/README
--rw-r--r--   0        0        0     2630 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      526 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     1157 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
--rw-r--r--   0        0        0     8770 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0     8433 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/5bf02391cfef_v2.py
--rw-r--r--   0        0        0     1632 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
--rw-r--r--   0        0        0     1353 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
--rw-r--r--   0        0        0     2684 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
--rw-r--r--   0        0        0     1115 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
--rw-r--r--   0        0        0     1057 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
--rw-r--r--   0        0        0      883 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
--rw-r--r--   0        0        0     1849 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
--rw-r--r--   0        0        0      867 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
--rw-r--r--   0        0        0      949 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
--rw-r--r--   0        0        0      963 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
--rw-r--r--   0        0        0     1221 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
--rw-r--r--   0        0        0      746 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/syringe.py
--rw-r--r--   0        0        0       23 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0     5379 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/endpoint_operations.py
--rw-r--r--   0        0        0     3278 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/utils.py
--rw-r--r--   0        0        0     3775 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v1/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v1/__init__.py
--rw-r--r--   0        0        0    11731 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v1/background_operations.py
--rw-r--r--   0        0        0      502 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v1/get_collection_data.py
--rw-r--r--   0        0        0     3775 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v2/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v2/__init__.py
--rw-r--r--   0        0        0    12922 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v2/background_operations.py
--rw-r--r--   0        0        0      502 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v2/get_collection_data.py
--rw-r--r--   0        0        0      448 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/urls.py
--rw-r--r--   0        0        0     2115 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/utils.py
--rw-r--r--   0        0        0     3052 2024-05-06 12:52:10.670958 fractal_server-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     4222 1970-01-01 00:00:00.000000 fractal_server-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-05-07 10:20:30.305004 fractal_server-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2486 2024-05-07 10:20:30.305004 fractal_server-2.0.5/README.md
+-rw-r--r--   0        0        0       22 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/__init__.py
+-rw-r--r--   0        0        0     4958 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     4042 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      267 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0      567 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     3378 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0      458 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v1/__init__.py
+-rw-r--r--   0        0        0     2017 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v1/dataset.py
+-rw-r--r--   0        0        0     3304 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v1/job.py
+-rw-r--r--   0        0        0      859 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v1/project.py
+-rw-r--r--   0        0        0     1095 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v1/state.py
+-rw-r--r--   0        0        0     2782 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v1/task.py
+-rw-r--r--   0        0        0     3950 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v1/workflow.py
+-rw-r--r--   0        0        0      473 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v2/__init__.py
+-rw-r--r--   0        0        0      588 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v2/collection_state.py
+-rw-r--r--   0        0        0     1455 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v2/dataset.py
+-rw-r--r--   0        0        0     1535 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v2/job.py
+-rw-r--r--   0        0        0      817 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v2/project.py
+-rw-r--r--   0        0        0     3257 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v2/task.py
+-rw-r--r--   0        0        0     1069 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v2/workflow.py
+-rw-r--r--   0        0        0     1532 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/models/v2/workflowtask.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/admin/__init__.py
+-rw-r--r--   0        0        0    13996 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/admin/v1.py
+-rw-r--r--   0        0        0    13757 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/admin/v2.py
+-rw-r--r--   0        0        0      315 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/__init__.py
+-rw-r--r--   0        0        0      958 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/__init__.py
+-rw-r--r--   0        0        0    11973 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0    16923 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/dataset.py
+-rw-r--r--   0        0        0     5436 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/job.py
+-rw-r--r--   0        0        0    15799 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/project.py
+-rw-r--r--   0        0        0     6129 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/task.py
+-rw-r--r--   0        0        0     8882 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/task_collection.py
+-rw-r--r--   0        0        0    10942 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/workflow.py
+-rw-r--r--   0        0        0     5582 2024-05-07 10:20:30.309004 fractal_server-2.0.5/fractal_server/app/routes/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     1487 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/__init__.py
+-rw-r--r--   0        0        0    14301 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/_aux_functions.py
+-rw-r--r--   0        0        0     8248 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/dataset.py
+-rw-r--r--   0        0        0     7894 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/images.py
+-rw-r--r--   0        0        0     5325 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/job.py
+-rw-r--r--   0        0        0     5594 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/project.py
+-rw-r--r--   0        0        0     6394 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/status.py
+-rw-r--r--   0        0        0     7672 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/submit.py
+-rw-r--r--   0        0        0     8297 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/task.py
+-rw-r--r--   0        0        0     8988 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/task_collection.py
+-rw-r--r--   0        0        0     1628 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/task_legacy.py
+-rw-r--r--   0        0        0    11863 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/workflow.py
+-rw-r--r--   0        0        0     8802 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/api/v2/workflowtask.py
+-rw-r--r--   0        0        0     4885 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/auth.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/aux/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/aux/_job.py
+-rw-r--r--   0        0        0      675 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/routes/aux/_runner.py
+-rw-r--r--   0        0        0       16 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0      829 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/async_wrap.py
+-rw-r--r--   0        0        0      119 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/components.py
+-rw-r--r--   0        0        0     4159 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/__init__.py
+-rw-r--r--   0        0        0     8841 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_batching.py
+-rw-r--r--   0        0        0     1908 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
+-rw-r--r--   0        0        0     4421 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    15552 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_slurm_config.py
+-rw-r--r--   0        0        0     5123 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    44655 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/executor.py
+-rw-r--r--   0        0        0     5852 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/remote.py
+-rw-r--r--   0        0        0      206 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/filenames.py
+-rw-r--r--   0        0        0     1254 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/set_start_and_last_task_index.py
+-rw-r--r--   0        0        0     3180 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/task_files.py
+-rw-r--r--   0        0        0    13620 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/__init__.py
+-rw-r--r--   0        0        0    21246 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/_common.py
+-rw-r--r--   0        0        0     6839 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/_local/__init__.py
+-rw-r--r--   0        0        0     3147 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/_local/_local_config.py
+-rw-r--r--   0        0        0     1493 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/_local/executor.py
+-rw-r--r--   0        0        0    10853 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/_slurm/__init__.py
+-rw-r--r--   0        0        0     2738 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     5977 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0     3294 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/common.py
+-rw-r--r--   0        0        0     4684 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v1/handle_failed_job.py
+-rw-r--r--   0        0        0    11952 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/__init__.py
+-rw-r--r--   0        0        0     5881 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/_local/__init__.py
+-rw-r--r--   0        0        0     3630 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/_local/_local_config.py
+-rw-r--r--   0        0        0     1614 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/_local/executor.py
+-rw-r--r--   0        0        0     4409 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/_slurm/__init__.py
+-rw-r--r--   0        0        0     2793 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     6726 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0      639 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/deduplicate_list.py
+-rw-r--r--   0        0        0     5415 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/handle_failed_job.py
+-rw-r--r--   0        0        0     1281 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/merge_outputs.py
+-rw-r--r--   0        0        0    14160 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/runner.py
+-rw-r--r--   0        0        0    11067 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/runner_functions.py
+-rw-r--r--   0        0        0     3710 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/runner_functions_low_level.py
+-rw-r--r--   0        0        0     1866 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/task_interface.py
+-rw-r--r--   0        0        0      912 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/runner/v2/v1_compat.py
+-rw-r--r--   0        0        0       40 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/__init__.py
+-rw-r--r--   0        0        0     3461 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/_validators.py
+-rw-r--r--   0        0        0      692 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/state.py
+-rw-r--r--   0        0        0     3113 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/user.py
+-rw-r--r--   0        0        0     1809 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     4302 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/v1/applyworkflow.py
+-rw-r--r--   0        0        0     3444 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/v1/dataset.py
+-rw-r--r--   0        0        0     1274 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/v1/dumps.py
+-rw-r--r--   0        0        0     3829 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/v1/manifest.py
+-rw-r--r--   0        0        0     1218 2024-05-07 10:20:30.313004 fractal_server-2.0.5/fractal_server/app/schemas/v1/project.py
+-rw-r--r--   0        0        0     3704 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v1/task.py
+-rw-r--r--   0        0        0     3057 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v1/task_collection.py
+-rw-r--r--   0        0        0     4618 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v1/workflow.py
+-rw-r--r--   0        0        0     1852 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/__init__.py
+-rw-r--r--   0        0        0     2599 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/dataset.py
+-rw-r--r--   0        0        0     2063 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/dumps.py
+-rw-r--r--   0        0        0     3250 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/job.py
+-rw-r--r--   0        0        0     6243 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/manifest.py
+-rw-r--r--   0        0        0      736 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/project.py
+-rw-r--r--   0        0        0      332 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/status.py
+-rw-r--r--   0        0        0     4672 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/task.py
+-rw-r--r--   0        0        0     3171 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/task_collection.py
+-rw-r--r--   0        0        0     1827 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/workflow.py
+-rw-r--r--   0        0        0     6552 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/schemas/v2/workflowtask.py
+-rw-r--r--   0        0        0    11203 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0    15048 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/config.py
+-rw-r--r--   0        0        0      398 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/data_migrations/README.md
+-rw-r--r--   0        0        0      196 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/images/__init__.py
+-rw-r--r--   0        0        0     4167 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/images/models.py
+-rw-r--r--   0        0        0     2209 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/images/tools.py
+-rw-r--r--   0        0        0     4178 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/logger.py
+-rw-r--r--   0        0        0     3381 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2630 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      526 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     1157 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
+-rw-r--r--   0        0        0     8770 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     8433 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/5bf02391cfef_v2.py
+-rw-r--r--   0        0        0     1632 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0     1353 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
+-rw-r--r--   0        0        0     2684 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
+-rw-r--r--   0        0        0     1115 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
+-rw-r--r--   0        0        0     1057 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
+-rw-r--r--   0        0        0      883 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
+-rw-r--r--   0        0        0     1849 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
+-rw-r--r--   0        0        0      867 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
+-rw-r--r--   0        0        0      949 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
+-rw-r--r--   0        0        0      963 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
+-rw-r--r--   0        0        0     1221 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
+-rw-r--r--   0        0        0      746 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/syringe.py
+-rw-r--r--   0        0        0       23 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0     5379 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/endpoint_operations.py
+-rw-r--r--   0        0        0     3278 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/utils.py
+-rw-r--r--   0        0        0     3775 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/v1/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/v1/__init__.py
+-rw-r--r--   0        0        0    11731 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/v1/background_operations.py
+-rw-r--r--   0        0        0      502 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/v1/get_collection_data.py
+-rw-r--r--   0        0        0     3775 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/v2/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/v2/__init__.py
+-rw-r--r--   0        0        0    12922 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/v2/background_operations.py
+-rw-r--r--   0        0        0      502 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/tasks/v2/get_collection_data.py
+-rw-r--r--   0        0        0      448 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/urls.py
+-rw-r--r--   0        0        0     2115 2024-05-07 10:20:30.317004 fractal_server-2.0.5/fractal_server/utils.py
+-rw-r--r--   0        0        0     3052 2024-05-07 10:20:30.317004 fractal_server-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4222 1970-01-01 00:00:00.000000 fractal_server-2.0.5/PKG-INFO
```

### Comparing `fractal_server-2.0.4/LICENSE` & `fractal_server-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/README.md` & `fractal_server-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/__main__.py` & `fractal_server-2.0.5/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/alembic.ini` & `fractal_server-2.0.5/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/db/__init__.py` & `fractal_server-2.0.5/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/linkuserproject.py` & `fractal_server-2.0.5/fractal_server/app/models/linkuserproject.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/security.py` & `fractal_server-2.0.5/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v1/dataset.py` & `fractal_server-2.0.5/fractal_server/app/models/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v1/job.py` & `fractal_server-2.0.5/fractal_server/app/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v1/project.py` & `fractal_server-2.0.5/fractal_server/app/models/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v1/state.py` & `fractal_server-2.0.5/fractal_server/app/models/v1/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v1/task.py` & `fractal_server-2.0.5/fractal_server/app/models/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v1/workflow.py` & `fractal_server-2.0.5/fractal_server/app/models/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v2/collection_state.py` & `fractal_server-2.0.5/fractal_server/app/models/v2/collection_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v2/dataset.py` & `fractal_server-2.0.5/fractal_server/app/models/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v2/job.py` & `fractal_server-2.0.5/fractal_server/app/models/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v2/project.py` & `fractal_server-2.0.5/fractal_server/app/models/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v2/task.py` & `fractal_server-2.0.5/fractal_server/app/models/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v2/workflow.py` & `fractal_server-2.0.5/fractal_server/app/models/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/models/v2/workflowtask.py` & `fractal_server-2.0.5/fractal_server/app/models/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/admin/v1.py` & `fractal_server-2.0.5/fractal_server/app/routes/admin/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/admin/v2.py` & `fractal_server-2.0.5/fractal_server/app/routes/admin/v2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 """
 Definition of `/admin` routes.
 """
 from datetime import datetime
 from datetime import timezone
 from pathlib import Path
+from typing import Literal
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 from fastapi.responses import StreamingResponse
 from pydantic import BaseModel
+from pydantic import EmailStr
+from pydantic import Field
 from sqlmodel import select
 
 from ....config import get_settings
 from ....syringe import Inject
 from ....utils import get_timestamp
 from ...db import AsyncSession
 from ...db import get_async_db
 from ...models.security import UserOAuth as User
 from ...models.v1 import Task
 from ...models.v2 import JobV2
 from ...models.v2 import ProjectV2
+from ...models.v2 import TaskV2
+from ...models.v2 import WorkflowTaskV2
+from ...models.v2 import WorkflowV2
 from ...runner.filenames import WORKFLOW_LOG_FILENAME
 from ...schemas.v2 import JobReadV2
 from ...schemas.v2 import JobStatusTypeV2
 from ...schemas.v2 import JobUpdateV2
 from ...schemas.v2 import ProjectReadV2
 from ...security import current_active_superuser
 from ..aux._job import _write_shutdown_file
@@ -303,7 +309,132 @@
         )
 
     task.is_v2_compatible = compatibility.is_v2_compatible
     await db.commit()
     await db.close()
 
     return Response(status_code=status.HTTP_200_OK)
+
+
+class TaskV2Minimal(BaseModel):
+
+    id: int
+    name: str
+    type: str
+    command_non_parallel: Optional[str]
+    command_parallel: Optional[str]
+    source: str
+    owner: Optional[str]
+    version: Optional[str]
+
+
+class ProjectUser(BaseModel):
+
+    id: int
+    email: EmailStr
+
+
+class TaskV2Relationship(BaseModel):
+
+    workflow_id: int
+    workflow_name: str
+    project_id: int
+    project_name: str
+    project_users: list[ProjectUser] = Field(default_factory=list)
+
+
+class TaskV2Info(BaseModel):
+
+    task: TaskV2Minimal
+    relationships: list[TaskV2Relationship]
+
+
+@router_admin_v2.get("/task/", response_model=list[TaskV2Info])
+async def query_tasks(
+    id: Optional[int] = None,
+    source: Optional[str] = None,
+    version: Optional[str] = None,
+    name: Optional[str] = None,
+    owner: Optional[str] = None,
+    kind: Optional[Literal["common", "users"]] = None,
+    max_number_of_results: int = 25,
+    user: User = Depends(current_active_superuser),
+    db: AsyncSession = Depends(get_async_db),
+) -> list[TaskV2Info]:
+    """
+    Query `TaskV2` table and get informations about related items
+    (WorkflowV2s and ProjectV2s)
+
+    Args:
+        id: If not `None`, query for matching `task.id`.
+        source: If not `None`, query for contained case insensitive
+            `task.source`.
+        version: If not `None`, query for matching `task.version`.
+        name: If not `None`, query for contained case insensitive `task.name`.
+        owner: If not `None`, query for matching `task.owner`.
+        kind: If not `None`, query for TaskV2s that have (`users`) or don't
+            have (`common`) a `task.owner`.
+        max_number_of_results: The maximum length of the response.
+    """
+
+    stm = select(TaskV2)
+
+    if id is not None:
+        stm = stm.where(TaskV2.id == id)
+    if source is not None:
+        stm = stm.where(TaskV2.source.icontains(source))
+    if version is not None:
+        stm = stm.where(TaskV2.version == version)
+    if name is not None:
+        stm = stm.where(TaskV2.name.icontains(name))
+    if owner is not None:
+        stm = stm.where(TaskV2.owner == owner)
+
+    if kind == "common":
+        stm = stm.where(TaskV2.owner == None)  # noqa E711
+    elif kind == "users":
+        stm = stm.where(TaskV2.owner != None)  # noqa E711
+
+    res = await db.execute(stm)
+    task_list = res.scalars().all()
+    if len(task_list) > max_number_of_results:
+        await db.close()
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                f"Too many Tasks ({len(task_list)} > {max_number_of_results})."
+                " Please add more query filters."
+            ),
+        )
+
+    task_info_list = []
+
+    for task in task_list:
+        stm = (
+            select(WorkflowV2)
+            .join(WorkflowTaskV2)
+            .where(WorkflowTaskV2.workflow_id == WorkflowV2.id)
+            .where(WorkflowTaskV2.task_id == task.id)
+        )
+        res = await db.execute(stm)
+        wf_list = res.scalars().all()
+
+        task_info_list.append(
+            dict(
+                task=task.model_dump(),
+                relationships=[
+                    dict(
+                        workflow_id=workflow.id,
+                        workflow_name=workflow.name,
+                        project_id=workflow.project.id,
+                        project_name=workflow.project.name,
+                        project_users=[
+                            dict(id=user.id, email=user.email)
+                            for user in workflow.project.user_list
+                        ],
+                    )
+                    for workflow in wf_list
+                ],
+            )
+        )
+
+    return task_info_list
```

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/__init__.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/_aux_functions.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/dataset.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/job.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/project.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/task.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/task_collection.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/workflow.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v1/workflowtask.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v1/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/__init__.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/_aux_functions.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/dataset.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/images.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/images.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/job.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/project.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/status.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/submit.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/submit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
+from pathlib import Path
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import BackgroundTasks
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import status
 from sqlmodel import select
 
 from .....config import get_settings
 from .....syringe import Inject
+from .....utils import get_timestamp
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models.v2 import JobV2
 from ....runner.set_start_and_last_task_index import (
     set_start_and_last_task_index,
 )
 from ....runner.v2 import submit_workflow
@@ -87,31 +89,25 @@
                 f"(with {num_tasks=}).\n"
                 f"Original error: {str(e)}"
             ),
         )
 
     # If backend is SLURM, check that the user has required attributes
     settings = Inject(get_settings)
-    backend = settings.FRACTAL_RUNNER_BACKEND
-    if backend == "slurm":
+    FRACTAL_RUNNER_BACKEND = settings.FRACTAL_RUNNER_BACKEND
+    if FRACTAL_RUNNER_BACKEND == "slurm":
         if not user.slurm_user:
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                detail=(
-                    f"FRACTAL_RUNNER_BACKEND={backend}, "
-                    f"but {user.slurm_user=}."
-                ),
+                detail=f"{FRACTAL_RUNNER_BACKEND=}, but {user.slurm_user=}.",
             )
         if not user.cache_dir:
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                detail=(
-                    f"FRACTAL_RUNNER_BACKEND={backend}, "
-                    f"but {user.cache_dir=}."
-                ),
+                detail=f"{FRACTAL_RUNNER_BACKEND=}, but {user.cache_dir=}.",
             )
 
     # Check that no other job with the same dataset_id is SUBMITTED
     stm = (
         select(JobV2)
         .where(JobV2.dataset_id == dataset_id)
         .where(JobV2.status == JobStatusTypeV2.SUBMITTED)
@@ -193,20 +189,43 @@
             ),
         )
 
     db.add(job)
     await db.commit()
     await db.refresh(job)
 
+    # Define server-side job directory
+    timestamp_string = get_timestamp().strftime("%Y%m%d_%H%M%S")
+    WORKFLOW_DIR = (
+        settings.FRACTAL_RUNNER_WORKING_BASE_DIR
+        / (
+            f"proj_v2_{project_id:07d}_wf_{workflow_id:07d}_job_{job.id:07d}"
+            f"_{timestamp_string}"
+        )
+    ).resolve()
+
+    # Define user-side job directory
+    if FRACTAL_RUNNER_BACKEND == "local":
+        WORKFLOW_DIR_USER = WORKFLOW_DIR
+    elif FRACTAL_RUNNER_BACKEND == "slurm":
+        WORKFLOW_DIR_USER = (
+            Path(user.cache_dir) / f"{WORKFLOW_DIR.name}"
+        ).resolve()
+
+    # Update job folders in the db
+    job.working_dir = WORKFLOW_DIR.as_posix()
+    job.working_dir_user = WORKFLOW_DIR_USER.as_posix()
+    await db.merge(job)
+    await db.commit()
+
     background_tasks.add_task(
         submit_workflow,
         workflow_id=workflow.id,
         dataset_id=dataset.id,
         job_id=job.id,
         worker_init=job.worker_init,
         slurm_user=user.slurm_user,
         user_cache_dir=user.cache_dir,
     )
 
     await db.close()
-
     return job
```

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/task.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/task.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from .....logger import set_logger
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models.v1 import Task as TaskV1
 from ....models.v2 import TaskV2
 from ....models.v2 import WorkflowTaskV2
+from ....models.v2 import WorkflowV2
 from ....schemas.v2 import TaskCreateV2
 from ....schemas.v2 import TaskReadV2
 from ....schemas.v2 import TaskUpdateV2
 from ....security import current_active_user
 from ....security import current_active_verified_user
 from ....security import User
 from ._aux_functions import _get_task_check_owner
@@ -200,23 +201,52 @@
     """
 
     db_task = await _get_task_check_owner(task_id=task_id, user=user, db=db)
 
     # Check that the TaskV2 is not in relationship with some WorkflowTaskV2
     stm = select(WorkflowTaskV2).filter(WorkflowTaskV2.task_id == task_id)
     res = await db.execute(stm)
-    workflowtask_list = res.scalars().all()
-    if workflowtask_list:
+    workflow_tasks = res.scalars().all()
+
+    if workflow_tasks:
+        # Find IDs of all affected workflows
+        workflow_ids = set(wftask.workflow_id for wftask in workflow_tasks)
+        # Fetch all affected workflows from DB
+        stm = select(WorkflowV2).where(WorkflowV2.id.in_(workflow_ids))
+        res = await db.execute(stm)
+        workflows = res.scalars().all()
+
+        # Find which workflows are associated to the current user
+        workflows_current_user = [
+            wf for wf in workflows if user in wf.project.user_list
+        ]
+        if workflows_current_user:
+            current_user_msg = (
+                "For the current-user workflows (listed below),"
+                " you can update the task or remove the workflows.\n"
+            )
+            current_user_msg += "\n".join(
+                [
+                    f"* '{wf.name}' (id={wf.id})"
+                    for wf in workflows_current_user
+                ]
+            )
+        else:
+            current_user_msg = ""
+
+        # Count workflows of current users or other users
+        num_workflows_current_user = len(workflows_current_user)
+        num_workflows_other_users = len(workflows) - num_workflows_current_user
+
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=(
-                f"Cannot remove TaskV2 {task_id} because it is currently "
-                "imported in WorkflowsV2 "
-                f"{[x.workflow_id for x in workflowtask_list]}. "
-                "If you want to remove this task, then you should first remove"
-                " the workflows.",
+                f"Cannot remove Task with id={task_id}: it is currently in "
+                f"use in {num_workflows_current_user} current-user workflows "
+                f"and in {num_workflows_other_users} other-users workflows.\n"
+                f"{current_user_msg}"
             ),
         )
 
     await db.delete(db_task)
     await db.commit()
     return Response(status_code=status.HTTP_204_NO_CONTENT)
```

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/task_collection.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/task_legacy.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/task_legacy.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/workflow.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/api/v2/workflowtask.py` & `fractal_server-2.0.5/fractal_server/app/routes/api/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/auth.py` & `fractal_server-2.0.5/fractal_server/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/aux/_job.py` & `fractal_server-2.0.5/fractal_server/app/routes/aux/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/routes/aux/_runner.py` & `fractal_server-2.0.5/fractal_server/app/routes/aux/_runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/async_wrap.py` & `fractal_server-2.0.5/fractal_server/app/runner/async_wrap.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/exceptions.py` & `fractal_server-2.0.5/fractal_server/app/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_batching.py` & `fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_check_jobs_status.py` & `fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_check_jobs_status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py` & `fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_slurm_config.py` & `fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py` & `fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/executor.py` & `fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/remote.py` & `fractal_server-2.0.5/fractal_server/app/runner/executors/slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/set_start_and_last_task_index.py` & `fractal_server-2.0.5/fractal_server/app/runner/set_start_and_last_task_index.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/task_files.py` & `fractal_server-2.0.5/fractal_server/app/runner/task_files.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/__init__.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/_common.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/_local/__init__.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/_local/_local_config.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/_local/_submit_setup.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/_local/executor.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/__init__.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/_submit_setup.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/get_slurm_config.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/common.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v1/handle_failed_job.py` & `fractal_server-2.0.5/fractal_server/app/runner/v1/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/__init__.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,53 +104,37 @@
             job.log = log_msg
             db_sync.merge(job)
             db_sync.commit()
             db_sync.close()
             return
 
         # Define and create server-side working folder
-        project_id = workflow.project_id
-        timestamp_string = get_timestamp().strftime("%Y%m%d_%H%M%S")
-        WORKFLOW_DIR = (
-            settings.FRACTAL_RUNNER_WORKING_BASE_DIR
-            / (
-                f"proj_{project_id:07d}_wf_{workflow_id:07d}_job_{job_id:07d}"
-                f"_{timestamp_string}"
-            )
-        ).resolve()
-
+        WORKFLOW_DIR = Path(job.working_dir)
         if WORKFLOW_DIR.exists():
-            raise RuntimeError(f"Workflow dir {WORKFLOW_DIR} already exists.")
+            job.status = JobStatusTypeV2.FAILED
+            job.end_timestamp = get_timestamp()
+            job.log = f"Workflow dir {WORKFLOW_DIR} already exists."
+            db_sync.merge(job)
+            db_sync.commit()
+            db_sync.close()
+            return
 
         # Create WORKFLOW_DIR with 755 permissions
         original_umask = os.umask(0)
         WORKFLOW_DIR.mkdir(parents=True, mode=0o755)
         os.umask(original_umask)
 
         # Define and create user-side working folder, if needed
-        if FRACTAL_RUNNER_BACKEND == "local":
-            WORKFLOW_DIR_USER = WORKFLOW_DIR
-        elif FRACTAL_RUNNER_BACKEND == "slurm":
-
+        WORKFLOW_DIR_USER = Path(job.working_dir_user)
+        if FRACTAL_RUNNER_BACKEND == "slurm":
             from ..executors.slurm._subprocess_run_as_user import (
                 _mkdir_as_user,
             )
 
-            WORKFLOW_DIR_USER = (
-                Path(user_cache_dir) / f"{WORKFLOW_DIR.name}"
-            ).resolve()
             _mkdir_as_user(folder=str(WORKFLOW_DIR_USER), user=slurm_user)
-        else:
-            raise ValueError(f"{FRACTAL_RUNNER_BACKEND=} not supported")
-
-        # Update db
-        job.working_dir = WORKFLOW_DIR.as_posix()
-        job.working_dir_user = WORKFLOW_DIR_USER.as_posix()
-        db_sync.merge(job)
-        db_sync.commit()
 
         # After Session.commit() is called, either explicitly or when using a
         # context manager, all objects associated with the Session are expired.
         # https://docs.sqlalchemy.org/en/14/orm/
         #   session_basics.html#opening-and-closing-a-session
         # https://docs.sqlalchemy.org/en/14/orm/
         #   session_state_management.html#refreshing-expiring
```

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/_local/__init__.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/_local/_local_config.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/_local/_submit_setup.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/_local/executor.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/__init__.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/_submit_setup.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/get_slurm_config.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/deduplicate_list.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/deduplicate_list.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/handle_failed_job.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/merge_outputs.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/merge_outputs.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/runner.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/runner_functions.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/runner_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/runner_functions_low_level.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/runner_functions_low_level.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/task_interface.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/task_interface.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/runner/v2/v1_compat.py` & `fractal_server-2.0.5/fractal_server/app/runner/v2/v1_compat.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/_validators.py` & `fractal_server-2.0.5/fractal_server/app/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/state.py` & `fractal_server-2.0.5/fractal_server/app/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/user.py` & `fractal_server-2.0.5/fractal_server/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/__init__.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/applyworkflow.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/dataset.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/dumps.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/manifest.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/project.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/task.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/task_collection.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v1/workflow.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/__init__.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/dataset.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/dumps.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/job.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/manifest.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/project.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/task.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/task_collection.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/workflow.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/schemas/v2/workflowtask.py` & `fractal_server-2.0.5/fractal_server/app/schemas/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/app/security/__init__.py` & `fractal_server-2.0.5/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/config.py` & `fractal_server-2.0.5/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/images/models.py` & `fractal_server-2.0.5/fractal_server/images/models.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/images/tools.py` & `fractal_server-2.0.5/fractal_server/images/tools.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/logger.py` & `fractal_server-2.0.5/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/main.py` & `fractal_server-2.0.5/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/env.py` & `fractal_server-2.0.5/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/script.py.mako` & `fractal_server-2.0.5/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/5bf02391cfef_v2.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/5bf02391cfef_v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-2.0.5/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/syringe.py` & `fractal_server-2.0.5/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/tasks/endpoint_operations.py` & `fractal_server-2.0.5/fractal_server/tasks/endpoint_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/tasks/utils.py` & `fractal_server-2.0.5/fractal_server/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/tasks/v1/_TaskCollectPip.py` & `fractal_server-2.0.5/fractal_server/tasks/v1/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/tasks/v1/background_operations.py` & `fractal_server-2.0.5/fractal_server/tasks/v1/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/tasks/v2/_TaskCollectPip.py` & `fractal_server-2.0.5/fractal_server/tasks/v2/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/tasks/v2/background_operations.py` & `fractal_server-2.0.5/fractal_server/tasks/v2/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/fractal_server/utils.py` & `fractal_server-2.0.5/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.4/pyproject.toml` & `fractal_server-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "2.0.4"
+version = "2.0.5"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Yuri Chiucconi <yuri.chiucconi@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
@@ -83,15 +83,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "2.0.4"
+current_version = "2.0.5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-2.0.4/PKG-INFO` & `fractal_server-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 2.0.4
+Version: 2.0.5
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

