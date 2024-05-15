# Comparing `tmp/scorecard_ai-1.0.0b0.tar.gz` & `tmp/scorecard_ai-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecard_ai-1.0.0b0.tar", max compression
+gzip compressed data, was "scorecard_ai-1.0.0b1.tar", max compression
```

## Comparing `scorecard_ai-1.0.0b0.tar` & `scorecard_ai-1.0.0b1.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0    11355 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/LICENSE
--rw-r--r--   0        0        0     3605 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/README.md
--rw-r--r--   0        0        0      657 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/pyproject.toml
--rw-r--r--   0        0        0     3218 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/__init__.py
--rw-r--r--   0        0        0     6675 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/base_client.py
--rw-r--r--   0        0        0     4257 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/client.py
--rw-r--r--   0        0        0     1006 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/api_error.py
--rw-r--r--   0        0        0     1494 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/unchecked_base_model.py
--rw-r--r--   0        0        0      162 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/environment.py
--rw-r--r--   0        0        0      363 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/__init__.py
--rw-r--r--   0        0        0      309 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/forbidden_error.py
--rw-r--r--   0        0        0      297 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/not_found_error.py
--rw-r--r--   0        0        0      308 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/unauthorized_error.py
--rw-r--r--   0        0        0      313 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/py.typed
--rw-r--r--   0        0        0       65 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/run/__init__.py
--rw-r--r--   0        0        0    24116 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/run/client.py
--rw-r--r--   0        0        0       65 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/score/__init__.py
--rw-r--r--   0        0        0    18323 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/score/client.py
--rw-r--r--   0        0        0      255 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/__init__.py
--rw-r--r--   0        0        0    23624 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/client.py
--rw-r--r--   0        0        0      347 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/types/__init__.py
--rw-r--r--   0        0        0      242 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/types/testcase_create_params_custom_inputs_value.py
--rw-r--r--   0        0        0      242 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/types/testcase_create_params_custom_labels_value.py
--rw-r--r--   0        0        0      567 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/__init__.py
--rw-r--r--   0        0        0    21204 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/client.py
--rw-r--r--   0        0        0      812 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/__init__.py
--rw-r--r--   0        0        0      244 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_custom_inputs_value.py
--rw-r--r--   0        0        0      244 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_custom_labels_value.py
--rw-r--r--   0        0        0      245 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_custom_outputs_value.py
--rw-r--r--   0        0        0      154 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_model_debug_info_value.py
--rw-r--r--   0        0        0      151 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_model_params_value.py
--rw-r--r--   0        0        0       65 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testset/__init__.py
--rw-r--r--   0        0        0    35470 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testset/client.py
--rw-r--r--   0        0        0     3222 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/__init__.py
--rw-r--r--   0        0        0      112 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/app_create_run_params.py
--rw-r--r--   0        0        0      113 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/app_test_record_create.py
--rw-r--r--   0        0        0      110 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/app_test_set_create.py
--rw-r--r--   0        0        0      120 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/create_github_workflow_params.py
--rw-r--r--   0        0        0      109 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/create_run_params.py
--rw-r--r--   0        0        0     1165 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/custom_schema.py
--rw-r--r--   0        0        0     1159 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/custom_variable.py
--rw-r--r--   0        0        0      171 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/data_type_enum.py
--rw-r--r--   0        0        0      109 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/execution_params.py
--rw-r--r--   0        0        0      988 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/file_url.py
--rw-r--r--   0        0        0     1447 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/grade.py
--rw-r--r--   0        0        0     1009 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/http_validation_error.py
--rw-r--r--   0        0        0     1244 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/json_object.py
--rw-r--r--   0        0        0      231 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/json_object_input_value.py
--rw-r--r--   0        0        0      232 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/json_object_output_value.py
--rw-r--r--   0        0        0      105 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/model_params.py
--rw-r--r--   0        0        0     1031 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/not_found_error_body.py
--rw-r--r--   0        0        0     1066 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/paginated_testcase_response.py
--rw-r--r--   0        0        0      172 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/role_enum.py
--rw-r--r--   0        0        0     1645 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/run.py
--rw-r--r--   0        0        0      339 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/run_status.py
--rw-r--r--   0        0        0      114 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/score_execution_params.py
--rw-r--r--   0        0        0      168 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/score_status.py
--rw-r--r--   0        0        0      107 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/scoring_params.py
--rw-r--r--   0        0        0     1441 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case.py
--rw-r--r--   0        0        0     1055 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case_create.py
--rw-r--r--   0        0        0      113 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case_create_input.py
--rw-r--r--   0        0        0      214 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case_custom_inputs_value.py
--rw-r--r--   0        0        0      214 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case_custom_labels_value.py
--rw-r--r--   0        0        0      110 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_record_create.py
--rw-r--r--   0        0        0      107 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_set_create.py
--rw-r--r--   0        0        0     2303 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord.py
--rw-r--r--   0        0        0      216 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_custom_inputs_value.py
--rw-r--r--   0        0        0      216 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_custom_labels_value.py
--rw-r--r--   0        0        0      217 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_custom_outputs_value.py
--rw-r--r--   0        0        0      142 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_model_debug_info_value.py
--rw-r--r--   0        0        0      139 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_model_params_value.py
--rw-r--r--   0        0        0     1486 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testset.py
--rw-r--r--   0        0        0     1034 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/unauthenticated_error.py
--rw-r--r--   0        0        0     1035 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/unauthorized_error_body.py
--rw-r--r--   0        0        0     1028 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       80 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/version.py
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 scorecard_ai-1.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     3605 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/README.md
+-rw-r--r--   0        0        0     1113 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3218 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/__init__.py
+-rw-r--r--   0        0        0     6675 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/base_client.py
+-rw-r--r--   0        0        0     4257 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/client.py
+-rw-r--r--   0        0        0     1006 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/api_error.py
+-rw-r--r--   0        0        0     1494 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      162 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/environment.py
+-rw-r--r--   0        0        0      363 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/errors/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/errors/forbidden_error.py
+-rw-r--r--   0        0        0      297 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/errors/not_found_error.py
+-rw-r--r--   0        0        0      308 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      313 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/py.typed
+-rw-r--r--   0        0        0       65 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/run/__init__.py
+-rw-r--r--   0        0        0    24116 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/run/client.py
+-rw-r--r--   0        0        0       65 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/score/__init__.py
+-rw-r--r--   0        0        0    18323 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/score/client.py
+-rw-r--r--   0        0        0     2481 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/telemetry.py
+-rw-r--r--   0        0        0      255 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testcase/__init__.py
+-rw-r--r--   0        0        0    23624 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testcase/client.py
+-rw-r--r--   0        0        0      347 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testcase/types/__init__.py
+-rw-r--r--   0        0        0      242 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testcase/types/testcase_create_params_custom_inputs_value.py
+-rw-r--r--   0        0        0      242 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testcase/types/testcase_create_params_custom_labels_value.py
+-rw-r--r--   0        0        0      567 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testrecord/__init__.py
+-rw-r--r--   0        0        0    21204 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testrecord/client.py
+-rw-r--r--   0        0        0      812 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testrecord/types/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testrecord/types/testrecord_create_params_custom_inputs_value.py
+-rw-r--r--   0        0        0      244 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testrecord/types/testrecord_create_params_custom_labels_value.py
+-rw-r--r--   0        0        0      245 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testrecord/types/testrecord_create_params_custom_outputs_value.py
+-rw-r--r--   0        0        0      154 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testrecord/types/testrecord_create_params_model_debug_info_value.py
+-rw-r--r--   0        0        0      151 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testrecord/types/testrecord_create_params_model_params_value.py
+-rw-r--r--   0        0        0       65 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testset/__init__.py
+-rw-r--r--   0        0        0    35470 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/testset/client.py
+-rw-r--r--   0        0        0     3222 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/app_create_run_params.py
+-rw-r--r--   0        0        0      113 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/app_test_record_create.py
+-rw-r--r--   0        0        0      110 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/app_test_set_create.py
+-rw-r--r--   0        0        0      120 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/create_github_workflow_params.py
+-rw-r--r--   0        0        0      109 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/create_run_params.py
+-rw-r--r--   0        0        0     1165 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/custom_schema.py
+-rw-r--r--   0        0        0     1159 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/custom_variable.py
+-rw-r--r--   0        0        0      171 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/data_type_enum.py
+-rw-r--r--   0        0        0      109 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/execution_params.py
+-rw-r--r--   0        0        0      988 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/file_url.py
+-rw-r--r--   0        0        0     1447 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/grade.py
+-rw-r--r--   0        0        0     1009 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/http_validation_error.py
+-rw-r--r--   0        0        0     1244 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/json_object.py
+-rw-r--r--   0        0        0      231 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/json_object_input_value.py
+-rw-r--r--   0        0        0      232 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/json_object_output_value.py
+-rw-r--r--   0        0        0      105 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/model_params.py
+-rw-r--r--   0        0        0     1031 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/not_found_error_body.py
+-rw-r--r--   0        0        0     1066 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/paginated_testcase_response.py
+-rw-r--r--   0        0        0      172 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/role_enum.py
+-rw-r--r--   0        0        0     1645 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/run.py
+-rw-r--r--   0        0        0      339 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/run_status.py
+-rw-r--r--   0        0        0      114 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/score_execution_params.py
+-rw-r--r--   0        0        0      168 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/score_status.py
+-rw-r--r--   0        0        0      107 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/scoring_params.py
+-rw-r--r--   0        0        0     1441 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/test_case.py
+-rw-r--r--   0        0        0     1055 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/test_case_create.py
+-rw-r--r--   0        0        0      113 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/test_case_create_input.py
+-rw-r--r--   0        0        0      214 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/test_case_custom_inputs_value.py
+-rw-r--r--   0        0        0      214 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/test_case_custom_labels_value.py
+-rw-r--r--   0        0        0      110 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/test_record_create.py
+-rw-r--r--   0        0        0      107 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/test_set_create.py
+-rw-r--r--   0        0        0     2303 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/testrecord.py
+-rw-r--r--   0        0        0      216 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/testrecord_custom_inputs_value.py
+-rw-r--r--   0        0        0      216 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/testrecord_custom_labels_value.py
+-rw-r--r--   0        0        0      217 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/testrecord_custom_outputs_value.py
+-rw-r--r--   0        0        0      142 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/testrecord_model_debug_info_value.py
+-rw-r--r--   0        0        0      139 2024-05-14 06:26:51.008930 scorecard_ai-1.0.0b1/src/scorecard/types/testrecord_model_params_value.py
+-rw-r--r--   0        0        0     1486 2024-05-14 06:26:51.012930 scorecard_ai-1.0.0b1/src/scorecard/types/testset.py
+-rw-r--r--   0        0        0     1034 2024-05-14 06:26:51.012930 scorecard_ai-1.0.0b1/src/scorecard/types/unauthenticated_error.py
+-rw-r--r--   0        0        0     1035 2024-05-14 06:26:51.012930 scorecard_ai-1.0.0b1/src/scorecard/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     1028 2024-05-14 06:26:51.012930 scorecard_ai-1.0.0b1/src/scorecard/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-14 06:26:51.012930 scorecard_ai-1.0.0b1/src/scorecard/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       80 2024-05-14 06:26:51.012930 scorecard_ai-1.0.0b1/src/scorecard/version.py
+-rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 scorecard_ai-1.0.0b1/PKG-INFO
```

### Comparing `scorecard_ai-1.0.0b0/LICENSE` & `scorecard_ai-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/README.md` & `scorecard_ai-1.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/__init__.py` & `scorecard_ai-1.0.0b1/src/scorecard/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/base_client.py` & `scorecard_ai-1.0.0b1/src/scorecard/base_client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/client.py` & `scorecard_ai-1.0.0b1/src/scorecard/client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/core/__init__.py` & `scorecard_ai-1.0.0b1/src/scorecard/core/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/core/client_wrapper.py` & `scorecard_ai-1.0.0b1/src/scorecard/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/core/datetime_utils.py` & `scorecard_ai-1.0.0b1/src/scorecard/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/core/file.py` & `scorecard_ai-1.0.0b1/src/scorecard/core/file.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/core/http_client.py` & `scorecard_ai-1.0.0b1/src/scorecard/core/http_client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/core/jsonable_encoder.py` & `scorecard_ai-1.0.0b1/src/scorecard/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/core/request_options.py` & `scorecard_ai-1.0.0b1/src/scorecard/core/request_options.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/core/unchecked_base_model.py` & `scorecard_ai-1.0.0b1/src/scorecard/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/run/client.py` & `scorecard_ai-1.0.0b1/src/scorecard/run/client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/score/client.py` & `scorecard_ai-1.0.0b1/src/scorecard/score/client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/testcase/client.py` & `scorecard_ai-1.0.0b1/src/scorecard/testcase/client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/testrecord/__init__.py` & `scorecard_ai-1.0.0b1/src/scorecard/testrecord/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/testrecord/client.py` & `scorecard_ai-1.0.0b1/src/scorecard/testrecord/client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/__init__.py` & `scorecard_ai-1.0.0b1/src/scorecard/testrecord/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/testset/client.py` & `scorecard_ai-1.0.0b1/src/scorecard/testset/client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/__init__.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/custom_schema.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/custom_schema.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/custom_variable.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/custom_variable.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/file_url.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/file_url.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/grade.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/grade.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/http_validation_error.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/json_object.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/json_object.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/not_found_error_body.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/not_found_error_body.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/paginated_testcase_response.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/paginated_testcase_response.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/run.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/run.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/test_case.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/test_case.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/test_case_create.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/test_case_create.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/testrecord.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/testrecord.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/testset.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/testset.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/unauthenticated_error.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/unauthenticated_error.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/unauthorized_error_body.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/unauthorized_error_body.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/src/scorecard/types/validation_error.py` & `scorecard_ai-1.0.0b1/src/scorecard/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b0/PKG-INFO` & `scorecard_ai-1.0.0b1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 2.1
 Name: scorecard-ai
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: 
 License: Apache-2.0
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.34.100,<2.0.0)
 Requires-Dist: httpx (>=0.21.2)
+Requires-Dist: openai (>=1.21.2,<2.0.0)
+Requires-Dist: openinference-instrumentation-bedrock (>=0.1.3,<0.2.0)
+Requires-Dist: openinference-instrumentation-dspy (>=0.1.7,<0.2.0)
+Requires-Dist: openinference-instrumentation-langchain (>=0.1.14,<0.2.0)
+Requires-Dist: openinference-instrumentation-llama-index (>=1.3.0,<2.0.0)
+Requires-Dist: openinference-instrumentation-mistralai (>=0.0.5,<0.0.6)
+Requires-Dist: openinference-instrumentation-openai (>=0.1.4,<0.2.0)
+Requires-Dist: opentelemetry-api (>=1.24.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.24.0,<2.0.0)
+Requires-Dist: opentelemetry-sdk (>=1.24.0,<2.0.0)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # Scorecard AI Python Library
```

