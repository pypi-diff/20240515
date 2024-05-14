# Comparing `tmp/structifyai-0.1.0a6.tar.gz` & `tmp/structifyai-0.1.0a7.tar.gz`

## Comparing `structifyai-0.1.0a6.tar` & `structifyai-0.1.0a7.tar`

### file list

```diff
@@ -1,77 +1,70 @@
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/__init__.py
--rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_base_client.py
--rw-r--r--   0        0        0    22039 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_constants.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_qs.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_resource.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_response.py
--rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_streaming.py
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_types.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/lib/.keep
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/__init__.py
--rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/datasets.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/documents.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/runs.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/server.py
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/sources.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/user.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/admin/__init__.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/admin/admin.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/admin/users.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/__init__.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/is_complete.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/job_status.py
--rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/run.py
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/run_async.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/structure/structure.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/usage/__init__.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/usage/get_job_info.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/resources/usage/usage.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/__init__.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_create_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_delete_params.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_descriptor.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_list_response.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_node.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_retrieve_params.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_view_params.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/dataset_view_response.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/document_download_response.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/document_list_response.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/document_upload_params.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/kg_entity.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/new_token.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/run_list_response.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/server_information.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/source.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/source_list_params.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/user_info.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/admin/__init__.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/admin/user_list_response.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/admin/user_node.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/is_complete.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/is_complete_create_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/job_status_create_params.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/run_async_create_params.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/structure/run_create_params.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/usage/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/src/structify/types/usage/get_job_info_create_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/.gitignore
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 structifyai-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/__init__.py
+-rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_base_client.py
+-rw-r--r--   0        0        0    22039 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_constants.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_qs.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_resource.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_response.py
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_streaming.py
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_types.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/lib/.keep
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/__init__.py
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/datasets.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/documents.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/runs.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/server.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/sources.py
+-rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/structure.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/user.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/admin/__init__.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/admin/admin.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/admin/users.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/usage/__init__.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/usage/get_job_info.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/usage/usage.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_create_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_delete_params.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_descriptor.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_list_response.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_retrieve_params.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_view_params.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_view_response.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/document_download_response.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/document_list_response.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/document_upload_params.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/is_complete.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/kg_entity.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/new_token.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/run_list_response.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/server_information.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/source.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/source_list_params.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/structure_is_complete_params.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/structure_job_status_params.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/structure_run_async_params.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/user_info.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/admin/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/admin/user.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/admin/user_list_response.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/usage/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/usage/get_job_info_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/.gitignore
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/LICENSE
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/PKG-INFO
```

### Comparing `structifyai-0.1.0a6/src/structify/__init__.py` & `structifyai-0.1.0a7/src/structify/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_base_client.py` & `structifyai-0.1.0a7/src/structify/_base_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_client.py` & `structifyai-0.1.0a7/src/structify/_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_compat.py` & `structifyai-0.1.0a7/src/structify/_compat.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_exceptions.py` & `structifyai-0.1.0a7/src/structify/_exceptions.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_files.py` & `structifyai-0.1.0a7/src/structify/_files.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_models.py` & `structifyai-0.1.0a7/src/structify/_models.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_qs.py` & `structifyai-0.1.0a7/src/structify/_qs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_resource.py` & `structifyai-0.1.0a7/src/structify/_resource.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_response.py` & `structifyai-0.1.0a7/src/structify/_response.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_streaming.py` & `structifyai-0.1.0a7/src/structify/_streaming.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_types.py` & `structifyai-0.1.0a7/src/structify/_types.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_utils/__init__.py` & `structifyai-0.1.0a7/src/structify/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_utils/_logs.py` & `structifyai-0.1.0a7/src/structify/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_utils/_proxy.py` & `structifyai-0.1.0a7/src/structify/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_utils/_sync.py` & `structifyai-0.1.0a7/src/structify/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_utils/_transform.py` & `structifyai-0.1.0a7/src/structify/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_utils/_typing.py` & `structifyai-0.1.0a7/src/structify/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/_utils/_utils.py` & `structifyai-0.1.0a7/src/structify/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/__init__.py` & `structifyai-0.1.0a7/src/structify/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/datasets.py` & `structifyai-0.1.0a7/src/structify/resources/datasets.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/documents.py` & `structifyai-0.1.0a7/src/structify/resources/documents.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/runs.py` & `structifyai-0.1.0a7/src/structify/resources/runs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/server.py` & `structifyai-0.1.0a7/src/structify/resources/server.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/sources.py` & `structifyai-0.1.0a7/src/structify/resources/sources.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/user.py` & `structifyai-0.1.0a7/src/structify/resources/user.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/admin/__init__.py` & `structifyai-0.1.0a7/src/structify/resources/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/admin/admin.py` & `structifyai-0.1.0a7/src/structify/resources/admin/admin.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/admin/users.py` & `structifyai-0.1.0a7/src/structify/resources/admin/users.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/structure/is_complete.py` & `structifyai-0.1.0a7/src/structify/resources/usage/get_job_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import List
-
 import httpx
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     maybe_transform,
     async_maybe_transform,
 )
@@ -15,134 +13,141 @@
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
+from ...types.usage import get_job_info_create_params
 from ..._base_client import (
     make_request_options,
 )
-from ...types.structure import is_complete_create_params
-from ...types.structure.is_complete import IsComplete
 
-__all__ = ["IsCompleteResource", "AsyncIsCompleteResource"]
+__all__ = ["GetJobInfoResource", "AsyncGetJobInfoResource"]
 
 
-class IsCompleteResource(SyncAPIResource):
+class GetJobInfoResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> IsCompleteResourceWithRawResponse:
-        return IsCompleteResourceWithRawResponse(self)
+    def with_raw_response(self) -> GetJobInfoResourceWithRawResponse:
+        return GetJobInfoResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> IsCompleteResourceWithStreamingResponse:
-        return IsCompleteResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> GetJobInfoResourceWithStreamingResponse:
+        return GetJobInfoResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
-        body: List[str],
+        job_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> IsComplete:
+    ) -> object:
         """
-        Wait for all specified async tasks to be completed.
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._post(
-            "/structure/is_complete",
-            body=maybe_transform(body, is_complete_create_params.IsCompleteCreateParams),
+            "/usage/get_job_info",
             options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                query=maybe_transform({"job_id": job_id}, get_job_info_create_params.GetJobInfoCreateParams),
             ),
-            cast_to=IsComplete,
+            cast_to=object,
         )
 
 
-class AsyncIsCompleteResource(AsyncAPIResource):
+class AsyncGetJobInfoResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncIsCompleteResourceWithRawResponse:
-        return AsyncIsCompleteResourceWithRawResponse(self)
+    def with_raw_response(self) -> AsyncGetJobInfoResourceWithRawResponse:
+        return AsyncGetJobInfoResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncIsCompleteResourceWithStreamingResponse:
-        return AsyncIsCompleteResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncGetJobInfoResourceWithStreamingResponse:
+        return AsyncGetJobInfoResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
-        body: List[str],
+        job_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> IsComplete:
+    ) -> object:
         """
-        Wait for all specified async tasks to be completed.
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
-            "/structure/is_complete",
-            body=await async_maybe_transform(body, is_complete_create_params.IsCompleteCreateParams),
+            "/usage/get_job_info",
             options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                query=await async_maybe_transform(
+                    {"job_id": job_id}, get_job_info_create_params.GetJobInfoCreateParams
+                ),
             ),
-            cast_to=IsComplete,
+            cast_to=object,
         )
 
 
-class IsCompleteResourceWithRawResponse:
-    def __init__(self, is_complete: IsCompleteResource) -> None:
-        self._is_complete = is_complete
+class GetJobInfoResourceWithRawResponse:
+    def __init__(self, get_job_info: GetJobInfoResource) -> None:
+        self._get_job_info = get_job_info
 
         self.create = to_raw_response_wrapper(
-            is_complete.create,
+            get_job_info.create,
         )
 
 
-class AsyncIsCompleteResourceWithRawResponse:
-    def __init__(self, is_complete: AsyncIsCompleteResource) -> None:
-        self._is_complete = is_complete
+class AsyncGetJobInfoResourceWithRawResponse:
+    def __init__(self, get_job_info: AsyncGetJobInfoResource) -> None:
+        self._get_job_info = get_job_info
 
         self.create = async_to_raw_response_wrapper(
-            is_complete.create,
+            get_job_info.create,
         )
 
 
-class IsCompleteResourceWithStreamingResponse:
-    def __init__(self, is_complete: IsCompleteResource) -> None:
-        self._is_complete = is_complete
+class GetJobInfoResourceWithStreamingResponse:
+    def __init__(self, get_job_info: GetJobInfoResource) -> None:
+        self._get_job_info = get_job_info
 
         self.create = to_streamed_response_wrapper(
-            is_complete.create,
+            get_job_info.create,
         )
 
 
-class AsyncIsCompleteResourceWithStreamingResponse:
-    def __init__(self, is_complete: AsyncIsCompleteResource) -> None:
-        self._is_complete = is_complete
+class AsyncGetJobInfoResourceWithStreamingResponse:
+    def __init__(self, get_job_info: AsyncGetJobInfoResource) -> None:
+        self._get_job_info = get_job_info
 
         self.create = async_to_streamed_response_wrapper(
-            is_complete.create,
+            get_job_info.create,
         )
```

### Comparing `structifyai-0.1.0a6/src/structify/resources/structure/run.py` & `structifyai-0.1.0a7/src/structify/resources/structure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,211 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Optional, overload
+from typing import List, Optional, overload
 
 import httpx
 
-from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._utils import (
+from ..types import structure_run_async_params, structure_job_status_params, structure_is_complete_params
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import (
     required_args,
     maybe_transform,
     async_maybe_transform,
 )
-from ..._compat import cached_property
-from ..._resource import SyncAPIResource, AsyncAPIResource
-from ..._response import (
+from .._compat import cached_property
+from .._resource import SyncAPIResource, AsyncAPIResource
+from .._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
-from ..._base_client import (
+from .._base_client import (
     make_request_options,
 )
-from ...types.structure import run_create_params
+from ..types.is_complete import IsComplete
 
-__all__ = ["RunResource", "AsyncRunResource"]
+__all__ = ["StructureResource", "AsyncStructureResource"]
 
 
-class RunResource(SyncAPIResource):
+class StructureResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> RunResourceWithRawResponse:
-        return RunResourceWithRawResponse(self)
+    def with_raw_response(self) -> StructureResourceWithRawResponse:
+        return StructureResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> RunResourceWithStreamingResponse:
-        return RunResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> StructureResourceWithStreamingResponse:
+        return StructureResourceWithStreamingResponse(self)
+
+    def is_complete(
+        self,
+        *,
+        body: List[str],
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> IsComplete:
+        """
+        Wait for all specified async tasks to be completed.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        return self._post(
+            "/structure/is_complete",
+            body=maybe_transform(body, structure_is_complete_params.StructureIsCompleteParams),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=IsComplete,
+        )
+
+    def job_status(
+        self,
+        *,
+        body: List[str],
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> object:
+        """
+        Wait for all specified async tasks to be completed.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        return self._post(
+            "/structure/job_status",
+            body=maybe_transform(body, structure_job_status_params.StructureJobStatusParams),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=object,
+        )
 
     @overload
-    def create(
+    def run_async(
         self,
         *,
         dataset_name: str,
-        text: run_create_params.Variant0Text,
+        text: structure_run_async_params.Variant0Text,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """There's a couple of different types of sources.
-
-        Right now, you can either add a
-        file path or the internet as a whole. In the future, we'll allow you to pare
-        down the internet to a specific domain or criterium.
+        """
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    def create(
+    def run_async(
         self,
         *,
         dataset_name: str,
-        document: run_create_params.Variant1Document,
+        document: structure_run_async_params.Variant1Document,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """There's a couple of different types of sources.
-
-        Right now, you can either add a
-        file path or the internet as a whole. In the future, we'll allow you to pare
-        down the internet to a specific domain or criterium.
+        """
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    def create(
+    def run_async(
         self,
         *,
         dataset_name: str,
-        web: run_create_params.Variant2Web,
+        web: structure_run_async_params.Variant2Web,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """There's a couple of different types of sources.
-
-        Right now, you can either add a
-        file path or the internet as a whole. In the future, we'll allow you to pare
-        down the internet to a specific domain or criterium.
+        """
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    def create(
+    def run_async(
         self,
         *,
         dataset_name: str,
-        sec_filing: run_create_params.Variant3SecFiling,
+        sec_filing: structure_run_async_params.Variant3SecFiling,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """There's a couple of different types of sources.
-
-        Right now, you can either add a
-        file path or the internet as a whole. In the future, we'll allow you to pare
-        down the internet to a specific domain or criterium.
+        """
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -160,179 +213,231 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @required_args(
         ["dataset_name", "text"], ["dataset_name", "document"], ["dataset_name", "web"], ["dataset_name", "sec_filing"]
     )
-    def create(
+    def run_async(
         self,
         *,
         dataset_name: str,
-        text: run_create_params.Variant0Text | NotGiven = NOT_GIVEN,
+        text: structure_run_async_params.Variant0Text | NotGiven = NOT_GIVEN,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
-        document: run_create_params.Variant1Document | NotGiven = NOT_GIVEN,
-        web: run_create_params.Variant2Web | NotGiven = NOT_GIVEN,
-        sec_filing: run_create_params.Variant3SecFiling | NotGiven = NOT_GIVEN,
+        document: structure_run_async_params.Variant1Document | NotGiven = NOT_GIVEN,
+        web: structure_run_async_params.Variant2Web | NotGiven = NOT_GIVEN,
+        sec_filing: structure_run_async_params.Variant3SecFiling | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         return self._post(
-            "/structure/run",
+            "/structure/run_async",
             body=maybe_transform(
                 {
                     "text": text,
                     "document": document,
                     "web": web,
                     "sec_filing": sec_filing,
                 },
-                run_create_params.RunCreateParams,
+                structure_run_async_params.StructureRunAsyncParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "dataset_name": dataset_name,
                         "custom_instruction": custom_instruction,
                     },
-                    run_create_params.RunCreateParams,
+                    structure_run_async_params.StructureRunAsyncParams,
                 ),
             ),
             cast_to=object,
         )
 
 
-class AsyncRunResource(AsyncAPIResource):
+class AsyncStructureResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncRunResourceWithRawResponse:
-        return AsyncRunResourceWithRawResponse(self)
+    def with_raw_response(self) -> AsyncStructureResourceWithRawResponse:
+        return AsyncStructureResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncRunResourceWithStreamingResponse:
-        return AsyncRunResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncStructureResourceWithStreamingResponse:
+        return AsyncStructureResourceWithStreamingResponse(self)
+
+    async def is_complete(
+        self,
+        *,
+        body: List[str],
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> IsComplete:
+        """
+        Wait for all specified async tasks to be completed.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        return await self._post(
+            "/structure/is_complete",
+            body=await async_maybe_transform(body, structure_is_complete_params.StructureIsCompleteParams),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=IsComplete,
+        )
+
+    async def job_status(
+        self,
+        *,
+        body: List[str],
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> object:
+        """
+        Wait for all specified async tasks to be completed.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        return await self._post(
+            "/structure/job_status",
+            body=await async_maybe_transform(body, structure_job_status_params.StructureJobStatusParams),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=object,
+        )
 
     @overload
-    async def create(
+    async def run_async(
         self,
         *,
         dataset_name: str,
-        text: run_create_params.Variant0Text,
+        text: structure_run_async_params.Variant0Text,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """There's a couple of different types of sources.
-
-        Right now, you can either add a
-        file path or the internet as a whole. In the future, we'll allow you to pare
-        down the internet to a specific domain or criterium.
+        """
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    async def create(
+    async def run_async(
         self,
         *,
         dataset_name: str,
-        document: run_create_params.Variant1Document,
+        document: structure_run_async_params.Variant1Document,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """There's a couple of different types of sources.
-
-        Right now, you can either add a
-        file path or the internet as a whole. In the future, we'll allow you to pare
-        down the internet to a specific domain or criterium.
+        """
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    async def create(
+    async def run_async(
         self,
         *,
         dataset_name: str,
-        web: run_create_params.Variant2Web,
+        web: structure_run_async_params.Variant2Web,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """There's a couple of different types of sources.
-
-        Right now, you can either add a
-        file path or the internet as a whole. In the future, we'll allow you to pare
-        down the internet to a specific domain or criterium.
+        """
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    async def create(
+    async def run_async(
         self,
         *,
         dataset_name: str,
-        sec_filing: run_create_params.Variant3SecFiling,
+        sec_filing: structure_run_async_params.Variant3SecFiling,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
-        """There's a couple of different types of sources.
-
-        Right now, you can either add a
-        file path or the internet as a whole. In the future, we'll allow you to pare
-        down the internet to a specific domain or criterium.
+        """
+        Returns a token that can be waited on until the request is finished.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -340,85 +445,109 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @required_args(
         ["dataset_name", "text"], ["dataset_name", "document"], ["dataset_name", "web"], ["dataset_name", "sec_filing"]
     )
-    async def create(
+    async def run_async(
         self,
         *,
         dataset_name: str,
-        text: run_create_params.Variant0Text | NotGiven = NOT_GIVEN,
+        text: structure_run_async_params.Variant0Text | NotGiven = NOT_GIVEN,
         custom_instruction: Optional[str] | NotGiven = NOT_GIVEN,
-        document: run_create_params.Variant1Document | NotGiven = NOT_GIVEN,
-        web: run_create_params.Variant2Web | NotGiven = NOT_GIVEN,
-        sec_filing: run_create_params.Variant3SecFiling | NotGiven = NOT_GIVEN,
+        document: structure_run_async_params.Variant1Document | NotGiven = NOT_GIVEN,
+        web: structure_run_async_params.Variant2Web | NotGiven = NOT_GIVEN,
+        sec_filing: structure_run_async_params.Variant3SecFiling | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> object:
         return await self._post(
-            "/structure/run",
+            "/structure/run_async",
             body=await async_maybe_transform(
                 {
                     "text": text,
                     "document": document,
                     "web": web,
                     "sec_filing": sec_filing,
                 },
-                run_create_params.RunCreateParams,
+                structure_run_async_params.StructureRunAsyncParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "dataset_name": dataset_name,
                         "custom_instruction": custom_instruction,
                     },
-                    run_create_params.RunCreateParams,
+                    structure_run_async_params.StructureRunAsyncParams,
                 ),
             ),
             cast_to=object,
         )
 
 
-class RunResourceWithRawResponse:
-    def __init__(self, run: RunResource) -> None:
-        self._run = run
+class StructureResourceWithRawResponse:
+    def __init__(self, structure: StructureResource) -> None:
+        self._structure = structure
 
-        self.create = to_raw_response_wrapper(
-            run.create,
+        self.is_complete = to_raw_response_wrapper(
+            structure.is_complete,
+        )
+        self.job_status = to_raw_response_wrapper(
+            structure.job_status,
+        )
+        self.run_async = to_raw_response_wrapper(
+            structure.run_async,
         )
 
 
-class AsyncRunResourceWithRawResponse:
-    def __init__(self, run: AsyncRunResource) -> None:
-        self._run = run
+class AsyncStructureResourceWithRawResponse:
+    def __init__(self, structure: AsyncStructureResource) -> None:
+        self._structure = structure
 
-        self.create = async_to_raw_response_wrapper(
-            run.create,
+        self.is_complete = async_to_raw_response_wrapper(
+            structure.is_complete,
+        )
+        self.job_status = async_to_raw_response_wrapper(
+            structure.job_status,
+        )
+        self.run_async = async_to_raw_response_wrapper(
+            structure.run_async,
         )
 
 
-class RunResourceWithStreamingResponse:
-    def __init__(self, run: RunResource) -> None:
-        self._run = run
+class StructureResourceWithStreamingResponse:
+    def __init__(self, structure: StructureResource) -> None:
+        self._structure = structure
 
-        self.create = to_streamed_response_wrapper(
-            run.create,
+        self.is_complete = to_streamed_response_wrapper(
+            structure.is_complete,
+        )
+        self.job_status = to_streamed_response_wrapper(
+            structure.job_status,
+        )
+        self.run_async = to_streamed_response_wrapper(
+            structure.run_async,
         )
 
 
-class AsyncRunResourceWithStreamingResponse:
-    def __init__(self, run: AsyncRunResource) -> None:
-        self._run = run
+class AsyncStructureResourceWithStreamingResponse:
+    def __init__(self, structure: AsyncStructureResource) -> None:
+        self._structure = structure
 
-        self.create = async_to_streamed_response_wrapper(
-            run.create,
+        self.is_complete = async_to_streamed_response_wrapper(
+            structure.is_complete,
+        )
+        self.job_status = async_to_streamed_response_wrapper(
+            structure.job_status,
+        )
+        self.run_async = async_to_streamed_response_wrapper(
+            structure.run_async,
         )
```

### Comparing `structifyai-0.1.0a6/src/structify/resources/usage/__init__.py` & `structifyai-0.1.0a7/src/structify/resources/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/resources/usage/usage.py` & `structifyai-0.1.0a7/src/structify/resources/usage/usage.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/types/__init__.py` & `structifyai-0.1.0a7/src/structify/types/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from .source import Source as Source
+from .dataset import Dataset as Dataset
 from .kg_entity import KgEntity as KgEntity
 from .new_token import NewToken as NewToken
 from .user_info import UserInfo as UserInfo
-from .dataset_node import DatasetNode as DatasetNode
+from .is_complete import IsComplete as IsComplete
 from .run_list_response import RunListResponse as RunListResponse
 from .dataset_descriptor import DatasetDescriptor as DatasetDescriptor
 from .server_information import ServerInformation as ServerInformation
 from .source_list_params import SourceListParams as SourceListParams
 from .dataset_view_params import DatasetViewParams as DatasetViewParams
 from .dataset_create_params import DatasetCreateParams as DatasetCreateParams
 from .dataset_delete_params import DatasetDeleteParams as DatasetDeleteParams
 from .dataset_list_response import DatasetListResponse as DatasetListResponse
 from .dataset_view_response import DatasetViewResponse as DatasetViewResponse
 from .document_list_response import DocumentListResponse as DocumentListResponse
 from .document_upload_params import DocumentUploadParams as DocumentUploadParams
 from .dataset_retrieve_params import DatasetRetrieveParams as DatasetRetrieveParams
 from .document_download_response import DocumentDownloadResponse as DocumentDownloadResponse
+from .structure_run_async_params import StructureRunAsyncParams as StructureRunAsyncParams
+from .structure_job_status_params import StructureJobStatusParams as StructureJobStatusParams
+from .structure_is_complete_params import StructureIsCompleteParams as StructureIsCompleteParams
```

### Comparing `structifyai-0.1.0a6/src/structify/types/dataset_create_params.py` & `structifyai-0.1.0a7/src/structify/types/dataset_create_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/types/dataset_descriptor.py` & `structifyai-0.1.0a7/src/structify/types/dataset_descriptor.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/types/source.py` & `structifyai-0.1.0a7/src/structify/types/source.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/src/structify/types/structure/run_async_create_params.py` & `structifyai-0.1.0a7/src/structify/types/structure_run_async_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Union, Optional
 from typing_extensions import Required, Annotated, TypedDict
 
-from ..._utils import PropertyInfo
+from .._utils import PropertyInfo
 
 __all__ = [
-    "RunAsyncCreateParams",
+    "StructureRunAsyncParams",
     "Variant0",
     "Variant0Text",
     "Variant1",
     "Variant1Document",
     "Variant2",
     "Variant2Web",
     "Variant3",
@@ -70,8 +70,8 @@
     accession_number: Optional[str]
 
     quarter: Optional[int]
 
     year: Optional[int]
 
 
-RunAsyncCreateParams = Union[Variant0, Variant1, Variant2, Variant3]
+StructureRunAsyncParams = Union[Variant0, Variant1, Variant2, Variant3]
```

### Comparing `structifyai-0.1.0a6/LICENSE` & `structifyai-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a6/pyproject.toml` & `structifyai-0.1.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "structifyai"
-version = "0.1.0-alpha.6"
+version = "0.1.0-alpha.7"
 description = "The official Python library for the structify API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Structify", email = "team@structify.ai" },
 ]
 dependencies = [
```

### Comparing `structifyai-0.1.0a6/PKG-INFO` & `structifyai-0.1.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: structifyai
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: The official Python library for the structify API
 Project-URL: Homepage, https://github.com/StructifyAI/structify-python
 Project-URL: Repository, https://github.com/StructifyAI/structify-python
 Author-email: Structify <team@structify.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

