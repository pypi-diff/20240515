# Comparing `tmp/wds_client-0.3.0.tar.gz` & `tmp/wds_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wds_client-0.3.0.tar", last modified: Mon May 13 14:06:37 2024, max compression
+gzip compressed data, was "wds_client-0.4.0.tar", last modified: Wed May 15 17:18:46 2024, max compression
```

## Comparing `wds_client-0.3.0.tar` & `wds_client-0.4.0.tar`

### file list

```diff
@@ -1,122 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.030501 wds_client-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 14:06:37.030501 wds_client-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-13 14:04:40.000000 wds_client-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 14:06:37.030501 wds_client-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-13 14:04:40.000000 wds_client-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.018501 wds_client-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_attribute_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_attribute_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_backup_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_backup_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_backup_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_backup_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_capabilities_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_clone_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_clone_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_clone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_db_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_generic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_generic_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_import_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_job_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_job_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.022501 wds_client-0.3.0/wds_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.022501 wds_client-0.3.0/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/capabilities_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17329 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/job_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    61562 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    34758 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26209 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.030501 wds_client-0.3.0/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/attribute_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/attribute_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/backup_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/backup_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/backup_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/backup_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/clone_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/clone_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/clone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/db_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/generic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/generic_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/import_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/job_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.030501 wds_client-0.3.0/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 14:06:36.000000 wds_client-0.3.0/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-13 14:06:37.000000 wds_client-0.3.0/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:06:36.000000 wds_client-0.3.0/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 14:06:36.000000 wds_client-0.3.0/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 14:06:36.000000 wds_client-0.3.0/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:18:46.060593 wds_client-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-15 17:18:46.060593 wds_client-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-05-15 17:17:15.000000 wds_client-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 17:18:46.064593 wds_client-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-15 17:17:15.000000 wds_client-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:18:46.052593 wds_client-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_attribute_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_attribute_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_capabilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_generic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_generic_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_import_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_job_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_job_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-15 17:17:15.000000 wds_client-0.4.0/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:18:46.052593 wds_client-0.4.0/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:18:46.056593 wds_client-0.4.0/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/capabilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17329 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/job_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61562 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34758 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26209 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:18:46.060593 wds_client-0.4.0/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/attribute_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/attribute_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/generic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/generic_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/import_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/job_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-05-15 17:17:15.000000 wds_client-0.4.0/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:18:46.060593 wds_client-0.4.0/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-15 17:18:46.000000 wds_client-0.4.0/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-15 17:18:46.000000 wds_client-0.4.0/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:18:46.000000 wds_client-0.4.0/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 17:18:46.000000 wds_client-0.4.0/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 17:18:46.000000 wds_client-0.4.0/wds_client.egg-info/top_level.txt
```

### Comparing `wds_client-0.3.0/README.md` & `wds_client-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This page lists current APIs.
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.3.0
+- Package version: 0.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -124,21 +124,14 @@
  - [BatchResponse](docs/BatchResponse.md)
  - [Build](docs/Build.md)
  - [Capabilities](docs/Capabilities.md)
  - [CloneJob](docs/CloneJob.md)
  - [CloneJobAllOf](docs/CloneJobAllOf.md)
  - [CloneResponse](docs/CloneResponse.md)
  - [Commit](docs/Commit.md)
- - [Component](docs/Component.md)
- - [Components](docs/Components.md)
- - [DbComponent](docs/DbComponent.md)
- - [DbValidationcomponent](docs/DbValidationcomponent.md)
- - [DbValidationcomponentDetails](docs/DbValidationcomponentDetails.md)
- - [DiskSpaceComponent](docs/DiskSpaceComponent.md)
- - [DiskSpaceComponentDetails](docs/DiskSpaceComponentDetails.md)
  - [ErrorResponse](docs/ErrorResponse.md)
  - [GenericJob](docs/GenericJob.md)
  - [GenericJobAllOf](docs/GenericJobAllOf.md)
  - [Git](docs/Git.md)
  - [ImportRequest](docs/ImportRequest.md)
  - [InlineObject](docs/InlineObject.md)
  - [Job](docs/Job.md)
```

### Comparing `wds_client-0.3.0/setup.py` & `wds_client-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wds-client"
-VERSION = "0.3.0"
+VERSION = "0.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wds_client-0.3.0/test/test_app.py` & `wds_client-0.4.0/test/test_app.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_attribute_data_type.py` & `wds_client-0.4.0/test/test_attribute_data_type.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_attribute_schema.py` & `wds_client-0.4.0/test/test_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_attribute_schema_update.py` & `wds_client-0.4.0/test/test_attribute_schema_update.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_backup_job.py` & `wds_client-0.4.0/test/test_backup_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_backup_job_all_of.py` & `wds_client-0.4.0/test/test_backup_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_backup_response.py` & `wds_client-0.4.0/test/test_backup_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_backup_restore_request.py` & `wds_client-0.4.0/test/test_backup_restore_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_batch_operation.py` & `wds_client-0.4.0/test/test_batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_batch_record_request.py` & `wds_client-0.4.0/test/test_batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_batch_response.py` & `wds_client-0.4.0/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_build.py` & `wds_client-0.4.0/test/test_build.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_capabilities.py` & `wds_client-0.4.0/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_capabilities_api.py` & `wds_client-0.4.0/test/test_capabilities_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_clone_job.py` & `wds_client-0.4.0/test/test_clone_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_clone_job_all_of.py` & `wds_client-0.4.0/test/test_clone_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_clone_response.py` & `wds_client-0.4.0/test/test_clone_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_cloning_api.py` & `wds_client-0.4.0/test/test_cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_commit.py` & `wds_client-0.4.0/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_component.py` & `wds_client-0.4.0/test/test_git.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,42 +12,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.component import Component  # noqa: E501
+from wds_client.models.git import Git  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestComponent(unittest.TestCase):
-    """Component unit test stubs"""
+class TestGit(unittest.TestCase):
+    """Git unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test Component
+        """Test Git
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.component.Component()  # noqa: E501
+        # model = wds_client.models.git.Git()  # noqa: E501
         if include_optional :
-            return Component(
-                status = '0', 
-                details = '0'
+            return Git(
+                branch = '0', 
+                commit = wds_client.models.commit.commit(
+                    id = '0', 
+                    time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
             )
         else :
-            return Component(
+            return Git(
         )
 
-    def testComponent(self):
-        """Test Component"""
+    def testGit(self):
+        """Test Git"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_db_component.py` & `wds_client-0.4.0/test/test_import_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,44 +12,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.db_component import DbComponent  # noqa: E501
+from wds_client.models.import_request import ImportRequest  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestDbComponent(unittest.TestCase):
-    """DbComponent unit test stubs"""
+class TestImportRequest(unittest.TestCase):
+    """ImportRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DbComponent
+        """Test ImportRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.db_component.DbComponent()  # noqa: E501
+        # model = wds_client.models.import_request.ImportRequest()  # noqa: E501
         if include_optional :
-            return DbComponent(
-                status = '0', 
-                components = wds_client.models.component.component(
-                    status = '0', 
-                    details = '0', )
+            return ImportRequest(
+                type = 'PFB', 
+                url = '0', 
+                options = { }
             )
         else :
-            return DbComponent(
+            return ImportRequest(
+                type = 'PFB',
+                url = '0',
         )
 
-    def testDbComponent(self):
-        """Test DbComponent"""
+    def testImportRequest(self):
+        """Test ImportRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_db_validationcomponent.py` & `wds_client-0.4.0/test/test_search_sort_direction.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,44 +12,40 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.db_validationcomponent import DbValidationcomponent  # noqa: E501
+from wds_client.models.search_sort_direction import SearchSortDirection  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestDbValidationcomponent(unittest.TestCase):
-    """DbValidationcomponent unit test stubs"""
+class TestSearchSortDirection(unittest.TestCase):
+    """SearchSortDirection unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DbValidationcomponent
+        """Test SearchSortDirection
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.db_validationcomponent.DbValidationcomponent()  # noqa: E501
+        # model = wds_client.models.search_sort_direction.SearchSortDirection()  # noqa: E501
         if include_optional :
-            return DbValidationcomponent(
-                status = '0', 
-                components = wds_client.models.db_validationcomponent_details.dbValidationcomponentDetails(
-                    database = '0', 
-                    validation_query = '0', )
+            return SearchSortDirection(
             )
         else :
-            return DbValidationcomponent(
+            return SearchSortDirection(
         )
 
-    def testDbValidationcomponent(self):
-        """Test DbValidationcomponent"""
+    def testSearchSortDirection(self):
+        """Test SearchSortDirection"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_db_validationcomponent_details.py` & `wds_client-0.4.0/test/test_generic_job_all_of.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.db_validationcomponent_details import DbValidationcomponentDetails  # noqa: E501
+from wds_client.models.generic_job_all_of import GenericJobAllOf  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestDbValidationcomponentDetails(unittest.TestCase):
-    """DbValidationcomponentDetails unit test stubs"""
+class TestGenericJobAllOf(unittest.TestCase):
+    """GenericJobAllOf unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DbValidationcomponentDetails
+        """Test GenericJobAllOf
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.db_validationcomponent_details.DbValidationcomponentDetails()  # noqa: E501
+        # model = wds_client.models.generic_job_all_of.GenericJobAllOf()  # noqa: E501
         if include_optional :
-            return DbValidationcomponentDetails(
-                database = '0', 
-                validation_query = '0'
+            return GenericJobAllOf(
+                input = None, 
+                result = None
             )
         else :
-            return DbValidationcomponentDetails(
+            return GenericJobAllOf(
         )
 
-    def testDbValidationcomponentDetails(self):
-        """Test DbValidationcomponentDetails"""
+    def testGenericJobAllOf(self):
+        """Test GenericJobAllOf"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_disk_space_component.py` & `wds_client-0.4.0/test/test_search_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,46 +12,48 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.disk_space_component import DiskSpaceComponent  # noqa: E501
+from wds_client.models.search_request import SearchRequest  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestDiskSpaceComponent(unittest.TestCase):
-    """DiskSpaceComponent unit test stubs"""
+class TestSearchRequest(unittest.TestCase):
+    """SearchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DiskSpaceComponent
+        """Test SearchRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.disk_space_component.DiskSpaceComponent()  # noqa: E501
+        # model = wds_client.models.search_request.SearchRequest()  # noqa: E501
         if include_optional :
-            return DiskSpaceComponent(
-                status = '0', 
-                details = wds_client.models.disk_space_component_details.diskSpaceComponentDetails(
-                    total = '0', 
-                    free = 1.337, 
-                    threshold = 1.337, 
-                    exists = True, )
+            return SearchRequest(
+                offset = 0, 
+                limit = 0, 
+                sort = 'ASC', 
+                sort_attribute = '0', 
+                filter = wds_client.models.search_filter.SearchFilter(
+                    ids = [
+                        '0'
+                        ], )
             )
         else :
-            return DiskSpaceComponent(
+            return SearchRequest(
         )
 
-    def testDiskSpaceComponent(self):
-        """Test DiskSpaceComponent"""
+    def testSearchRequest(self):
+        """Test SearchRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_error_response.py` & `wds_client-0.4.0/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_general_wds_information_api.py` & `wds_client-0.4.0/test/test_general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_generic_job.py` & `wds_client-0.4.0/test/test_generic_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_generic_job_all_of.py` & `wds_client-0.4.0/test/test_status_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.generic_job_all_of import GenericJobAllOf  # noqa: E501
+from wds_client.models.status_response import StatusResponse  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestGenericJobAllOf(unittest.TestCase):
-    """GenericJobAllOf unit test stubs"""
+class TestStatusResponse(unittest.TestCase):
+    """StatusResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GenericJobAllOf
+        """Test StatusResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.generic_job_all_of.GenericJobAllOf()  # noqa: E501
+        # model = wds_client.models.status_response.StatusResponse()  # noqa: E501
         if include_optional :
-            return GenericJobAllOf(
-                input = None, 
-                result = None
+            return StatusResponse(
+                status = '0', 
+                components = None
             )
         else :
-            return GenericJobAllOf(
+            return StatusResponse(
         )
 
-    def testGenericJobAllOf(self):
-        """Test GenericJobAllOf"""
+    def testStatusResponse(self):
+        """Test StatusResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_git.py` & `wds_client-0.4.0/test/test_inline_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,44 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.git import Git  # noqa: E501
+from wds_client.models.inline_object import InlineObject  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestGit(unittest.TestCase):
-    """Git unit test stubs"""
+class TestInlineObject(unittest.TestCase):
+    """InlineObject unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test Git
+        """Test InlineObject
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.git.Git()  # noqa: E501
+        # model = wds_client.models.inline_object.InlineObject()  # noqa: E501
         if include_optional :
-            return Git(
-                branch = '0', 
-                commit = wds_client.models.commit.commit(
-                    id = '0', 
-                    time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+            return InlineObject(
+                records = bytes(b'blah')
             )
         else :
-            return Git(
+            return InlineObject(
+                records = bytes(b'blah'),
         )
 
-    def testGit(self):
-        """Test Git"""
+    def testInlineObject(self):
+        """Test InlineObject"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_import_api.py` & `wds_client-0.4.0/test/test_import_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_import_request.py` & `wds_client-0.4.0/test/test_version_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,45 +12,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.import_request import ImportRequest  # noqa: E501
+from wds_client.models.version_response import VersionResponse  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestImportRequest(unittest.TestCase):
-    """ImportRequest unit test stubs"""
+class TestVersionResponse(unittest.TestCase):
+    """VersionResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ImportRequest
+        """Test VersionResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.import_request.ImportRequest()  # noqa: E501
+        # model = wds_client.models.version_response.VersionResponse()  # noqa: E501
         if include_optional :
-            return ImportRequest(
-                type = 'PFB', 
-                url = '0', 
-                options = { }
+            return VersionResponse(
+                app = wds_client.models.app.app(
+                    chart_version = '0', 
+                    image = '0', ), 
+                git = wds_client.models.git.git(
+                    branch = '0', 
+                    commit = wds_client.models.commit.commit(
+                        id = '0', 
+                        time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), ), 
+                build = wds_client.models.build.build(
+                    artifact = '0', 
+                    name = '0', 
+                    time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    version = '0', 
+                    group = '0', )
             )
         else :
-            return ImportRequest(
-                type = 'PFB',
-                url = '0',
+            return VersionResponse(
         )
 
-    def testImportRequest(self):
-        """Test ImportRequest"""
+    def testVersionResponse(self):
+        """Test VersionResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_inline_object.py` & `wds_client-0.4.0/test/test_tsv_upload_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,42 +12,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.inline_object import InlineObject  # noqa: E501
+from wds_client.models.tsv_upload_response import TsvUploadResponse  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestInlineObject(unittest.TestCase):
-    """InlineObject unit test stubs"""
+class TestTsvUploadResponse(unittest.TestCase):
+    """TsvUploadResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test InlineObject
+        """Test TsvUploadResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.inline_object.InlineObject()  # noqa: E501
+        # model = wds_client.models.tsv_upload_response.TsvUploadResponse()  # noqa: E501
         if include_optional :
-            return InlineObject(
-                records = bytes(b'blah')
+            return TsvUploadResponse(
+                message = '0', 
+                records_modified = 56
             )
         else :
-            return InlineObject(
-                records = bytes(b'blah'),
+            return TsvUploadResponse(
+                message = '0',
+                records_modified = 56,
         )
 
-    def testInlineObject(self):
-        """Test InlineObject"""
+    def testTsvUploadResponse(self):
+        """Test TsvUploadResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds_client-0.3.0/test/test_instances_api.py` & `wds_client-0.4.0/test/test_instances_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_job.py` & `wds_client-0.4.0/test/test_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_job_api.py` & `wds_client-0.4.0/test/test_job_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_job_v1.py` & `wds_client-0.4.0/test/test_job_v1.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_record_query_response.py` & `wds_client-0.4.0/test/test_record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_record_request.py` & `wds_client-0.4.0/test/test_record_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_record_response.py` & `wds_client-0.4.0/test/test_record_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_record_type_schema.py` & `wds_client-0.4.0/test/test_record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_records_api.py` & `wds_client-0.4.0/test/test_records_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_schema_api.py` & `wds_client-0.4.0/test/test_schema_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/test/test_search_filter.py` & `wds_client-0.4.0/test/test_search_filter.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/__init__.py` & `wds_client-0.4.0/wds_client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 # import apis into sdk package
 from wds_client.api.capabilities_api import CapabilitiesApi
 from wds_client.api.cloning_api import CloningApi
 from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
 from wds_client.api.import_api import ImportApi
 from wds_client.api.instances_api import InstancesApi
@@ -48,21 +48,14 @@
 from wds_client.models.batch_response import BatchResponse
 from wds_client.models.build import Build
 from wds_client.models.capabilities import Capabilities
 from wds_client.models.clone_job import CloneJob
 from wds_client.models.clone_job_all_of import CloneJobAllOf
 from wds_client.models.clone_response import CloneResponse
 from wds_client.models.commit import Commit
-from wds_client.models.component import Component
-from wds_client.models.components import Components
-from wds_client.models.db_component import DbComponent
-from wds_client.models.db_validationcomponent import DbValidationcomponent
-from wds_client.models.db_validationcomponent_details import DbValidationcomponentDetails
-from wds_client.models.disk_space_component import DiskSpaceComponent
-from wds_client.models.disk_space_component_details import DiskSpaceComponentDetails
 from wds_client.models.error_response import ErrorResponse
 from wds_client.models.generic_job import GenericJob
 from wds_client.models.generic_job_all_of import GenericJobAllOf
 from wds_client.models.git import Git
 from wds_client.models.import_request import ImportRequest
 from wds_client.models.inline_object import InlineObject
 from wds_client.models.job import Job
```

### Comparing `wds_client-0.3.0/wds_client/api/__init__.py` & `wds_client-0.4.0/wds_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api/capabilities_api.py` & `wds_client-0.4.0/wds_client/api/capabilities_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api/cloning_api.py` & `wds_client-0.4.0/wds_client/api/cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api/general_wds_information_api.py` & `wds_client-0.4.0/wds_client/api/general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api/import_api.py` & `wds_client-0.4.0/wds_client/api/import_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api/instances_api.py` & `wds_client-0.4.0/wds_client/api/instances_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api/job_api.py` & `wds_client-0.4.0/wds_client/api/job_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api/records_api.py` & `wds_client-0.4.0/wds_client/api/records_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api/schema_api.py` & `wds_client-0.4.0/wds_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/api_client.py` & `wds_client-0.4.0/wds_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'wds-client/0.3.0/python'
+        self.user_agent = 'wds-client/0.4.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds_client-0.3.0/wds_client/configuration.py` & `wds_client-0.4.0/wds_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.3.0".\
+               "SDK Package Version: 0.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds_client-0.3.0/wds_client/exceptions.py` & `wds_client-0.4.0/wds_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/__init__.py` & `wds_client-0.4.0/wds_client/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,21 +27,14 @@
 from wds_client.models.batch_response import BatchResponse
 from wds_client.models.build import Build
 from wds_client.models.capabilities import Capabilities
 from wds_client.models.clone_job import CloneJob
 from wds_client.models.clone_job_all_of import CloneJobAllOf
 from wds_client.models.clone_response import CloneResponse
 from wds_client.models.commit import Commit
-from wds_client.models.component import Component
-from wds_client.models.components import Components
-from wds_client.models.db_component import DbComponent
-from wds_client.models.db_validationcomponent import DbValidationcomponent
-from wds_client.models.db_validationcomponent_details import DbValidationcomponentDetails
-from wds_client.models.disk_space_component import DiskSpaceComponent
-from wds_client.models.disk_space_component_details import DiskSpaceComponentDetails
 from wds_client.models.error_response import ErrorResponse
 from wds_client.models.generic_job import GenericJob
 from wds_client.models.generic_job_all_of import GenericJobAllOf
 from wds_client.models.git import Git
 from wds_client.models.import_request import ImportRequest
 from wds_client.models.inline_object import InlineObject
 from wds_client.models.job import Job
```

### Comparing `wds_client-0.3.0/wds_client/models/app.py` & `wds_client-0.4.0/wds_client/models/app.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/attribute_data_type.py` & `wds_client-0.4.0/wds_client/models/attribute_data_type.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/attribute_schema.py` & `wds_client-0.4.0/wds_client/models/attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/attribute_schema_update.py` & `wds_client-0.4.0/wds_client/models/attribute_schema_update.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/backup_job.py` & `wds_client-0.4.0/wds_client/models/backup_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/backup_job_all_of.py` & `wds_client-0.4.0/wds_client/models/backup_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/backup_response.py` & `wds_client-0.4.0/wds_client/models/backup_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/backup_restore_request.py` & `wds_client-0.4.0/wds_client/models/backup_restore_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/batch_operation.py` & `wds_client-0.4.0/wds_client/models/batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/batch_record_request.py` & `wds_client-0.4.0/wds_client/models/batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/batch_response.py` & `wds_client-0.4.0/wds_client/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/build.py` & `wds_client-0.4.0/wds_client/models/build.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/capabilities.py` & `wds_client-0.4.0/wds_client/models/capabilities.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/clone_job.py` & `wds_client-0.4.0/wds_client/models/clone_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/clone_job_all_of.py` & `wds_client-0.4.0/wds_client/models/clone_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/clone_response.py` & `wds_client-0.4.0/wds_client/models/clone_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/commit.py` & `wds_client-0.4.0/wds_client/models/commit.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/component.py` & `wds_client-0.4.0/wds_client/models/status_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class Component(object):
+class StatusResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,78 +30,78 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'status': 'str',
-        'details': 'str'
+        'components': 'object'
     }
 
     attribute_map = {
         'status': 'status',
-        'details': 'details'
+        'components': 'components'
     }
 
-    def __init__(self, status=None, details=None, local_vars_configuration=None):  # noqa: E501
-        """Component - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, status=None, components=None, local_vars_configuration=None):  # noqa: E501
+        """StatusResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._status = None
-        self._details = None
+        self._components = None
         self.discriminator = None
 
         if status is not None:
             self.status = status
-        if details is not None:
-            self.details = details
+        if components is not None:
+            self.components = components
 
     @property
     def status(self):
-        """Gets the status of this Component.  # noqa: E501
+        """Gets the status of this StatusResponse.  # noqa: E501
 
 
-        :return: The status of this Component.  # noqa: E501
+        :return: The status of this StatusResponse.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this Component.
+        """Sets the status of this StatusResponse.
 
 
-        :param status: The status of this Component.  # noqa: E501
+        :param status: The status of this StatusResponse.  # noqa: E501
         :type: str
         """
 
         self._status = status
 
     @property
-    def details(self):
-        """Gets the details of this Component.  # noqa: E501
+    def components(self):
+        """Gets the components of this StatusResponse.  # noqa: E501
 
 
-        :return: The details of this Component.  # noqa: E501
-        :rtype: str
+        :return: The components of this StatusResponse.  # noqa: E501
+        :rtype: object
         """
-        return self._details
+        return self._components
 
-    @details.setter
-    def details(self, details):
-        """Sets the details of this Component.
+    @components.setter
+    def components(self, components):
+        """Sets the components of this StatusResponse.
 
 
-        :param details: The details of this Component.  # noqa: E501
-        :type: str
+        :param components: The components of this StatusResponse.  # noqa: E501
+        :type: object
         """
 
-        self._details = details
+        self._components = components
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -129,18 +129,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Component):
+        if not isinstance(other, StatusResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Component):
+        if not isinstance(other, StatusResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/components.py` & `wds_client-0.4.0/wds_client/models/import_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,146 +14,134 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class Components(object):
+class ImportRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'db': 'DbComponent',
-        'disk_space': 'DiskSpaceComponent',
-        'ping': 'Component',
-        'main_db': 'DbValidationcomponent'
+        'type': 'str',
+        'url': 'str',
+        'options': 'dict(str, object)'
     }
 
     attribute_map = {
-        'db': 'db',
-        'disk_space': 'diskSpace',
-        'ping': 'ping',
-        'main_db': 'mainDb'
+        'type': 'type',
+        'url': 'url',
+        'options': 'options'
     }
 
-    def __init__(self, db=None, disk_space=None, ping=None, main_db=None, local_vars_configuration=None):  # noqa: E501
-        """Components - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, type=None, url=None, options=None, local_vars_configuration=None):  # noqa: E501
+        """ImportRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._db = None
-        self._disk_space = None
-        self._ping = None
-        self._main_db = None
+        self._type = None
+        self._url = None
+        self._options = None
         self.discriminator = None
 
-        if db is not None:
-            self.db = db
-        if disk_space is not None:
-            self.disk_space = disk_space
-        if ping is not None:
-            self.ping = ping
-        if main_db is not None:
-            self.main_db = main_db
+        self.type = type
+        self.url = url
+        if options is not None:
+            self.options = options
 
     @property
-    def db(self):
-        """Gets the db of this Components.  # noqa: E501
+    def type(self):
+        """Gets the type of this ImportRequest.  # noqa: E501
 
+        format of file to import  # noqa: E501
 
-        :return: The db of this Components.  # noqa: E501
-        :rtype: DbComponent
+        :return: The type of this ImportRequest.  # noqa: E501
+        :rtype: str
         """
-        return self._db
+        return self._type
 
-    @db.setter
-    def db(self, db):
-        """Sets the db of this Components.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ImportRequest.
 
+        format of file to import  # noqa: E501
 
-        :param db: The db of this Components.  # noqa: E501
-        :type: DbComponent
+        :param type: The type of this ImportRequest.  # noqa: E501
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        allowed_values = ["PFB", "RAWLSJSON", "TDRMANIFEST"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
-        self._db = db
+        self._type = type
 
     @property
-    def disk_space(self):
-        """Gets the disk_space of this Components.  # noqa: E501
+    def url(self):
+        """Gets the url of this ImportRequest.  # noqa: E501
 
+        url from which to import  # noqa: E501
 
-        :return: The disk_space of this Components.  # noqa: E501
-        :rtype: DiskSpaceComponent
+        :return: The url of this ImportRequest.  # noqa: E501
+        :rtype: str
         """
-        return self._disk_space
+        return self._url
 
-    @disk_space.setter
-    def disk_space(self, disk_space):
-        """Sets the disk_space of this Components.
+    @url.setter
+    def url(self, url):
+        """Sets the url of this ImportRequest.
 
+        url from which to import  # noqa: E501
 
-        :param disk_space: The disk_space of this Components.  # noqa: E501
-        :type: DiskSpaceComponent
+        :param url: The url of this ImportRequest.  # noqa: E501
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and url is None:  # noqa: E501
+            raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
 
-        self._disk_space = disk_space
+        self._url = url
 
     @property
-    def ping(self):
-        """Gets the ping of this Components.  # noqa: E501
+    def options(self):
+        """Gets the options of this ImportRequest.  # noqa: E501
 
+        key-value pairs to configure this import. Options vary based on the import file type.  # noqa: E501
 
-        :return: The ping of this Components.  # noqa: E501
-        :rtype: Component
+        :return: The options of this ImportRequest.  # noqa: E501
+        :rtype: dict(str, object)
         """
-        return self._ping
+        return self._options
 
-    @ping.setter
-    def ping(self, ping):
-        """Sets the ping of this Components.
+    @options.setter
+    def options(self, options):
+        """Sets the options of this ImportRequest.
 
+        key-value pairs to configure this import. Options vary based on the import file type.  # noqa: E501
 
-        :param ping: The ping of this Components.  # noqa: E501
-        :type: Component
+        :param options: The options of this ImportRequest.  # noqa: E501
+        :type: dict(str, object)
         """
 
-        self._ping = ping
-
-    @property
-    def main_db(self):
-        """Gets the main_db of this Components.  # noqa: E501
-
-
-        :return: The main_db of this Components.  # noqa: E501
-        :rtype: DbValidationcomponent
-        """
-        return self._main_db
-
-    @main_db.setter
-    def main_db(self, main_db):
-        """Sets the main_db of this Components.
-
-
-        :param main_db: The main_db of this Components.  # noqa: E501
-        :type: DbValidationcomponent
-        """
-
-        self._main_db = main_db
+        self._options = options
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -181,18 +169,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Components):
+        if not isinstance(other, ImportRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Components):
+        if not isinstance(other, ImportRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/db_component.py` & `wds_client-0.4.0/wds_client/models/version_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,94 +14,120 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class DbComponent(object):
+class VersionResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'status': 'str',
-        'components': 'Component'
+        'app': 'App',
+        'git': 'Git',
+        'build': 'Build'
     }
 
     attribute_map = {
-        'status': 'status',
-        'components': 'components'
+        'app': 'app',
+        'git': 'git',
+        'build': 'build'
     }
 
-    def __init__(self, status=None, components=None, local_vars_configuration=None):  # noqa: E501
-        """DbComponent - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, app=None, git=None, build=None, local_vars_configuration=None):  # noqa: E501
+        """VersionResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._status = None
-        self._components = None
+        self._app = None
+        self._git = None
+        self._build = None
         self.discriminator = None
 
-        if status is not None:
-            self.status = status
-        if components is not None:
-            self.components = components
+        if app is not None:
+            self.app = app
+        if git is not None:
+            self.git = git
+        if build is not None:
+            self.build = build
 
     @property
-    def status(self):
-        """Gets the status of this DbComponent.  # noqa: E501
+    def app(self):
+        """Gets the app of this VersionResponse.  # noqa: E501
 
 
-        :return: The status of this DbComponent.  # noqa: E501
-        :rtype: str
+        :return: The app of this VersionResponse.  # noqa: E501
+        :rtype: App
         """
-        return self._status
+        return self._app
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this DbComponent.
+    @app.setter
+    def app(self, app):
+        """Sets the app of this VersionResponse.
 
 
-        :param status: The status of this DbComponent.  # noqa: E501
-        :type: str
+        :param app: The app of this VersionResponse.  # noqa: E501
+        :type: App
         """
 
-        self._status = status
+        self._app = app
 
     @property
-    def components(self):
-        """Gets the components of this DbComponent.  # noqa: E501
+    def git(self):
+        """Gets the git of this VersionResponse.  # noqa: E501
 
 
-        :return: The components of this DbComponent.  # noqa: E501
-        :rtype: Component
+        :return: The git of this VersionResponse.  # noqa: E501
+        :rtype: Git
         """
-        return self._components
+        return self._git
 
-    @components.setter
-    def components(self, components):
-        """Sets the components of this DbComponent.
+    @git.setter
+    def git(self, git):
+        """Sets the git of this VersionResponse.
 
 
-        :param components: The components of this DbComponent.  # noqa: E501
-        :type: Component
+        :param git: The git of this VersionResponse.  # noqa: E501
+        :type: Git
         """
 
-        self._components = components
+        self._git = git
+
+    @property
+    def build(self):
+        """Gets the build of this VersionResponse.  # noqa: E501
+
+
+        :return: The build of this VersionResponse.  # noqa: E501
+        :rtype: Build
+        """
+        return self._build
+
+    @build.setter
+    def build(self, build):
+        """Sets the build of this VersionResponse.
+
+
+        :param build: The build of this VersionResponse.  # noqa: E501
+        :type: Build
+        """
+
+        self._build = build
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -129,18 +155,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DbComponent):
+        if not isinstance(other, VersionResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DbComponent):
+        if not isinstance(other, VersionResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/db_validationcomponent.py` & `wds_client-0.4.0/wds_client/models/generic_job_all_of.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,94 +14,98 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class DbValidationcomponent(object):
+class GenericJobAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'status': 'str',
-        'components': 'DbValidationcomponentDetails'
+        'input': 'object',
+        'result': 'object'
     }
 
     attribute_map = {
-        'status': 'status',
-        'components': 'components'
+        'input': 'input',
+        'result': 'result'
     }
 
-    def __init__(self, status=None, components=None, local_vars_configuration=None):  # noqa: E501
-        """DbValidationcomponent - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, input=None, result=None, local_vars_configuration=None):  # noqa: E501
+        """GenericJobAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._status = None
-        self._components = None
+        self._input = None
+        self._result = None
         self.discriminator = None
 
-        if status is not None:
-            self.status = status
-        if components is not None:
-            self.components = components
+        if input is not None:
+            self.input = input
+        if result is not None:
+            self.result = result
 
     @property
-    def status(self):
-        """Gets the status of this DbValidationcomponent.  # noqa: E501
+    def input(self):
+        """Gets the input of this GenericJobAllOf.  # noqa: E501
 
+        Input arguments for this job  # noqa: E501
 
-        :return: The status of this DbValidationcomponent.  # noqa: E501
-        :rtype: str
+        :return: The input of this GenericJobAllOf.  # noqa: E501
+        :rtype: object
         """
-        return self._status
+        return self._input
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this DbValidationcomponent.
+    @input.setter
+    def input(self, input):
+        """Sets the input of this GenericJobAllOf.
 
+        Input arguments for this job  # noqa: E501
 
-        :param status: The status of this DbValidationcomponent.  # noqa: E501
-        :type: str
+        :param input: The input of this GenericJobAllOf.  # noqa: E501
+        :type: object
         """
 
-        self._status = status
+        self._input = input
 
     @property
-    def components(self):
-        """Gets the components of this DbValidationcomponent.  # noqa: E501
+    def result(self):
+        """Gets the result of this GenericJobAllOf.  # noqa: E501
 
+        Result of this job  # noqa: E501
 
-        :return: The components of this DbValidationcomponent.  # noqa: E501
-        :rtype: DbValidationcomponentDetails
+        :return: The result of this GenericJobAllOf.  # noqa: E501
+        :rtype: object
         """
-        return self._components
+        return self._result
 
-    @components.setter
-    def components(self, components):
-        """Sets the components of this DbValidationcomponent.
+    @result.setter
+    def result(self, result):
+        """Sets the result of this GenericJobAllOf.
 
+        Result of this job  # noqa: E501
 
-        :param components: The components of this DbValidationcomponent.  # noqa: E501
-        :type: DbValidationcomponentDetails
+        :param result: The result of this GenericJobAllOf.  # noqa: E501
+        :type: object
         """
 
-        self._components = components
+        self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -129,18 +133,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DbValidationcomponent):
+        if not isinstance(other, GenericJobAllOf):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DbValidationcomponent):
+        if not isinstance(other, GenericJobAllOf):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/disk_space_component_details.py` & `wds_client-0.4.0/wds_client/models/record_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,146 +14,129 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class DiskSpaceComponentDetails(object):
+class RecordResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'total': 'str',
-        'free': 'float',
-        'threshold': 'float',
-        'exists': 'bool'
+        'id': 'str',
+        'type': 'str',
+        'attributes': 'dict(str, object)'
     }
 
     attribute_map = {
-        'total': 'total',
-        'free': 'free',
-        'threshold': 'threshold',
-        'exists': 'exists'
+        'id': 'id',
+        'type': 'type',
+        'attributes': 'attributes'
     }
 
-    def __init__(self, total=None, free=None, threshold=None, exists=None, local_vars_configuration=None):  # noqa: E501
-        """DiskSpaceComponentDetails - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, type=None, attributes=None, local_vars_configuration=None):  # noqa: E501
+        """RecordResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._total = None
-        self._free = None
-        self._threshold = None
-        self._exists = None
+        self._id = None
+        self._type = None
+        self._attributes = None
         self.discriminator = None
 
-        if total is not None:
-            self.total = total
-        if free is not None:
-            self.free = free
-        if threshold is not None:
-            self.threshold = threshold
-        if exists is not None:
-            self.exists = exists
+        self.id = id
+        self.type = type
+        self.attributes = attributes
 
     @property
-    def total(self):
-        """Gets the total of this DiskSpaceComponentDetails.  # noqa: E501
+    def id(self):
+        """Gets the id of this RecordResponse.  # noqa: E501
 
+        Record id  # noqa: E501
 
-        :return: The total of this DiskSpaceComponentDetails.  # noqa: E501
+        :return: The id of this RecordResponse.  # noqa: E501
         :rtype: str
         """
-        return self._total
+        return self._id
 
-    @total.setter
-    def total(self, total):
-        """Sets the total of this DiskSpaceComponentDetails.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this RecordResponse.
 
+        Record id  # noqa: E501
 
-        :param total: The total of this DiskSpaceComponentDetails.  # noqa: E501
+        :param id: The id of this RecordResponse.  # noqa: E501
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
-        self._total = total
+        self._id = id
 
     @property
-    def free(self):
-        """Gets the free of this DiskSpaceComponentDetails.  # noqa: E501
+    def type(self):
+        """Gets the type of this RecordResponse.  # noqa: E501
 
+        Record type  # noqa: E501
 
-        :return: The free of this DiskSpaceComponentDetails.  # noqa: E501
-        :rtype: float
-        """
-        return self._free
-
-    @free.setter
-    def free(self, free):
-        """Sets the free of this DiskSpaceComponentDetails.
-
-
-        :param free: The free of this DiskSpaceComponentDetails.  # noqa: E501
-        :type: float
-        """
-
-        self._free = free
-
-    @property
-    def threshold(self):
-        """Gets the threshold of this DiskSpaceComponentDetails.  # noqa: E501
-
-
-        :return: The threshold of this DiskSpaceComponentDetails.  # noqa: E501
-        :rtype: float
+        :return: The type of this RecordResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._threshold
+        return self._type
 
-    @threshold.setter
-    def threshold(self, threshold):
-        """Sets the threshold of this DiskSpaceComponentDetails.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this RecordResponse.
 
+        Record type  # noqa: E501
 
-        :param threshold: The threshold of this DiskSpaceComponentDetails.  # noqa: E501
-        :type: float
+        :param type: The type of this RecordResponse.  # noqa: E501
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
-        self._threshold = threshold
+        self._type = type
 
     @property
-    def exists(self):
-        """Gets the exists of this DiskSpaceComponentDetails.  # noqa: E501
+    def attributes(self):
+        """Gets the attributes of this RecordResponse.  # noqa: E501
 
+        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
-        :return: The exists of this DiskSpaceComponentDetails.  # noqa: E501
-        :rtype: bool
+        :return: The attributes of this RecordResponse.  # noqa: E501
+        :rtype: dict(str, object)
         """
-        return self._exists
+        return self._attributes
 
-    @exists.setter
-    def exists(self, exists):
-        """Sets the exists of this DiskSpaceComponentDetails.
+    @attributes.setter
+    def attributes(self, attributes):
+        """Sets the attributes of this RecordResponse.
 
+        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
-        :param exists: The exists of this DiskSpaceComponentDetails.  # noqa: E501
-        :type: bool
+        :param attributes: The attributes of this RecordResponse.  # noqa: E501
+        :type: dict(str, object)
         """
+        if self.local_vars_configuration.client_side_validation and attributes is None:  # noqa: E501
+            raise ValueError("Invalid value for `attributes`, must not be `None`")  # noqa: E501
 
-        self._exists = exists
+        self._attributes = attributes
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -181,18 +164,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DiskSpaceComponentDetails):
+        if not isinstance(other, RecordResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DiskSpaceComponentDetails):
+        if not isinstance(other, RecordResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/error_response.py` & `wds_client-0.4.0/wds_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/generic_job.py` & `wds_client-0.4.0/wds_client/models/generic_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/generic_job_all_of.py` & `wds_client-0.4.0/wds_client/models/git.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,98 +14,94 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class GenericJobAllOf(object):
+class Git(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'input': 'object',
-        'result': 'object'
+        'branch': 'str',
+        'commit': 'Commit'
     }
 
     attribute_map = {
-        'input': 'input',
-        'result': 'result'
+        'branch': 'branch',
+        'commit': 'commit'
     }
 
-    def __init__(self, input=None, result=None, local_vars_configuration=None):  # noqa: E501
-        """GenericJobAllOf - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, branch=None, commit=None, local_vars_configuration=None):  # noqa: E501
+        """Git - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._input = None
-        self._result = None
+        self._branch = None
+        self._commit = None
         self.discriminator = None
 
-        if input is not None:
-            self.input = input
-        if result is not None:
-            self.result = result
+        if branch is not None:
+            self.branch = branch
+        if commit is not None:
+            self.commit = commit
 
     @property
-    def input(self):
-        """Gets the input of this GenericJobAllOf.  # noqa: E501
+    def branch(self):
+        """Gets the branch of this Git.  # noqa: E501
 
-        Input arguments for this job  # noqa: E501
 
-        :return: The input of this GenericJobAllOf.  # noqa: E501
-        :rtype: object
+        :return: The branch of this Git.  # noqa: E501
+        :rtype: str
         """
-        return self._input
+        return self._branch
 
-    @input.setter
-    def input(self, input):
-        """Sets the input of this GenericJobAllOf.
+    @branch.setter
+    def branch(self, branch):
+        """Sets the branch of this Git.
 
-        Input arguments for this job  # noqa: E501
 
-        :param input: The input of this GenericJobAllOf.  # noqa: E501
-        :type: object
+        :param branch: The branch of this Git.  # noqa: E501
+        :type: str
         """
 
-        self._input = input
+        self._branch = branch
 
     @property
-    def result(self):
-        """Gets the result of this GenericJobAllOf.  # noqa: E501
+    def commit(self):
+        """Gets the commit of this Git.  # noqa: E501
 
-        Result of this job  # noqa: E501
 
-        :return: The result of this GenericJobAllOf.  # noqa: E501
-        :rtype: object
+        :return: The commit of this Git.  # noqa: E501
+        :rtype: Commit
         """
-        return self._result
+        return self._commit
 
-    @result.setter
-    def result(self, result):
-        """Sets the result of this GenericJobAllOf.
+    @commit.setter
+    def commit(self, commit):
+        """Sets the commit of this Git.
 
-        Result of this job  # noqa: E501
 
-        :param result: The result of this GenericJobAllOf.  # noqa: E501
-        :type: object
+        :param commit: The commit of this Git.  # noqa: E501
+        :type: Commit
         """
 
-        self._result = result
+        self._commit = commit
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -133,18 +129,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GenericJobAllOf):
+        if not isinstance(other, Git):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, GenericJobAllOf):
+        if not isinstance(other, Git):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/git.py` & `wds_client-0.4.0/wds_client/models/search_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,94 +14,70 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class Git(object):
+class SearchFilter(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'branch': 'str',
-        'commit': 'Commit'
+        'ids': 'list[str]'
     }
 
     attribute_map = {
-        'branch': 'branch',
-        'commit': 'commit'
+        'ids': 'ids'
     }
 
-    def __init__(self, branch=None, commit=None, local_vars_configuration=None):  # noqa: E501
-        """Git - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, ids=None, local_vars_configuration=None):  # noqa: E501
+        """SearchFilter - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._branch = None
-        self._commit = None
+        self._ids = None
         self.discriminator = None
 
-        if branch is not None:
-            self.branch = branch
-        if commit is not None:
-            self.commit = commit
+        if ids is not None:
+            self.ids = ids
 
     @property
-    def branch(self):
-        """Gets the branch of this Git.  # noqa: E501
+    def ids(self):
+        """Gets the ids of this SearchFilter.  # noqa: E501
 
+        Record ids by which to filter the query  # noqa: E501
 
-        :return: The branch of this Git.  # noqa: E501
-        :rtype: str
+        :return: The ids of this SearchFilter.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._branch
+        return self._ids
 
-    @branch.setter
-    def branch(self, branch):
-        """Sets the branch of this Git.
+    @ids.setter
+    def ids(self, ids):
+        """Sets the ids of this SearchFilter.
 
+        Record ids by which to filter the query  # noqa: E501
 
-        :param branch: The branch of this Git.  # noqa: E501
-        :type: str
+        :param ids: The ids of this SearchFilter.  # noqa: E501
+        :type: list[str]
         """
 
-        self._branch = branch
-
-    @property
-    def commit(self):
-        """Gets the commit of this Git.  # noqa: E501
-
-
-        :return: The commit of this Git.  # noqa: E501
-        :rtype: Commit
-        """
-        return self._commit
-
-    @commit.setter
-    def commit(self, commit):
-        """Sets the commit of this Git.
-
-
-        :param commit: The commit of this Git.  # noqa: E501
-        :type: Commit
-        """
-
-        self._commit = commit
+        self._ids = ids
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -129,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Git):
+        if not isinstance(other, SearchFilter):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Git):
+        if not isinstance(other, SearchFilter):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/import_request.py` & `wds_client-0.4.0/wds_client/models/record_query_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,134 +14,127 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class ImportRequest(object):
+class RecordQueryResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'type': 'str',
-        'url': 'str',
-        'options': 'dict(str, object)'
+        'search_request': 'SearchRequest',
+        'total_records': 'int',
+        'records': 'list[RecordResponse]'
     }
 
     attribute_map = {
-        'type': 'type',
-        'url': 'url',
-        'options': 'options'
+        'search_request': 'searchRequest',
+        'total_records': 'totalRecords',
+        'records': 'records'
     }
 
-    def __init__(self, type=None, url=None, options=None, local_vars_configuration=None):  # noqa: E501
-        """ImportRequest - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, search_request=None, total_records=None, records=None, local_vars_configuration=None):  # noqa: E501
+        """RecordQueryResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
-        self._url = None
-        self._options = None
+        self._search_request = None
+        self._total_records = None
+        self._records = None
         self.discriminator = None
 
-        self.type = type
-        self.url = url
-        if options is not None:
-            self.options = options
+        self.search_request = search_request
+        self.total_records = total_records
+        self.records = records
 
     @property
-    def type(self):
-        """Gets the type of this ImportRequest.  # noqa: E501
+    def search_request(self):
+        """Gets the search_request of this RecordQueryResponse.  # noqa: E501
 
-        format of file to import  # noqa: E501
 
-        :return: The type of this ImportRequest.  # noqa: E501
-        :rtype: str
+        :return: The search_request of this RecordQueryResponse.  # noqa: E501
+        :rtype: SearchRequest
         """
-        return self._type
+        return self._search_request
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this ImportRequest.
+    @search_request.setter
+    def search_request(self, search_request):
+        """Sets the search_request of this RecordQueryResponse.
 
-        format of file to import  # noqa: E501
 
-        :param type: The type of this ImportRequest.  # noqa: E501
-        :type: str
+        :param search_request: The search_request of this RecordQueryResponse.  # noqa: E501
+        :type: SearchRequest
         """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["PFB", "RAWLSJSON", "TDRMANIFEST"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
-                .format(type, allowed_values)
-            )
+        if self.local_vars_configuration.client_side_validation and search_request is None:  # noqa: E501
+            raise ValueError("Invalid value for `search_request`, must not be `None`")  # noqa: E501
 
-        self._type = type
+        self._search_request = search_request
 
     @property
-    def url(self):
-        """Gets the url of this ImportRequest.  # noqa: E501
+    def total_records(self):
+        """Gets the total_records of this RecordQueryResponse.  # noqa: E501
 
-        url from which to import  # noqa: E501
+        number of records in the record type  # noqa: E501
 
-        :return: The url of this ImportRequest.  # noqa: E501
-        :rtype: str
+        :return: The total_records of this RecordQueryResponse.  # noqa: E501
+        :rtype: int
         """
-        return self._url
+        return self._total_records
 
-    @url.setter
-    def url(self, url):
-        """Sets the url of this ImportRequest.
+    @total_records.setter
+    def total_records(self, total_records):
+        """Sets the total_records of this RecordQueryResponse.
 
-        url from which to import  # noqa: E501
+        number of records in the record type  # noqa: E501
 
-        :param url: The url of this ImportRequest.  # noqa: E501
-        :type: str
+        :param total_records: The total_records of this RecordQueryResponse.  # noqa: E501
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and url is None:  # noqa: E501
-            raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and total_records is None:  # noqa: E501
+            raise ValueError("Invalid value for `total_records`, must not be `None`")  # noqa: E501
 
-        self._url = url
+        self._total_records = total_records
 
     @property
-    def options(self):
-        """Gets the options of this ImportRequest.  # noqa: E501
+    def records(self):
+        """Gets the records of this RecordQueryResponse.  # noqa: E501
 
-        key-value pairs to configure this import. Options vary based on the import file type.  # noqa: E501
+        list of records found  # noqa: E501
 
-        :return: The options of this ImportRequest.  # noqa: E501
-        :rtype: dict(str, object)
+        :return: The records of this RecordQueryResponse.  # noqa: E501
+        :rtype: list[RecordResponse]
         """
-        return self._options
+        return self._records
 
-    @options.setter
-    def options(self, options):
-        """Sets the options of this ImportRequest.
+    @records.setter
+    def records(self, records):
+        """Sets the records of this RecordQueryResponse.
 
-        key-value pairs to configure this import. Options vary based on the import file type.  # noqa: E501
+        list of records found  # noqa: E501
 
-        :param options: The options of this ImportRequest.  # noqa: E501
-        :type: dict(str, object)
+        :param records: The records of this RecordQueryResponse.  # noqa: E501
+        :type: list[RecordResponse]
         """
+        if self.local_vars_configuration.client_side_validation and records is None:  # noqa: E501
+            raise ValueError("Invalid value for `records`, must not be `None`")  # noqa: E501
 
-        self._options = options
+        self._records = records
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -169,18 +162,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ImportRequest):
+        if not isinstance(other, RecordQueryResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ImportRequest):
+        if not isinstance(other, RecordQueryResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/inline_object.py` & `wds_client-0.4.0/wds_client/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/job.py` & `wds_client-0.4.0/wds_client/models/job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/job_v1.py` & `wds_client-0.4.0/wds_client/models/job_v1.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/record_request.py` & `wds_client-0.4.0/wds_client/models/record_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/record_response.py` & `wds_client-0.4.0/wds_client/models/tsv_upload_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,129 +14,96 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class RecordResponse(object):
+class TsvUploadResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'str',
-        'type': 'str',
-        'attributes': 'dict(str, object)'
+        'message': 'str',
+        'records_modified': 'int'
     }
 
     attribute_map = {
-        'id': 'id',
-        'type': 'type',
-        'attributes': 'attributes'
+        'message': 'message',
+        'records_modified': 'recordsModified'
     }
 
-    def __init__(self, id=None, type=None, attributes=None, local_vars_configuration=None):  # noqa: E501
-        """RecordResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, message=None, records_modified=None, local_vars_configuration=None):  # noqa: E501
+        """TsvUploadResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._type = None
-        self._attributes = None
+        self._message = None
+        self._records_modified = None
         self.discriminator = None
 
-        self.id = id
-        self.type = type
-        self.attributes = attributes
+        self.message = message
+        self.records_modified = records_modified
 
     @property
-    def id(self):
-        """Gets the id of this RecordResponse.  # noqa: E501
+    def message(self):
+        """Gets the message of this TsvUploadResponse.  # noqa: E501
 
-        Record id  # noqa: E501
 
-        :return: The id of this RecordResponse.  # noqa: E501
+        :return: The message of this TsvUploadResponse.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._message
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this RecordResponse.
+    @message.setter
+    def message(self, message):
+        """Sets the message of this TsvUploadResponse.
 
-        Record id  # noqa: E501
 
-        :param id: The id of this RecordResponse.  # noqa: E501
+        :param message: The message of this TsvUploadResponse.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and message is None:  # noqa: E501
+            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
-        self._id = id
+        self._message = message
 
     @property
-    def type(self):
-        """Gets the type of this RecordResponse.  # noqa: E501
+    def records_modified(self):
+        """Gets the records_modified of this TsvUploadResponse.  # noqa: E501
 
-        Record type  # noqa: E501
 
-        :return: The type of this RecordResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this RecordResponse.
-
-        Record type  # noqa: E501
-
-        :param type: The type of this RecordResponse.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-
-        self._type = type
-
-    @property
-    def attributes(self):
-        """Gets the attributes of this RecordResponse.  # noqa: E501
-
-        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
-
-        :return: The attributes of this RecordResponse.  # noqa: E501
-        :rtype: dict(str, object)
+        :return: The records_modified of this TsvUploadResponse.  # noqa: E501
+        :rtype: int
         """
-        return self._attributes
+        return self._records_modified
 
-    @attributes.setter
-    def attributes(self, attributes):
-        """Sets the attributes of this RecordResponse.
+    @records_modified.setter
+    def records_modified(self, records_modified):
+        """Sets the records_modified of this TsvUploadResponse.
 
-        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
-        :param attributes: The attributes of this RecordResponse.  # noqa: E501
-        :type: dict(str, object)
+        :param records_modified: The records_modified of this TsvUploadResponse.  # noqa: E501
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and attributes is None:  # noqa: E501
-            raise ValueError("Invalid value for `attributes`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and records_modified is None:  # noqa: E501
+            raise ValueError("Invalid value for `records_modified`, must not be `None`")  # noqa: E501
 
-        self._attributes = attributes
+        self._records_modified = records_modified
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -164,18 +131,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RecordResponse):
+        if not isinstance(other, TsvUploadResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RecordResponse):
+        if not isinstance(other, TsvUploadResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/record_type_schema.py` & `wds_client-0.4.0/wds_client/models/record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/models/search_filter.py` & `wds_client-0.4.0/wds_client/models/search_sort_direction.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,71 +14,49 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class SearchFilter(object):
+class SearchSortDirection(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    ASC = "ASC"
+    DESC = "DESC"
+
+    allowable_values = [ASC, DESC]  # noqa: E501
+
+    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'ids': 'list[str]'
     }
 
     attribute_map = {
-        'ids': 'ids'
     }
 
-    def __init__(self, ids=None, local_vars_configuration=None):  # noqa: E501
-        """SearchFilter - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """SearchSortDirection - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._ids = None
         self.discriminator = None
 
-        if ids is not None:
-            self.ids = ids
-
-    @property
-    def ids(self):
-        """Gets the ids of this SearchFilter.  # noqa: E501
-
-        Record ids by which to filter the query  # noqa: E501
-
-        :return: The ids of this SearchFilter.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._ids
-
-    @ids.setter
-    def ids(self, ids):
-        """Sets the ids of this SearchFilter.
-
-        Record ids by which to filter the query  # noqa: E501
-
-        :param ids: The ids of this SearchFilter.  # noqa: E501
-        :type: list[str]
-        """
-
-        self._ids = ids
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -105,18 +83,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SearchFilter):
+        if not isinstance(other, SearchSortDirection):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SearchFilter):
+        if not isinstance(other, SearchSortDirection):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds_client-0.3.0/wds_client/models/search_request.py` & `wds_client-0.4.0/wds_client/models/search_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client/rest.py` & `wds_client-0.4.0/wds_client/rest.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.3.0/wds_client.egg-info/SOURCES.txt` & `wds_client-0.4.0/wds_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,21 +16,14 @@
 test/test_capabilities.py
 test/test_capabilities_api.py
 test/test_clone_job.py
 test/test_clone_job_all_of.py
 test/test_clone_response.py
 test/test_cloning_api.py
 test/test_commit.py
-test/test_component.py
-test/test_components.py
-test/test_db_component.py
-test/test_db_validationcomponent.py
-test/test_db_validationcomponent_details.py
-test/test_disk_space_component.py
-test/test_disk_space_component_details.py
 test/test_error_response.py
 test/test_general_wds_information_api.py
 test/test_generic_job.py
 test/test_generic_job_all_of.py
 test/test_git.py
 test/test_import_api.py
 test/test_import_request.py
@@ -84,21 +77,14 @@
 wds_client/models/batch_response.py
 wds_client/models/build.py
 wds_client/models/capabilities.py
 wds_client/models/clone_job.py
 wds_client/models/clone_job_all_of.py
 wds_client/models/clone_response.py
 wds_client/models/commit.py
-wds_client/models/component.py
-wds_client/models/components.py
-wds_client/models/db_component.py
-wds_client/models/db_validationcomponent.py
-wds_client/models/db_validationcomponent_details.py
-wds_client/models/disk_space_component.py
-wds_client/models/disk_space_component_details.py
 wds_client/models/error_response.py
 wds_client/models/generic_job.py
 wds_client/models/generic_job_all_of.py
 wds_client/models/git.py
 wds_client/models/import_request.py
 wds_client/models/inline_object.py
 wds_client/models/job.py
```

