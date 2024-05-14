# Comparing `tmp/structifyai-0.1.0a7.tar.gz` & `tmp/structifyai-0.1.0a8.tar.gz`

## Comparing `structifyai-0.1.0a7.tar` & `structifyai-0.1.0a8.tar`

### file list

```diff
@@ -1,70 +1,75 @@
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/__init__.py
--rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_base_client.py
--rw-r--r--   0        0        0    22039 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_constants.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_qs.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_resource.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_response.py
--rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_streaming.py
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_types.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/lib/.keep
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/__init__.py
--rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/datasets.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/documents.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/runs.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/server.py
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/sources.py
--rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/structure.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/user.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/admin/__init__.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/admin/admin.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/admin/users.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/usage/__init__.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/usage/get_job_info.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/resources/usage/usage.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_create_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_delete_params.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_descriptor.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_list_response.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_retrieve_params.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_view_params.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/dataset_view_response.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/document_download_response.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/document_list_response.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/document_upload_params.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/is_complete.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/kg_entity.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/new_token.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/run_list_response.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/server_information.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/source.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/source_list_params.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/structure_is_complete_params.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/structure_job_status_params.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/structure_run_async_params.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/user_info.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/admin/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/admin/user.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/admin/user_list_response.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/usage/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/src/structify/types/usage/get_job_info_create_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/.gitignore
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/LICENSE
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 structifyai-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/__init__.py
+-rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_base_client.py
+-rw-r--r--   0        0        0    22539 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_constants.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_qs.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_resource.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_response.py
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_streaming.py
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_types.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/lib/.keep
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/__init__.py
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/datasets.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/documents.py
+-rw-r--r--   0        0        0    20198 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/label.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/runs.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/sources.py
+-rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/structure.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/usage.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/user.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/admin/__init__.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/admin/admin.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/admin/users.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/server/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/server/server.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/server/version.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_create_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_delete_params.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_descriptor.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_list_response.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_retrieve_params.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_view_params.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_view_response.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/document_download_response.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/document_list_response.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/document_upload_params.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/is_complete.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/kg_entity.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/label_get_messages_response.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/label_run_params.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/label_submit_params.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/label_submit_response.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/new_token.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/run_list_response.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/source.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/source_list_params.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/structure_is_complete_params.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/structure_job_status_params.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/structure_run_async_params.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/usage_get_job_info_params.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/user_info.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/admin/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/admin/user.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/admin/user_list_response.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/server/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/server/server_information.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/.gitignore
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/LICENSE
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0    12242 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/PKG-INFO
```

### Comparing `structifyai-0.1.0a7/src/structify/__init__.py` & `structifyai-0.1.0a8/src/structify/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_base_client.py` & `structifyai-0.1.0a8/src/structify/_base_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_client.py` & `structifyai-0.1.0a8/src/structify/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     admin: resources.AdminResource
     datasets: resources.DatasetsResource
     documents: resources.DocumentsResource
     runs: resources.RunsResource
     server: resources.ServerResource
     sources: resources.SourcesResource
     structure: resources.StructureResource
+    label: resources.LabelResource
     usage: resources.UsageResource
     with_raw_response: StructifyWithRawResponse
     with_streaming_response: StructifyWithStreamedResponse
 
     # client options
     api_key: str
 
@@ -146,14 +147,15 @@
         self.admin = resources.AdminResource(self)
         self.datasets = resources.DatasetsResource(self)
         self.documents = resources.DocumentsResource(self)
         self.runs = resources.RunsResource(self)
         self.server = resources.ServerResource(self)
         self.sources = resources.SourcesResource(self)
         self.structure = resources.StructureResource(self)
+        self.label = resources.LabelResource(self)
         self.usage = resources.UsageResource(self)
         self.with_raw_response = StructifyWithRawResponse(self)
         self.with_streaming_response = StructifyWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
@@ -266,14 +268,15 @@
     admin: resources.AsyncAdminResource
     datasets: resources.AsyncDatasetsResource
     documents: resources.AsyncDocumentsResource
     runs: resources.AsyncRunsResource
     server: resources.AsyncServerResource
     sources: resources.AsyncSourcesResource
     structure: resources.AsyncStructureResource
+    label: resources.AsyncLabelResource
     usage: resources.AsyncUsageResource
     with_raw_response: AsyncStructifyWithRawResponse
     with_streaming_response: AsyncStructifyWithStreamedResponse
 
     # client options
     api_key: str
 
@@ -356,14 +359,15 @@
         self.admin = resources.AsyncAdminResource(self)
         self.datasets = resources.AsyncDatasetsResource(self)
         self.documents = resources.AsyncDocumentsResource(self)
         self.runs = resources.AsyncRunsResource(self)
         self.server = resources.AsyncServerResource(self)
         self.sources = resources.AsyncSourcesResource(self)
         self.structure = resources.AsyncStructureResource(self)
+        self.label = resources.AsyncLabelResource(self)
         self.usage = resources.AsyncUsageResource(self)
         self.with_raw_response = AsyncStructifyWithRawResponse(self)
         self.with_streaming_response = AsyncStructifyWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
@@ -477,52 +481,56 @@
         self.admin = resources.AdminResourceWithRawResponse(client.admin)
         self.datasets = resources.DatasetsResourceWithRawResponse(client.datasets)
         self.documents = resources.DocumentsResourceWithRawResponse(client.documents)
         self.runs = resources.RunsResourceWithRawResponse(client.runs)
         self.server = resources.ServerResourceWithRawResponse(client.server)
         self.sources = resources.SourcesResourceWithRawResponse(client.sources)
         self.structure = resources.StructureResourceWithRawResponse(client.structure)
+        self.label = resources.LabelResourceWithRawResponse(client.label)
         self.usage = resources.UsageResourceWithRawResponse(client.usage)
 
 
 class AsyncStructifyWithRawResponse:
     def __init__(self, client: AsyncStructify) -> None:
         self.user = resources.AsyncUserResourceWithRawResponse(client.user)
         self.admin = resources.AsyncAdminResourceWithRawResponse(client.admin)
         self.datasets = resources.AsyncDatasetsResourceWithRawResponse(client.datasets)
         self.documents = resources.AsyncDocumentsResourceWithRawResponse(client.documents)
         self.runs = resources.AsyncRunsResourceWithRawResponse(client.runs)
         self.server = resources.AsyncServerResourceWithRawResponse(client.server)
         self.sources = resources.AsyncSourcesResourceWithRawResponse(client.sources)
         self.structure = resources.AsyncStructureResourceWithRawResponse(client.structure)
+        self.label = resources.AsyncLabelResourceWithRawResponse(client.label)
         self.usage = resources.AsyncUsageResourceWithRawResponse(client.usage)
 
 
 class StructifyWithStreamedResponse:
     def __init__(self, client: Structify) -> None:
         self.user = resources.UserResourceWithStreamingResponse(client.user)
         self.admin = resources.AdminResourceWithStreamingResponse(client.admin)
         self.datasets = resources.DatasetsResourceWithStreamingResponse(client.datasets)
         self.documents = resources.DocumentsResourceWithStreamingResponse(client.documents)
         self.runs = resources.RunsResourceWithStreamingResponse(client.runs)
         self.server = resources.ServerResourceWithStreamingResponse(client.server)
         self.sources = resources.SourcesResourceWithStreamingResponse(client.sources)
         self.structure = resources.StructureResourceWithStreamingResponse(client.structure)
+        self.label = resources.LabelResourceWithStreamingResponse(client.label)
         self.usage = resources.UsageResourceWithStreamingResponse(client.usage)
 
 
 class AsyncStructifyWithStreamedResponse:
     def __init__(self, client: AsyncStructify) -> None:
         self.user = resources.AsyncUserResourceWithStreamingResponse(client.user)
         self.admin = resources.AsyncAdminResourceWithStreamingResponse(client.admin)
         self.datasets = resources.AsyncDatasetsResourceWithStreamingResponse(client.datasets)
         self.documents = resources.AsyncDocumentsResourceWithStreamingResponse(client.documents)
         self.runs = resources.AsyncRunsResourceWithStreamingResponse(client.runs)
         self.server = resources.AsyncServerResourceWithStreamingResponse(client.server)
         self.sources = resources.AsyncSourcesResourceWithStreamingResponse(client.sources)
         self.structure = resources.AsyncStructureResourceWithStreamingResponse(client.structure)
+        self.label = resources.AsyncLabelResourceWithStreamingResponse(client.label)
         self.usage = resources.AsyncUsageResourceWithStreamingResponse(client.usage)
 
 
 Client = Structify
 
 AsyncClient = AsyncStructify
```

### Comparing `structifyai-0.1.0a7/src/structify/_compat.py` & `structifyai-0.1.0a8/src/structify/_compat.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_exceptions.py` & `structifyai-0.1.0a8/src/structify/_exceptions.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_files.py` & `structifyai-0.1.0a8/src/structify/_files.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_models.py` & `structifyai-0.1.0a8/src/structify/_models.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_qs.py` & `structifyai-0.1.0a8/src/structify/_qs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_resource.py` & `structifyai-0.1.0a8/src/structify/_resource.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_response.py` & `structifyai-0.1.0a8/src/structify/_response.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_streaming.py` & `structifyai-0.1.0a8/src/structify/_streaming.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_types.py` & `structifyai-0.1.0a8/src/structify/_types.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_utils/__init__.py` & `structifyai-0.1.0a8/src/structify/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_utils/_logs.py` & `structifyai-0.1.0a8/src/structify/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_utils/_proxy.py` & `structifyai-0.1.0a8/src/structify/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_utils/_sync.py` & `structifyai-0.1.0a8/src/structify/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_utils/_transform.py` & `structifyai-0.1.0a8/src/structify/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_utils/_typing.py` & `structifyai-0.1.0a8/src/structify/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/_utils/_utils.py` & `structifyai-0.1.0a8/src/structify/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/__init__.py` & `structifyai-0.1.0a8/src/structify/resources/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     AdminResource,
     AsyncAdminResource,
     AdminResourceWithRawResponse,
     AsyncAdminResourceWithRawResponse,
     AdminResourceWithStreamingResponse,
     AsyncAdminResourceWithStreamingResponse,
 )
+from .label import (
+    LabelResource,
+    AsyncLabelResource,
+    LabelResourceWithRawResponse,
+    AsyncLabelResourceWithRawResponse,
+    LabelResourceWithStreamingResponse,
+    AsyncLabelResourceWithStreamingResponse,
+)
 from .usage import (
     UsageResource,
     AsyncUsageResource,
     UsageResourceWithRawResponse,
     AsyncUsageResourceWithRawResponse,
     UsageResourceWithStreamingResponse,
     AsyncUsageResourceWithStreamingResponse,
@@ -118,14 +126,20 @@
     "AsyncSourcesResourceWithStreamingResponse",
     "StructureResource",
     "AsyncStructureResource",
     "StructureResourceWithRawResponse",
     "AsyncStructureResourceWithRawResponse",
     "StructureResourceWithStreamingResponse",
     "AsyncStructureResourceWithStreamingResponse",
+    "LabelResource",
+    "AsyncLabelResource",
+    "LabelResourceWithRawResponse",
+    "AsyncLabelResourceWithRawResponse",
+    "LabelResourceWithStreamingResponse",
+    "AsyncLabelResourceWithStreamingResponse",
     "UsageResource",
     "AsyncUsageResource",
     "UsageResourceWithRawResponse",
     "AsyncUsageResourceWithRawResponse",
     "UsageResourceWithStreamingResponse",
     "AsyncUsageResourceWithStreamingResponse",
 ]
```

### Comparing `structifyai-0.1.0a7/src/structify/resources/datasets.py` & `structifyai-0.1.0a8/src/structify/resources/datasets.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/documents.py` & `structifyai-0.1.0a8/src/structify/resources/documents.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/runs.py` & `structifyai-0.1.0a8/src/structify/resources/runs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/server.py` & `structifyai-0.1.0a8/src/structify/resources/server/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import httpx
 
-from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from .._compat import cached_property
-from .._resource import SyncAPIResource, AsyncAPIResource
-from .._response import (
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._compat import cached_property
+from ..._resource import SyncAPIResource, AsyncAPIResource
+from ..._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
-from .._base_client import (
+from ..._base_client import (
     make_request_options,
 )
-from ..types.server_information import ServerInformation
+from ...types.server.server_information import ServerInformation
 
-__all__ = ["ServerResource", "AsyncServerResource"]
+__all__ = ["VersionResource", "AsyncVersionResource"]
 
 
-class ServerResource(SyncAPIResource):
+class VersionResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> ServerResourceWithRawResponse:
-        return ServerResourceWithRawResponse(self)
+    def with_raw_response(self) -> VersionResourceWithRawResponse:
+        return VersionResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> ServerResourceWithStreamingResponse:
-        return ServerResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> VersionResourceWithStreamingResponse:
+        return VersionResourceWithStreamingResponse(self)
 
-    def version(
+    def retrieve(
         self,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -46,24 +46,24 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ServerInformation,
         )
 
 
-class AsyncServerResource(AsyncAPIResource):
+class AsyncVersionResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncServerResourceWithRawResponse:
-        return AsyncServerResourceWithRawResponse(self)
+    def with_raw_response(self) -> AsyncVersionResourceWithRawResponse:
+        return AsyncVersionResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncServerResourceWithStreamingResponse:
-        return AsyncServerResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncVersionResourceWithStreamingResponse:
+        return AsyncVersionResourceWithStreamingResponse(self)
 
-    async def version(
+    async def retrieve(
         self,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -75,41 +75,41 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ServerInformation,
         )
 
 
-class ServerResourceWithRawResponse:
-    def __init__(self, server: ServerResource) -> None:
-        self._server = server
+class VersionResourceWithRawResponse:
+    def __init__(self, version: VersionResource) -> None:
+        self._version = version
 
-        self.version = to_raw_response_wrapper(
-            server.version,
+        self.retrieve = to_raw_response_wrapper(
+            version.retrieve,
         )
 
 
-class AsyncServerResourceWithRawResponse:
-    def __init__(self, server: AsyncServerResource) -> None:
-        self._server = server
+class AsyncVersionResourceWithRawResponse:
+    def __init__(self, version: AsyncVersionResource) -> None:
+        self._version = version
 
-        self.version = async_to_raw_response_wrapper(
-            server.version,
+        self.retrieve = async_to_raw_response_wrapper(
+            version.retrieve,
         )
 
 
-class ServerResourceWithStreamingResponse:
-    def __init__(self, server: ServerResource) -> None:
-        self._server = server
+class VersionResourceWithStreamingResponse:
+    def __init__(self, version: VersionResource) -> None:
+        self._version = version
 
-        self.version = to_streamed_response_wrapper(
-            server.version,
+        self.retrieve = to_streamed_response_wrapper(
+            version.retrieve,
         )
 
 
-class AsyncServerResourceWithStreamingResponse:
-    def __init__(self, server: AsyncServerResource) -> None:
-        self._server = server
+class AsyncVersionResourceWithStreamingResponse:
+    def __init__(self, version: AsyncVersionResource) -> None:
+        self._version = version
 
-        self.version = async_to_streamed_response_wrapper(
-            server.version,
+        self.retrieve = async_to_streamed_response_wrapper(
+            version.retrieve,
         )
```

### Comparing `structifyai-0.1.0a7/src/structify/resources/sources.py` & `structifyai-0.1.0a8/src/structify/resources/sources.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/structure.py` & `structifyai-0.1.0a8/src/structify/resources/structure.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/user.py` & `structifyai-0.1.0a8/src/structify/resources/user.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/admin/__init__.py` & `structifyai-0.1.0a8/src/structify/resources/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/admin/admin.py` & `structifyai-0.1.0a8/src/structify/resources/admin/admin.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/admin/users.py` & `structifyai-0.1.0a8/src/structify/resources/admin/users.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/resources/usage/get_job_info.py` & `structifyai-0.1.0a8/src/structify/resources/usage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import httpx
 
-from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._utils import (
+from ..types import usage_get_job_info_params
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import (
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
-from ...types.usage import get_job_info_create_params
-from ..._base_client import (
+from .._base_client import (
     make_request_options,
 )
 
-__all__ = ["GetJobInfoResource", "AsyncGetJobInfoResource"]
+__all__ = ["UsageResource", "AsyncUsageResource"]
 
 
-class GetJobInfoResource(SyncAPIResource):
+class UsageResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> GetJobInfoResourceWithRawResponse:
-        return GetJobInfoResourceWithRawResponse(self)
+    def with_raw_response(self) -> UsageResourceWithRawResponse:
+        return UsageResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> GetJobInfoResourceWithStreamingResponse:
-        return GetJobInfoResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> UsageResourceWithStreamingResponse:
+        return UsageResourceWithStreamingResponse(self)
 
-    def create(
+    def get_job_info(
         self,
         *,
         job_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -60,30 +60,30 @@
         return self._post(
             "/usage/get_job_info",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=maybe_transform({"job_id": job_id}, get_job_info_create_params.GetJobInfoCreateParams),
+                query=maybe_transform({"job_id": job_id}, usage_get_job_info_params.UsageGetJobInfoParams),
             ),
             cast_to=object,
         )
 
 
-class AsyncGetJobInfoResource(AsyncAPIResource):
+class AsyncUsageResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncGetJobInfoResourceWithRawResponse:
-        return AsyncGetJobInfoResourceWithRawResponse(self)
+    def with_raw_response(self) -> AsyncUsageResourceWithRawResponse:
+        return AsyncUsageResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncGetJobInfoResourceWithStreamingResponse:
-        return AsyncGetJobInfoResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncUsageResourceWithStreamingResponse:
+        return AsyncUsageResourceWithStreamingResponse(self)
 
-    async def create(
+    async def get_job_info(
         self,
         *,
         job_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -105,49 +105,47 @@
         return await self._post(
             "/usage/get_job_info",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=await async_maybe_transform(
-                    {"job_id": job_id}, get_job_info_create_params.GetJobInfoCreateParams
-                ),
+                query=await async_maybe_transform({"job_id": job_id}, usage_get_job_info_params.UsageGetJobInfoParams),
             ),
             cast_to=object,
         )
 
 
-class GetJobInfoResourceWithRawResponse:
-    def __init__(self, get_job_info: GetJobInfoResource) -> None:
-        self._get_job_info = get_job_info
+class UsageResourceWithRawResponse:
+    def __init__(self, usage: UsageResource) -> None:
+        self._usage = usage
 
-        self.create = to_raw_response_wrapper(
-            get_job_info.create,
+        self.get_job_info = to_raw_response_wrapper(
+            usage.get_job_info,
         )
 
 
-class AsyncGetJobInfoResourceWithRawResponse:
-    def __init__(self, get_job_info: AsyncGetJobInfoResource) -> None:
-        self._get_job_info = get_job_info
+class AsyncUsageResourceWithRawResponse:
+    def __init__(self, usage: AsyncUsageResource) -> None:
+        self._usage = usage
 
-        self.create = async_to_raw_response_wrapper(
-            get_job_info.create,
+        self.get_job_info = async_to_raw_response_wrapper(
+            usage.get_job_info,
         )
 
 
-class GetJobInfoResourceWithStreamingResponse:
-    def __init__(self, get_job_info: GetJobInfoResource) -> None:
-        self._get_job_info = get_job_info
+class UsageResourceWithStreamingResponse:
+    def __init__(self, usage: UsageResource) -> None:
+        self._usage = usage
 
-        self.create = to_streamed_response_wrapper(
-            get_job_info.create,
+        self.get_job_info = to_streamed_response_wrapper(
+            usage.get_job_info,
         )
 
 
-class AsyncGetJobInfoResourceWithStreamingResponse:
-    def __init__(self, get_job_info: AsyncGetJobInfoResource) -> None:
-        self._get_job_info = get_job_info
+class AsyncUsageResourceWithStreamingResponse:
+    def __init__(self, usage: AsyncUsageResource) -> None:
+        self._usage = usage
 
-        self.create = async_to_streamed_response_wrapper(
-            get_job_info.create,
+        self.get_job_info = async_to_streamed_response_wrapper(
+            usage.get_job_info,
         )
```

### Comparing `structifyai-0.1.0a7/src/structify/types/__init__.py` & `structifyai-0.1.0a8/src/structify/types/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 
 from .source import Source as Source
 from .dataset import Dataset as Dataset
 from .kg_entity import KgEntity as KgEntity
 from .new_token import NewToken as NewToken
 from .user_info import UserInfo as UserInfo
 from .is_complete import IsComplete as IsComplete
+from .label_run_params import LabelRunParams as LabelRunParams
 from .run_list_response import RunListResponse as RunListResponse
 from .dataset_descriptor import DatasetDescriptor as DatasetDescriptor
-from .server_information import ServerInformation as ServerInformation
 from .source_list_params import SourceListParams as SourceListParams
 from .dataset_view_params import DatasetViewParams as DatasetViewParams
+from .label_submit_params import LabelSubmitParams as LabelSubmitParams
 from .dataset_create_params import DatasetCreateParams as DatasetCreateParams
 from .dataset_delete_params import DatasetDeleteParams as DatasetDeleteParams
 from .dataset_list_response import DatasetListResponse as DatasetListResponse
 from .dataset_view_response import DatasetViewResponse as DatasetViewResponse
+from .label_submit_response import LabelSubmitResponse as LabelSubmitResponse
 from .document_list_response import DocumentListResponse as DocumentListResponse
 from .document_upload_params import DocumentUploadParams as DocumentUploadParams
 from .dataset_retrieve_params import DatasetRetrieveParams as DatasetRetrieveParams
+from .usage_get_job_info_params import UsageGetJobInfoParams as UsageGetJobInfoParams
 from .document_download_response import DocumentDownloadResponse as DocumentDownloadResponse
 from .structure_run_async_params import StructureRunAsyncParams as StructureRunAsyncParams
+from .label_get_messages_response import LabelGetMessagesResponse as LabelGetMessagesResponse
 from .structure_job_status_params import StructureJobStatusParams as StructureJobStatusParams
 from .structure_is_complete_params import StructureIsCompleteParams as StructureIsCompleteParams
```

### Comparing `structifyai-0.1.0a7/src/structify/types/dataset_create_params.py` & `structifyai-0.1.0a8/src/structify/types/dataset_create_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/types/dataset_descriptor.py` & `structifyai-0.1.0a8/src/structify/types/dataset_descriptor.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/types/source.py` & `structifyai-0.1.0a8/src/structify/types/source.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/src/structify/types/structure_run_async_params.py` & `structifyai-0.1.0a8/src/structify/types/structure_run_async_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/LICENSE` & `structifyai-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a7/pyproject.toml` & `structifyai-0.1.0a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "structifyai"
-version = "0.1.0-alpha.7"
+version = "0.1.0-alpha.8"
 description = "The official Python library for the structify API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Structify", email = "team@structify.ai" },
 ]
 dependencies = [
```

### Comparing `structifyai-0.1.0a7/PKG-INFO` & `structifyai-0.1.0a8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: structifyai
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: The official Python library for the structify API
 Project-URL: Homepage, https://github.com/StructifyAI/structify-python
 Project-URL: Repository, https://github.com/StructifyAI/structify-python
 Author-email: Structify <team@structify.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -63,15 +63,15 @@
 client = Structify(
     # This is the default and can be omitted
     api_key=os.environ.get("STRUCTIFY_API_TOKEN"),
     # defaults to "production".
     environment="deployment",
 )
 
-server_information = client.server.version()
+server_information = client.server.version.retrieve()
 print(server_information.version)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `STRUCTIFY_API_TOKEN="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
@@ -90,15 +90,15 @@
     api_key=os.environ.get("STRUCTIFY_API_TOKEN"),
     # defaults to "production".
     environment="deployment",
 )
 
 
 async def main() -> None:
-    server_information = await client.server.version()
+    server_information = await client.server.version.retrieve()
     print(server_information.version)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
@@ -124,15 +124,15 @@
 ```python
 import structify
 from structify import Structify
 
 client = Structify()
 
 try:
-    client.server.version()
+    client.server.version.retrieve()
 except structify.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except structify.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
 except structify.APIStatusError as e:
     print("Another non-200-range status code was received")
@@ -167,15 +167,15 @@
 # Configure the default for all requests:
 client = Structify(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
-client.with_options(max_retries=5).server.version()
+client.with_options(max_retries=5).server.version.retrieve()
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
 
@@ -190,15 +190,15 @@
 
 # More granular control:
 client = Structify(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-client.with_options(timeout=5.0).server.version()
+client.with_options(timeout=5.0).server.version.retrieve()
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/StructifyAI/structify-python/tree/main/#retries).
 
 ## Advanced
@@ -229,33 +229,33 @@
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
 from structify import Structify
 
 client = Structify()
-response = client.server.with_raw_response.version()
+response = client.server.version.with_raw_response.retrieve()
 print(response.headers.get('X-My-Header'))
 
-server = response.parse()  # get the object that `server.version()` would have returned
-print(server.version)
+version = response.parse()  # get the object that `server.version.retrieve()` would have returned
+print(version.version)
 ```
 
 These methods return an [`APIResponse`](https://github.com/StructifyAI/structify-python/tree/main/src/structify/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/StructifyAI/structify-python/tree/main/src/structify/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
-with client.server.with_streaming_response.version() as response:
+with client.server.version.with_streaming_response.retrieve() as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
```

