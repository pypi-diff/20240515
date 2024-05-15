# Comparing `tmp/antimatter-0.2.2-py3-none-any.whl.zip` & `tmp/antimatter-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,37 +1,54 @@
-Zip file size: 358237 bytes, number of entries: 263
--rw-r--r--  2.0 unx      314 b- defN 20-Apr-16 12:00 antimatter/__init__.py
--rw-r--r--  2.0 unx    11741 b- defN 20-Apr-16 12:00 antimatter/capsule.py
+Zip file size: 385927 bytes, number of entries: 284
+-rw-r--r--  2.0 unx      327 b- defN 20-Apr-16 12:00 antimatter/__init__.py
+-rw-r--r--  2.0 unx    10768 b- defN 20-Apr-16 12:00 antimatter/capsule.py
 -rw-r--r--  2.0 unx      928 b- defN 20-Apr-16 12:00 antimatter/cell_path.py
 -rw-r--r--  2.0 unx     3410 b- defN 20-Apr-16 12:00 antimatter/extra_helper.py
--rw-r--r--  2.0 unx    17576 b- defN 20-Apr-16 12:00 antimatter/session.py
+-rw-r--r--  2.0 unx    25527 b- defN 20-Apr-16 12:00 antimatter/session.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/auth/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/auth/config/__init__.py
+-rw-r--r--  2.0 unx    11557 b- defN 20-Apr-16 12:00 antimatter/auth/config/auth_config.py
+-rw-r--r--  2.0 unx     1930 b- defN 20-Apr-16 12:00 antimatter/auth/config/global_identity.py
+-rw-r--r--  2.0 unx      535 b- defN 20-Apr-16 12:00 antimatter/auth/config/profiles.py
+-rw-r--r--  2.0 unx      429 b- defN 20-Apr-16 12:00 antimatter/auth/config/tokens.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/auth/google/__init__.py
+-rw-r--r--  2.0 unx      495 b- defN 20-Apr-16 12:00 antimatter/auth/google/models.py
 -rw-r--r--  2.0 unx      759 b- defN 20-Apr-16 12:00 antimatter/builders/__init__.py
 -rw-r--r--  2.0 unx     1630 b- defN 20-Apr-16 12:00 antimatter/builders/capability.py
 -rw-r--r--  2.0 unx     2386 b- defN 20-Apr-16 12:00 antimatter/builders/fact_policy.py
 -rw-r--r--  2.0 unx     3338 b- defN 20-Apr-16 12:00 antimatter/builders/read_context.py
 -rw-r--r--  2.0 unx     4831 b- defN 20-Apr-16 12:00 antimatter/builders/read_context_rule.py
--rw-r--r--  2.0 unx     4117 b- defN 20-Apr-16 12:00 antimatter/builders/root_encryption_key.py
--rw-r--r--  2.0 unx     2216 b- defN 20-Apr-16 12:00 antimatter/builders/settings_patch.py
+-rw-r--r--  2.0 unx     4174 b- defN 20-Apr-16 12:00 antimatter/builders/root_encryption_key.py
+-rw-r--r--  2.0 unx     2118 b- defN 20-Apr-16 12:00 antimatter/builders/settings_patch.py
 -rw-r--r--  2.0 unx     4390 b- defN 20-Apr-16 12:00 antimatter/builders/write_context.py
 -rw-r--r--  2.0 unx     2460 b- defN 20-Apr-16 12:00 antimatter/builders/write_context_rule.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/cap_prep/__init__.py
 -rw-r--r--  2.0 unx     3158 b- defN 20-Apr-16 12:00 antimatter/cap_prep/applicator.py
 -rw-r--r--  2.0 unx     3811 b- defN 20-Apr-16 12:00 antimatter/cap_prep/prep.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/cap_prep/tests/__init__.py
 -rw-r--r--  2.0 unx     3875 b- defN 20-Apr-16 12:00 antimatter/cap_prep/tests/test_applicator.py
 -rw-r--r--  2.0 unx     2558 b- defN 20-Apr-16 12:00 antimatter/cap_prep/tests/test_prep.py
--rw-r--r--  2.0 unx    13233 b- defN 20-Apr-16 12:00 antimatter/client/__init__.py
+-rw-r--r--  2.0 unx       66 b- defN 20-Apr-16 12:00 antimatter/capabilities/__init__.py
+-rw-r--r--  2.0 unx     1714 b- defN 20-Apr-16 12:00 antimatter/capabilities/converter.py
+-rw-r--r--  2.0 unx    13909 b- defN 20-Apr-16 12:00 antimatter/client/__init__.py
 -rw-r--r--  2.0 unx    24612 b- defN 20-Apr-16 12:00 antimatter/client/api_client.py
 -rw-r--r--  2.0 unx      674 b- defN 20-Apr-16 12:00 antimatter/client/api_response.py
 -rw-r--r--  2.0 unx    14983 b- defN 20-Apr-16 12:00 antimatter/client/configuration.py
 -rw-r--r--  2.0 unx     5954 b- defN 20-Apr-16 12:00 antimatter/client/exceptions.py
 -rw-r--r--  2.0 unx     9799 b- defN 20-Apr-16 12:00 antimatter/client/rest.py
--rw-r--r--  2.0 unx      105 b- defN 20-Apr-16 12:00 antimatter/client/api/__init__.py
--rw-r--r--  2.0 unx  1079678 b- defN 20-Apr-16 12:00 antimatter/client/api/default_api.py
--rw-r--r--  2.0 unx    12605 b- defN 20-Apr-16 12:00 antimatter/client/models/__init__.py
+-rw-r--r--  2.0 unx      549 b- defN 20-Apr-16 12:00 antimatter/client/api/__init__.py
+-rw-r--r--  2.0 unx    31800 b- defN 20-Apr-16 12:00 antimatter/client/api/account_management_api.py
+-rw-r--r--  2.0 unx   199539 b- defN 20-Apr-16 12:00 antimatter/client/api/authentication_api.py
+-rw-r--r--  2.0 unx   146264 b- defN 20-Apr-16 12:00 antimatter/client/api/capsules_api.py
+-rw-r--r--  2.0 unx   201452 b- defN 20-Apr-16 12:00 antimatter/client/api/contexts_api.py
+-rw-r--r--  2.0 unx   107683 b- defN 20-Apr-16 12:00 antimatter/client/api/encryption_api.py
+-rw-r--r--  2.0 unx   162476 b- defN 20-Apr-16 12:00 antimatter/client/api/general_api.py
+-rw-r--r--  2.0 unx    79499 b- defN 20-Apr-16 12:00 antimatter/client/api/internal_api.py
+-rw-r--r--  2.0 unx   175071 b- defN 20-Apr-16 12:00 antimatter/client/api/policy_api.py
+-rw-r--r--  2.0 unx    12837 b- defN 20-Apr-16 12:00 antimatter/client/models/__init__.py
 -rw-r--r--  2.0 unx     6771 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_entry.py
 -rw-r--r--  2.0 unx     3245 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_entry_create_info.py
 -rw-r--r--  2.0 unx     3085 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_entry_open_info.py
 -rw-r--r--  2.0 unx     5291 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_entry_read_info.py
 -rw-r--r--  2.0 unx     3151 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_results.py
 -rw-r--r--  2.0 unx     3077 b- defN 20-Apr-16 12:00 antimatter/client/models/active_root_encryption_key_id.py
 -rw-r--r--  2.0 unx     3041 b- defN 20-Apr-16 12:00 antimatter/client/models/add_capsule_log_entry_request.py
@@ -88,15 +105,15 @@
 -rw-r--r--  2.0 unx      928 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_provider_type.py
 -rw-r--r--  2.0 unx     3297 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_insert_identity_provider_principal200_response.py
 -rw-r--r--  2.0 unx     2964 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_insert_write_context_regex_rule200_response.py
 -rw-r--r--  2.0 unx    14602 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_peer_config.py
 -rw-r--r--  2.0 unx     2920 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_peer_list.py
 -rw-r--r--  2.0 unx     3461 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_peer_list_peers_inner.py
 -rw-r--r--  2.0 unx     3450 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_policy.py
--rw-r--r--  2.0 unx     5691 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_policy_rule.py
+-rw-r--r--  2.0 unx     7142 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_policy_rule.py
 -rw-r--r--  2.0 unx     3911 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_private_info.py
 -rw-r--r--  2.0 unx     3907 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_public_info.py
 -rw-r--r--  2.0 unx     3037 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_resource_summary.py
 -rw-r--r--  2.0 unx     3367 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_resource_summary_schema_inner.py
 -rw-r--r--  2.0 unx     4011 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_settings.py
 -rw-r--r--  2.0 unx     2865 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_settings_disaster_recovery.py
 -rw-r--r--  2.0 unx     2887 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_settings_patch.py
@@ -124,20 +141,23 @@
 -rw-r--r--  2.0 unx     6166 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_tst_value.py
 -rw-r--r--  2.0 unx     3009 b- defN 20-Apr-16 12:00 antimatter/client/models/key_infos.py
 -rw-r--r--  2.0 unx     6812 b- defN 20-Apr-16 12:00 antimatter/client/models/key_infos_key_information.py
 -rw-r--r--  2.0 unx     3448 b- defN 20-Apr-16 12:00 antimatter/client/models/new_access_log_entry.py
 -rw-r--r--  2.0 unx     4607 b- defN 20-Apr-16 12:00 antimatter/client/models/new_access_log_entry_read_info.py
 -rw-r--r--  2.0 unx     3178 b- defN 20-Apr-16 12:00 antimatter/client/models/new_capability_definition.py
 -rw-r--r--  2.0 unx     2720 b- defN 20-Apr-16 12:00 antimatter/client/models/new_domain.py
+-rw-r--r--  2.0 unx     4777 b- defN 20-Apr-16 12:00 antimatter/client/models/new_domain_policy_rule.py
 -rw-r--r--  2.0 unx     3006 b- defN 20-Apr-16 12:00 antimatter/client/models/new_domain_response.py
 -rw-r--r--  2.0 unx     2683 b- defN 20-Apr-16 12:00 antimatter/client/models/new_fact.py
 -rw-r--r--  2.0 unx     3261 b- defN 20-Apr-16 12:00 antimatter/client/models/new_fact_type_definition.py
 -rw-r--r--  2.0 unx     3131 b- defN 20-Apr-16 12:00 antimatter/client/models/new_fact_type_definition_arguments_inner.py
 -rw-r--r--  2.0 unx     6187 b- defN 20-Apr-16 12:00 antimatter/client/models/new_read_context_config_rule.py
 -rw-r--r--  2.0 unx     9083 b- defN 20-Apr-16 12:00 antimatter/client/models/patch_request_inner.py
+-rw-r--r--  2.0 unx      857 b- defN 20-Apr-16 12:00 antimatter/client/models/policy_rule_operation.py
+-rw-r--r--  2.0 unx      834 b- defN 20-Apr-16 12:00 antimatter/client/models/policy_rule_result.py
 -rw-r--r--  2.0 unx     4070 b- defN 20-Apr-16 12:00 antimatter/client/models/principal_info.py
 -rw-r--r--  2.0 unx     3447 b- defN 20-Apr-16 12:00 antimatter/client/models/principal_summary.py
 -rw-r--r--  2.0 unx     7791 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_config_rule.py
 -rw-r--r--  2.0 unx     6947 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_details.py
 -rw-r--r--  2.0 unx     3003 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_list.py
 -rw-r--r--  2.0 unx     2865 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_parameter.py
 -rw-r--r--  2.0 unx     4935 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_required_hook.py
@@ -169,15 +189,15 @@
 -rw-r--r--  2.0 unx     3000 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_list.py
 -rw-r--r--  2.0 unx     4337 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_regex_rule.py
 -rw-r--r--  2.0 unx     3202 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_regex_tag.py
 -rw-r--r--  2.0 unx      561 b- defN 20-Apr-16 12:00 antimatter/constants/__init__.py
 -rw-r--r--  2.0 unx      227 b- defN 20-Apr-16 12:00 antimatter/constants/capability.py
 -rw-r--r--  2.0 unx      284 b- defN 20-Apr-16 12:00 antimatter/constants/domain_policy.py
 -rw-r--r--  2.0 unx      378 b- defN 20-Apr-16 12:00 antimatter/constants/fact_policy.py
--rw-r--r--  2.0 unx      236 b- defN 20-Apr-16 12:00 antimatter/constants/hooks.py
+-rw-r--r--  2.0 unx      237 b- defN 20-Apr-16 12:00 antimatter/constants/hooks.py
 -rw-r--r--  2.0 unx      358 b- defN 20-Apr-16 12:00 antimatter/constants/identity_provider.py
 -rw-r--r--  2.0 unx     1083 b- defN 20-Apr-16 12:00 antimatter/constants/read_context_rule.py
 -rw-r--r--  2.0 unx      251 b- defN 20-Apr-16 12:00 antimatter/constants/settings_patch.py
 -rw-r--r--  2.0 unx      174 b- defN 20-Apr-16 12:00 antimatter/constants/write_context.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/datatype/__init__.py
 -rw-r--r--  2.0 unx      556 b- defN 20-Apr-16 12:00 antimatter/datatype/datatypes.py
 -rw-r--r--  2.0 unx     1791 b- defN 20-Apr-16 12:00 antimatter/datatype/infer.py
@@ -186,33 +206,33 @@
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/dependencies/__init__.py
 -rw-r--r--  2.0 unx     3340 b- defN 20-Apr-16 12:00 antimatter/dependencies/package_hint.py
 -rw-r--r--  2.0 unx     2489 b- defN 20-Apr-16 12:00 antimatter/dependencies/versions.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/dependencies/tests/__init__.py
 -rw-r--r--  2.0 unx      252 b- defN 20-Apr-16 12:00 antimatter/dependencies/tests/test_package_hint.py
 -rw-r--r--  2.0 unx      339 b- defN 20-Apr-16 12:00 antimatter/dependencies/tests/test_versions.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/errors/__init__.py
--rw-r--r--  2.0 unx     2049 b- defN 20-Apr-16 12:00 antimatter/errors/errors.py
+-rw-r--r--  2.0 unx     2156 b- defN 20-Apr-16 12:00 antimatter/errors/errors.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/fieldtype/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 20-Apr-16 12:00 antimatter/fieldtype/converters.py
+-rw-r--r--  2.0 unx     3677 b- defN 20-Apr-16 12:00 antimatter/fieldtype/converters.py
 -rw-r--r--  2.0 unx      567 b- defN 20-Apr-16 12:00 antimatter/fieldtype/fieldtypes.py
 -rw-r--r--  2.0 unx     1324 b- defN 20-Apr-16 12:00 antimatter/fieldtype/infer.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/fieldtype/tests/__init__.py
 -rw-r--r--  2.0 unx     1268 b- defN 20-Apr-16 12:00 antimatter/fieldtype/tests/test_fieldtypes.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/filetype/__init__.py
--rw-r--r--  2.0 unx     3186 b- defN 20-Apr-16 12:00 antimatter/filetype/extract.py
+-rw-r--r--  2.0 unx     3142 b- defN 20-Apr-16 12:00 antimatter/filetype/extract.py
 -rw-r--r--  2.0 unx     2607 b- defN 20-Apr-16 12:00 antimatter/filetype/infer.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/__init__.py
 -rw-r--r--  2.0 unx     1491 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/test_filetypes.py
 -rw-r--r--  2.0 unx     1446 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/test_infer.py
 -rw-r--r--  2.0 unx      176 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data-ndjson.json
 -rw-r--r--  2.0 unx      103 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data.csv
 -rw-r--r--  2.0 unx      194 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data.json
 -rw-r--r--  2.0 unx     2913 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data.parquet
 -rw-r--r--  2.0 unx      179 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data.txt
--rw-r--r--  2.0 unx     1377 b- defN 20-Apr-16 12:00 antimatter/handlers/__init__.py
+-rw-r--r--  2.0 unx     1473 b- defN 20-Apr-16 12:00 antimatter/handlers/__init__.py
 -rw-r--r--  2.0 unx     3602 b- defN 20-Apr-16 12:00 antimatter/handlers/base.py
 -rw-r--r--  2.0 unx     2662 b- defN 20-Apr-16 12:00 antimatter/handlers/dict_list.py
 -rw-r--r--  2.0 unx     2100 b- defN 20-Apr-16 12:00 antimatter/handlers/dictionary.py
 -rw-r--r--  2.0 unx     8735 b- defN 20-Apr-16 12:00 antimatter/handlers/langchain.py
 -rw-r--r--  2.0 unx     5001 b- defN 20-Apr-16 12:00 antimatter/handlers/pandas_dataframe.py
 -rw-r--r--  2.0 unx     5617 b- defN 20-Apr-16 12:00 antimatter/handlers/pytorch_dataloader.py
 -rw-r--r--  2.0 unx     1639 b- defN 20-Apr-16 12:00 antimatter/handlers/scalar.py
@@ -225,41 +245,42 @@
 -rw-r--r--  2.0 unx     1522 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_scalar.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/location/__init__.py
 -rw-r--r--  2.0 unx      791 b- defN 20-Apr-16 12:00 antimatter/location/infer.py
 -rw-r--r--  2.0 unx      290 b- defN 20-Apr-16 12:00 antimatter/location/locations.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/location/tests/__init__.py
 -rw-r--r--  2.0 unx      681 b- defN 20-Apr-16 12:00 antimatter/location/tests/test_infer.py
 -rw-r--r--  2.0 unx      118 b- defN 20-Apr-16 12:00 antimatter/requirements/all.txt
--rw-r--r--  2.0 unx      220 b- defN 24-Apr-15 17:08 antimatter/requirements/core.txt
+-rw-r--r--  2.0 unx      227 b- defN 24-May-14 23:57 antimatter/requirements/core.txt
 -rw-r--r--  2.0 unx       12 b- defN 20-Apr-16 12:00 antimatter/requirements/dev.txt
 -rw-r--r--  2.0 unx       66 b- defN 20-Apr-16 12:00 antimatter/requirements/langchain-huggingface.txt
 -rw-r--r--  2.0 unx       36 b- defN 20-Apr-16 12:00 antimatter/requirements/langchain.txt
 -rw-r--r--  2.0 unx       14 b- defN 20-Apr-16 12:00 antimatter/requirements/numpy.txt
 -rw-r--r--  2.0 unx       24 b- defN 20-Apr-16 12:00 antimatter/requirements/pandas.txt
 -rw-r--r--  2.0 unx       38 b- defN 20-Apr-16 12:00 antimatter/requirements/pyarrow.txt
 -rw-r--r--  2.0 unx       11 b- defN 20-Apr-16 12:00 antimatter/requirements/pytorch.txt
 -rw-r--r--  2.0 unx      949 b- defN 20-Apr-16 12:00 antimatter/session_mixins/__init__.py
--rw-r--r--  2.0 unx     3126 b- defN 20-Apr-16 12:00 antimatter/session_mixins/capability_mixin.py
--rw-r--r--  2.0 unx     4676 b- defN 20-Apr-16 12:00 antimatter/session_mixins/capsule_mixin.py
--rw-r--r--  2.0 unx    14365 b- defN 20-Apr-16 12:00 antimatter/session_mixins/domain_mixin.py
--rw-r--r--  2.0 unx     1044 b- defN 20-Apr-16 12:00 antimatter/session_mixins/encryption_mixin.py
--rw-r--r--  2.0 unx     5639 b- defN 20-Apr-16 12:00 antimatter/session_mixins/fact_mixin.py
--rw-r--r--  2.0 unx    11226 b- defN 20-Apr-16 12:00 antimatter/session_mixins/general_mixin.py
--rw-r--r--  2.0 unx    10686 b- defN 20-Apr-16 12:00 antimatter/session_mixins/identity_provider_mixin.py
--rw-r--r--  2.0 unx     5727 b- defN 20-Apr-16 12:00 antimatter/session_mixins/policy_rule_mixin.py
--rw-r--r--  2.0 unx     5201 b- defN 20-Apr-16 12:00 antimatter/session_mixins/read_context_mixin.py
--rw-r--r--  2.0 unx     4982 b- defN 20-Apr-16 12:00 antimatter/session_mixins/root_encryption_key_mixin.py
--rw-r--r--  2.0 unx     2298 b- defN 20-Apr-16 12:00 antimatter/session_mixins/token.py
--rw-r--r--  2.0 unx     1614 b- defN 20-Apr-16 12:00 antimatter/session_mixins/verification_mixin.py
--rw-r--r--  2.0 unx     5286 b- defN 20-Apr-16 12:00 antimatter/session_mixins/write_context_mixin.py
+-rw-r--r--  2.0 unx     3391 b- defN 20-Apr-16 12:00 antimatter/session_mixins/capability_mixin.py
+-rw-r--r--  2.0 unx     5037 b- defN 20-Apr-16 12:00 antimatter/session_mixins/capsule_mixin.py
+-rw-r--r--  2.0 unx    14894 b- defN 20-Apr-16 12:00 antimatter/session_mixins/domain_mixin.py
+-rw-r--r--  2.0 unx     1141 b- defN 20-Apr-16 12:00 antimatter/session_mixins/encryption_mixin.py
+-rw-r--r--  2.0 unx     6208 b- defN 20-Apr-16 12:00 antimatter/session_mixins/fact_mixin.py
+-rw-r--r--  2.0 unx    11843 b- defN 20-Apr-16 12:00 antimatter/session_mixins/general_mixin.py
+-rw-r--r--  2.0 unx    12478 b- defN 20-Apr-16 12:00 antimatter/session_mixins/identity_provider_mixin.py
+-rw-r--r--  2.0 unx     6063 b- defN 20-Apr-16 12:00 antimatter/session_mixins/policy_rule_mixin.py
+-rw-r--r--  2.0 unx     6281 b- defN 20-Apr-16 12:00 antimatter/session_mixins/read_context_mixin.py
+-rw-r--r--  2.0 unx     5713 b- defN 20-Apr-16 12:00 antimatter/session_mixins/root_encryption_key_mixin.py
+-rw-r--r--  2.0 unx     2265 b- defN 20-Apr-16 12:00 antimatter/session_mixins/token.py
+-rw-r--r--  2.0 unx     1727 b- defN 20-Apr-16 12:00 antimatter/session_mixins/verification_mixin.py
+-rw-r--r--  2.0 unx     5977 b- defN 20-Apr-16 12:00 antimatter/session_mixins/write_context_mixin.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/session_mixins/serializers/__init__.py
 -rw-r--r--  2.0 unx     1202 b- defN 20-Apr-16 12:00 antimatter/session_mixins/serializers/identity_details.py
 -rw-r--r--  2.0 unx       56 b- defN 20-Apr-16 12:00 antimatter/tags/__init__.py
 -rw-r--r--  2.0 unx     1458 b- defN 20-Apr-16 12:00 antimatter/tags/tag.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/tests/__init__.py
--rw-r--r--  2.0 unx     8076 b- defN 20-Apr-16 12:00 antimatter/tests/test_capsule.py
+-rw-r--r--  2.0 unx     3444 b- defN 20-Apr-16 12:00 antimatter/tests/test_capabilities.py
+-rw-r--r--  2.0 unx     8051 b- defN 20-Apr-16 12:00 antimatter/tests/test_capsule.py
 -rw-r--r--  2.0 unx      281 b- defN 20-Apr-16 12:00 antimatter/tests/test_cell_path.py
--rw-r--r--  2.0 unx     1794 b- defN 24-Apr-15 17:08 antimatter-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 17:08 antimatter-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-15 17:08 antimatter-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    26829 b- defN 24-Apr-15 17:08 antimatter-0.2.2.dist-info/RECORD
-263 files, 1977471 bytes uncompressed, 314271 bytes compressed:  84.1%
+-rw-r--r--  2.0 unx     1815 b- defN 24-May-14 23:57 antimatter-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 23:57 antimatter-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-14 23:57 antimatter-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    28821 b- defN 24-May-14 23:57 antimatter-1.0.0.dist-info/RECORD
+284 files, 2047187 bytes uncompressed, 338767 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -9,14 +9,38 @@
 
 Filename: antimatter/extra_helper.py
 Comment: 
 
 Filename: antimatter/session.py
 Comment: 
 
+Filename: antimatter/auth/__init__.py
+Comment: 
+
+Filename: antimatter/auth/config/__init__.py
+Comment: 
+
+Filename: antimatter/auth/config/auth_config.py
+Comment: 
+
+Filename: antimatter/auth/config/global_identity.py
+Comment: 
+
+Filename: antimatter/auth/config/profiles.py
+Comment: 
+
+Filename: antimatter/auth/config/tokens.py
+Comment: 
+
+Filename: antimatter/auth/google/__init__.py
+Comment: 
+
+Filename: antimatter/auth/google/models.py
+Comment: 
+
 Filename: antimatter/builders/__init__.py
 Comment: 
 
 Filename: antimatter/builders/capability.py
 Comment: 
 
 Filename: antimatter/builders/fact_policy.py
@@ -54,14 +78,20 @@
 
 Filename: antimatter/cap_prep/tests/test_applicator.py
 Comment: 
 
 Filename: antimatter/cap_prep/tests/test_prep.py
 Comment: 
 
+Filename: antimatter/capabilities/__init__.py
+Comment: 
+
+Filename: antimatter/capabilities/converter.py
+Comment: 
+
 Filename: antimatter/client/__init__.py
 Comment: 
 
 Filename: antimatter/client/api_client.py
 Comment: 
 
 Filename: antimatter/client/api_response.py
@@ -75,15 +105,36 @@
 
 Filename: antimatter/client/rest.py
 Comment: 
 
 Filename: antimatter/client/api/__init__.py
 Comment: 
 
-Filename: antimatter/client/api/default_api.py
+Filename: antimatter/client/api/account_management_api.py
+Comment: 
+
+Filename: antimatter/client/api/authentication_api.py
+Comment: 
+
+Filename: antimatter/client/api/capsules_api.py
+Comment: 
+
+Filename: antimatter/client/api/contexts_api.py
+Comment: 
+
+Filename: antimatter/client/api/encryption_api.py
+Comment: 
+
+Filename: antimatter/client/api/general_api.py
+Comment: 
+
+Filename: antimatter/client/api/internal_api.py
+Comment: 
+
+Filename: antimatter/client/api/policy_api.py
 Comment: 
 
 Filename: antimatter/client/models/__init__.py
 Comment: 
 
 Filename: antimatter/client/models/access_log_entry.py
 Comment: 
@@ -381,14 +432,17 @@
 
 Filename: antimatter/client/models/new_capability_definition.py
 Comment: 
 
 Filename: antimatter/client/models/new_domain.py
 Comment: 
 
+Filename: antimatter/client/models/new_domain_policy_rule.py
+Comment: 
+
 Filename: antimatter/client/models/new_domain_response.py
 Comment: 
 
 Filename: antimatter/client/models/new_fact.py
 Comment: 
 
 Filename: antimatter/client/models/new_fact_type_definition.py
@@ -399,14 +453,20 @@
 
 Filename: antimatter/client/models/new_read_context_config_rule.py
 Comment: 
 
 Filename: antimatter/client/models/patch_request_inner.py
 Comment: 
 
+Filename: antimatter/client/models/policy_rule_operation.py
+Comment: 
+
+Filename: antimatter/client/models/policy_rule_result.py
+Comment: 
+
 Filename: antimatter/client/models/principal_info.py
 Comment: 
 
 Filename: antimatter/client/models/principal_summary.py
 Comment: 
 
 Filename: antimatter/client/models/read_context_config_rule.py
@@ -765,26 +825,29 @@
 
 Filename: antimatter/tags/tag.py
 Comment: 
 
 Filename: antimatter/tests/__init__.py
 Comment: 
 
+Filename: antimatter/tests/test_capabilities.py
+Comment: 
+
 Filename: antimatter/tests/test_capsule.py
 Comment: 
 
 Filename: antimatter/tests/test_cell_path.py
 Comment: 
 
-Filename: antimatter-0.2.2.dist-info/METADATA
+Filename: antimatter-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: antimatter-0.2.2.dist-info/WHEEL
+Filename: antimatter-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: antimatter-0.2.2.dist-info/top_level.txt
+Filename: antimatter-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: antimatter-0.2.2.dist-info/RECORD
+Filename: antimatter-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## antimatter/__init__.py

```diff
@@ -1,6 +1,6 @@
 from antimatter.builders import *
 from antimatter.tags import CapsuleTag, ColumnTag, SpanTag, TagType
 from antimatter.cell_path import cell_path
 from antimatter.datatype.datatypes import Datatype
 from antimatter.fieldtype.fieldtypes import FieldType
-from antimatter.session import Session, new_domain, with_domain
+from antimatter.session import Session, new_domain, with_domain, load_domain
```

## antimatter/capsule.py

```diff
@@ -11,69 +11,61 @@
 from antimatter.datatype.datatypes import Datatype
 from antimatter.extra_helper import META_TYPE_KEY
 from antimatter.fieldtype import converters
 from antimatter.tags import SpanTag, ColumnTag, CapsuleTag
 
 
 class CapsuleBindings:
-    def __init__(self, capsule_session: ae.PySessionCapsule, failed: List[str]):
+    def __init__(self, capsule_session: ae.PySessionCapsule):
         """
         CapsuleBindings holds the capsule session for the underlying Antimatter Capsule.
 
         :param capsule_session: The bundle session for the underlying Antimatter Capsule Bundle
         :param failed: A list of capsules in the Antimatter Capsule Bundle that could not be opened.
         """
         self._capsule_session = capsule_session
-        self._failed = failed
+        if capsule_session is not None:
+            self.capsule_tags, self.column_names, self.column_tags, self.redacted_data, self.data_span_tags, self.extra_info = capsule_session.read_all_with_tags([])
 
-    def read_extras(self, read_params: Dict[List[str], List[str]]) -> List[str]:
+    def read_extras(self) -> List[str]:
         """
         Get the extras field stored in the capsule.
 
-        :param read_params: The parameters for reading the capsule's data.
         :return: The extras string.
         """
-        # TODO: Do we really want to read_all everytime? Should we cache this instead? It seems expensive.
-        _, _, _, extra_info = self._capsule_session.read_all(read_params)
-        return extra_info
+        return self.extra_info
 
-    def read_all(self, read_params: Dict) -> Tuple[List[str], List[List[bytes]], str]:
+    def read_all(self) -> Tuple[List[str], List[List[bytes]], str]:
         """
         Get the column definitions, redacted data and extras from the underlying capsule.
 
-        :param read_params: The parameters for reading the capsule's data.
         :return: The column definition list, a 2D list of list of string containing the redacted data, and the extras
                  string.
         """
-        # TODO: handle column_tags coming back.
-        column_names, _, redacted_data, extra_info = self._capsule_session.read_all(read_params or {})             
-        return column_names, redacted_data, extra_info
+        return self.column_names, self.redacted_data, self.extra_info
 
-    def read_all_with_tags(self, read_params: Dict) -> Tuple[
+    def read_all_with_tags(self) -> Tuple[
             List[ae.PyTag], 
             List[str], 
             List[List[ae.PyTag]], 
             List[List[List[bytes]]], 
             List[List[List[ae.PySpanTag]]], 
             str,
         ]:
         """
         Get the tag information (capsule, column, etc.), column definitions, redacted 
         data and extras from the underlying capsule. This method is meant to provide
         insight into what is being tagged along with the corresponding tag that was
         applied.
 
-        :param read_params: The parameters for reading the capsule's data.
         :return: The list of capsule tags, column definition list, list of column tags,
                  a 2D list of list of string containing the redacted data, a list of data span 
                  tags, and the extras string.
         """
-        capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info = \
-            self._capsule_session.read_all_with_tags(read_params or {})
-        return capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info
+        return self.capsule_tags, self.column_names, self.column_tags, self.redacted_data, self.data_span_tags, self.extra_info
 
     def capsule_ids(self) -> List[str]:
         """
         Get a list capsule IDs associated with this CapsuleBinding.
         """
         return self._capsule_session.capsule_ids()
 
@@ -111,46 +103,44 @@
         """
         Get the capsule binding for the underlying Antimatter Capsule.
 
         :return: The Antimatter Capsule binding.
         """
         return self._capsule
 
-    def data(self, read_params: Dict[str, str] = None, **kwargs) -> Any:
+    def data(self, **kwargs) -> Any:
         """
         Get the data from the underlying Antimatter Capsule using the supplied
         read parameters. This will raise an error if the capsule is sealed.
 
-        :param read_params: The parameters for reading the capsule's data.
         :param kwargs: The extra arguments to pass to the data handler.
         :return: The data in its default format.
         """
-        column_names, rows, extra = self._capsule.read_all(read_params)
+        column_names, rows, extra = self._capsule.read_all()
 
         extra = json.loads(extra)
         default_dt_val = extra.get(META_TYPE_KEY, Datatype.Unknown.value)
         default_dt = Datatype(default_dt_val)
 
         h = handlers.factory(default_dt)  # TODO: try/except
         e = extra_helper.extra_for_capsule(default_dt, extra, **kwargs)
         d = h.from_generic(column_names, rows, e)
         return d
 
-    def data_as(self, dt: Union[Datatype, str], read_params: Dict[str, str] = None, **kwargs) -> Any:
+    def data_as(self, dt: Union[Datatype, str], **kwargs) -> Any:
         """
         Get the data from the underlying Antimatter Capsule using the supplied
         read parameters. This will raise an error if the capsule is sealed.
 
-        :param read_params: The parameters for reading the capsule's data.
         :param dt: The datatype to use for reading data.
         :param kwargs: The extra arguments to pass to the data handler.
         :return: The data in the specified format.
         """
         dt = Datatype(dt)
-        column_names, rows, extra = self._capsule.read_all(read_params)
+        column_names, rows, extra = self._capsule.read_all()
         extra = json.loads(extra)
 
         h = handlers.factory(dt)  # TODO: try/except
         e = extra_helper.extra_for_capsule(dt, extra, **kwargs)
         d = h.from_generic(column_names, rows, e)
         return d
 
@@ -196,32 +186,31 @@
                         start=t.start, end=t.end, tag_type=t.tag.tag_type, tag_value="")
                 for t in data_span_tags[rowidx][colidx]
             ],
             "row": rowidx,
         }
         return item
 
-    def data_with_tags(self, read_params: Dict[str, str]=None, column_major: bool=False, inline=False, **kwargs) -> List[List[Dict]]:
+    def data_with_tags(self, column_major: bool=False, inline=False, **kwargs) -> List[List[Dict]]:
         """
         Get the data and related tag information from the underlying Antimatter 
         Capsule using the supplied read parameters. This will raise an error if 
         the capsule is sealed.
 
-        :param read_params: The parameters for reading the capsule's data.
         :param column_major: The orientation to use for the return list. A value of True
                      results in data being grouped together by column versus a value
                      of False which results in data being grouped together by row.
         :param inline: The option to markup the data with SpanTag information similar
                        to applying HTML blocks.
         :param kwargs: The extra arguments to pass to the data handler.
         :return: The list of dictionaries providing insight to the Tags that were
                  found within a data item.
         """
         capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info = \
-            self._capsule.read_all_with_tags(read_params)
+            self._capsule.read_all_with_tags()
         
         extra_info = json.loads(extra_info)
 
         if not column_major:  
             iterate_func = self._iterate_rows_first
         else:
             iterate_func = self._iterate_columns_first
```

## antimatter/session.py

```diff
@@ -1,33 +1,210 @@
 import json
 import os
+import sys
 from dataclasses import dataclass
-from typing import Any, Callable, List, Optional, Union
+from typing import Any, Callable, List, Optional, Union, Dict
+from urllib.parse import quote_plus, urlparse
 
 import antimatter_engine as am
 
+from antimatter.auth.config.auth_config import AuthConfig
 from antimatter.filetype.extract import extract_from_file
 from antimatter.filetype.infer import infer_filetype
 
 import antimatter.client as openapi_client
 import antimatter.handlers as handlers
 from antimatter.cap_prep.prep import Preparer
 from antimatter.tags import ColumnTag, SpanTag
 from antimatter.capsule import Capsule, CapsuleBindings
-from antimatter.client import ApiClient, Configuration, DefaultApi
+from antimatter.client import ApiClient, Configuration, GeneralApi
 from antimatter.datatype.datatypes import Datatype
 from antimatter.datatype.infer import infer_datatype
 from antimatter.errors import errors
 from antimatter.extra_helper import extra_for_session
 from antimatter.session_mixins import *
 
 # #version
 API_TARGET_VERSION = "v1"
 
 
+def new_domain(
+    email: str,
+    display_name: Optional[str] = None,
+    config_path: Optional[str] = None,
+    add_to_config: bool = True,
+    make_active: bool = False,
+) -> "Session":
+    """
+    Create a new domain with the provided email as the admin contact. A
+    verification email will be sent to that email. Verification must be completed
+    before the Antimatter API can be interacted with.
+
+    :param email: The admin contact email used for email verification
+    :param display_name: The display name for the new domain
+    :param config_path: The path to the domain profile config file; default is ~/.antimatter/config
+    :param add_to_config: Whether to add the new domain to the config file; default is True
+    :param make_active: Whether to make the new domain the active profile in the config file; default is False
+    :return: A Session holding the newly created domain_id and api_key
+    """
+    host = os.getenv("ANTIMATTER_API_URL", "https://api.antimatter.io")
+    client = GeneralApi(
+        api_client=ApiClient(
+            configuration=Configuration(
+                host=f"{host}/{API_TARGET_VERSION}",
+            )
+        )
+    )
+    dm = client.domain_add_new(openapi_client.NewDomain(admin_email=email, display_name=display_name))
+
+    # Try to create the Session before potentially adding to the config file - if creating
+    # the Session produces an erroneous result, we don't want to add it to the config
+    sess = Session(domain=dm.id, api_key=dm.api_key, email=email)
+
+    if add_to_config or make_active:
+        auth_conf = AuthConfig.from_file(config_path)
+        try:
+            auth_conf.add_profile(
+                domain_id=dm.id,
+                api_key=dm.api_key,
+                name=display_name,
+                mark_active=make_active,
+                write_to_file=True,
+            )
+        except Exception as e:
+            # Catch any failures as we don't want the caller to lose the domain ID and API key
+            # if saving to a config file goes wrong
+            print(f"error saving profile to config file: {e}", file=sys.stderr)
+
+    # Finally, return the Session
+    return sess
+
+
+def with_domain(domain_id: str, api_key: str) -> "Session":
+    """
+    Create a session using an existing domain ID and API key.
+
+    :param domain_id: The domain ID
+    :param api_key: The API key for the domain
+    :return: A Session holding the existing domain_id and api_key
+    """
+    return load_domain(domain_id=domain_id, api_key=api_key)
+
+
+def load_domain(
+    domain_id: Optional[str] = None,
+    api_key: Optional[str] = None,
+    display_name: Optional[str] = None,
+    config_path: Optional[str] = None,
+    add_to_config: bool = False,
+    make_active: bool = False,
+) -> "Session":
+    """
+    Load an existing domain. There are several different ways to specify the domain
+    credentials to use, from highest to lowest priority.
+
+    1. Using display name. If this is present, it will attempt to load a profile
+    from the config file with this name.
+    2. Using domain_id and api_key as the credentials.
+    3. Using only domain_id. If this is present, it will attempt to load a profile
+    from the config file that matches this domain ID.
+
+    If domain_id is not provided, this will check the ANTIMATTER_DOMAIN_ID env var
+    for a domain ID.
+
+    If api_key is not provided, this will check the ANTIMATTER_API_KEY env var for
+    an API key.
+
+    The config file is by default expected to exist at ~/.antimatter/config, but an
+    override location can be provided with the config_path argument, or the
+    ANTIMATTER_CONFIG_PATH env var.
+
+    By default, loading an existing domain will not add the credentials to the profile
+    auth config file. Set add_to_config to True to add this domain to the config. To
+    make this domain the active profile, set make_active to True. Note that setting
+    make_active to True implicitly sets add_to_config to True.
+
+    :param domain_id: The domain ID of the domain to load
+    :param api_key: The API key of the domain to load
+    :param display_name: The display name in the auth config file of the domain to load
+    :param config_path: The path to the domain profile config file; default is ~/.antimatter/config
+    :param add_to_config: Whether to add the domain to the config file; default is False
+    :param make_active: Whether to make the domain the active profile in the config file; default is False
+    :return: A Session holding the existing domain_id and api_key
+    """
+    if not domain_id:
+        domain_id = os.getenv("ANTIMATTER_DOMAIN_ID", None)
+    if not api_key:
+        api_key = os.getenv("ANTIMATTER_API_KEY", None)
+    if not config_path:
+        config_path = os.getenv("ANTIMATTER_CONFIG_PATH", None)
+
+    # If a domain and API key are available, and no display name was specified, and no flags
+    # have been set to save to the config file, skip loading the auth config profiles
+    # because we won't use them
+    if not display_name and domain_id and api_key and not add_to_config and not make_active:
+        auth_conf = AuthConfig()
+    else:
+        auth_conf = AuthConfig.from_file(config_path)
+
+    name = None
+    from_conf = False
+
+    # If a display name is specified, load that profile
+    if display_name:
+        pconf = auth_conf.get_profile(name=display_name)
+        if pconf is None:
+            raise errors.SessionLoadError(f"could not find profile {display_name} in profile config")
+        name = pconf.name
+        domain_id = pconf.domain_id
+        api_key = pconf.api_key
+        from_conf = True
+    # If a domain ID is specified, but not an API key, load the profile with that domain ID
+    elif domain_id and not api_key:
+        pconf = auth_conf.get_profile(domain_id=domain_id)
+        if pconf is None:
+            raise errors.SessionLoadError(f"could not find profile with domain ID {domain_id} in profile config")
+        name = pconf.name
+        api_key = pconf.api_key
+        from_conf = True
+    # If no display name or domain ID were specified, load the active profile from the auth config
+    # We deliberately aren't confirming the API key is unset here, due in part to the issue where the
+    # Session sets the env var
+    elif not domain_id:
+        pconf = auth_conf.get_profile()
+        if pconf is None:
+            raise errors.SessionLoadError("no active profile found")
+        name = pconf.name
+        domain_id = pconf.domain_id
+        api_key = pconf.api_key
+        from_conf = True
+
+    # If we get to this point without a domain ID and API key, we somehow failed to load the domain
+    if not domain_id or not api_key:
+        raise errors.SessionLoadError("failed to load domain - no domain ID or API key found")
+
+    # Try to initialize the Session before potentially adding to the config file - if initializing
+    # the Session produces an erroneous result, we don't want to add it to the config
+    sess = Session(domain=domain_id, api_key=api_key)
+
+    # If the flag is set to add to the auth config, and the profile didn't already come from the
+    # auth config, then write it to the config, marking as active if that flag is also set
+    if (add_to_config or make_active) and not from_conf:
+        auth_conf.add_profile(
+            domain_id=domain_id,
+            api_key=api_key,
+            name=name,
+            mark_active=make_active,
+            write_to_file=True,
+        )
+
+    # Finally, return the session
+    return sess
+
+
 @dataclass
 class EncapsulateResponse:
     """
     EncapsulateResponse contains metadata from encapsulating data, including
     the capsule ID or IDs, and the raw bytes if the capsule was not exported.
     """
     capsule_ids: List[str]
@@ -53,46 +230,14 @@
         """
         Save the capsule to a file
         """
         with open(filename, "wb") as f:
             f.write(self.raw)
 
 
-def new_domain(email: str) -> "Session":
-    """
-    Create a new domain with the provided email as the admin contact. A
-    verification email will be sent to that email. Verification must be completed
-    before the Antimatter API can be interacted with.
-
-    :param email: The admin contact email used for email verification
-    :return: A Session holding the newly created domain_id and api_key
-    """
-    host = os.getenv("ANTIMATTER_API_URL", "https://api.antimatter.io")
-    client = DefaultApi(
-        api_client=ApiClient(
-            configuration=Configuration(
-                host=f"{host}/{API_TARGET_VERSION}",
-            )
-        )
-    )
-    dm = client.domain_add_new(openapi_client.NewDomain(admin_email=email))
-    return Session(domain=dm.id, api_key=dm.api_key, email=email)
-
-
-def with_domain(domain_id: str, api_key: str) -> "Session":
-    """
-    Create a session using an existing domain ID and API key.
-
-    :param domain_id: The domain ID
-    :param api_key: The API key for the domain
-    :return: A Session holding the existing domain_id and api_key
-    """
-    return Session(domain=domain_id, api_key=api_key)
-
-
 class Session(
     CapabilityMixin, CapsuleMixin, DomainMixin, EncryptionMixin,
     FactMixin, GeneralMixin, IdentityProviderMixin, PolicyRuleMixin,
     ReadContextMixin, WriteContextMixin, VerificationMixin, RootEncryptionKeyMixin
 ):
     """
     The Session establishes auth and the domain you are working with, providing
@@ -132,15 +277,15 @@
         # TODO: handle any resources/auth; call python rust wrapper to create a rust session
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         # TODO: close any resources/auth; call python rust wrapper to close the rust session
         return
 
-    def _get_client(self) -> DefaultApi:
+    def _get_client(self) -> ApiClient:
         return self._client
 
     def config(self):
         """
         Returns the configuration of this Session
         """
         return {
@@ -158,19 +303,17 @@
 
         :param default_values_on_failure: Whether to set default client and session values on failure
         :return: True if the client and session were authenticated
         """
         host = os.getenv("ANTIMATTER_API_URL", "https://api.antimatter.io")
         try:
             self._session = am.PySession(self._domain)
-            self._client = DefaultApi(
-                api_client=ApiClient(
-                    configuration=Configuration(
-                        host=f"{host}/{API_TARGET_VERSION}", access_token=self._api_key
-                    )
+            self._client = ApiClient(
+                configuration=Configuration(
+                    host=f"{host}/{API_TARGET_VERSION}", access_token=self._api_key,
                 )
             )
         except Exception as e:
             str_e = str(e).lower()
             # Catch the error where the domain is still awaiting verification
             if "code: 401" not in str_e or "domain contains no verified contacts" not in str_e:
                 if "domain auth error" in str_e:
@@ -189,30 +332,25 @@
                     else:
                         raise
                 else:
                     raise
             if default_values_on_failure:
                 # Set up a default empty session and client without auth
                 self._session = None
-                self._client = DefaultApi(
-                    api_client=ApiClient(
-                        configuration=Configuration(
-                            host=f"{host}/{API_TARGET_VERSION}"
-                        )
-                    )
-                )
+                self._client = ApiClient(configuration=Configuration(host=f"{host}/{API_TARGET_VERSION}"))
             return False
 
         return True
 
     def load_capsule(
         self,
         path: Optional[str] = None,
         data: Optional[Union[bytes, EncapsulateResponse]] = None,
         read_context: str = None,
+        read_params: Dict[str, str] = {},
     ) -> Optional[Capsule]:
         """
         load_capsule creates a capsule, extracting data from an Antimatter
         Capsule binary blob, either provided in raw bytes or as a string path
         to a local or remote file.
 
         If the `as_datatype` parameter is supplied and the data is a binary blob
@@ -234,17 +372,16 @@
         if not path and not data:
             raise ValueError("specify a 'path' or the raw 'data' when loading a capsule")
 
         if data and isinstance(data, EncapsulateResponse):
             data = data.raw
 
         try:
-            (capsule_session, failed_capsules) = self._session.open_capsule(path, data, read_context)
-            cap = CapsuleBindings(capsule_session, failed_capsules)
-
+            capsule_session = self._session.open_capsule(read_context, read_params, path, data)
+            cap = CapsuleBindings(capsule_session)
             capsule = Capsule(capsule_binding=cap)
             return capsule
         except Exception as e:
             str_e = str(e).lower()
             if "read_context" in str_e or "readcontext" in str_e:
                 raise errors.CapsuleLoadError(
                     f"failed to load capsule: check that read context {read_context} exists for domain",
@@ -331,37 +468,38 @@
             if not st.cell_path:
                 span_tags[idx].cell_path = f"{col_names[0]}[0]"
 
         try:
             raw, capsule_ids = self._session.encapsulate(
                 *Preparer.prepare(col_names, column_tags, skip_classify_on_column_names, raw, span_tags, extra),
                 write_context,
-                path,
                 [],
                 jextra,
+                path,
                 subdomains_from,
                 create_subdomains)
         except Exception as e:
             str_e = str(e).lower()
             if (
                 "write_context" in str_e
                 or "writecontext" in str_e
                 or ("failed to create capsule" in str_e and "404 not found" in str_e)
                 or ("failed to create capsule" in str_e and "400 bad request" in str_e)
             ):
                 raise errors.CapsuleSaveError(
                     f"failed to encapsulate data: check that write context {write_context} exists for domain",
                 ) from None
             raise errors.CapsuleSaveError("encapsulating data") from e
+
         if raw is not None:
             raw = bytes(raw)
         return EncapsulateResponse(capsule_ids=capsule_ids, raw=raw, load_capsule_func=self.load_capsule)
 
     def refresh_token(self):
-        return self._client.domain_authenticate(
+        return openapi_client.AuthenticationApi(self._get_client()).domain_authenticate(
             self._domain,
             domain_authenticate=openapi_client.DomainAuthenticate(token=self._api_key)).token
 
     def with_new_peer_domain(
         self,
         import_alias_for_child: str,
         display_name_for_child: str,
@@ -414,7 +552,49 @@
             link_capabilities=link_capabilities,
             link_domain_policy=link_domain_policy,
             link_capsule_access_log=link_capsule_access_log,
             link_control_log=link_control_log,
             link_capsule_manifest=link_capsule_manifest,
         )
         return Session(dm.get("id"), dm.get("api_key"))
+
+    @exec_with_token
+    def get_admin_url(
+        self,
+        company_name: str,
+        peer_domain_id: Optional[str] = None,
+        nickname: Optional[str] = None,
+        alias: Optional[str] = None,
+    ) -> Optional[str]:
+        """
+        Generate the admin URL for the domain. By default, this is the domain
+        for this session. If one of the peer_domain_id, nickname, or alias are
+        provided, the admin URL will be generated for the subdomain that
+        matches.
+
+        :param company_name: The name of the company to display
+        :param peer_domain_id: The domain ID of the peer
+        :param nickname: The nickname for the peer domain
+        :param alias: One of the aliases of the peer domain
+        :return: The admin URL
+        """
+        if not peer_domain_id and (nickname or alias):
+            peer_domain_id = self.get_peer(nickname=nickname, alias=alias)
+
+        api_client = self._get_client()
+        auth_api = openapi_client.AuthenticationApi(api_client=api_client)
+
+        _id = self.domain_id
+        tkn = api_client.configuration.access_token
+        if peer_domain_id:
+            _id = peer_domain_id
+            tkn = auth_api.domain_authenticate(
+                domain_id=peer_domain_id,
+                domain_authenticate=openapi_client.DomainAuthenticate(token=tkn),
+                token_exchange=True,
+            ).token
+
+        url = urlparse(api_client.configuration.host)
+        url = f"{url.scheme}://{url.netloc}".replace('api', 'app')
+        company_name = quote_plus(company_name)
+        tkn = quote_plus(tkn)
+        return f"{url}/settings/{_id}/byok?vendor={company_name}&token=${tkn}"
```

## antimatter/builders/root_encryption_key.py

```diff
@@ -1,22 +1,22 @@
-
 import base64
 
-from typing import List
+from typing import List, Union
 
 from antimatter.client import (
     AWSServiceAccountKeyInfo, GCPServiceAccountKeyInfo, AntimatterDelegatedAWSKeyInfo, KeyInfosKeyInformation,
     KeyInfos
 )
 
+
 class OverrideKeyInfosKeyInformation(KeyInfosKeyInformation):
     one_of_schemas: List[str] = ["AWSServiceAccountKeyInfo", "AntimatterDelegatedAWSKeyInfo", "GCPServiceAccountKeyInfo"]
 
 
-def aws_service_account_key_info(access_key_id: str, secret_access_key: str, key_arn: str) -> KeyInfos:
+def aws_service_account_key_info(access_key_id: str, secret_access_key: str, key_arn: str = "") -> KeyInfos:
     """
     Create a KeyInfos object with AWS service account key information
 
     Example usage:
     ```
     key_info = aws_service_account_key_info(
         access_key_id="access_key_id", secret_access_key="secret_access_key", key_arn="key_arn"
@@ -53,27 +53,32 @@
     return KeyInfos(
         keyInformation=OverrideKeyInfosKeyInformation(
             actual_instance=AntimatterDelegatedAWSKeyInfo(key_arn=key_arn, provider_name="aws_am"),
         )
     )
 
 def gcp_service_account_key_info(
-        project_id: str, location: str, key_ring_id: str, key_id: str,
+        project_id: str,
+        location: str,
+        key_ring_id: str = "",
+        key_id: str = "",
         service_account_credentials: str = "",
-        service_account_credentials_path: str = ""
+        service_account_credentials_path: str = "",
     ) -> KeyInfos:
     """
     Create a KeyInfos object with GCP service account key information
 
     Example usage:
     ```
     key_info = gcp_service_account_key_info(
-        project_id="project_id", location="location",
-        key_ring_id="key_ring_id", key_id="key_id",
-        service_account_credentials="<service_account_credentials_as_json_string>", 
+        project_id="project_id",
+        location="location",
+        key_ring_id="key_ring_id",
+        key_id="key_id",
+        service_account_credentials="<service_account_credentials_as_json_string>",
         service_account_credentials_path="/path/to/service_account_credentials.json"
     )
     ```
     Either `service_account_credentials` or `service_account_credentials_path` should be provided.
 
     :param project_id: The project ID
     :param location: The location
@@ -85,15 +90,15 @@
     :return: A KeyInfos object with the specified key information
     """
     if not service_account_credentials and not service_account_credentials_path:
         raise ValueError("Either service_account_credentials or service_account_credentials_path should be provided")
 
     if service_account_credentials and service_account_credentials_path:
         raise ValueError("Only one of service_account_credentials or service_account_credentials_path should be provided")
-    
+
     encoded_service_account_credentials = None
     if service_account_credentials_path:
         with open(service_account_credentials_path, "r") as f:
             encoded_service_account_credentials = base64.b64encode(f.read().encode()).decode('utf-8')
 
     if service_account_credentials:
         encoded_service_account_credentials = base64.b64encode(service_account_credentials.encode()).decode('utf-8')
@@ -101,8 +106,8 @@
     return KeyInfos(
         keyInformation=OverrideKeyInfosKeyInformation(
             actual_instance=GCPServiceAccountKeyInfo(
                 service_account_credentials=encoded_service_account_credentials, project_id=project_id, location=location,
                 keyring_id=key_ring_id, key_id=key_id, provider_name="gcp_sa"
             )
         )
-    )
+    )
```

## antimatter/builders/settings_patch.py

```diff
@@ -22,39 +22,36 @@
         """
         Build the patch.
 
         :return: The built patch.
         """
         self.operation = PatchOperation(self.operation)
         inner = None
-        match self.operation:
-            case PatchOperation.Add:
-                inner = openapi_client.JSONPatchRequestAdd(
-                    path=self.path,
-                    value=openapi_client.JSONPatchRequestAddValue(self.value),
-                    op=self.operation.Add.value,
-                )
-            case PatchOperation.Replace:
-                inner = openapi_client.JSONPatchRequestReplace(
-                    path=self.path,
-                    value=openapi_client.JSONPatchRequestReplaceValue(self.value),
-                    op=self.operation.Replace.value,
-                )
-            case PatchOperation.Test:
-                inner = openapi_client.JSONPatchRequestTst(
-                    path=self.path,
-                    value=openapi_client.JSONPatchRequestTstValue(self.value),
-                    op=self.operation.Test.value,
-                )
-            case PatchOperation.Remove:
-                inner = openapi_client.JSONPatchRequestRemove(
-                    path=self.path, op=self.operation.Remove.value,
-                )
-            case PatchOperation.Move:
-                inner = openapi_client.JSONPatchRequestMove(
-                    path=self.path, op=self.operation.Move.value,
-                )
-            case PatchOperation.Copy:
-                inner = openapi_client.JSONPatchRequestCopy(
-                    path=self.path, op=self.operation.Copy.value,
-                )
-        return openapi_client.PatchRequestInner(inner)
+        operations = {
+            PatchOperation.Add: openapi_client.JSONPatchRequestAdd(
+                path=self.path,
+                value=openapi_client.JSONPatchRequestAddValue(self.value),
+                op=self.operation.Add.value,
+            ),
+            PatchOperation.Replace: openapi_client.JSONPatchRequestReplace(
+                path=self.path,
+                value=openapi_client.JSONPatchRequestReplaceValue(self.value),
+                op=self.operation.Replace.value,
+            ),
+            PatchOperation.Test: openapi_client.JSONPatchRequestTst(
+                path=self.path,
+                value=openapi_client.JSONPatchRequestTstValue(self.value),
+                op=self.operation.Test.value,
+            ),
+            PatchOperation.Remove: openapi_client.JSONPatchRequestRemove(
+                path=self.path, op=self.operation.Remove.value,
+            ),
+            PatchOperation.Move: openapi_client.JSONPatchRequestMove(
+                path=self.path, op=self.operation.Move.value,
+            ),
+            PatchOperation.Copy: openapi_client.JSONPatchRequestCopy(
+                path=self.path, op=self.operation.Copy.value,
+            ),
+        }
+        if self.operation not in operations:
+            raise ValueError(f"Invalid operation: {self.operation}")
+        return openapi_client.PatchRequestInner(operations.get(self.operation))
```

## antimatter/client/__init__.py

```diff
@@ -3,26 +3,33 @@
 # flake8: noqa
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "1.0.0"
 
 # import apis into sdk package
-from antimatter.client.api.default_api import DefaultApi
+from antimatter.client.api.account_management_api import AccountManagementApi
+from antimatter.client.api.authentication_api import AuthenticationApi
+from antimatter.client.api.capsules_api import CapsulesApi
+from antimatter.client.api.contexts_api import ContextsApi
+from antimatter.client.api.encryption_api import EncryptionApi
+from antimatter.client.api.general_api import GeneralApi
+from antimatter.client.api.internal_api import InternalApi
+from antimatter.client.api.policy_api import PolicyApi
 
 # import ApiClient
 from antimatter.client.api_response import ApiResponse
 from antimatter.client.api_client import ApiClient
 from antimatter.client.configuration import Configuration
 from antimatter.client.exceptions import OpenApiException
 from antimatter.client.exceptions import ApiTypeError
@@ -128,20 +135,23 @@
 from antimatter.client.models.json_patch_request_tst_value import JSONPatchRequestTstValue
 from antimatter.client.models.key_infos import KeyInfos
 from antimatter.client.models.key_infos_key_information import KeyInfosKeyInformation
 from antimatter.client.models.new_access_log_entry import NewAccessLogEntry
 from antimatter.client.models.new_access_log_entry_read_info import NewAccessLogEntryReadInfo
 from antimatter.client.models.new_capability_definition import NewCapabilityDefinition
 from antimatter.client.models.new_domain import NewDomain
+from antimatter.client.models.new_domain_policy_rule import NewDomainPolicyRule
 from antimatter.client.models.new_domain_response import NewDomainResponse
 from antimatter.client.models.new_fact import NewFact
 from antimatter.client.models.new_fact_type_definition import NewFactTypeDefinition
 from antimatter.client.models.new_fact_type_definition_arguments_inner import NewFactTypeDefinitionArgumentsInner
 from antimatter.client.models.new_read_context_config_rule import NewReadContextConfigRule
 from antimatter.client.models.patch_request_inner import PatchRequestInner
+from antimatter.client.models.policy_rule_operation import PolicyRuleOperation
+from antimatter.client.models.policy_rule_result import PolicyRuleResult
 from antimatter.client.models.principal_info import PrincipalInfo
 from antimatter.client.models.principal_summary import PrincipalSummary
 from antimatter.client.models.read_context_config_rule import ReadContextConfigRule
 from antimatter.client.models.read_context_details import ReadContextDetails
 from antimatter.client.models.read_context_list import ReadContextList
 from antimatter.client.models.read_context_parameter import ReadContextParameter
 from antimatter.client.models.read_context_required_hook import ReadContextRequiredHook
```

## antimatter/client/api_client.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/configuration.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -381,15 +381,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.1.3\n"\
+               "Version of the API: 1.2.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

## antimatter/client/exceptions.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

## antimatter/client/rest.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/api/__init__.py

```diff
@@ -1,5 +1,12 @@
 # flake8: noqa
 
 # import apis into api package
-from antimatter.client.api.default_api import DefaultApi
+from antimatter.client.api.account_management_api import AccountManagementApi
+from antimatter.client.api.authentication_api import AuthenticationApi
+from antimatter.client.api.capsules_api import CapsulesApi
+from antimatter.client.api.contexts_api import ContextsApi
+from antimatter.client.api.encryption_api import EncryptionApi
+from antimatter.client.api.general_api import GeneralApi
+from antimatter.client.api.internal_api import InternalApi
+from antimatter.client.api.policy_api import PolicyApi
```

## antimatter/client/models/__init__.py

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -111,20 +111,23 @@
 from antimatter.client.models.json_patch_request_tst_value import JSONPatchRequestTstValue
 from antimatter.client.models.key_infos import KeyInfos
 from antimatter.client.models.key_infos_key_information import KeyInfosKeyInformation
 from antimatter.client.models.new_access_log_entry import NewAccessLogEntry
 from antimatter.client.models.new_access_log_entry_read_info import NewAccessLogEntryReadInfo
 from antimatter.client.models.new_capability_definition import NewCapabilityDefinition
 from antimatter.client.models.new_domain import NewDomain
+from antimatter.client.models.new_domain_policy_rule import NewDomainPolicyRule
 from antimatter.client.models.new_domain_response import NewDomainResponse
 from antimatter.client.models.new_fact import NewFact
 from antimatter.client.models.new_fact_type_definition import NewFactTypeDefinition
 from antimatter.client.models.new_fact_type_definition_arguments_inner import NewFactTypeDefinitionArgumentsInner
 from antimatter.client.models.new_read_context_config_rule import NewReadContextConfigRule
 from antimatter.client.models.patch_request_inner import PatchRequestInner
+from antimatter.client.models.policy_rule_operation import PolicyRuleOperation
+from antimatter.client.models.policy_rule_result import PolicyRuleResult
 from antimatter.client.models.principal_info import PrincipalInfo
 from antimatter.client.models.principal_summary import PrincipalSummary
 from antimatter.client.models.read_context_config_rule import ReadContextConfigRule
 from antimatter.client.models.read_context_details import ReadContextDetails
 from antimatter.client.models.read_context_list import ReadContextList
 from antimatter.client.models.read_context_parameter import ReadContextParameter
 from antimatter.client.models.read_context_required_hook import ReadContextRequiredHook
```

## antimatter/client/models/access_log_entry.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/access_log_entry_create_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/access_log_entry_open_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/access_log_entry_read_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/access_log_results.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/active_root_encryption_key_id.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/add_capsule_log_entry_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/add_read_context.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/add_write_context.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/antimatter_delegated_aws_key_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/api_key_domain_identity_provider_details.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/available_delegated_root_encryption_key_provider.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/available_root_encryption_key_providers.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/available_root_encryption_key_providers_providers_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/available_service_account_root_encryption_key_provider.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/aws_service_account_key_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capability.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capability_definition.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capability_definition_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capability_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capability_rule.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capability_rule_match_expressions_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capsule_create_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capsule_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capsule_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capsule_open_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capsule_open_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capsule_open_response_read_context_configuration.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/capsule_seal_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/conflict_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/create_peer_domain.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -31,16 +31,16 @@
 class CreatePeerDomain(BaseModel):
     """
     Configuration options for creating a new subdomain. 
     """ # noqa: E501
     nicknames: Optional[List[Annotated[str, Field(strict=True, max_length=128)]]] = Field(default=None, description="a list of names for this domain. These can be used to look up this domain later by using domainFromNickname. All nicknames for peer domains must be unique within a domain ")
     import_alias_for_parent: Optional[Annotated[str, Field(strict=True)]] = Field(default=None, description="An alias for a peer domain. It must be unique within a domain. The alias is used to refer to the peer domain in policies. A peer may have only one alias ", alias="importAliasForParent")
     import_alias_for_child: Annotated[str, Field(strict=True)] = Field(description="An alias for a peer domain. It must be unique within a domain. The alias is used to refer to the peer domain in policies. A peer may have only one alias ", alias="importAliasForChild")
-    display_name_for_parent: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=40)]] = Field(default=None, description="The default display name used for this domain. THe display name is also treated as a nickname and so can be used from domainFromNickname. ", alias="displayNameForParent")
-    display_name_for_child: Annotated[str, Field(min_length=1, strict=True, max_length=40)] = Field(description="The default display name used for this domain. THe display name is also treated as a nickname and so can be used from domainFromNickname. ", alias="displayNameForChild")
+    display_name_for_parent: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=40)]] = Field(default=None, description="The default display name used for this domain. The display name is also treated as a nickname and so can be used from domainFromNickname. ", alias="displayNameForParent")
+    display_name_for_child: Annotated[str, Field(min_length=1, strict=True, max_length=40)] = Field(description="The default display name used for this domain. The display name is also treated as a nickname and so can be used from domainFromNickname. ", alias="displayNameForChild")
     link_all: Optional[StrictBool] = Field(default=False, alias="linkAll")
     link_identity_providers: Optional[StrictBool] = Field(default=False, alias="linkIdentityProviders")
     link_facts: Optional[StrictBool] = Field(default=False, alias="linkFacts")
     link_read_contexts: Optional[StrictBool] = Field(default=False, alias="linkReadContexts")
     link_write_contexts: Optional[StrictBool] = Field(default=False, alias="linkWriteContexts")
     link_capabilities: Optional[StrictBool] = Field(default=False, alias="linkCapabilities")
     link_domain_policy: Optional[StrictBool] = Field(default=False, alias="linkDomainPolicy")
```

## antimatter/client/models/data_tagging_hook_input.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/data_tagging_hook_input_records_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/data_tagging_hook_input_records_inner_elements_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/data_tagging_hook_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/data_tagging_hook_response_records_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/delete_tags.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_add_read_context_rule200_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_authenticate.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_authenticate_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_contact_issue_verify_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_control_log_entry.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_control_log_results.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_fact_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_hooks_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_hooks_list_hooks_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_api_key_principal_params.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_email_principal_params.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_hosted_domain_principal_params.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_principal_details.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_provider_details.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_provider_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_provider_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_provider_principal_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_provider_principal_params.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_provider_principal_type.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_identity_provider_type.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_insert_identity_provider_principal200_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_insert_write_context_regex_rule200_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_peer_config.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -63,15 +63,15 @@
     import_capabilities: Optional[List[Annotated[str, Field(strict=True)]]] = Field(default=None, description="A list of capabilities to import from the peer domain ", alias="importCapabilities")
     import_all_capabilities: Optional[StrictBool] = Field(default=None, description="If present and true, this overrides importCapabilities and imports  all available capabilities ", alias="importAllCapabilities")
     import_domain_policy: Optional[StrictBool] = Field(default=None, description="Import all domain policy (limited by the imported capabilities and facts) into this domain ", alias="importDomainPolicy")
     import_precedence: Optional[StrictInt] = Field(default=None, description="For read contexts and domain policy, is the peer domain higher precedence  (<0) or lower precedence (>0) than the rules configured in the current domain (0). The precedence is also used to order the imported read context rules and domain policy rules with respect to policy imported from other peers. Note  that imported policy is always executed as an atomic unit, so interleaving  of imported rules and rules that exist in this domain is not possible. ", alias="importPrecedence")
     import_capsule_access_log: Optional[StrictBool] = Field(default=None, description="When querying the capsule access log, should results from this peer domain automatically be merged in ", alias="importCapsuleAccessLog")
     import_control_log: Optional[StrictBool] = Field(default=None, description="When querying the control audit log, should results from this peer domain automatically be merged in ", alias="importControlLog")
     import_capsule_manifest: Optional[StrictBool] = Field(default=None, description="When querying for capsules, should results from this peer domain automatically be merged in ", alias="importCapsuleManifest")
-    display_name: Annotated[str, Field(min_length=1, strict=True, max_length=40)] = Field(description="The default display name used for this domain. THe display name is also treated as a nickname and so can be used from domainFromNickname. ", alias="displayName")
+    display_name: Annotated[str, Field(min_length=1, strict=True, max_length=40)] = Field(description="The default display name used for this domain. The display name is also treated as a nickname and so can be used from domainFromNickname. ", alias="displayName")
     __properties: ClassVar[List[str]] = ["exportIdentityProviders", "exportAllIdentityProviders", "exportFacts", "exportAllFacts", "exportReadContexts", "exportAllReadContexts", "exportWriteContexts", "exportAllWriteContexts", "exportCapabilities", "exportAllCapabilities", "exportDomainPolicy", "exportCapsuleAccessLog", "exportControlLog", "exportCapsuleManifest", "exportBilling", "exportAdminContact", "nicknames", "importAlias", "forwardBilling", "forwardAdminCommunications", "importIdentityProviders", "importAllIdentityProviders", "importFacts", "importAllFacts", "importReadContexts", "importAllReadContexts", "importWriteContexts", "importAllWriteContexts", "importCapabilities", "importAllCapabilities", "importDomainPolicy", "importPrecedence", "importCapsuleAccessLog", "importControlLog", "importCapsuleManifest", "displayName"]
 
     @field_validator('import_alias')
     def import_alias_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if value is None:
             return value
```

## antimatter/client/models/domain_peer_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_peer_list_peers_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_policy.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_policy_rule.py

```diff
@@ -1,75 +1,75 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, StrictBool, StrictInt, StrictStr, field_validator
 from pydantic import Field
 from typing_extensions import Annotated
 from antimatter.client.models.capability_rule import CapabilityRule
 from antimatter.client.models.fact_policy_rules_inner import FactPolicyRulesInner
+from antimatter.client.models.policy_rule_operation import PolicyRuleOperation
+from antimatter.client.models.policy_rule_result import PolicyRuleResult
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class DomainPolicyRule(BaseModel):
     """
-    A rule governing the domain's policy. All domain identity capabilities must match (AND) for the action to take effect. If the domainIdentity or facts sections are omitted, they match all domain identities and any fact configurations respectively. When updating or creating a rule, the id field may be omitted. 
+    A rule governing the domain's policy. All domain identity capabilities must match (AND) for the action to take effect. If the domainIdentity or facts sections are omitted, they match all domain identities and any fact configurations respectively. 
     """ # noqa: E501
-    id: Optional[Annotated[str, Field(strict=True)]] = Field(default=None, description="An identifier for a rule")
+    id: Annotated[str, Field(strict=True)] = Field(description="An identifier for a domain policy rule that might be imported from a peer domain. If it is, it will bear an imported resource prefix (either a domain identifier or an alias, followed by ::) ")
     domain_identity: Optional[CapabilityRule] = Field(default=None, alias="domainIdentity")
     facts: Optional[List[FactPolicyRulesInner]] = Field(default=None, description="assert the existence or nonexistence of facts that reference the domainIdentity. These assertions will be ANDed together, and ANDed with the domainIdentity expression ")
     path: StrictStr = Field(description="the path this rule governs. This pattern may contain glob expressions (e.g. '*' and '**'). ")
-    operation: StrictStr
-    result: StrictStr
+    operation: PolicyRuleOperation
+    result: PolicyRuleResult
     priority: Annotated[int, Field(strict=True, ge=0)] = Field(description="This rule's priority. Lower priority numbers rules are evaluated first")
     disabled: StrictBool = Field(description="If this rule is disabled or not.")
-    __properties: ClassVar[List[str]] = ["id", "domainIdentity", "facts", "path", "operation", "result", "priority", "disabled"]
+    imported: StrictBool = Field(description="true if this write context is imported")
+    source_domain_id: Optional[Annotated[str, Field(strict=True)]] = Field(default=None, description="A globally unique identifier for a domain", alias="sourceDomainID")
+    source_domain_name: Optional[StrictStr] = Field(default=None, alias="sourceDomainName")
+    precedence: StrictInt = Field(description="for imported rules, whether this rule is evaluated before (<0) or after (>0) the current domain's rules. Always 0 for non-imported rules ")
+    invalid: Optional[StrictBool] = Field(default=None, description="If the rule was created referencing a resource that was valid at the time of the rule's creation, but has since become invalid (e.g. if it was a peered resource and the peering has changed) then the rule will be ignored during policy evaluation, and \"invalid\" will be true when listing the domain policy rules ")
+    __properties: ClassVar[List[str]] = ["id", "domainIdentity", "facts", "path", "operation", "result", "priority", "disabled", "imported", "sourceDomainID", "sourceDomainName", "precedence", "invalid"]
 
     @field_validator('id')
     def id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if value is None:
-            return value
-
-        if not re.match(r"^rl-[a-z0-9]{16}$", value):
-            raise ValueError(r"must validate the regular expression /^rl-[a-z0-9]{16}$/")
+        if not re.match(r"^((dm-[1-9A-HJ-NP-Za-km-z]{11}|[a-z][a-z0-9_]{2,31})::)?rl-[a-z0-9]{16}$$", value):
+            raise ValueError(r"must validate the regular expression /^((dm-[1-9A-HJ-NP-Za-km-z]{11}|[a-z][a-z0-9_]{2,31})::)?rl-[a-z0-9]{16}$$/")
         return value
 
-    @field_validator('operation')
-    def operation_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in ('edit', 'view', 'use'):
-            raise ValueError("must be one of enum values ('edit', 'view', 'use')")
-        return value
+    @field_validator('source_domain_id')
+    def source_domain_id_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if value is None:
+            return value
 
-    @field_validator('result')
-    def result_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in ('allow', 'deny'):
-            raise ValueError("must be one of enum values ('allow', 'deny')")
+        if not re.match(r"^dm-[1-9A-HJ-NP-Za-km-z]{11}$", value):
+            raise ValueError(r"must validate the regular expression /^dm-[1-9A-HJ-NP-Za-km-z]{11}$/")
         return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -130,12 +130,17 @@
             "id": obj.get("id"),
             "domainIdentity": CapabilityRule.from_dict(obj.get("domainIdentity")) if obj.get("domainIdentity") is not None else None,
             "facts": [FactPolicyRulesInner.from_dict(_item) for _item in obj.get("facts")] if obj.get("facts") is not None else None,
             "path": obj.get("path"),
             "operation": obj.get("operation"),
             "result": obj.get("result"),
             "priority": obj.get("priority"),
-            "disabled": obj.get("disabled")
+            "disabled": obj.get("disabled"),
+            "imported": obj.get("imported"),
+            "sourceDomainID": obj.get("sourceDomainID"),
+            "sourceDomainName": obj.get("sourceDomainName"),
+            "precedence": obj.get("precedence"),
+            "invalid": obj.get("invalid")
         })
         return _obj
```

## antimatter/client/models/domain_private_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_public_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_resource_summary.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_resource_summary_schema_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_settings.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_settings_disaster_recovery.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_settings_patch.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_status.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_status_notifications_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/domain_tag_info_results.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/fact.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/fact_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/fact_policy_rules_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/fact_policy_rules_inner_arguments_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/fact_type_definition.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/gcp_service_account_key_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/google_o_auth_domain_identity_provider_details.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/hook_invocation.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/invalid_request_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_add.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_add_value.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_copy.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_move.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_remove.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_replace.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_replace_value.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_tst.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/json_patch_request_tst_value.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/key_infos.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/key_infos_key_information.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_access_log_entry.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_access_log_entry_read_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_capability_definition.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_domain.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_domain_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_fact.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_fact_type_definition.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_fact_type_definition_arguments_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/new_read_context_config_rule.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/patch_request_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/principal_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/principal_summary.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_config_rule.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_details.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_parameter.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_required_hook.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_rule_facts_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_rule_facts_inner_arguments_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_rule_match_expressions_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/read_context_short_details.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/resource_exhausted_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/resource_not_found_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/root_encryption_key_id_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/root_encryption_key_item.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/root_encryption_key_test_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/rotate_key_encryption_key_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/starred_domain_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/tag.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/tag_meta.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/tag_set.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/tag_set_span_tags_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/tag_summary.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/tag_summary_elided_tags_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/tag_summary_unique_tags_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/tag_type_field.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/unauthorized_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/upsert_span_tags_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/verify_contact_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/write_context_config_info.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/write_context_config_info_required_hooks_inner.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/write_context_details.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/write_context_list.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/write_context_regex_rule.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/client/models/write_context_regex_tag.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Antimatter Public API
 
     Interact with the Antimatter Cloud API
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.2.0
     Contact: support@antimatter.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## antimatter/constants/hooks.py

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 
+
 class Hook(str, Enum):
     """
     Enum representing the available hooks.
     """
     Fast = "fast-pii"
     Accurate = "accurate-pii"
     Regex = "regex-classifier"
```

## antimatter/errors/errors.py

```diff
@@ -2,14 +2,19 @@
 
 
 class SessionError(Exception):
     """Base class for Session errors."""
     pass
 
 
+class SessionLoadError(SessionError):
+    """Error when a session encounters issues loading."""
+    pass
+
+
 class SessionVerificationPendingError(SessionError):
     """Error when a session has not yet had its admin contact verified."""
     pass
 
 
 class SessionVerificationMissingEmailError(SessionError):
     """Error when resending a verification email with unknown email."""
```

## antimatter/fieldtype/converters.py

```diff
@@ -17,73 +17,61 @@
 
         :param ft: the FieldType to get the converter function for
         :return: a function that can convert field values from generic form
         """
         # In all the lambdas below, if the value is 'redacted', it should be converted
         # to a default redacted value based on the FieldType
         redacted = b'{redacted}'
-        match ft:
-            case FieldType.String:
-                return lambda x: x.decode("utf-8", errors="replace")
-
-            case FieldType.Bytes:
-                return lambda x: bytes(x)
-
-            case FieldType.Bool:
-                return lambda x: False if redacted in x else x == b'True'
-
-            case FieldType.Int:
-                return lambda x: 0 if redacted in x else int(x.decode("utf-8", errors="replace"))
-
-            case FieldType.Timestamp:
-                return lambda x: 0 if redacted in x else int(x.decode("utf-8", errors="replace"))
-
-            case FieldType.Float:
-                return lambda x: 0.0 if redacted in x else float(x.decode("utf-8", errors="replace"))
-
-            case FieldType.Decimal:
-                return lambda x: decimal.Decimal(0) if redacted in x else decimal.Decimal(
+        if ft is FieldType.String:
+            return lambda x: x.decode("utf-8", errors="replace")
+        elif ft is FieldType.Bytes:
+            return lambda x: bytes(x)
+        elif ft is FieldType.Bool:
+            return lambda x: False if redacted in x else x == b'True'
+        elif ft is FieldType.Int:
+            return lambda x: 0 if redacted in x else int(x.decode("utf-8", errors="replace"))
+        elif ft is FieldType.Timestamp:
+            return lambda x: 0 if redacted in x else int(x.decode("utf-8", errors="replace"))
+        elif ft is FieldType.Float:
+            return lambda x: 0.0 if redacted in x else float(x.decode("utf-8", errors="replace"))
+        elif ft is FieldType.Decimal:
+            return lambda x: decimal.Decimal(0) if redacted in x else decimal.Decimal(
                     x.decode("utf-8", errors="replace"))
-
-            case FieldType.Date:
-                return lambda x: datetime.date(1970, 1, 1) \
+        elif ft is FieldType.Date:
+            return lambda x: datetime.date(1970, 1, 1) \
                     if redacted in x else datetime.date.fromisoformat(x.decode("utf-8", errors="replace"))
-
-            case FieldType.DateTime:
-                return lambda x: datetime.datetime(1970, 1, 1) \
+        elif ft is FieldType.DateTime:
+            return lambda x: datetime.datetime(1970, 1, 1) \
                     if redacted in x else datetime.datetime.fromisoformat(x.decode("utf-8", errors="replace"))
-
-            case FieldType.Time:
-                return lambda x: datetime.time(0, 0, 0) \
+        elif ft is FieldType.Time:
+            return lambda x: datetime.time(0, 0, 0) \
                     if redacted in x else datetime.time.fromisoformat(x.decode("utf-8", errors="replace"))
-
-            case FieldType.Timedelta:
-                return lambda x: datetime.timedelta(0) if redacted in x else datetime.timedelta(
+        elif ft is FieldType.Timedelta:
+            return lambda x: datetime.timedelta(0) if redacted in x else datetime.timedelta(
                     microseconds=int(x.decode("utf-8", errors="replace")) / 1000)
 
         return None
 
     @staticmethod
     def field_converter_to_generic(ft: FieldType) -> Optional[Callable[[Any], bytes]]:
         """
         field_converter_to_generic gets a field converter function for the given
         field type that can be used to convert fields from their specific type
         to their generic type.
 
         :param ft: the FieldType to get the converter function for
         :return: a function that can convert field values to generic form
         """
-        match ft:
-            case FieldType.String:
-                return lambda x: x.encode("utf-8")
-            case FieldType.Bytes:
-                return lambda x: x
-            case FieldType.Float | FieldType.Decimal | FieldType.Bool | FieldType.Timestamp | FieldType.Int:
-                return lambda x: str(x).encode("utf-8")
-            case FieldType.Date | FieldType.Time | FieldType.DateTime:
-                return lambda x: x.isoformat().encode("utf-8")
-            case FieldType.Timedelta:
-                return lambda x: str(
+        if ft is FieldType.String:
+            return lambda x: x.encode("utf-8")
+        elif ft is FieldType.Bytes:
+            return lambda x: x
+        elif ft in [FieldType.Float, FieldType.Decimal, FieldType.Bool, FieldType.Timestamp, FieldType.Int]:
+            return lambda x: str(x).encode("utf-8")
+        elif ft in [FieldType.Date, FieldType.Time, FieldType.DateTime]:
+            return lambda x: x.isoformat().encode("utf-8")
+        elif ft is FieldType.Timedelta:
+            return lambda x: str(
                     (x.days * 86_400_000_000 + x.seconds * 1_000_000 + x.microseconds) * 1000
                 ).encode("utf-8")
 
         return None
```

## antimatter/filetype/extract.py

```diff
@@ -10,29 +10,28 @@
     Extracts data from a file based on the provided hint about the file's format.
 
     :param path: The path to the file.
     :param hint: A hint about the file format. Supported hints are 'csv', 'json', 'parquet', and 'txt'.
     :return: The extracted data.
     :raises errors.DataFormatError: If the file format hinted is not supported.
     """
-    match hint:
-        case "csv":
-            return extract_from_csv(path)
-        case "json":
-            # assume ndjson format first
-            try:
-                return extract_from_ndjson(path)
-            except:
-                return extract_from_json(path)
-        case "parquet":
-            return extract_from_parquet(path)
-        case "txt":
-            return extract_from_txt(path)
-        case _:
-            raise DataFormatError(f"file format with hint '{hint}' is not supported")
+    if hint == "csv":
+        return extract_from_csv(path)
+    elif hint == "json":
+        # assume ndjson format first
+        try:
+            return extract_from_ndjson(path)
+        except:
+            return extract_from_json(path)
+    elif hint == "parquet":
+        return extract_from_parquet(path)
+    elif hint == "txt":
+        return extract_from_txt(path)
+    else:
+        raise DataFormatError(f"file format with hint '{hint}' is not supported")
 
 
 def extract_from_csv(path: str) -> List[Dict]:
     """
     Extracts data from a CSV file.
 
     This function sniffs the dialect of the CSV file and reads it into a list of dictionaries,
```

## antimatter/handlers/__init__.py

```diff
@@ -14,22 +14,23 @@
     Factory returns an instance of a DataHandler matching the provided Datatype.
 
     :param datatype: The Datatype to get a handler for.
     :return:
     An implementation of the abstract DataHandler for handling data of the
     given type.
     """
-    match datatype:
-        case Datatype.Unknown:
-            raise HandlerFactoryError("cannot create factory from 'Unknown' Datatype")
-        case Datatype.Scalar:
-            return ScalarHandler()
-        case Datatype.Dict:
-            return Dictionary()
-        case Datatype.DictList:
-            return DictList()
-        case Datatype.PandasDataframe:
-            return PandasDataFrame()
-        case Datatype.PytorchDataLoader:
-            return PytorchDataLoader()
-        case Datatype.LangchainRetriever:
-            return LangchainHandler()
+    if datatype is Datatype.Unknown:
+        raise HandlerFactoryError("cannot create factory from 'Unknown' Datatype")
+    elif datatype is Datatype.Scalar:
+        return ScalarHandler()
+    elif datatype is Datatype.Dict:
+        return Dictionary()
+    elif datatype is Datatype.DictList:
+        return DictList()
+    elif datatype is Datatype.PandasDataframe:
+        return PandasDataFrame()
+    elif datatype is Datatype.PytorchDataLoader:
+        return PytorchDataLoader()
+    elif datatype is Datatype.LangchainRetriever:
+        return LangchainHandler()
+    else:
+        raise HandlerFactoryError(f"no handler found for Datatype: {datatype}")
```

## antimatter/requirements/core.txt

```diff
@@ -1,8 +1,9 @@
 annotated_types>=0.6
 packaging>=21.1
 pydantic>=2.0
 python-dateutil>=2.1
+pyyaml
 cbor2~=5.5
 urllib3>=2.0.2
 # This will be replaced by the build system with the appropriate version from client/VERSION.txt
-antimatter-engine==0.2.2
+antimatter-engine==1.0.0
```

## antimatter/session_mixins/capability_mixin.py

```diff
@@ -1,20 +1,19 @@
 from typing import Any, Callable, Dict, List, Optional
 
 import antimatter.client as openapi_client
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.token import exec_with_token
 
 
 class CapabilityMixin:
     """
     Session mixin defining CRUD functionality for capabilities.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
@@ -22,27 +21,29 @@
     def get_capabilities(self) -> List[Dict[str, Any]]:
         """
         Get the capabilities for the session's domain.
 
         :return: A list of capabilities.
         """
         capabilities = []
-        for capability in self._client_func().domain_get_capabilities(domain_id=self._domain).capabilities:
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        for capability in auth_api.domain_get_capabilities(domain_id=self._domain).capabilities:
             capabilities.append(capability.model_dump())
         return capabilities
 
     @exec_with_token
     def get_capability(self, name: str) -> Dict[str, Any]:
         """
         Get a specific capability for the session's domain.
 
         :param name: The name for this capability, like "admin"
         :return: The details of the capability.
         """
-        return self._client_func().domain_get_capability(domain_id=self._domain, capability=name).model_dump()
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        return auth_api.domain_get_capability(domain_id=self._domain, capability=name).model_dump()
 
     @exec_with_token
     def put_capability(
             self,
             name: str,
             summary: str,
             description: Optional[str] = None,
@@ -60,15 +61,16 @@
         :param description: An optional longer form description of this capability
         :param unary: A unary capability does not have a value
         :param create_only:
         If True, an error will be returned if a capability with the name already exists
         """
         if description is None:
             description = ""
-        self._client_func().domain_put_capability(
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        auth_api.domain_put_capability(
             domain_id=self._domain,
             capability=name,
             new_capability_definition=openapi_client.NewCapabilityDefinition(
                 unary=unary,
                 summary=summary,
                 description=description,
             ),
@@ -78,8 +80,9 @@
     @exec_with_token
     def delete_capability(self, name: str) -> None:
         """
         Delete a capability.
 
         :param name: The name of the capability, like "admin"
         """
-        self._client_func().domain_delete_capability(domain_id=self._domain, capability=name)
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        auth_api.domain_delete_capability(domain_id=self._domain, capability=name)
```

## antimatter/session_mixins/capsule_mixin.py

```diff
@@ -1,25 +1,24 @@
 from datetime import datetime
 from typing import Any, Callable, Dict, Iterator, List, Optional
 
 import antimatter.client as openapi_client
 from antimatter.tags import CapsuleTag
 from antimatter.cap_prep.applicator import TAG_SOURCE, TAG_VERSION
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.token import exec_with_token
 
 
 class CapsuleMixin:
     """
     Session mixin defining CRUD functionality for capsules and tags.
     """
 
     _page_res_size: int = 100
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
@@ -31,23 +30,35 @@
         span_tag: Optional[str] = None,
         sort_on: Optional[str] = None,
         ascending: Optional[bool] = None,
     ) -> Iterator[Dict[str, Any]]:
         """
         Returns an iterator over the capsules available for the current domain and auth
 
-        :param start_date: The earlier date of the date range. As results are returned in reverse chronological order, this date corresponds with the end of the result set.
-        :param end_date: The later date of the date range. As results are returned in reverse chronological order, this date corresponds with the beginning of the result set. If not specified, defaults to the current time.
-        :param span_tag: The span tag you would like to filter on. This accepts a tag key only and will return all span tag key results matching the provided tag key. If not specified, this field is ignored.
-        :param sort_on: The capsule field you would like to sort on. This accepts the field only and will return results ordered on the provided field. If not specified, this field is ignored.
-        :param ascending: This defines whether a sorted result should be order ascending. This accepts a boolean value and when true will work in combination with the sort_on and start_after parameters to return values in ascending order. If not specified, this field is ignored and treated as false.
+        :param start_date:
+        The earlier date of the date range. As results are returned in reverse chronological order, this date
+        corresponds with the end of the result set.
+        :param end_date:
+        The later date of the date range. As results are returned in reverse chronological order, this date
+        corresponds with the beginning of the result set. If not specified, defaults to the current time.
+        :param span_tag:
+        The span tag you would like to filter on. This accepts a tag key only and will return all span tag key
+        results matching the provided tag key. If not specified, this field is ignored.
+        :param sort_on:
+        The capsule field you would like to sort on. This accepts the field only and will return results ordered
+        on the provided field. If not specified, this field is ignored.
+        :param ascending:
+        This defines whether a sorted result should be order ascending. This accepts a boolean value and when true
+        will work in combination with the sort_on and start_after parameters to return values in ascending order.
+        If not specified, this field is ignored and treated as false.
         """
         pagination = None
+        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
         while True:
-            res = self._client_func().domain_list_capsules(
+            res = capsules_api.domain_list_capsules(
                 domain_id=self._domain,
                 start_date=start_date,
                 end_date=end_date,
                 num_results=self._page_res_size,
                 span_tags=span_tag,
                 sort_on=sort_on,
                 start_after=pagination,
@@ -63,27 +74,29 @@
     def get_capsule_info(self, capsule_id: str) -> Dict[str, Any]:
         """
         Get the summary information about the capsule.
 
         :param capsule_id: The identifier for the capsule
         :return: The summary information about the capsule
         """
-        return self._client_func().domain_get_capsule_info(
+        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
+        return capsules_api.domain_get_capsule_info(
             domain_id=self._domain, capsule_id=capsule_id,
         ).model_dump()
 
     @exec_with_token
     def upsert_capsule_tags(self, capsule_id: str, tags: List[CapsuleTag]) -> None:
         """
         Upsert the capsule-level tags to apply to a capsule.
 
         :param capsule_id: The capsule to apply tags to
         :param tags: The tags to apply to the capsule
         """
-        self._client_func().domain_upsert_capsule_tags(
+        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
+        capsules_api.domain_upsert_capsule_tags(
             domain_id=self._domain, capsule_id=capsule_id, tag=[
                 openapi_client.Tag(
                     name=tag.name,
                     value=tag.tag_value,
                     type=tag.tag_type.name.lower(),
                     hook_version=f"{TAG_VERSION[0]}.{TAG_VERSION[1]}.{TAG_VERSION[2]}",
                     source=TAG_SOURCE,
@@ -95,12 +108,13 @@
     def delete_capsule_tags(self, capsule_id: str, tag_names: List[str]) -> None:
         """
         Delete capsule-level tags
 
         :param capsule_id: The capsule to delete tags from
         :param tag_names: The names of the tags to delete
         """
-        self._client_func().domain_delete_capsule_tags(
+        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
+        capsules_api.domain_delete_capsule_tags(
             domain_id=self._domain,
             capsule_id=capsule_id,
             delete_tags=openapi_client.DeleteTags(names=tag_names),
         )
```

## antimatter/session_mixins/domain_mixin.py

```diff
@@ -1,33 +1,33 @@
 from typing import Any, Callable, Dict, List, Optional
 
 import antimatter.client as openapi_client
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.token import exec_with_token
 
 
 class DomainMixin:
     """
     Session mixin defining CRUD functionality for domains, including peering.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
     @exec_with_token
     def new_domain(self, admin_email: str) -> Dict[str, Any]:
         """
         Create a new domain with no default peer relationships.
         """
-        return self._client_func().domain_add_new(
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        return general_api.domain_add_new(
             new_domain=openapi_client.NewDomain(admin_email=admin_email),
         ).model_dump()
 
     @exec_with_token
     def new_peer_domain(
         self,
         import_alias_for_child: str,
@@ -63,15 +63,16 @@
         :param link_domain_policy: Whether to link domain policy
         :param link_capsule_access_log: Whether to link capsule access log
         :param link_control_log: Whether to link control log
         :param link_capsule_manifest: Whether to link capsule manifest
 
         :return: The new peer domain
         """
-        return self._client_func().domain_create_peer_domain(
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        return general_api.domain_create_peer_domain(
             domain_id=self._domain,
             create_peer_domain=openapi_client.CreatePeerDomain(
                 import_alias_for_child=import_alias_for_child,
                 display_name_for_child=display_name_for_child,
                 nicknames=nicknames,
                 import_alias_for_parent=import_alias_for_parent,
                 display_name_for_parent=display_name_for_parent,
@@ -94,24 +95,26 @@
         Retrieve the domain ID of a domain that is configured as a peer of this
         session's domain by using either its alias or one of its nicknames.
 
         :param nickname: The nickname for the peer domain
         :param alias: One of the aliases of the peer domain
         :return: The domain ID
         """
-        return self._client_func().domain_get_peer(domain_id=self._domain, nickname=nickname, alias=alias).id
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        return general_api.domain_get_peer(domain_id=self._domain, nickname=nickname, alias=alias).id
 
     @exec_with_token
     def list_peers(self):
         """
         Return a list of the peers of this session's domain.
 
         :return: The peer list, containing IDs and other information about the domains
         """
-        return [p.model_dump() for p in self._client_func().domain_list_peers(domain_id=self._domain).peers]
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        return [p.model_dump() for p in general_api.domain_list_peers(domain_id=self._domain).peers]
 
     @exec_with_token
     def get_peer_config(
         self,
         peer_domain_id: Optional[str] = None,
         nickname: Optional[str] = None,
         alias: Optional[str] = None,
@@ -123,15 +126,16 @@
         :param peer_domain_id: The domain ID of the peer
         :param nickname: The nickname for the peer domain
         :param alias: One of the aliases of the peer domain
         :return: The full peer configuration
         """
         if not peer_domain_id and (nickname or alias):
             peer_domain_id = self.get_peer(nickname=nickname, alias=alias)
-        return self._client_func().domain_get_peer_config(
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        return general_api.domain_get_peer_config(
             domain_id=self._domain, peer_domain_id=peer_domain_id,
         ).model_dump()
 
     @exec_with_token
     def update_peer(
         self,
         display_name: str,
@@ -218,15 +222,16 @@
         :param import_precedence: The precedence of the import
         :param import_capsule_access_log: Whether to import the capsule access log
         :param import_control_log: Whether to import the control log
         :param import_capsule_manifest: Whether to import the capsule manifest
         """
         if not peer_domain_id and (nickname or alias):
             peer_domain_id = self.get_peer(nickname=nickname, alias=alias)
-        self._client_func().domain_update_peer(
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        general_api.domain_update_peer(
             domain_id=self._domain,
             peer_domain_id=peer_domain_id,
             domain_peer_config=openapi_client.DomainPeerConfig(
                 display_name=display_name,
                 export_identity_providers=export_identity_providers,
                 export_all_identity_providers=export_all_identity_providers,
                 export_facts=export_facts,
@@ -278,18 +283,18 @@
 
         :param peer_domain_id: The domain ID of the peer
         :param nickname: The nickname for the peer domain
         :param alias: One of the aliases of the peer domain
         """
         if not peer_domain_id and (nickname or alias):
             peer_domain_id = self.get_peer(nickname=nickname, alias=alias)
-        self._client_func().domain_delete_peer(domain_id=self._domain, peer_domain_id=peer_domain_id)
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        general_api.domain_delete_peer(domain_id=self._domain, peer_domain_id=peer_domain_id)
 
     @exec_with_token
     def get_top_tags(self) -> List[str]:
         """
         Get domain tag info returns a list containing the top 100 tag names for the current session's domain.
         """
-        res = self._client_func().domain_get_tag_info(
-            domain_id=self._domain,
-        )
+        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
+        res = capsules_api.domain_get_tag_info(domain_id=self._domain)
         return [r.name for r in res.tags]
```

## antimatter/session_mixins/encryption_mixin.py

```diff
@@ -1,29 +1,30 @@
 from typing import Callable
 
-from antimatter.client import DefaultApi
+import antimatter.client as openapi_client
 from antimatter.session_mixins.token import exec_with_token
 
 
 class EncryptionMixin:
     """
     Session mixin defining CRUD functionality for encryption functionality.
 
     :param domain: The domain to use for the session.
     :param client: The client to use for the session.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
     @exec_with_token
     def flush_encryption_keys(self):
         """
         Flush all keys in memory. The keys will be immediately reloaded from persistent
         storage, forcing a check that the domain's root key is still available
         """
-        self._client_func().domain_flush_encryption_keys(domain_id=self._domain)
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
+        encryption_api.domain_flush_encryption_keys(domain_id=self._domain)
```

## antimatter/session_mixins/fact_mixin.py

```diff
@@ -1,43 +1,44 @@
 from typing import Any, Callable, Dict, List, Optional
 
 import antimatter.client as openapi_client
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.token import exec_with_token
 
 
 class FactMixin:
     """
     Session mixin defining CRUD functionality for facts and fact types.
 
     :param domain: The domain to use for the session.
     :param client: The client to use for the session.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
     @exec_with_token
     def list_fact_types(self):
         """
         Returns a list of fact types available for the current domain and auth
         """
-        return [fact.model_dump() for fact in self._client_func().domain_list_fact_types(self._domain).fact_types]
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        return [fact.model_dump() for fact in policy_api.domain_list_fact_types(self._domain).fact_types]
 
     @exec_with_token
     def list_facts(self, fact_type: str):
         """
         Returns a list of facts for the given fact type
         """
-        return [fact.model_dump() for fact in self._client_func().domain_list_facts(self._domain, fact_type=fact_type).facts]
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        return [fact.model_dump() for fact in policy_api.domain_list_facts(self._domain, fact_type=fact_type).facts]
 
     @exec_with_token
     def add_fact_type(
         self,
         name: str,
         description: str,
         arguments: Dict[str, str],
@@ -45,15 +46,16 @@
         """
         Upserts a fact type for the current domain and auth
 
         :param name: The "type name" for this fact, like "has_role"
         :param description: The human-readable description of the fact type
         :param arguments: Name:description argument pairs for the fact type
         """
-        self._client_func().domain_put_fact_type(
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        policy_api.domain_put_fact_type(
             domain_id=self._domain,
             fact_type=name,
             new_fact_type_definition=openapi_client.NewFactTypeDefinition(
                 description=description,
                 arguments=[
                     openapi_client.NewFactTypeDefinitionArgumentsInner(name=name, description=desc)
                     for name, desc in arguments.items()
@@ -70,82 +72,88 @@
         """
         Upserts a fact for the current domain and auth
 
         :param fact_type: The name of the type of fact being added
         :param arguments: The fact arguments to add
         :return: The upserted fact
         """
-        return self._client_func().domain_upsert_fact(
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        return policy_api.domain_upsert_fact(
             domain_id=self._domain,
             fact_type=fact_type,
             new_fact=openapi_client.NewFact(arguments=arguments)
         ).model_dump()
 
     @exec_with_token
     def get_fact_type(self, fact_type: str) -> Dict[str, Any]:
         """
         Get the fact type details for the given fact type
 
         :param fact_type: The "type name" for this fact, like "has_role"
         :return: The fact type details
         """
-        return self._client_func().domain_get_fact_type(
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        return policy_api.domain_get_fact_type(
             domain_id=self._domain, fact_type=fact_type
         ).model_dump()
 
     @exec_with_token
     def get_fact(self, fact_type: str, fact_id: str) -> Dict[str, Any]:
         """
         Returns the fact details for the given fact type and name
 
         :param fact_type: The "type name" for this fact, like "has_role"
         :param fact_id: The ID for the fact to be retrieved
         :return: The fact details
         """
-        return self._client_func().domain_get_fact_by_id(
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        return policy_api.domain_get_fact_by_id(
             domain_id=self._domain, fact_type=fact_type, fact_id=fact_id
         ).model_dump()
 
     @exec_with_token
     def delete_fact_type(self, fact_type: str) -> None:
         """
         Delete a fact type AND ALL FACTS INSIDE IT.
 
         :param fact_type: The "type name" for this fact, like "has_role"
         """
-        self._client_func().domain_delete_fact_type(domain_id=self._domain, fact_type=fact_type, confirm=fact_type)
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        policy_api.domain_delete_fact_type(domain_id=self._domain, fact_type=fact_type, confirm=fact_type)
 
     @exec_with_token
     def delete_fact(
         self,
         fact_type: str,
+        *arguments: str,
         fact_id: Optional[str] = None,
-        arguments: Optional[List[str]] = None,
     ) -> None:
         """
         Delete a fact by ID or argument. One of 'fact_id' or 'arguments' must be
         provided. If 'fact_id' is provided, it will be used solely. If arguments
         are provided, each must fully match the name and/or arguments of the fact
         for it to be deleted.
 
         :param fact_type: The "type name" for this fact, like "has_role"
         :param fact_id: The ID for the fact to be deleted
         :param arguments: The arguments for the fact to be deleted
         """
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
         if fact_id is None and arguments is not None:
             for fact in self.list_facts(fact_type=fact_type):
-                if arguments == fact.get("arguments", []):
-                    self._client_func().domain_delete_fact_by_id(
+                if list(arguments) == fact.get("arguments", []):
+                    policy_api.domain_delete_fact_by_id(
                         domain_id=self._domain, fact_type=fact_type, fact_id=fact["id"])
         else:
-            self._client_func().domain_delete_fact_by_id(domain_id=self._domain, fact_type=fact_type, fact_id=fact_id)
+            policy_api.domain_delete_fact_by_id(domain_id=self._domain, fact_type=fact_type, fact_id=fact_id)
 
     @exec_with_token
     def delete_all_facts(self, fact_type: str) -> None:
         """
         Delete all the facts for the given fact type.
 
         :param fact_type: The "type name" for this fact, like "has_role"
         """
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
         for fact in self.list_facts(fact_type=fact_type):
-            self._client_func().domain_delete_fact_by_id(
+            policy_api.domain_delete_fact_by_id(
                 domain_id=self._domain, fact_type=fact_type, fact_id=fact["id"])
```

## antimatter/session_mixins/general_mixin.py

```diff
@@ -1,28 +1,27 @@
 from datetime import datetime, timezone
 from typing import Any, Callable, Dict, Iterator, List, Optional
 
 import antimatter.client as openapi_client
 from antimatter.builders.settings_patch import SettingsPatchBuilder
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.serializers.identity_details import serialize_identity_provider_info_dict
 from antimatter.session_mixins.token import exec_with_token
 
 
 class GeneralMixin:
     """
     Session mixin defining CRUD functionality for other general functionality.
 
     :param domain: The domain to use for the session.
     :param client: The client to use for the session.
     """
 
     _page_res_size: int = 100
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
@@ -30,81 +29,88 @@
     def get_private_info(self) -> Dict[str, Any]:
         """
         Returns a Domain's summary information.
 
         :return: The private summary info for a domain
         """
         # Disable warnings because of a bug in DomainIdentityProviderDetails autogenerated code
-        res = self._client_func().domain_get_private_info(domain_id=self._domain).model_dump(warnings=False)
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        res = general_api.domain_get_private_info(domain_id=self._domain).model_dump(warnings=False)
         if "identity_providers" in res:
             res["identity_providers"] = [
                 serialize_identity_provider_info_dict(prov) for prov in res["identity_providers"]
             ]
         return res
 
     def get_public_info(self) -> Dict[str, Any]:
         """
         Returns a Domain's summary information. This endpoint does not require
         authorization
 
         :return: The public summary info for a domain
         """
         # Disable warnings because of a bug in DomainIdentityProviderDetails autogenerated code
-        res = self._client_func().domain_get_public_info(domain_id=self._domain).model_dump(warnings=False)
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        res = general_api.domain_get_public_info(domain_id=self._domain).model_dump(warnings=False)
         if "identity_providers" in res:
             res["identity_providers"] = [
                 serialize_identity_provider_info_dict(prov) for prov in res["identity_providers"]
             ]
         return res
 
     @exec_with_token
     def get_settings(self) -> Dict[str, Any]:
         """
         Return the domain settings.
         """
-        return self._client_func().domain_get_settings(domain_id=self._domain).model_dump()
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        return general_api.domain_get_settings(domain_id=self._domain).model_dump()
 
     @exec_with_token
     def patch_settings(self, *patch: SettingsPatchBuilder) -> Dict[str, Any]:
         """
         Applies the given patch to the domain settings. The user must have
         permissions on all resources the patch references.
 
         :param patch: The patch or patches to make to the settings. The path is the patch is
                         a JSON pointer path.
         :return: The domain settings after applying the patch
         """
-        return self._client_func().domain_patch_settings(
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        return general_api.domain_patch_settings(
             domain_id=self._domain,
             domain_settings_patch=openapi_client.DomainSettingsPatch(patch=[p.build() for p in patch])
         ).model_dump()
 
     @exec_with_token
     def get_status(self) -> Dict[str, Any]:
         """
         Return the domain status, which contains important notifications for
         administrators of the domain.
         """
-        return self._client_func().domain_get_status(domain_id=self._domain).model_dump()
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
+        return general_api.domain_get_status(domain_id=self._domain).model_dump()
 
     @exec_with_token
     def list_hooks(self) -> List[Dict[str, Any]]:
         """
         Return a list of available hooks in this domain. A hook is a data processor,
         like a PII classifier
         """
-        return [h.model_dump() for h in self._client_func().domain_list_hooks(domain_id=self._domain).hooks]
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return [h.model_dump() for h in contexts_api.domain_list_hooks(domain_id=self._domain).hooks]
 
     @exec_with_token
     def list_resources(self) -> Dict[str, Any]:
         """
         Return a list of resource strings that can be used in policy rules, and
         the set of permissions that you can assign to them.
         """
-        return self._client_func().domain_list_resources(domain_id=self._domain).model_dump()
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        return policy_api.domain_list_resources(domain_id=self._domain).model_dump()
 
     @exec_with_token
     def query_access_log(
         self,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
         session: Optional[str] = None,
@@ -145,14 +151,15 @@
                     not specified, this field is ignored
         :param redacted_or_tokenized_tag: The redacted or tokenized tag key you would like ot filter on. This accepts
                     a tag key only and will return all redacted and tokenized tag key results
                     matching the provided tag key. If not specified, this field is ignored
         :param capsule_id: The ID for a specific capsule. Use this to limit results to a single capsule
         :return: An iterator over the access logs matching the filters
         """
+        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
         pagination = None
         has_more = True
         if start_date is not None:
             start_date = start_date.astimezone(timezone.utc)
         if end_date is not None:
             end_date = end_date.astimezone(timezone.utc)
         while has_more:
@@ -165,17 +172,17 @@
                 "location": location,
                 "location_prefixed": location_prefixed,
                 "operation_type": operation_type,
                 "allowed_tag": allowed_tag,
                 "redacted_or_tokenized_tag": redacted_or_tokenized_tag,
             }
             if capsule_id is None:
-                res = self._client_func().domain_query_access_log(domain_id=self._domain, **kwargs)
+                res = capsules_api.domain_query_access_log(domain_id=self._domain, **kwargs)
             else:
-                res = self._client_func().domain_query_access_log_single_capsule(
+                res = capsules_api.domain_query_access_log_single_capsule(
                     domain_id=self._domain, capsule_id=capsule_id, **kwargs,
                 )
             has_more = res.has_more
             for log in res.results:
                 pagination = log.id
                 yield log.model_dump()
 
@@ -207,22 +214,23 @@
                     will return results starting with the provided string. If not specified,
                     this field is ignored
         :param description: The description you would like to filter on. This is an in matched filter
                     and will return results that  contain the provided string. If not specified,
                     this field is ignored
         :return: An iterator over the control logs matching the filters
         """
+        general_api = openapi_client.GeneralApi(api_client=self._client_func())
         pagination = None
         has_more = True
         if start_date is not None:
             start_date = start_date.astimezone(timezone.utc)
         if end_date is not None:
             end_date = end_date.astimezone(timezone.utc)
         while has_more:
-            res = self._client_func().domain_query_control_log(
+            res = general_api.domain_query_control_log(
                 domain_id=self._domain,
                 start_date=start_date,
                 end_date=end_date,
                 num_results=self._page_res_size,
                 start_from_id=pagination,
                 session=session,
                 url=url,
```

## antimatter/session_mixins/identity_provider_mixin.py

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import antimatter.client as openapi_client
 from antimatter.constants.identity_provider import PrincipalType, ProviderType
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.serializers.identity_details import serialize_identity_principal_details_dict, \
     serialize_identity_provider_info_dict
 from antimatter.session_mixins.token import exec_with_token
+from antimatter.capabilities import CapabilityConverter
 
 
 class OverrideDomainIdentityPrincipalDetails(openapi_client.DomainIdentityPrincipalDetails):
     """
     This override provides a local way to pass domain identity principal details
     to the openapi generated client that mitigates the pydantic serializing error
     it produces due to a bug in the generator.
@@ -36,15 +36,15 @@
     """
     Session mixin defining identity provider CRUD functionality.
 
     :param domain: The domain to use for the session.
     :param client: The client to use for the session.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
@@ -59,97 +59,108 @@
         Create or update an identity provider.
 
         :param provider_name: The name of a new or existing identity provider
         :param provider_type: The provider type for identity management
         :param client_id: If the provider type is 'GoogleOAuth', a client ID must be provided
         :return: The identity provider summary
         """
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
         provider_type = ProviderType(provider_type)
         provider_params = None
-        match ProviderType(provider_type):
-            case ProviderType.GoogleOAuth:
-                provider_params = openapi_client.GoogleOAuthDomainIdentityProviderDetails(
-                    type=ProviderType.GoogleOAuth.value,
-                    client_id=client_id,
-                )
-            case ProviderType.ApiKey:
-                provider_params = openapi_client.APIKeyDomainIdentityProviderDetails(
-                    type=ProviderType.ApiKey.value,
-                )
-
+        if ProviderType(provider_type) is ProviderType.GoogleOAuth:
+            provider_params = openapi_client.GoogleOAuthDomainIdentityProviderDetails(
+                type=ProviderType.GoogleOAuth.value,
+                client_id=client_id,
+            )
+        elif ProviderType(provider_type) is ProviderType.ApiKey:
+            provider_params = openapi_client.APIKeyDomainIdentityProviderDetails(
+                type=ProviderType.ApiKey.value,
+            )
         # Disable warnings because of a bug in DomainIdentityProviderDetails autogenerated code
-        res = self._client_func().domain_upsert_identity_provider(
+        res = auth_api.domain_upsert_identity_provider(
             domain_id=self._domain,
             identity_provider_name=provider_name,
             domain_identity_provider_details=openapi_client.DomainIdentityProviderDetails(provider_params)
         ).model_dump(warnings=False)
         return serialize_identity_provider_info_dict(res)
 
     @exec_with_token
     def insert_identity_provider_principal(
         self,
         provider_name: str,
-        capabilities: Dict[str, str],
+        capabilities: List[Union[str, Dict[str, Any]]],
         principal_type: Union[str, PrincipalType],
         principal_value: Optional[str] = None,
         comment: Optional[str] = None,
     ) -> Dict[str, str]:
         """
         Creates a new principal for the provider. Note that the provider_name
         must refer to an existing identity provider. The principal_value is
         optional if the type is APIKey.
 
         :param provider_name: The name of an existing identity provider
-        :param capabilities: The capabilities to attach to the principal
+        :param capabilities: The capabilities to attach to the principal. These can be in one of the following forms:
+                - A list of unary capabilities, like ['admin', 'read_only']
+                - A list of key-value pairs, like ["admin=True", "read_only=False"]
+                - A list of dictionaries, like [{"admin": "True"}, {"read_only": "False"}]
+                - A list of dictionaries as a name/value pair, like [{"name": "admin", "value": "True"}, {"name": "read_only", "value": "False"}]
+                - Any combination of the above
         :param principal_type: The type of principal to create. One of 'APIKey', 'Email', or 'HostedDomain'
         :param principal_value: The appropriate identifying value for the principal, depending on type
+        :param comment: An optional comment for the identity provider principal
         :return: The ID of the inserted principal and any additional metadata
         """
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        capabilities = CapabilityConverter.convert_capabilities(capabilities)
         principal_type = PrincipalType(principal_type)
         inner_params = None
-        match PrincipalType(principal_type):
-            case PrincipalType.ApiKey:
-                inner_params = openapi_client.DomainIdentityAPIKeyPrincipalParams(
-                    type=principal_type.value, api_key_id=principal_value,
-                    comment=comment,
-                )
-            case PrincipalType.Email:
-                inner_params = openapi_client.DomainIdentityEmailPrincipalParams(
-                    type=principal_type.value, email=principal_value,
-                    comment=comment,
-                )
-            case PrincipalType.HostedDomain:
-                inner_params = openapi_client.DomainIdentityHostedDomainPrincipalParams(
-                    type=principal_type.value, hosted_domain=principal_value,
-                    comment=comment,
-                )
-        return self._client_func().domain_insert_identity_provider_principal(
+        if PrincipalType(principal_type) is PrincipalType.ApiKey:
+            inner_params = openapi_client.DomainIdentityAPIKeyPrincipalParams(
+                type=principal_type.value, api_key_id=principal_value,
+                comment=comment,
+            )
+        elif PrincipalType(principal_type) is PrincipalType.Email:
+            inner_params = openapi_client.DomainIdentityEmailPrincipalParams(
+                type=principal_type.value, email=principal_value, comment=comment,
+            )
+        elif PrincipalType(principal_type) is PrincipalType.HostedDomain:
+            inner_params = openapi_client.DomainIdentityHostedDomainPrincipalParams(
+                type=principal_type.value, hosted_domain=principal_value, comment=comment,
+            )
+        return auth_api.domain_insert_identity_provider_principal(
             domain_id=self._domain,
             identity_provider_name=provider_name,
             domain_identity_provider_principal_params=openapi_client.DomainIdentityProviderPrincipalParams(
                 capabilities=[openapi_client.Capability(name=k, value=v) for k, v in capabilities.items()],
                 details=OverrideDomainIdentityPrincipalDetails(inner_params)
             ),
         ).model_dump(exclude_none=True)
 
     @exec_with_token
     def update_identity_provider_principal(
         self,
         provider_name: str,
         principal_id: str,
-        capabilities: Dict[str, str],
+        capabilities: List[Union[str, Dict[str, Any]]],
     ) -> None:
         """
         Update the capabilities for an identity provider principal.
 
         :param provider_name: The name of an existing identity provider
         :param principal_id: The ID of the principal
-        :param capabilities: The capabilities to attach to the principal
-        """
-        self._client_func().domain_update_identity_provider_principal(
+        :param capabilities: The capabilities to attach to the principal. These can be in one of the following forms:
+                - A list of unary capabilities, like ['admin', 'read_only']
+                - A list of key-value pairs, like ["admin=True", "read_only=False"]
+                - A list of dictionaries, like [{"admin": "True"}, {"read_only": "False"}]
+                - A list of dictionaries as a name/value pair, like [{"name": "admin", "value": "True"}, {"name": "read_only", "value": "False"}]
+                - Any combination of the above
+        """
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        capabilities = CapabilityConverter.convert_capabilities(capabilities)
+        auth_api.domain_update_identity_provider_principal(
             domain_id=self._domain,
             identity_provider_name=provider_name,
             principal_id=principal_id,
             capability_list=openapi_client.CapabilityList(
                 capabilities=[openapi_client.Capability(name=k, value=v) for k, v in capabilities.items()]
             ),
         )
@@ -158,26 +169,28 @@
     def get_identity_provider(self, provider_name: str) -> Dict[str, Any]:
         """
         Retrieve detailed information and configuration of an identity provider
 
         :param provider_name: The name of an existing identity provider
         :return: The identity provider details
         """
-        res = self._client_func().domain_get_identity_provider(
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        res = auth_api.domain_get_identity_provider(
             domain_id=self._domain, identity_provider_name=provider_name,
         ).model_dump(warnings=False)
         return serialize_identity_provider_info_dict(res)
 
     @exec_with_token
     def list_identity_providers(self) -> List[Dict[str, Any]]:
         """
         Retrieve the domain's identity providers and a brief overview of their
         configuration.
         """
-        res = self._client_func().domain_list_identity_providers(domain_id=self._domain)
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        res = auth_api.domain_list_identity_providers(domain_id=self._domain)
         if not res.identity_providers:
             return []
 
         # Disable warnings because of a bug in DomainIdentityProviderDetails autogenerated code
         return [
             serialize_identity_provider_info_dict(prov.model_dump(warnings=False))
             for prov in res.identity_providers
@@ -194,27 +207,28 @@
         detailed information about a single principal if a principal_id is
         provided
 
         :param provider_name: The name of an existing identity provider
         :param principal_id: The ID of the principal; None to get all principals
         :return: The principal information
         """
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
         if principal_id is None:
-            res = self._client_func().domain_get_identity_provider_principals(
+            res = auth_api.domain_get_identity_provider_principals(
                 domain_id=self._domain, identity_provider_name=provider_name,
             )
             principals = []
             for principal in res.principals:
                 principal = principal.model_dump()
                 if t := principal.get("principal_type"):
                     principal["principal_type"] = t.value
                 principals.append(principal)
             return principals
         else:
-            res = self._client_func().domain_get_identity_provider_principal(
+            res = auth_api.domain_get_identity_provider_principal(
                 domain_id=self._domain,
                 identity_provider_name=provider_name,
                 principal_id=principal_id,
             )
             return serialize_identity_principal_details_dict(res.model_dump(warnings=False))
 
     @exec_with_token
@@ -223,24 +237,26 @@
         Delete an identity provider. All domain tokens created using this
         identity provider will be invalidated. Take care not to remove the
         identity provider that is providing you admin access to your domain, as
         you may lock yourself out.
 
         :param provider_name: The name of the identity provider to fully delete
         """
-        self._client_func().domain_delete_identity_provider(domain_id=self._domain, identity_provider_name=provider_name)
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        auth_api.domain_delete_identity_provider(domain_id=self._domain, identity_provider_name=provider_name)
 
     @exec_with_token
     def delete_identity_provider_principal(
         self, provider_name: str, principal_id: str,
     ) -> None:
         """
         Delete an identity provider principal.
 
         :param provider_name: The name of the identity provider to delete a principal from
         :param principal_id: The ID of the principal to delete
         """
-        self._client_func().domain_delete_identity_provider_principal(
+        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        auth_api.domain_delete_identity_provider_principal(
             domain_id=self._domain,
             identity_provider_name=provider_name,
             principal_id=principal_id,
         )
```

## antimatter/session_mixins/policy_rule_mixin.py

```diff
@@ -1,41 +1,40 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import antimatter.client as openapi_client
 from antimatter.constants import domain_policy
 from antimatter.builders.capability import CapabilityRulesBuilder
 from antimatter.builders.fact_policy import FactPoliciesBuilder
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.token import exec_with_token
 
 
 class PolicyRuleMixin:
     """
     Session mixin defining policy rule CRUD functionality.
 
     :param domain: The domain to use for the session.
     :param client: The client to use for the session.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
     @exec_with_token
     def create_policy_rule(
             self,
             capability_rules: CapabilityRulesBuilder,
             path: str,
             operation: Union[str, domain_policy.Operation],
             result: Union[str, domain_policy.Result],
-            priority: int,
+            priority: int = 0,
             facts: Optional[FactPoliciesBuilder] = None,
             disabled: bool = False,
     ) -> Dict[str, Any]:
         """
         Create a policy rule for the domain.
 
         :param capability_rules: Rules referring to domain identity capabilities. These rules are ANDed together
@@ -44,17 +43,18 @@
         :param path: The path this rule governs. May contain glob expressions (e.g. '*' and '**')
         :param operation: The operation to apply the policy to
         :param result: Whether to 'allow' or 'deny' the operation performed that matches this rule
         :param priority: The priority of this rule. Lower priority rules are evaluated first
         :param disabled: If this rule is disabled or not
         :return: A dictionary containing the created rule from the server
         """
-        res = self._client_func().domain_create_policy_rule(
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        res = policy_api.domain_create_policy_rule(
             domain_id=self._domain,
-            domain_policy_rule=openapi_client.DomainPolicyRule(
+            new_domain_policy_rule=openapi_client.NewDomainPolicyRule(
                 domain_identity=capability_rules.build(),
                 facts=facts.build(),
                 path=path,
                 operation=domain_policy.Operation(operation).value,
                 result=domain_policy.Result(result).value,
                 priority=priority,
                 disabled=disabled,
@@ -66,24 +66,26 @@
     @exec_with_token
     def delete_policy_rule(self, rule_id: str):
         """
         Delete a domain policy rule on the session's domain.
 
         :param rule_id: Identifier of the policy rule to delete
         """
-        self._client_func().domain_delete_policy_rule(domain_id=self._domain, rule_id=rule_id)
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        policy_api.domain_delete_policy_rule(domain_id=self._domain, rule_id=rule_id)
 
     @exec_with_token
     def list_policy_rules(self):
         """
         Get the domain's policy rules.
 
         :return: A list of policy rules.
         """
-        res = self._client_func().domain_list_policy_rules(domain_id=self._domain)
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        res = policy_api.domain_list_policy_rules(domain_id=self._domain)
         policy_rules = []
         for rule in res.rules:
             policy_rules.append(rule.model_dump())
         return policy_rules
 
     @exec_with_token
     def update_policy_rule(
@@ -106,18 +108,19 @@
                     These assertions will be ANDed together, and ANDed with the capability rules.
         :param path: The path this rule governs. May contain glob expressions (e.g. '*' and '**')
         :param operation: The operation to apply the policy to
         :param result: Whether to 'allow' or 'deny' the operation performed that matches this rule
         :param priority: The priority of this rule. Lower priority rules are evaluated first
         :param disabled: If this rule is disabled or not
         """
-        self._client_func().domain_update_policy_rule(
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        policy_api.domain_update_policy_rule(
             domain_id=self._domain,
             rule_id=rule_id,
-            domain_policy_rule=openapi_client.DomainPolicyRule(
+            new_domain_policy_rule=openapi_client.NewDomainPolicyRule(
                 domain_identity=capability_rules.build(),
                 facts=facts.build(),
                 path=path,
                 operation=domain_policy.Operation(operation).value,
                 result=domain_policy.Result(result).value,
                 priority=priority,
                 disabled=disabled,
@@ -127,12 +130,13 @@
     @exec_with_token
     def renumber_policy_rules(self) -> List[Dict[str, Any]]:
         """
         Re-assign rule priority numbers for the session's domain to integer multiples of 10
 
         :return: The full list of renumbered policy rules in this domain
         """
-        res = self._client_func().domain_renumber_policy_rules(domain_id=self._domain)
+        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
+        res = policy_api.domain_renumber_policy_rules(domain_id=self._domain)
         policy_rules = []
         for rule in res.rules:
             policy_rules.append(rule.model_dump())
         return policy_rules
```

## antimatter/session_mixins/read_context_mixin.py

```diff
@@ -1,22 +1,22 @@
 from typing import Any, Callable, Dict, List
 
+import antimatter.client as openapi_client
 from antimatter.builders import ReadContextBuilder, ReadContextRuleBuilder
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.token import exec_with_token
 
 
 class ReadContextMixin:
     """
     Session mixin defining CRUD functionality for read contexts.
 
     :param domain: The domain to use for the session.
     :param client: The client to use for the session.
     """
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
@@ -28,70 +28,76 @@
     ) -> None:
         """
         Upserts a read context for the current domain and auth
 
         :param name: The name of the read context to add or update
         :param builder: The builder containing read context configuration
         """
-        self._client_func().domain_upsert_read_context(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_upsert_read_context(
             domain_id=self._domain, context_name=name, add_read_context=builder.build(),
         )
 
     @exec_with_token
     def list_read_context(self) -> List[Dict[str, Any]]:
         """
         Returns a list of read contexts available for the current domain and auth
         """
-        return [ctx.model_dump() for ctx in self._client_func().domain_list_read_contexts(self._domain).read_contexts]
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return [ctx.model_dump() for ctx in contexts_api.domain_list_read_contexts(self._domain).read_contexts]
 
     @exec_with_token
     def describe_read_context(self, name: str) -> Dict[str, Any]:
         """
         Returns the read context with the given name for the current domain and auth
 
         :param name: The name of the read context to describe
         :return: The full details of the read context
         """
-        return self._client_func().domain_get_read_context(self._domain, context_name=name).model_dump()
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return contexts_api.domain_get_read_context(self._domain, context_name=name).model_dump()
 
     @exec_with_token
     def delete_read_context(self, name: str) -> None:
         """
         Delete a read context. All configuration associated with this read
         context will also be deleted. Domain policy rules referencing this read
         context will be left as-is.
 
         :param name: The name of the read context to delete
         """
-        self._client_func().domain_delete_read_context(domain_id=self._domain, context_name=name)
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_delete_read_context(domain_id=self._domain, context_name=name)
 
     @exec_with_token
     def list_read_context_rules(self, name: str) -> List[Dict[str, Any]]:
         """
         List all rules for the read context
 
         :param name: The name of the read context to list rules from
         :return: The list of read context rules
         """
-        return [r.model_dump() for r in self._client_func().domain_get_read_context(self._domain, context_name=name).rules]
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return [r.model_dump() for r in contexts_api.domain_get_read_context(self._domain, context_name=name).rules]
 
     @exec_with_token
     def add_read_context_rules(
         self,
         name: str,
         rule_builder: ReadContextRuleBuilder,
     ) -> str:
         """
         Adds rules to a read context
 
         :param name: The name of the read context to add rules to
         :param rule_builder: The builder containing rule configuration for the read context
         :return: The unique ID for the added read context rule
         """
-        return self._client_func().domain_add_read_context_rule(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return contexts_api.domain_add_read_context_rule(
             domain_id=self._domain,
             context_name=name,
             new_read_context_config_rule=rule_builder.build()
         ).id
 
     @exec_with_token
     def update_read_context_rule(
@@ -103,15 +109,16 @@
         """
         Update a read context configuration rule. The rule must already exist.
 
         :param name: The name of the read context to update a rule for
         :param rule_id: The unique ID of the rule to update
         :param rule_builder: The builder containing rule configuration
         """
-        self._client_func().domain_update_read_context_rule(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_update_read_context_rule(
             domain_id=self._domain,
             context_name=name,
             rule_id=rule_id,
             new_read_context_config_rule=rule_builder.build()
         )
 
     @exec_with_token
@@ -122,26 +129,38 @@
     ) -> None:
         """
         Deletes a rule from a read context
 
         :param name: The name of the read context to delete a rule from
         :param rule_id: The unique ID of the rule to delete
         """
-        self._client_func().domain_delete_read_context_rule(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_delete_read_context_rule(
             domain_id=self._domain,
             context_name=name,
             rule_id=rule_id,
         )
 
     @exec_with_token
     def delete_read_context_rules(self, name: str) -> None:
         """
         Deletes all the read context rules
 
         :param name: The name of the read context to delete all the rules from
         """
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
         for rule in self.list_read_context_rules(name):
-            self._client_func().domain_delete_read_context_rule(
+            contexts_api.domain_delete_read_context_rule(
                 domain_id=self._domain,
                 context_name=name,
                 rule_id=rule["id"],
             )
+
+    @exec_with_token
+    def flush_read_context(self, name: str) -> None:
+        """
+        Flushes the read context and all associated rules
+
+        :param name: The name of the read context to flush
+        """
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_read_context_flush(domain_id=self._domain, context_name=name)
```

## antimatter/session_mixins/root_encryption_key_mixin.py

```diff
@@ -1,61 +1,64 @@
 from typing import Any, Callable, Dict, List
 
-from antimatter.client import DefaultApi, KeyInfos, ActiveRootEncryptionKeyID
+import antimatter.client as openapi_client
 from antimatter.session_mixins.token import exec_with_token
 
 
 class RootEncryptionKeyMixin:
     """
     Session mixin defining CRUD functionality for root encryption keys
 
     :param domain: The domain to use for the session.
     :param client: The client to use for the session.
     """
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
     @exec_with_token
     def get_active_root_encryption_key(self) -> Dict[str, Any]:
         """
         Get the active root encryption key
 
         :return: The active root encryption key
         """
-        return self._client_func().domain_get_active_external_root_encryption_key(domain_id=self._domain).model_dump()
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
+        return encryption_api.domain_get_active_external_root_encryption_key(domain_id=self._domain).model_dump()
 
     @exec_with_token
     def list_root_encryption_keys(self) -> List[Dict[str, Any]]:
         """
         List all root encryption keys
 
         :return: A list of root encryption keys
         """
-        return [key.model_dump() for key in self._client_func().domain_list_external_root_encryption_key(domain_id=self._domain)]
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
+        return [key.model_dump() for key in encryption_api.domain_list_external_root_encryption_key(domain_id=self._domain)]
 
     @exec_with_token
     def test_root_encryption_key(self, root_encryption_key_id: str) -> Dict[str, Any]:
         """
         Attempt to test a root encryption key to encrypt and decrypt
 
         :param key: The key to test
         :return: The result of the test
         """
-        return self._client_func().domain_external_root_encryption_key_test(
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
+        return encryption_api.domain_external_root_encryption_key_test(
             domain_id=self._domain,root_encryption_key_id=root_encryption_key_id,
             body={}
         ).model_dump()
     
     @exec_with_token
-    def add_root_encryption_key(self, key_infos: KeyInfos, description: str = "") -> str:
+    def add_root_encryption_key(self, key_infos: openapi_client.KeyInfos, description: str = "") -> str:
         """
         Add a new root encryption key.
         Use the builder functions in `antimatter.builders.root_encryption_key` to create the key information.
 
         For example:
         ```
         key_info = antimatter.builders.antimatter_delegated_aws_key_info(key_arn="key_arn")
@@ -68,61 +71,71 @@
 
         key_info = antimatter.builders.gcp_service_account_key_info(
             service_account_credentials="service_account_credentials", project_id="project_id", location="location"
         )
         key_id = session.add_root_encryption_key(key_info)
         ```
 
-        :param key: The key to add
+        :param key_infos: The key information to add
         :param description: The description of the key
         """
         assert key_infos is not None, "Key information is required"
+
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
         key_infos.description = description
-        return self._client_func().domain_add_external_root_encryption_key(
+        return encryption_api.domain_add_external_root_encryption_key(
             domain_id=self._domain,
             key_infos=key_infos
         ).rek_id
 
     @exec_with_token
     def delete_root_encryption_key(self, root_encryption_key_id: str):
         """
         Delete a root encryption key. Only possible if key is not in use by any data key encryption keys
 
         :param key: The key to delete
         """
-        self._client_func().domain_delete_external_root_encryption_key(
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
+        encryption_api.domain_delete_external_root_encryption_key(
             domain_id=self._domain,
             root_encryption_key_id=root_encryption_key_id
         )
 
     @exec_with_token
     def set_active_root_encryption_key(self, root_encryption_key_id: str) -> None:
         """
         Set the active root encryption key for the domain
 
         :param key: The key to set as active
         """
-        self._client_func().domain_set_active_external_root_encryption_key(
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
+        encryption_api.domain_set_active_external_root_encryption_key(
             domain_id=self._domain,
-            active_root_encryption_key_id=ActiveRootEncryptionKeyID(key_id=root_encryption_key_id)
+            active_root_encryption_key_id=openapi_client.ActiveRootEncryptionKeyID(key_id=root_encryption_key_id)
         )
 
     @exec_with_token
-    def rotate_encryption_keys(self) -> None:
+    def rotate_encryption_keys(self) -> bool:
         """
-        Rotates the root encryption keys. This is a batched operation and "has_more"
-        will indicate whether there are more key encryption keys that can be rotated.
+        Rotates the root encryption keys. This is a batched operation and if 'True' is
+        returned, this indicates whether there are more key encryption keys that can be rotated.
         """
-        return self._client_func().domain_rotate_root_encryption_keys(
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
+        return encryption_api.domain_rotate_root_encryption_keys(
             domain_id=self._domain, body={},
-        ).model_dump()
+        ).has_more
 
     @exec_with_token
     def list_key_providers(self) -> List[Dict[str, Any]]:
         """
         Retrieve the domain's key providers and a brief overview of their
         configuration.
         """
-        res = self._client_func().domain_get_external_root_encryption_key_providers(domain_id=self._domain)
+        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
+        res = encryption_api.domain_get_external_root_encryption_key_providers(domain_id=self._domain)
         if not res.providers:
             return []
-        return [provider.actual_instance.model_dump() for provider in res.providers if provider.actual_instance is not None]
+        return [
+            provider.actual_instance.model_dump()
+            for provider in res.providers
+            if provider.actual_instance is not None
+        ]
```

## antimatter/session_mixins/token.py

```diff
@@ -31,31 +31,31 @@
                 return None, None
             return not_before, not_after
 
         def is_token_valid(not_before, not_after):
             now_time = datetime.now(timezone.utc)
             return not_before and not_after and (not_before <= now_time <= not_after)
 
-        token = self._client_func().api_client.configuration.access_token
+        token = self._client_func().configuration.access_token
         if not token:
             if not self._try_init_client():
                 raise errors.SessionVerificationPendingError(ADMIN_VERIFICATION_PROMPT)
-            token = self._client_func().api_client.configuration.access_token
+            token = self._client_func().configuration.access_token
 
         not_before, not_after = decode_token(token)
 
         if not is_token_valid(not_before, not_after):
             token = self.refresh_token()
             not_before, not_after = decode_token(token)
 
             if not is_token_valid(not_before, not_after):
                 if not (not_before and not_after):
                     raise errors.TokenMalformed("malformed token detected")
                 raise errors.TokenExpiredError("token has expired")
 
         # If all is good, we store the token.
-        self._client_func().api_client.configuration.access_token = token
+        self._client_func().configuration.access_token = token
 
         # Call the decorated function.
         return f(self, *args, **kwargs)
 
     return wrapper
```

## antimatter/session_mixins/verification_mixin.py

```diff
@@ -1,25 +1,30 @@
 from typing import Callable, Optional
 
 import antimatter.client as openapi_client
-from antimatter.client import DefaultApi
 from antimatter.errors import errors
 
 ADMIN_VERIFICATION_PROMPT = (
     "domain not authenticated - check email to verify account; verification email "
     "can be sent again with session.resend_verification_email()"
 )
 
 
 class VerificationMixin:
     """
     Session mixin defining CRUD functionality for verification actions.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], email: Optional[str], **kwargs):
+    def __init__(
+        self,
+        domain: str,
+        client_func: Callable[[], openapi_client.ApiClient],
+        email: Optional[str],
+        **kwargs,
+    ):
         try:
             super().__init__(domain=domain, client_func=client_func, email=email, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
         self._email = email
@@ -30,13 +35,14 @@
         was called with an email, that will be used if none is provided.
 
         :param email: The email to resend the verification email for.
         """
         if not email and not self._email:
             raise errors.SessionVerificationPendingError("unable to resend verification email: email unknown")
 
-        self._client_func().domain_contact_issue_verify(
+        authentication_api = openapi_client.AuthenticationApi(api_client=self._client_func())
+        authentication_api.domain_contact_issue_verify(
             domain_id=self._domain,
             domain_contact_issue_verify_request=openapi_client.DomainContactIssueVerifyRequest(
                 admin_email=email or self._email,
             )
         )
```

## antimatter/session_mixins/write_context_mixin.py

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Callable, Dict, List
 
+import antimatter.client as openapi_client
 from antimatter.builders import WriteContextBuilder, WriteContextConfigurationBuilder, WriteContextRegexRuleBuilder
-from antimatter.client import DefaultApi
 from antimatter.session_mixins.token import exec_with_token
 
 
 class WriteContextMixin:
     """
     Session mixin defining CRUD functionality for write contexts.
 
     :param domain: The domain to use for the session.
     :param client: The client to use for the session.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], DefaultApi], **kwargs):
+    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
         try:
             super().__init__(domain=domain, client_func=client_func, **kwargs)
         except TypeError:
             super().__init__()  # If this is last mixin, super() will be object()
         self._domain = domain
         self._client_func = client_func
 
@@ -29,73 +29,79 @@
     ) -> None:
         """
         Upserts a write context for the current domain and auth
 
         :param name: The name of the write context to add or update
         :param builder: The builder containing write context configuration
         """
-        self._client_func().domain_upsert_write_context(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_upsert_write_context(
             domain_id=self._domain, context_name=name, add_write_context=builder.build(),
         )
 
     @exec_with_token
     def list_write_context(self) -> List[Dict[str, Any]]:
         """
         Returns a list of write contexts available for the current domain and auth
         """
-        return [ctx.model_dump() for ctx in self._client_func().domain_list_write_contexts(self._domain).write_contexts]
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return [ctx.model_dump() for ctx in contexts_api.domain_list_write_contexts(self._domain).write_contexts]
 
     @exec_with_token
     def describe_write_context(self, name: str) -> Dict[str, Any]:
         """
         Returns the write context with the given name for the current domain and auth
 
         :param name: The name of the write context to describe
         :return: The full details of the write context
         """
-        return self._client_func().domain_describe_write_context(self._domain, context_name=name).model_dump()
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return contexts_api.domain_describe_write_context(self._domain, context_name=name).model_dump()
 
     @exec_with_token
     def upsert_write_context_configuration(
         self,
         name: str,
         builder: WriteContextConfigurationBuilder,
     ) -> None:
         """
         Update a write context configuration. The write context must already exist.
 
         :param name: The name of the write context to update the configuration for
         :param builder: The builder containing write context configuration
         """
-        self._client_func().domain_upsert_write_context_configuration(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_upsert_write_context_configuration(
             domain_id=self._domain,
             context_name=name,
             write_context_config_info=builder.build(),
         )
 
     @exec_with_token
     def delete_write_context(self, name: str) -> None:
         """
         Delete a write context. All configuration associated with this write
         context will also be deleted. Domain policy rules referencing this write
         context will be left as-is.
 
         :param name: The name of the write context to delete
         """
-        self._client_func().domain_delete_write_context(domain_id=self._domain, context_name=name)
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_delete_write_context(domain_id=self._domain, context_name=name)
 
     @exec_with_token
     def list_write_context_regex_rules(self, context_name: str) -> List[Dict[str, Any]]:
         """
         List all regex rules for the write context.
 
         :param context_name: The name of the write context
         :return: The list of rules
         """
-        return [rule.model_dump() for rule in self._client_func().domain_get_write_context_regex_rules(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return [rule.model_dump() for rule in contexts_api.domain_get_write_context_regex_rules(
             domain_id=self._domain,
             context_name=context_name,
         )]
 
     @exec_with_token
     def insert_write_context_regex_rule(
         self,
@@ -104,40 +110,43 @@
     ) -> str:
         """
         Create a new regex rule for a write context.
 
         :param context_name: The name of the write context
         :param builder: The builder containing write context regex rule configuration
         """
-        return self._client_func().domain_insert_write_context_regex_rule(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        return contexts_api.domain_insert_write_context_regex_rule(
             domain_id=self._domain,
             context_name=context_name,
             write_context_regex_rule=builder.build(),
         ).rule_id
 
     @exec_with_token
     def delete_write_context_regex_rule(self, context_name: str, rule_id: str) -> None:
         """
         Delete a regex classifier rule for the context.
 
         :param context_name: The name of the write context
         :param rule_id: The ID of the rule to delete
         """
-        self._client_func().domain_delete_write_context_regex_rule(
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
+        contexts_api.domain_delete_write_context_regex_rule(
             domain_id=self._domain,
             context_name=context_name,
             rule_id=rule_id,
         )
 
     @exec_with_token
     def delete_write_context_regex_rules(self, context_name: str) -> None:
         """
         Delete the regex classifier rules for the context.
 
         :param context_name: The name of the write context
         """
+        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
         for rule in self.list_write_context_regex_rules(context_name=context_name):
-            self._client_func().domain_delete_write_context_regex_rule(
+            contexts_api.domain_delete_write_context_regex_rule(
                 domain_id=self._domain,
                 context_name=context_name,
                 rule_id=rule["id"],
             )
```

## antimatter/tests/test_capsule.py

```diff
@@ -4,21 +4,21 @@
 
 from antimatter.tags import ColumnTag, SpanTag
 from antimatter.capsule import Capsule, CapsuleBindings, _markup_bytes
 import antimatter_engine as ae
 
 @pytest.fixture
 def mock_capsule_bindings(monkeypatch, capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info):
-    mock_capsule_bindings = CapsuleBindings(None, [])
+    mock_capsule_bindings = CapsuleBindings(None)
     
     # mock the read_all_with_tags method
     monkeypatch.setattr(
         mock_capsule_bindings, 
         'read_all_with_tags', 
-        lambda _: (capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info)
+        lambda: (capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info)
     )
 
     return mock_capsule_bindings
 
 @pytest.mark.parametrize(
     "capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info",
     [
@@ -38,15 +38,15 @@
             '{"dict_list": {}, "_coltype": {"email": "string", "bytes": "bytes", "fname": "string", "bio": "string", "duration": "timedelta", "dt": "date_time", "float": "float", "age": "int", "status": "bool", "id": "int"}, "_metadtype": "dict_list"}'  # extra_info
         ),
         # Additional test cases can be added here
     ]
 )
 def test_data_with_tags(mock_capsule_bindings):
     capsule = Capsule(mock_capsule_bindings)
-    result = capsule.data_with_tags(read_params={}, column_major=False, inline=False)
+    result = capsule.data_with_tags(column_major=False, inline=False)
 
     # validate expected list lengths for result
     assert len(result) == 2
     assert len(result[0]) == 10
     assert len(result[1]) == 10
 
     # validate span tags were created
@@ -163,8 +163,8 @@
     "Exact overlap example 2",
     "Partially overlapping tags",
     "Nested overlaps with different starts and ends",
     "Test case with invalid UTF-8 byte",
 ]
 @pytest.mark.parametrize("input_bytes, span_tags, expected_output", test_data, ids=test_ids)
 def test_markup_bytes(input_bytes, span_tags, expected_output):
-    assert _markup_bytes(input_bytes, span_tags) == expected_output    
+    assert _markup_bytes(input_bytes, span_tags) == expected_output
```

## Comparing `antimatter-0.2.2.dist-info/METADATA` & `antimatter-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: antimatter
-Version: 0.2.2
+Version: 1.0.0
 Summary: library for interacting with capsules in various formats
 Author: Antimatter Team
 Author-email: support@antimatter.io
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: annotated-types >=0.6
 Requires-Dist: packaging >=21.1
 Requires-Dist: pydantic >=2.0
 Requires-Dist: python-dateutil >=2.1
+Requires-Dist: pyyaml
 Requires-Dist: cbor2 ~=5.5
 Requires-Dist: urllib3 >=2.0.2
-Requires-Dist: antimatter-engine ==0.2.2
+Requires-Dist: antimatter-engine ==1.0.0
 Provides-Extra: all
 Requires-Dist: langchain >=0.0.341 ; extra == 'all'
 Requires-Dist: faiss-cpu >=1.7.3 ; extra == 'all'
 Requires-Dist: transformers >=4.23 ; extra == 'all'
 Requires-Dist: torch >=2.0 ; extra == 'all'
 Requires-Dist: numpy >=1.23.3 ; extra == 'all'
 Requires-Dist: pandas[performance] >=2.0 ; extra == 'all'
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: antimatter Version: 0.2.2 Summary: library for
+Metadata-Version: 2.1 Name: antimatter Version: 1.0.0 Summary: library for
 interacting with capsules in various formats Author: Antimatter Team Author-
-email: support@antimatter.io Requires-Python: >=3.10 Requires-Dist: annotated-
+email: support@antimatter.io Requires-Python: >=3.8 Requires-Dist: annotated-
 types >=0.6 Requires-Dist: packaging >=21.1 Requires-Dist: pydantic >=2.0
-Requires-Dist: python-dateutil >=2.1 Requires-Dist: cbor2 ~=5.5 Requires-Dist:
-urllib3 >=2.0.2 Requires-Dist: antimatter-engine ==0.2.2 Provides-Extra: all
-Requires-Dist: langchain >=0.0.341 ; extra == 'all' Requires-Dist: faiss-cpu
->=1.7.3 ; extra == 'all' Requires-Dist: transformers >=4.23 ; extra == 'all'
-Requires-Dist: torch >=2.0 ; extra == 'all' Requires-Dist: numpy >=1.23.3 ;
-extra == 'all' Requires-Dist: pandas[performance] >=2.0 ; extra == 'all'
-Requires-Dist: pyarrow >=2.0 ; extra == 'all' Provides-Extra: dev Requires-
-Dist: pytest >=7.0 ; extra == 'dev' Provides-Extra: langchain Requires-Dist:
-langchain >=0.0.341 ; extra == 'langchain' Requires-Dist: faiss-cpu >=1.7.3 ;
-extra == 'langchain' Provides-Extra: langchain-huggingface Requires-Dist:
-langchain >=0.0.341 ; extra == 'langchain-huggingface' Requires-Dist: faiss-cpu
->=1.7.3 ; extra == 'langchain-huggingface' Requires-Dist: transformers >=4.23 ;
-extra == 'langchain-huggingface' Requires-Dist: torch >=2.0 ; extra ==
-'langchain-huggingface' Provides-Extra: numpy Requires-Dist: numpy >=1.23.3 ;
-extra == 'numpy' Provides-Extra: pandas Requires-Dist: pandas[performance]
->=1.5 ; extra == 'pandas' Provides-Extra: pyarrow Requires-Dist: pandas
-[performance] >=2.0 ; extra == 'pyarrow' Requires-Dist: pyarrow >=2.0 ; extra
-== 'pyarrow' Provides-Extra: pytorch Requires-Dist: torch >=2.0 ; extra ==
-'pytorch' For more information, please visit the docs at _P_y_t_h_o_n_ _d_o_c_s.
+Requires-Dist: python-dateutil >=2.1 Requires-Dist: pyyaml Requires-Dist: cbor2
+~=5.5 Requires-Dist: urllib3 >=2.0.2 Requires-Dist: antimatter-engine ==1.0.0
+Provides-Extra: all Requires-Dist: langchain >=0.0.341 ; extra == 'all'
+Requires-Dist: faiss-cpu >=1.7.3 ; extra == 'all' Requires-Dist: transformers
+>=4.23 ; extra == 'all' Requires-Dist: torch >=2.0 ; extra == 'all' Requires-
+Dist: numpy >=1.23.3 ; extra == 'all' Requires-Dist: pandas[performance] >=2.0
+; extra == 'all' Requires-Dist: pyarrow >=2.0 ; extra == 'all' Provides-Extra:
+dev Requires-Dist: pytest >=7.0 ; extra == 'dev' Provides-Extra: langchain
+Requires-Dist: langchain >=0.0.341 ; extra == 'langchain' Requires-Dist: faiss-
+cpu >=1.7.3 ; extra == 'langchain' Provides-Extra: langchain-huggingface
+Requires-Dist: langchain >=0.0.341 ; extra == 'langchain-huggingface' Requires-
+Dist: faiss-cpu >=1.7.3 ; extra == 'langchain-huggingface' Requires-Dist:
+transformers >=4.23 ; extra == 'langchain-huggingface' Requires-Dist: torch
+>=2.0 ; extra == 'langchain-huggingface' Provides-Extra: numpy Requires-Dist:
+numpy >=1.23.3 ; extra == 'numpy' Provides-Extra: pandas Requires-Dist: pandas
+[performance] >=1.5 ; extra == 'pandas' Provides-Extra: pyarrow Requires-Dist:
+pandas[performance] >=2.0 ; extra == 'pyarrow' Requires-Dist: pyarrow >=2.0 ;
+extra == 'pyarrow' Provides-Extra: pytorch Requires-Dist: torch >=2.0 ; extra
+== 'pytorch' For more information, please visit the docs at _P_y_t_h_o_n_ _d_o_c_s.
```

## Comparing `antimatter-0.2.2.dist-info/RECORD` & `antimatter-1.0.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,182 +1,202 @@
-antimatter/__init__.py,sha256=hgcDptQmJWE_dIKE58mPPXaoMnJpZ5VAVgpxUCnDE9Q,314
-antimatter/capsule.py,sha256=vq2bGBJ59p1m1oYr0pGqxh-W99ojBYasgi4ajxnMzSQ,11741
+antimatter/__init__.py,sha256=GyavNjWFX-uW3oA_leOJGN0H58f6TtJy_Oqlw64-mP4,327
+antimatter/capsule.py,sha256=GVO1ema_XuwW6-6-k7ztSo_dPoJa0H6g-xb8fpkt2rs,10768
 antimatter/cell_path.py,sha256=F1JsdAD0adLOW0hIoCW40CFMQYMi811JaxKnC1-Ob3o,928
 antimatter/extra_helper.py,sha256=YF8Trh3y8GrNEzaJI9vh_6lMJ1cy4MtqVSftVW0VGsE,3410
-antimatter/session.py,sha256=78lxOJHuwFUXjjnNIyDHimGcx1rsmOf9d8aoyL9J-3c,17576
+antimatter/session.py,sha256=Qw0r4oQmGkMmWrqCcNKMrz121zg1wPHx6xW7RfrRCMg,25527
+antimatter/auth/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+antimatter/auth/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+antimatter/auth/config/auth_config.py,sha256=1vNRCt4AGQyIpY6NZZndXV12Dc7VeUeQdnp6gVoSaSo,11557
+antimatter/auth/config/global_identity.py,sha256=fWmk_w5h32J9-B8c94_JxrEcW5MUTT4zrja0-GkjiiQ,1930
+antimatter/auth/config/profiles.py,sha256=Z69s7XHXG2lOo9hh9hZDcPpFTnMnWlsLOMuVkle9eAE,535
+antimatter/auth/config/tokens.py,sha256=n-JpF5xTkVc7nEAvp6rWlIKevPRx8oAteI1gD97srGM,429
+antimatter/auth/google/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+antimatter/auth/google/models.py,sha256=J_iAz_JID15fDXzWQsfFwB0ZhKjmOO2i91RFTtKDL5o,495
 antimatter/builders/__init__.py,sha256=_g-IuE-knAlcGOqyOyz4AQ5yy6Os3KOJ0HYIIITM8lQ,759
 antimatter/builders/capability.py,sha256=wtfXs7sR9TZPOxYoXhnbV_gfSWle2J858AAgxVHF-ng,1630
 antimatter/builders/fact_policy.py,sha256=6kyQ-NZXaCqnaK8F02-9iWGRehHVJzX0Cvoe_M8n7g0,2386
 antimatter/builders/read_context.py,sha256=0SOfV5ZxcxC2tr48tPJcpg9tG5Im2dGqdbSaVZ4qFdc,3338
 antimatter/builders/read_context_rule.py,sha256=tiXCc43uO2XAZLVhtN-ERNXDGDTlrf8KLKYsHmR2GpA,4831
-antimatter/builders/root_encryption_key.py,sha256=lnZ75Gcor6-_bqvekHDBYpNdWgsIwty1ZvBta87PfHY,4117
-antimatter/builders/settings_patch.py,sha256=4UHB8YC7EYkp03LYO1GpdIR9BWQu17zZmXCkMlZHTv0,2216
+antimatter/builders/root_encryption_key.py,sha256=qKXbABO_yOqyNDnm0ltEkedVtKCW_u6Ch_oDCtlfYLI,4174
+antimatter/builders/settings_patch.py,sha256=W0SalyLzEMOMfos0Z3-DPTtmtMFYcJuxQkMEJuMg860,2118
 antimatter/builders/write_context.py,sha256=C9wTX6k5AHRaig-KIHHFxsHl5fMmH-RKx3j07CMH0cE,4390
 antimatter/builders/write_context_rule.py,sha256=RDnGB1U3N5F61KgSPd4J0jR4i2nOgikR6NTB_q51deg,2460
 antimatter/cap_prep/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/cap_prep/applicator.py,sha256=-ynx8nuibRmLRassveV6IWbCE3riLhYu3LJulHAhPIo,3158
 antimatter/cap_prep/prep.py,sha256=aosQuE_x8lClbUANXYt-uDu8hsnkj9fyQrtinXE0FTQ,3811
 antimatter/cap_prep/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/cap_prep/tests/test_applicator.py,sha256=xVlAhbwPQC1klFsW0wzT2sqiLesLiiAjlNno_mbJbks,3875
 antimatter/cap_prep/tests/test_prep.py,sha256=uMOTZye-jA_b8ddk0UxxQ7suLCCKeOuouKv_yCgG2VM,2558
-antimatter/client/__init__.py,sha256=-O49Xl7ihmKKuT-Q71AFX5-3r4jOr91YFsqOtktSF5w,13233
-antimatter/client/api_client.py,sha256=mkrq3RikSMnHwNI_T1G-3HphAIxOJY5mI3SHI9kV8Gw,24612
+antimatter/capabilities/__init__.py,sha256=DV5cGlaqHQ9XWOrBRQo94-H4prNCAyz45c-UBKFPdTQ,66
+antimatter/capabilities/converter.py,sha256=pG0kEu0Cv9wO8sYZ55hYaoEiOxoWR-RM182uz-djPTM,1714
+antimatter/client/__init__.py,sha256=jagYnhHiZzCz9fAubodzxfViWeKr43eP8KnDTFfraAQ,13909
+antimatter/client/api_client.py,sha256=e_XQsPHBBvtOa-4FWHP14EyqiOE8LGcI983vdf542l8,24612
 antimatter/client/api_response.py,sha256=A7O_XgliD6y7jEv82fgIaxR3T8KiwaOqHR6djpZyh_o,674
-antimatter/client/configuration.py,sha256=opMJkg_BknbT42Qu4pP0XszzgAL3IvTDhBW-Nu1wLac,14983
-antimatter/client/exceptions.py,sha256=H7mD47ohZ0oVixgOj3cCPZWcI24YSr_vSGANxyDK9Ks,5954
-antimatter/client/rest.py,sha256=gAhZvadMmVOaxLNqf6w2R_oQDPCf9V-jBo06hdVOhdw,9799
-antimatter/client/api/__init__.py,sha256=SZYMvw4bwlhRKKOpa_R5kKZ7hDOUeaJqbmWMs8n2f9s,105
-antimatter/client/api/default_api.py,sha256=qPVb7Pi5zkludMfif44btYlNSGds4Oegtj3eifstheM,1079678
-antimatter/client/models/__init__.py,sha256=en09efXWIMC2Sjp4n4KEn29IuhKlfkDGZUeub8xsY9k,12605
-antimatter/client/models/access_log_entry.py,sha256=5_4XVnQpD4g9YJtoJTRKVk6G_tAF4wXLMFfidbzj98U,6771
-antimatter/client/models/access_log_entry_create_info.py,sha256=1q92PoVhpuwRn2rgKzgo-JI5rK1hsHwpaJuyXWU-u6U,3245
-antimatter/client/models/access_log_entry_open_info.py,sha256=6ADGIBbH5Hg5w6IDuOColeneEQwC5G6jUcMtQvdTDj8,3085
-antimatter/client/models/access_log_entry_read_info.py,sha256=BHySDLKqfYBIBt9BIGqALj0DqNl_6ldo4Zi1AQS0y_Y,5291
-antimatter/client/models/access_log_results.py,sha256=IzU33V7a79CSOAy0JVVpABNuCwESwGZe89s9jbLdXEQ,3151
-antimatter/client/models/active_root_encryption_key_id.py,sha256=jEOsC3LTG0J-0XEggeJp2XSGRgFwiKV_afJlOoC1cGY,3077
-antimatter/client/models/add_capsule_log_entry_request.py,sha256=frN3Fno5_UICv-BnCAOqyVv9M6nV5L_6X-prskI-u4I,3041
-antimatter/client/models/add_read_context.py,sha256=-fW-4ioS8gy8T1rvjRGE7ifNNBBBkMijc4by9XgiUIY,4841
-antimatter/client/models/add_write_context.py,sha256=VWNIfcb5yCW-alb2iwzhhPKzGw4MD-H7vcXToaYzJsY,3214
-antimatter/client/models/antimatter_delegated_aws_key_info.py,sha256=vZdO03oAKUIxIdybfeYLxNBexhvTGtUCI972x6VgNm4,3170
-antimatter/client/models/api_key_domain_identity_provider_details.py,sha256=GFaLKGcnKaa-BnWTES4LBhs3Pr0WqcG1n1FxJtBRwr8,2801
-antimatter/client/models/available_delegated_root_encryption_key_provider.py,sha256=8ZZWYKZKwVUenv7-gg5d_pWVhJS6tSEawgBTnRa43mU,3305
-antimatter/client/models/available_root_encryption_key_providers.py,sha256=_V5QZ1vdVrvJkfywtZgeGOP83mSLrfChWqbWxlTe9ig,3121
-antimatter/client/models/available_root_encryption_key_providers_providers_inner.py,sha256=ZR_m42iWDmBeO7TOgyzwJNhWkFQdNAkGU4eVmidvYgM,6728
-antimatter/client/models/available_service_account_root_encryption_key_provider.py,sha256=wqkZk2UYluuYMhUApGzV2TYrXVlYbXbenIiDOSPOSdY,3197
-antimatter/client/models/aws_service_account_key_info.py,sha256=rGBl1g5RtWISSc_R0_jLwcnTqBJXBgAsZ6PV4igr3oo,3459
-antimatter/client/models/capability.py,sha256=IcmLsga2JdNEsOmh3r-ve8Dni0rUsTvptng6DPaaOXU,3154
-antimatter/client/models/capability_definition.py,sha256=PT8asOjyyvTYYLBQ2j-yniVaYfSNwpVSppBZ27QBOLs,4985
-antimatter/client/models/capability_definition_list.py,sha256=zfdLwtZLGAI-TCgdoWI-tNdlVFV85WUvQpdwVM6zX4E,2964
-antimatter/client/models/capability_list.py,sha256=_0_tCPKrPn5e5zMxwY5z8NfT6EmOPZw6OeTfixvqsoo,2883
-antimatter/client/models/capability_rule.py,sha256=1-YHfDaNGVHY104LMdjOD7AMBpFzQP7oz_P3CdIyZH4,3267
-antimatter/client/models/capability_rule_match_expressions_inner.py,sha256=Cdzh44GRxMIbgox-BgqI8xfdzuKld3eoa0P9hELNvWY,3640
-antimatter/client/models/capsule_create_response.py,sha256=ESfmrVZIjrEmbzxq-28Cs6Qv5OtK4vVLPSkx7pCwLNM,4572
-antimatter/client/models/capsule_info.py,sha256=wuyiaaf9QY1WktEwCGisgc5wrwSAJYLqBwevj1pNnok,4883
-antimatter/client/models/capsule_list.py,sha256=JvJ4PJXSwXU_rhQ0BESFIYrIMBaoJcPu4KqgyNYKFlU,3039
-antimatter/client/models/capsule_open_request.py,sha256=-_KbmIWaJW5yBYVY8BfNTAVCrDffaDnirbAgAuCGtFA,2745
-antimatter/client/models/capsule_open_response.py,sha256=xzn68Nluo38EsgwBwWTlmkN-kJQ486XfGrRkyuSmoFk,4211
-antimatter/client/models/capsule_open_response_read_context_configuration.py,sha256=95a_PwpWaLfxRTkMvPWWt-N7sUZnKeJYESsskgBrDwQ,3444
-antimatter/client/models/capsule_seal_request.py,sha256=NvJ5AuYj82taq_hHKjYJF1PHgxOv1ASbI9XmGPssOws,3787
-antimatter/client/models/conflict_error.py,sha256=j_iLtX6f8aL4zVBhkiC6vuSTu9X8v_uBeCPD48qpHiU,2962
-antimatter/client/models/create_peer_domain.py,sha256=bTamTxye_ivLEjQhdT_jhNKLRVsrT4pwWPBDeQ2qcq0,7314
-antimatter/client/models/data_tagging_hook_input.py,sha256=WK7COLIE8pPpNnLI8ZnbCgtnxexmAMtL1Xd3dZZGsr0,3122
-antimatter/client/models/data_tagging_hook_input_records_inner.py,sha256=GqH9FtwCXkmAxeRwIV76r9oM-WHF2jKjAXGqq5s7ycY,3199
-antimatter/client/models/data_tagging_hook_input_records_inner_elements_inner.py,sha256=2tZ-hwwrx1JIoGhb9_56AV8Vh6nT9doVtGQushpmwh0,2860
-antimatter/client/models/data_tagging_hook_response.py,sha256=NuCWBfFF22QabAI4klB7NzIChhUBleJ-ChHkRpa_J64,3559
-antimatter/client/models/data_tagging_hook_response_records_inner.py,sha256=B5AZ_D3wGVl89jYIjrduN3kz6o_igQPIcZ3d-2EU1eU,3032
-antimatter/client/models/delete_tags.py,sha256=QX3NG61Ih2dWvTRUs2X-qf6mbTTUWDKT1blq6ESFvXg,2481
-antimatter/client/models/domain.py,sha256=MqCoSSBIrxiZea4sSCQG7IW7j7gO8hpAXBvx02ekePA,2830
-antimatter/client/models/domain_add_read_context_rule200_response.py,sha256=LHbs9nljdK3r9EjoT7xyeymhGqyJ5eQqM9zzoSppzm8,2971
-antimatter/client/models/domain_authenticate.py,sha256=ayfQh6ABoVsAi7OexqTPlcNQ5_tCFGonWjfCfhg0gIw,2467
-antimatter/client/models/domain_authenticate_response.py,sha256=VdAGq8dIPsyM4mInAyLk4Seiu9EokVWHz0vQ8a0LfJc,2420
-antimatter/client/models/domain_contact_issue_verify_request.py,sha256=HW6bUcReeCRoacAUPMAiJ2gj3CkPIr4yV7bfDkY7czE,2600
-antimatter/client/models/domain_control_log_entry.py,sha256=2p-WdjcMAHRwZKpNzl8HSoy8xYk5RXmtk4t9XxmqMD8,4350
-antimatter/client/models/domain_control_log_results.py,sha256=FQlqGPYnb2sAxKjX6_N5jNPYceLIqr_COCwUvoiBZ6Y,3201
-antimatter/client/models/domain_fact_list.py,sha256=0oi1ewBArSbSL0KohvPpAi-DbY8eJuaAIpeUWOdpYS4,2969
-antimatter/client/models/domain_hooks_list.py,sha256=xY11Jxt03Jrhc8GCavbBCTbDH4RigwQEHr9FobsCK_A,2933
-antimatter/client/models/domain_hooks_list_hooks_inner.py,sha256=0UYLy5LE2S_HR_H_xkEzvtd5XeCJ-EGddPOI155S4Tk,3653
-antimatter/client/models/domain_identity_api_key_principal_params.py,sha256=HOXB0C6X2PaD4ezwRhGy7uOr7sPLdUUnsQCutEdeIWs,3039
-antimatter/client/models/domain_identity_email_principal_params.py,sha256=iGi0f-5VZ-k442o5Alj1dV5kA-tcjZCrAOYorE37guM,2966
-antimatter/client/models/domain_identity_hosted_domain_principal_params.py,sha256=NkxfkO9S4XU4silEZZqaj0ahYOmTEmGnSEYf_diaIIo,3086
-antimatter/client/models/domain_identity_principal_details.py,sha256=SOjwPBWy0hjM6_5jcv15KSGVgEd5CE0DaC4DRY30488,7406
-antimatter/client/models/domain_identity_provider_details.py,sha256=WcrKLPfkABmagR6njjAZoQvmTnpnAg1C1vsWYTY-k2c,6312
-antimatter/client/models/domain_identity_provider_info.py,sha256=jzmtw3uuZArmx6NU2pmOOktwWzBJ3espF8sxgVvoA7s,5177
-antimatter/client/models/domain_identity_provider_list.py,sha256=z055AA6CHKP3I-GBpGBkyxgtrhJZfvU_6CJN1MDciHs,3204
-antimatter/client/models/domain_identity_provider_principal_list.py,sha256=lYYR-j2GoYz2uIJ6OTqwwDi2iPG5JxrXaUtc5gQV8vM,2975
-antimatter/client/models/domain_identity_provider_principal_params.py,sha256=24-GnbckJUF_81JdNvHHmz3_WLcjHkNvV74-M7B-7Ao,3426
-antimatter/client/models/domain_identity_provider_principal_type.py,sha256=_gElYy_bjQ-vEygnpD6nD-_f_QZ88Qe79iL_3gGuWQQ,942
-antimatter/client/models/domain_identity_provider_type.py,sha256=aajSNauTYXVkIudPxJwsGGJuGvopSvOkwVBCZUU75os,928
-antimatter/client/models/domain_insert_identity_provider_principal200_response.py,sha256=BpkoLLtGozTpOA0-03Ocr4nWSicIksBcgv8daMZdMP4,3297
-antimatter/client/models/domain_insert_write_context_regex_rule200_response.py,sha256=ZvfbCxDsIAKzYrLveUCvUHTDzbUvIJZcYfXYEYHMQM8,2964
-antimatter/client/models/domain_peer_config.py,sha256=bS4mn6G7eudlfrZdOggadThUawSkQP9Nn8gGnx74Ejs,14602
-antimatter/client/models/domain_peer_list.py,sha256=GTApfaxKJpOm-3gtUwrhJtF9zP1nyo9bd9bUeR4t-IE,2920
-antimatter/client/models/domain_peer_list_peers_inner.py,sha256=yaPevlEHR7kl1TZ-uXzHvWOwaluYxBMhfF96OG4ALLM,3461
-antimatter/client/models/domain_policy.py,sha256=1HS0I-qoFvJRpjxc-QTX64KzIl0T-LBjOBwLbwoOD2A,3450
-antimatter/client/models/domain_policy_rule.py,sha256=zHngdClHCCpYUhrH8diY-gJRwAHZ0D85ToMnfL0nxrU,5691
-antimatter/client/models/domain_private_info.py,sha256=07ipg42hdw6ef5j2i__83ClXHdc2r8-UI97S--xAY24,3911
-antimatter/client/models/domain_public_info.py,sha256=P6W-4lSwj48pQVS7MYPjqnimnrkCYIrDeaqM4ZnjkBw,3907
-antimatter/client/models/domain_resource_summary.py,sha256=BN9qC9-zQPQLpg8GuSZhjGacnHcUp14pcK3mE51JaKU,3037
-antimatter/client/models/domain_resource_summary_schema_inner.py,sha256=qGRReAUUXDjTxIdhGDenaLCAhvCfA5ArID2QHBZi3ro,3367
-antimatter/client/models/domain_settings.py,sha256=tE_hh0Nu2gxPFINhnZ8mP3Cc6f25ouU0FYJnMhtSDRo,4011
-antimatter/client/models/domain_settings_disaster_recovery.py,sha256=eijJ51RkPsLUi7mnVfzFJaWvBis2NDDyYis4ZNuHmmw,2865
-antimatter/client/models/domain_settings_patch.py,sha256=pPYjj7VKgHnbaVJm1cHC3XDXiw08OWGqiMrnYJOGtTg,2887
-antimatter/client/models/domain_status.py,sha256=teyYGOB0I6SZSTYwY14U3uoo9VPoWBOkvItCMB9UjCM,3016
-antimatter/client/models/domain_status_notifications_inner.py,sha256=iK6NP3aJwTiBuVBHFc0vMm3xze3lJVaO0gUbj1nQNqk,2866
-antimatter/client/models/domain_tag_info_results.py,sha256=66V_wi9IAuFPJF-PQBhu7JKeN9HenNaVNjVzwezWanA,3039
-antimatter/client/models/error.py,sha256=1HUEeew-NaYe1PjaqEAR2kxIlGqLsyqsMR1CbFOptQc,2489
-antimatter/client/models/fact.py,sha256=0f2qQddoJrXdyUDKyY6W1PXCdIBJpHJgbnbXfKC_DEQ,3824
-antimatter/client/models/fact_list.py,sha256=gMbP4M6H5R7s-sHNG-Ihe0aD3Eetb76oQMTjQvOUpiM,2772
-antimatter/client/models/fact_policy_rules_inner.py,sha256=Ur69mxqpYpYvee53agd7Gjsj0XNL4sDiOvGFGxreHOE,4250
-antimatter/client/models/fact_policy_rules_inner_arguments_inner.py,sha256=5lXaau_W_TYMlI1etChzyD9MkirGwp1ifQ6BYp8Jl9Q,4318
-antimatter/client/models/fact_type_definition.py,sha256=Pg2Oa-9YboE05DTYew4fgu56epCUctHOMSbKu8e2sbA,4953
-antimatter/client/models/gcp_service_account_key_info.py,sha256=zHepvmcwG99zNQ2dkbmVGxmxVQmzsN1npjyxIKzc2MI,3892
-antimatter/client/models/google_o_auth_domain_identity_provider_details.py,sha256=BeonT6_b1LKaqAlC_GvCEpnsRr7HUh8x9QjznSADfBI,3057
-antimatter/client/models/hook_invocation.py,sha256=BCHF6HFBtcabV_78ClEkf_8uK0uwL-PEFQvU36XhBzY,2501
-antimatter/client/models/invalid_request_error.py,sha256=q2uGrB2yCm86PrIsYGiHBoMTTfYPGXL7IMLXZDcwFE8,2689
-antimatter/client/models/json_patch_request_add.py,sha256=XRpGQn2xpQPj6Y9zC05GXX4U0osGcWnGjCsyslimEfI,3215
-antimatter/client/models/json_patch_request_add_value.py,sha256=w88zSmM2AhWU3S_PmMnHqLaQX4BA2_Y7rI6HptcxOGw,6165
-antimatter/client/models/json_patch_request_copy.py,sha256=QFK7fK7UvIFZEHbx_e98FWxdDCthW-aevQG6VMJjfTo,2811
-antimatter/client/models/json_patch_request_move.py,sha256=bAundNdHQeA8sC0OEUOWduKtkHa_Bnu45qWm-9UQtRc,2811
-antimatter/client/models/json_patch_request_remove.py,sha256=N4hs-uiXOGyFFhWAW0hfkytHEO8altH9KKIx9TDqvW0,2823
-antimatter/client/models/json_patch_request_replace.py,sha256=pz-4vkJWgJNk1vFlIifiYzEOd1R9cWDn7NQ1-cZh1Mw,3255
-antimatter/client/models/json_patch_request_replace_value.py,sha256=6wSgJ3QPMH9JZXpB6VJAmgz7TEOluVo-e4O4aLKSuAA,6197
-antimatter/client/models/json_patch_request_tst.py,sha256=IwpLu1R0kflfQ7RY34h3rHmx-bW-l2vh7rmYhP-dYMM,3217
-antimatter/client/models/json_patch_request_tst_value.py,sha256=3JveWlbK_tLGemH-1ze59vJ_vzDlBO3b9W0wdTXKJis,6166
-antimatter/client/models/key_infos.py,sha256=fgYn3rfdYjJhPKLOKsltjYODBxI7yrB-AGN0gKkNsX4,3009
-antimatter/client/models/key_infos_key_information.py,sha256=IS0CFMn8LnBV6QyvFWGzTXNnXrRsKuNxgFLxV_sIyk4,6812
-antimatter/client/models/new_access_log_entry.py,sha256=KVW2vPF4cOt97CcrUcuaNY3tFx6Z4atxIaKKnbuTUog,3448
-antimatter/client/models/new_access_log_entry_read_info.py,sha256=flXb3Vn_F6Iff8qNVAbPT0DTj-hRPONLVAvWspIW7x8,4607
-antimatter/client/models/new_capability_definition.py,sha256=8fJFextAaQ9WpBeXH1pJqGhwlPNLe8xJIdVGoEuvUCw,3178
-antimatter/client/models/new_domain.py,sha256=NsI-RhODVmoZKnRhwmjHy9T1GeCGpZwWvYeyzEG5hVw,2720
-antimatter/client/models/new_domain_response.py,sha256=GpuCcczPM4bJIGT2ramuf84rzg5-7B5g9p7iHaZPLxo,3006
-antimatter/client/models/new_fact.py,sha256=351ywrKFHvbHrPZHaro8G3zyE27rvNxUOLPDdVTb_O8,2683
-antimatter/client/models/new_fact_type_definition.py,sha256=FABg6lx3Y6qObiAs8C48CVAxJdWP8glAWVqZl3Nvuz8,3261
-antimatter/client/models/new_fact_type_definition_arguments_inner.py,sha256=6dE6RYqlcb_0134eOKPUO0-y7qZUYBndpQwx15n3pW0,3131
-antimatter/client/models/new_read_context_config_rule.py,sha256=2IAzepH1d3rDvwWw0U47rZRd8H9ydfVLycJtLJm9_LA,6187
-antimatter/client/models/patch_request_inner.py,sha256=-WjwrYNBJNIcKU9XORc42JtZ5acTgdYgwICbMpi6MX0,9083
-antimatter/client/models/principal_info.py,sha256=pJvJ1-NrehEfevdi_bXrH0xd2YHtx0bwPzpvIZm5Eks,4070
-antimatter/client/models/principal_summary.py,sha256=43oHJXPWndv9k-ejOcpY5M5r_4wK_O8WXcN3U5x5lN8,3447
-antimatter/client/models/read_context_config_rule.py,sha256=hJq4oPJ1zpvlZ-mRlAzgmnrb5Kb3gPSjtkYJ-_ufcZQ,7791
-antimatter/client/models/read_context_details.py,sha256=6siN7MntGX6e4_HalIKOKi5Ymlpp_U8x5DZB8Z8jgwY,6947
-antimatter/client/models/read_context_list.py,sha256=TM7a1NQrB_kiHxvzE0BLGkGI_JVIQZfmAgy9ov88Njs,3003
-antimatter/client/models/read_context_parameter.py,sha256=sfxXT2Hke4I5SVlTDs2Pdv2W8Wm0RONOlpdEiC_Ds3w,2865
-antimatter/client/models/read_context_required_hook.py,sha256=DaDVybZQafJYpr7yc5MlpH0OkZ-55hmhDeFXtCDNWUo,4935
-antimatter/client/models/read_context_rule_facts_inner.py,sha256=p5wGOWdbSh-x2TB67UKk8zcVkR_b34IhlQLkFWNqP3c,3743
-antimatter/client/models/read_context_rule_facts_inner_arguments_inner.py,sha256=kh6Z5RQuv57t4cYWxf6XbSzakjtSb6TMUg35VKc0Iws,3259
-antimatter/client/models/read_context_rule_match_expressions_inner.py,sha256=yYdCU9AUK-mbAD24JW5JEq5LC5utY26uenozxE-YHqQ,4218
-antimatter/client/models/read_context_short_details.py,sha256=jCRAPKhXH29imXaf_KFa2uTi2YJr2jCUZjzalgXMgwM,5704
-antimatter/client/models/resource_exhausted_error.py,sha256=zUY2rRPoce7X3K7WegI_nQNzeFopNMR5RbDhCqT-XQ0,2920
-antimatter/client/models/resource_not_found_error.py,sha256=0PqHSX-lSXL9LG4SxDc-nGjhdgRDwWX4UJ4IcyDlL_k,2912
-antimatter/client/models/root_encryption_key_id_response.py,sha256=iqMl8Q1g-KKSX-Sv9sBORTQ5G1UXqlmxeSt5wxpz6Bc,2538
-antimatter/client/models/root_encryption_key_item.py,sha256=S2ABsPI5dz-MMNwc0iThcQiBG8JrxfUYIH74Pb2smI8,3016
-antimatter/client/models/root_encryption_key_test_response.py,sha256=Y4NbtS-AfeNNSTRA4ghtu0P6LDxnjYCCt9YQ8e7nxq8,4204
-antimatter/client/models/rotate_key_encryption_key_response.py,sha256=zTfOq8N0Sz90gkVUNEktvYK4chod1G6zJ2IioPSNQv8,2642
-antimatter/client/models/starred_domain_list.py,sha256=2b7qSFZ4ODdrNqcKBBp-xKYn0fcH6lZawy1NvNX1akc,2499
-antimatter/client/models/tag.py,sha256=Yk81_L1nT8V3OjQziso-Jnc0BHdhK2rHkovdaUOPreI,4076
-antimatter/client/models/tag_meta.py,sha256=ncyFz-42k6RIoaQdmnVNnqUqV7Dem7ZXzeVUNrsMrb0,2488
-antimatter/client/models/tag_set.py,sha256=tE5xU3nQIKSz1_NgyvF84ioVxo1wMlzEOQbQwZ7Tz6E,3480
-antimatter/client/models/tag_set_span_tags_inner.py,sha256=DZTMF531-ndPgOqYZGPXSNmsuZiuVP8KmpoSfU3FRk8,3107
-antimatter/client/models/tag_summary.py,sha256=k-5Mq1JDR65X1idI5_0D6XC3LxMSxd7WtBnlFFZzbec,3764
-antimatter/client/models/tag_summary_elided_tags_inner.py,sha256=ouTnqbPpK8iAbGpQCJkczAYo2u6aJySq4IRMX6mw-Xg,2988
-antimatter/client/models/tag_summary_unique_tags_inner.py,sha256=S-LMxwSAxuUHf-qQhpm-LGhd8-xX5EPoibd4_yHVsHQ,2843
-antimatter/client/models/tag_type_field.py,sha256=ETjEQ2PHjmiqZvQqUteycD5ztczp2hVkaTFeb7LdN5o,898
-antimatter/client/models/unauthorized_error.py,sha256=IQhkMzukpfJfgg8U00dzjy1kHNHScKbQJUPUkcZuf-c,2523
-antimatter/client/models/upsert_span_tags_request.py,sha256=huKHFtGqUW137nGwZzfxE2DMRV5S3e1oQQ1NsEnQEks,3011
-antimatter/client/models/verify_contact_response.py,sha256=6gXQNd0uHUaXv1Ypujk_Qo9sgdQB-hSoaayAwo5dXIY,3079
-antimatter/client/models/write_context_config_info.py,sha256=bL-TvhntUGFAE07Jicf-uc4GU12d7LOvoHEzIbHbo-A,3515
-antimatter/client/models/write_context_config_info_required_hooks_inner.py,sha256=hJZ9alqMaX_s_iT861Jh6B1Qd3vWkfHJI020sIorrbE,4649
-antimatter/client/models/write_context_details.py,sha256=K39dqPpJGm54_mV8Dm8zsb_5LhdIbb3IyCaSS_Hu9aM,4932
-antimatter/client/models/write_context_list.py,sha256=kuchdYPej5hUrpZia7s1OjErM2UeemJP7eu0mjGmGYY,3000
-antimatter/client/models/write_context_regex_rule.py,sha256=GUna_IX_-F9UqESDno9rfyLTvy9M-dcv0oKPYIeD-wo,4337
-antimatter/client/models/write_context_regex_tag.py,sha256=72IHuO429w9nNo8mUy2pqIKmWGVtR2fzRNlP6B2KcIA,3202
+antimatter/client/configuration.py,sha256=0DWgKsLfTXioxofP77W8I0vvAJ0LnxGdTwKolAaToGc,14983
+antimatter/client/exceptions.py,sha256=_KiGIYmniZf2RfwxIjUNdIFPb6hMD1ffB-d-ePqMqeA,5954
+antimatter/client/rest.py,sha256=WsOiRqjKpLhhCibD-cgz40cDeGKZgFxwQqFCTq0eMG8,9799
+antimatter/client/api/__init__.py,sha256=twILSDqIpQW78keNVNClrM_ep8WN-NVLL43uldxHgTU,549
+antimatter/client/api/account_management_api.py,sha256=Fo9AJpFug9PuGHAecWS2ljDO26Hj1ghASj_bDuh0XNI,31800
+antimatter/client/api/authentication_api.py,sha256=Avk6LAQr9UYvpqdpxLlurk_GPZQyI_3Eb5k0CVDOaRA,199539
+antimatter/client/api/capsules_api.py,sha256=dWwix1JqQvNALnvuJJr9PXFAoDl6tbl4BQ1uAvHa-74,146264
+antimatter/client/api/contexts_api.py,sha256=hnCEcBK3K5IqumVGdyjpn-908vWfwe2CtiJpzCgmcqA,201452
+antimatter/client/api/encryption_api.py,sha256=-cbHoSzn-pQdGJYoXUpPXl8zLPJKaY7UEs49Rd30U10,107683
+antimatter/client/api/general_api.py,sha256=xMF8tkpXngw4g_Mq6OKLylLYc08Q7-cfBOKq2Utv_yg,162476
+antimatter/client/api/internal_api.py,sha256=E18QqWCoFT4A2T_XLA32-J_lPRZHiYpjzGcaWafGYGQ,79499
+antimatter/client/api/policy_api.py,sha256=5SLrRkwtzrHAZngJM0j_sCok9bDp2MKLPFGE8eIjfKA,175071
+antimatter/client/models/__init__.py,sha256=ON4Esg6dWelLcjPo8ibuw42-Y943TqzIqDP_icsBpkc,12837
+antimatter/client/models/access_log_entry.py,sha256=tEIE5OtpA85EKphFiQqngtP4Kr0cCkj76VegoS9usOE,6771
+antimatter/client/models/access_log_entry_create_info.py,sha256=_S8CKlGaYTT_dvwf_vlhqL9el97RUAwy5YMLcmAPqEY,3245
+antimatter/client/models/access_log_entry_open_info.py,sha256=rHKgzlVwVzYdYgDWS1StRfFNb6528dB3krCbK2BqBoQ,3085
+antimatter/client/models/access_log_entry_read_info.py,sha256=QwjVzcQioyLFjmHWsTeIWBVHFjnOEcBZifE7ehwZnf0,5291
+antimatter/client/models/access_log_results.py,sha256=zKN-KbmRvJcXKhd_UFyw06draIgJ1oxd9XZ1gb9tF_c,3151
+antimatter/client/models/active_root_encryption_key_id.py,sha256=PWEsa6o5apUdxO0WNtpZUnnKNzj1Z-GLnWHmgoQbRrY,3077
+antimatter/client/models/add_capsule_log_entry_request.py,sha256=8UxCUQqvy7XbqCe7-vRL-sq-0U7Q81wljXg7j5SklVM,3041
+antimatter/client/models/add_read_context.py,sha256=kDsjPANqk0F0wvhb1l5DcSym_pGx5DzDb_n8DCUvlcc,4841
+antimatter/client/models/add_write_context.py,sha256=udTb4PWgXerSDrEllOQp_pi78I9ReDuSonDqdlNs9z8,3214
+antimatter/client/models/antimatter_delegated_aws_key_info.py,sha256=8BNpO-0xxwB6OlgR1jb8o0G6Af1ZkbRnnfB1M2ktHuo,3170
+antimatter/client/models/api_key_domain_identity_provider_details.py,sha256=iG-45sEy9ZfjinbXOJNRiZ-sfz2Kzy0UJEY9b8v6gLk,2801
+antimatter/client/models/available_delegated_root_encryption_key_provider.py,sha256=p2SrP_-qQsfdQ6J66MilXnzsyoz7qRp5UOTG1_YPymU,3305
+antimatter/client/models/available_root_encryption_key_providers.py,sha256=ybFAaq3WBDbOqzYDbEo018olhWA7bREoyTBxp8R0SyA,3121
+antimatter/client/models/available_root_encryption_key_providers_providers_inner.py,sha256=kq3xnWFXhsSCQCCCabUuPm1BV3wc6k-HyZg1S0No5HI,6728
+antimatter/client/models/available_service_account_root_encryption_key_provider.py,sha256=KL4GDdce7nTKcYGQAgyI7C3RdGHWMSP1mVguShHyhus,3197
+antimatter/client/models/aws_service_account_key_info.py,sha256=yTviIsl5quDkaiF0ig1fNmwQokge9GzldoldQesJ-9o,3459
+antimatter/client/models/capability.py,sha256=CskGXj1G4hgluBxbAHP6x2OA5p4zYrPnuzXaENBoXMY,3154
+antimatter/client/models/capability_definition.py,sha256=g3qJ_D0-YgeSU7lXUai72bqW9GzrY_lz1-6VeqG-a4g,4985
+antimatter/client/models/capability_definition_list.py,sha256=dfT2ZKsZtKqn9hGQOkJvIf-5miPhs6S7b52DqGl9LrY,2964
+antimatter/client/models/capability_list.py,sha256=D5eQow9SbZy5dCwUD3nb4wkaJ6E7fUsC8uLlSyMSFAg,2883
+antimatter/client/models/capability_rule.py,sha256=cApHDhYO1fZ-ftwudYB2uZOt7YYb1g-VWva8p33DTdk,3267
+antimatter/client/models/capability_rule_match_expressions_inner.py,sha256=zCmjj_XN2Uaud8TnRwOuFCswNLKXGKQ4UQy2BekKc2Q,3640
+antimatter/client/models/capsule_create_response.py,sha256=lTAGC-X7AXcByG0jadRATCdFEPinHIvNnvQzAN_atSo,4572
+antimatter/client/models/capsule_info.py,sha256=5Z3bWAWRt4uU3GG8oEikIdDa3PoF864lvmakctQWXnQ,4883
+antimatter/client/models/capsule_list.py,sha256=Wgx6NsXPhgvZc6AD1Lvl0DjoPRL1Kbdg_kcmpAsoCxs,3039
+antimatter/client/models/capsule_open_request.py,sha256=wJ4OagmouKLokKHfteGmp6N7j3VLnDYn_7vNBHTURQg,2745
+antimatter/client/models/capsule_open_response.py,sha256=x1F39Fm1mBu-3W19KEUapZB5xjALcAyujFJjgLpasqQ,4211
+antimatter/client/models/capsule_open_response_read_context_configuration.py,sha256=OfY0G3aQxOImb74_e78jcbBsX2TEKRd1M9YGEfuSZjs,3444
+antimatter/client/models/capsule_seal_request.py,sha256=ZNp-9dfR4JBxYQFEVBzmtR-dKZtjtLL_xkw1LDhxR4s,3787
+antimatter/client/models/conflict_error.py,sha256=wwem9wFUICNyqWDF2WuLd6P69Wwne3sgXkjTzj4vENs,2962
+antimatter/client/models/create_peer_domain.py,sha256=hNcxq4btjqHaWkjGxuY-_LoDglZy_Y5nEyp3cre-AOU,7314
+antimatter/client/models/data_tagging_hook_input.py,sha256=ycVzYM-OE02VEZ9exZZwCODG3Ay3nS-H8Mk9V21-YOo,3122
+antimatter/client/models/data_tagging_hook_input_records_inner.py,sha256=4bb6cSwZidMaSmtIda4FF3S4FBua5hDOHFDhT_AXcmE,3199
+antimatter/client/models/data_tagging_hook_input_records_inner_elements_inner.py,sha256=eWB2t07CoMdj6qS7lNqkk-p6ubhipWan0B-6hJXYoG4,2860
+antimatter/client/models/data_tagging_hook_response.py,sha256=RhqWlOG6g4QjsAIw38TUBgCSBYMrh5LD6AIgnzIv7f8,3559
+antimatter/client/models/data_tagging_hook_response_records_inner.py,sha256=8gaTO8l1um4CdS0dREV3riW2ClWxN6nG1UBnCEHdpeg,3032
+antimatter/client/models/delete_tags.py,sha256=tto6FSj4QBvjIpCQ4RJJoq1pUWv-TGgM1hxlxMlWIgk,2481
+antimatter/client/models/domain.py,sha256=0NqW-lv5Wwzp_FouRhQ-vpB1vvOiaiJC00HyHxoqjZw,2830
+antimatter/client/models/domain_add_read_context_rule200_response.py,sha256=wrMRFvSUCeZupqaHstnhOGUbPi04u_6glzIdBASMzLA,2971
+antimatter/client/models/domain_authenticate.py,sha256=om4ruq-w_KKoNLIYeqApT5TKJyAA1n2GXhD1qK32vl0,2467
+antimatter/client/models/domain_authenticate_response.py,sha256=JCcZRWKzfYZPtJJ-demvBgEZv1o3nB75DROMzycTYrM,2420
+antimatter/client/models/domain_contact_issue_verify_request.py,sha256=UNbnANJSaQxEeQNapvvgYg0Rz-1iWL-VnCo0IIH15m4,2600
+antimatter/client/models/domain_control_log_entry.py,sha256=IDyDMH0RCiHO42jDNeWmgYbUAixOpwe_JPiHxVtLahY,4350
+antimatter/client/models/domain_control_log_results.py,sha256=PRc4lO2ogAfiyIvYg-GbcT7m2YqyN0RhVIQGtHmN6IY,3201
+antimatter/client/models/domain_fact_list.py,sha256=NJVgaLpTsZW92C3C1Z0RxxihvAd9cbEGqnYBocYXEoM,2969
+antimatter/client/models/domain_hooks_list.py,sha256=8iIV1QT9rhFL1kq2qyISLN_0nVdBwWtV32kMkGkgQcw,2933
+antimatter/client/models/domain_hooks_list_hooks_inner.py,sha256=zPNRtCXi1PMKbP9k-hZzk6G0-xfiWcpaVgaA9lUgKYs,3653
+antimatter/client/models/domain_identity_api_key_principal_params.py,sha256=JS7WGmZhE8QdMuyPLHDbeXoj0iAFMtSJ_TMpfLtzvAs,3039
+antimatter/client/models/domain_identity_email_principal_params.py,sha256=DPKaZpQA5tk0bShw74xn4AoQcoJMHxzqnvHiqlAoiHo,2966
+antimatter/client/models/domain_identity_hosted_domain_principal_params.py,sha256=e_AkmV0fBtcYkJsd99NFEc90LdmcqRCiifliGzSw5DI,3086
+antimatter/client/models/domain_identity_principal_details.py,sha256=O__4cDGdZQI3DSxB1mqLWeyFGRUEjf_aeUcLba289h4,7406
+antimatter/client/models/domain_identity_provider_details.py,sha256=ZUS-7iQY-uLLBgyuQ0nmoKTyNwzCuxlzVYlXx40xS4A,6312
+antimatter/client/models/domain_identity_provider_info.py,sha256=3a2phzbWxUq6IFdS3he6g1wWZw5juCQE4VZS4LUVamw,5177
+antimatter/client/models/domain_identity_provider_list.py,sha256=8Mz0mqIVs4hYHV61nBPvhR6qV_GKKfnxAoMaB2ETeKE,3204
+antimatter/client/models/domain_identity_provider_principal_list.py,sha256=XZjT-M0e6nhlKZ8GxR6oRAs4tC9aDu1uIog0ivHjCPM,2975
+antimatter/client/models/domain_identity_provider_principal_params.py,sha256=8I0C0OI0ONAULVVYY_VeapTdmJI6lwN90yr9nqkTlbA,3426
+antimatter/client/models/domain_identity_provider_principal_type.py,sha256=wBrMGpdQWYmWtSUNevwhNh2ongVMpFyGShpo-PBM0vs,942
+antimatter/client/models/domain_identity_provider_type.py,sha256=cyDeWrNddnMzsIttO1TnZ35R-PmHWTHxaGrni1rPkss,928
+antimatter/client/models/domain_insert_identity_provider_principal200_response.py,sha256=Bdv-Is9oZF_816GmZAzXxHyDuDgk4tUzLYmDTE5Kiug,3297
+antimatter/client/models/domain_insert_write_context_regex_rule200_response.py,sha256=LeHWJ2Zn7TlnsdtUDSXP-84eI8UaGgCS-mXUCdPKI_k,2964
+antimatter/client/models/domain_peer_config.py,sha256=3YgmKGkrji1ryXIV3lb4zxg0HbKfkdyK7RPu5oHCBcU,14602
+antimatter/client/models/domain_peer_list.py,sha256=kz8gmaG1Jka8FsXLZNrbmu6T-fXgfMXA7jg2T-ewVX0,2920
+antimatter/client/models/domain_peer_list_peers_inner.py,sha256=vMBKdzOhaYCehiyX0L8F5zucGNZ1EIFWPoLCbu8zfNg,3461
+antimatter/client/models/domain_policy.py,sha256=PaT5R85HucZu_drgvdcXMvqZYZDOIGA_Oror-CdaPCM,3450
+antimatter/client/models/domain_policy_rule.py,sha256=M68IOBPkeriUFSIGn4TCvflVwSHwgKuPCs7oWuZwc2Q,7142
+antimatter/client/models/domain_private_info.py,sha256=aWD8CHy2m9fyrM7QqILqYJhyqPeA2GXopzwbE6dn8oo,3911
+antimatter/client/models/domain_public_info.py,sha256=GQ-g3Eijx1svteiFhm9D3FvR9M-K3k2TA2-I1xzbiyA,3907
+antimatter/client/models/domain_resource_summary.py,sha256=qcSvup1IlW8D7XuxuynvjiOuWVNkdiOGQ3qvZaHBVY8,3037
+antimatter/client/models/domain_resource_summary_schema_inner.py,sha256=Nrw-VmhG6dFjoN4Aken5SYmky9U64KEV0l7gEE6GDco,3367
+antimatter/client/models/domain_settings.py,sha256=7TOwnA0YgKBts3W3SF5NjQ0IbEyecn8d-phst400Tos,4011
+antimatter/client/models/domain_settings_disaster_recovery.py,sha256=4r9t7jCyOStcrG4Q6txo42VSwDNkVe5fkuwEzZIwdpc,2865
+antimatter/client/models/domain_settings_patch.py,sha256=L9bsSoVW77BldipOARGmzGVN0_GE89rDKrFzXhrt6xs,2887
+antimatter/client/models/domain_status.py,sha256=LEFVsCgjPLbsQii2M98nNJsW4IwvJmZ_jBZIQVWoNJ8,3016
+antimatter/client/models/domain_status_notifications_inner.py,sha256=bMDb9Pmeo3JbTY9OZ69QKW-eWiG_FHwqX35GboXiZ7I,2866
+antimatter/client/models/domain_tag_info_results.py,sha256=wN8YCVzmC0QPk7aUcmoj08UxM6YumPFW04XkBJJgS7I,3039
+antimatter/client/models/error.py,sha256=6a8A3DEnWUGzj7rU5GKOqLlce7p-gUhqb6WSpa-sgLo,2489
+antimatter/client/models/fact.py,sha256=epvRtmi37RV_JTtKG1Xd2I7WZiLmrELrCSwVfhzUuRg,3824
+antimatter/client/models/fact_list.py,sha256=a5vYchqzAJKv1MdjDLJq8krDKFnc7PSqV-p3rLY3l9A,2772
+antimatter/client/models/fact_policy_rules_inner.py,sha256=gCozuhtmW3C9XNWTM27nfnoPYcTWmO07F4HkW-3hW78,4250
+antimatter/client/models/fact_policy_rules_inner_arguments_inner.py,sha256=SIEyrkH0b1jYiYuxHxh6nRA7tGofxzIViFyhL2RZkmg,4318
+antimatter/client/models/fact_type_definition.py,sha256=dc3WxzcNUvJJupG-jQTBa2HJ9SmOPGd_AGTKpokEcyY,4953
+antimatter/client/models/gcp_service_account_key_info.py,sha256=i0iYNv8-4vMhn-VgNkAR4vVZhm9hGd6T8U0WeBhPFis,3892
+antimatter/client/models/google_o_auth_domain_identity_provider_details.py,sha256=jW0q95w7QBdLJBERdGXcfIGkPl2OYJu0dInsPKowyJs,3057
+antimatter/client/models/hook_invocation.py,sha256=X-9ekUNb0h2Vwrok9KBV5s_pPqaBFxAi2qNAEbxvpBI,2501
+antimatter/client/models/invalid_request_error.py,sha256=V8ulEX1MbXPUjBI7VxcDlw-F65eZSUubP4Vamw0ZeJI,2689
+antimatter/client/models/json_patch_request_add.py,sha256=j6J5CFgB5bT_ar6YM4_de0_Gq45B8gM5CYmNFCzLzxU,3215
+antimatter/client/models/json_patch_request_add_value.py,sha256=x4IqbmQ1DJf_hiVohoJhKcJqfyzrt0PDQya7qP9G2LE,6165
+antimatter/client/models/json_patch_request_copy.py,sha256=9V_gR8LOzBJFQrMqHNczl_CWCdClNgAS43YfLzFG4wg,2811
+antimatter/client/models/json_patch_request_move.py,sha256=cbZ7lW0B_fR6EHYSVq3aWrquF3dxeQN8WgE0WYMfvaA,2811
+antimatter/client/models/json_patch_request_remove.py,sha256=k33hEvcpwazEUAWYtGcNHu7pcQN91PaTXuyvUvhSaSw,2823
+antimatter/client/models/json_patch_request_replace.py,sha256=bakl00rWCNJ-QcRH7ScPg5XBDdatCQ5BbTbKyTSAY0g,3255
+antimatter/client/models/json_patch_request_replace_value.py,sha256=D4w3tw7qKUiBGPghQzH5JcRygrCrm1eh_uhEw5F327Y,6197
+antimatter/client/models/json_patch_request_tst.py,sha256=S27-LlU9OhIYxAmSXIsBtp0RsgL6SOqCJCxNIo0EDt4,3217
+antimatter/client/models/json_patch_request_tst_value.py,sha256=PBCiCH9HyJoo0BVEPZuO2krU7rzNA02iFiXrSAd8nDQ,6166
+antimatter/client/models/key_infos.py,sha256=7O6DppITLSJaddRrRUPWO8uQIi2VLafNzRLJ3e5G2Mc,3009
+antimatter/client/models/key_infos_key_information.py,sha256=AM3IXJDTus67iwGhrCiLdMqZ0mGOn4ED92Bn3mqCfws,6812
+antimatter/client/models/new_access_log_entry.py,sha256=craox9mMPdN6afBHl7zeDUlDm9Twv6Ehv1aVmkiRAgQ,3448
+antimatter/client/models/new_access_log_entry_read_info.py,sha256=wGlUvAU7oXrNy7ZAlziycnIGHDKAS1SVz4ULaBjXlwA,4607
+antimatter/client/models/new_capability_definition.py,sha256=fqotWdLavwauj3Cpc8scEmSxtCLO3NqGQQE9-TAfIf0,3178
+antimatter/client/models/new_domain.py,sha256=srMuhMReC_xqNEsPRWfzXIVlwRWjQkd5g74ESGNEdxE,2720
+antimatter/client/models/new_domain_policy_rule.py,sha256=kQczTdmnyop_Bp_PUaDGV1AxSJLG8abwtqlBGKx2cSM,4777
+antimatter/client/models/new_domain_response.py,sha256=oBbozrPPPy757xZbE73tDapzcRFMD9fs252h2Wktbpc,3006
+antimatter/client/models/new_fact.py,sha256=5quLb52Y6y0OYGXV1GYjRuQt7LY-B11XzQ79vg7LP_8,2683
+antimatter/client/models/new_fact_type_definition.py,sha256=s9OlEq3ugeg1kec4SprDVOdI3B7tVcbhooZ-ciwGeV0,3261
+antimatter/client/models/new_fact_type_definition_arguments_inner.py,sha256=0RGUevYOtz-maKD-b5wtImKZm4cBHTveHvZE37BBWdo,3131
+antimatter/client/models/new_read_context_config_rule.py,sha256=A86u7NR_3QtYoQ13F-1u-Elj3fqPunUL0Umx9HJc15I,6187
+antimatter/client/models/patch_request_inner.py,sha256=lDfwuYM9rSWCIDmY-6wAf9cOTH0DQBCuUtV1AITi86Y,9083
+antimatter/client/models/policy_rule_operation.py,sha256=trRuuOCvzfBC1TCJsGAWIEFpKltocAa3zvUd1srLNm4,857
+antimatter/client/models/policy_rule_result.py,sha256=wepEHwNl_abSZea4fq2_r_TAPl0uAT19z0GuaWeeoo0,834
+antimatter/client/models/principal_info.py,sha256=dX95U2YV4cYYzKKWSxfaUiP96Xa2SlxeMdqZv4ECjjc,4070
+antimatter/client/models/principal_summary.py,sha256=hR8pAAblZqplmh6EXtwlDERjBPgz8YDIg1tNqhsq5B8,3447
+antimatter/client/models/read_context_config_rule.py,sha256=WOcvCeUrnAr5IFbK_rMWvBg9Z6AbMKNZUUmha2s_kxM,7791
+antimatter/client/models/read_context_details.py,sha256=D4ZSL-2om_YEcbDt6WN8l8Igt0hCgOe6YBX1cCn6yH0,6947
+antimatter/client/models/read_context_list.py,sha256=pPi5oBWLdDULOmWxjbAMgRYZN9jiePtNnLgVOw_a7EM,3003
+antimatter/client/models/read_context_parameter.py,sha256=nrj4ELxRBIhNr94oQhH-c8qYhVB1MXkc8SDUINkq5x8,2865
+antimatter/client/models/read_context_required_hook.py,sha256=BGRkBaF0IXVZfkWpLRG4vXLvtaUI8xA81yBdo6mVIec,4935
+antimatter/client/models/read_context_rule_facts_inner.py,sha256=jZm87oqDFyhsD4K6erMQ3MeF7SZ75J74h5ndwMYg44s,3743
+antimatter/client/models/read_context_rule_facts_inner_arguments_inner.py,sha256=uMx76N_Kv6L8T3XO007g0xwrfzjh9FZph6Q95Zk51CQ,3259
+antimatter/client/models/read_context_rule_match_expressions_inner.py,sha256=x6S8pzyewTrMFWUdMf10l2XOhhR8UdhEeO8H_kNKL2c,4218
+antimatter/client/models/read_context_short_details.py,sha256=Hw9augF6IPmYL1F85pZvexKyvxhkAvx4o942vtUWr18,5704
+antimatter/client/models/resource_exhausted_error.py,sha256=9DbAoZiPO33TIsDCLuQCpJ7UczLsqlFAZ50bQiGUiPc,2920
+antimatter/client/models/resource_not_found_error.py,sha256=BQyNekESkzlR5STqX3yRbT5LDRE68BKmefVkNDQ8Dp8,2912
+antimatter/client/models/root_encryption_key_id_response.py,sha256=uy3uvXDyRLBujYrhdh0Y2K5Qtj-3Gc9LFM1YBimgZyc,2538
+antimatter/client/models/root_encryption_key_item.py,sha256=M8K3GUWUWDuciPv5H4Hj_rv-0ZA-mJn7cPrLp8Tst5g,3016
+antimatter/client/models/root_encryption_key_test_response.py,sha256=d2XC7EOSMv5kw_HOvI2eoMc19wB-WZBJLluyCkXHSZg,4204
+antimatter/client/models/rotate_key_encryption_key_response.py,sha256=QcA8U4dbTxXWPYajruuSxnYNq_V0qRj0uNlu8WzgELU,2642
+antimatter/client/models/starred_domain_list.py,sha256=8jPCtNQaMmZ-BAoA9e6Aa9ooY5BWkLsco8EY_Kjlc3Q,2499
+antimatter/client/models/tag.py,sha256=b3uCx5fN6HC2HH1f9eyqlGYsZZGnhgIZZGNmHSYnR1s,4076
+antimatter/client/models/tag_meta.py,sha256=BTMTm6MSFHrLBruN1QAngTKWaSS1UwcL55mDDh-g6_E,2488
+antimatter/client/models/tag_set.py,sha256=hcXlGmkPC4W_5fTlqykdQOQ9Vg85Q_9JQkaTm7P2s68,3480
+antimatter/client/models/tag_set_span_tags_inner.py,sha256=O2-BWQEECpJBww6U8PQvIDOC6BUVWwp6CzMYH3JSfL4,3107
+antimatter/client/models/tag_summary.py,sha256=os-VkEbDRdznPgOlig94HzIbr2JKJexjcEOArZrTaYc,3764
+antimatter/client/models/tag_summary_elided_tags_inner.py,sha256=yZXFfvVcL2qThuYjaBTyoh6UzGphdXE352Z6GEy_fvg,2988
+antimatter/client/models/tag_summary_unique_tags_inner.py,sha256=p4BKurq-gpefGmIih6KK8zAGLpkNCwnBjENhqgOQ60I,2843
+antimatter/client/models/tag_type_field.py,sha256=4rSmYLFpQv4LDzpj4zpr9mVy08-F2t-4526u2Xukl8g,898
+antimatter/client/models/unauthorized_error.py,sha256=Zreb6rWmcqoH0h06qUuU3F--5WXEE4H9_R1tmFTJR5g,2523
+antimatter/client/models/upsert_span_tags_request.py,sha256=1BgzW_lvaXys7ScxzVTfqdKSOqKWw2uaWn_QjUSoywc,3011
+antimatter/client/models/verify_contact_response.py,sha256=7RW74aBHyrd3kzEYGTcEj0hR0bxmTupe6mFblSLwjwg,3079
+antimatter/client/models/write_context_config_info.py,sha256=p3dZs7_uqUJFapUm24IrQjfD1FylL4GZBbOpXXScOXg,3515
+antimatter/client/models/write_context_config_info_required_hooks_inner.py,sha256=wdYFbGzaZoTuMfCWwzxSaLenEEAZfFOrnOpvhPjHZB8,4649
+antimatter/client/models/write_context_details.py,sha256=feesjiNLBPV80Idi8rr1PnplCIUNg0CBBAN1Cbo21tk,4932
+antimatter/client/models/write_context_list.py,sha256=HUCRTy2gu2DOjXoYiyvIH0hpXIhfHGMul4Gfl9BF5CY,3000
+antimatter/client/models/write_context_regex_rule.py,sha256=CqGUYRpkyni7C-VGZvBQU7RqQwDDENz3weTC9p_posc,4337
+antimatter/client/models/write_context_regex_tag.py,sha256=cpBr0Wz-Uaa2GcxnIbrblmslJ7SqI-fGbrjF7gEd2cg,3202
 antimatter/constants/__init__.py,sha256=dv0iL9v9W3rYkHSFXc0ZFZvUnCGc49dYZHJOOclZXZs,561
 antimatter/constants/capability.py,sha256=TthAuTVV-j3RbtepBmkdyhvwrnxRepHxdUf9ZdXQJVI,227
 antimatter/constants/domain_policy.py,sha256=pkHOLQPS7ghEjVLzu9z6LYiZ_nEdp8iy5zRHnqT8n7I,284
 antimatter/constants/fact_policy.py,sha256=odFi-qdCThCwnB5xM6nIThRUVX3d7UhzwiLRoBXnw3s,378
-antimatter/constants/hooks.py,sha256=kHU63-EX4AJXW92JAthf1tJavsOBQt0z4PyCsEnhVSU,236
+antimatter/constants/hooks.py,sha256=Pfb_RTzumihirX8ecZ-_aSCp1QjjPcXvY7NneS2HxnQ,237
 antimatter/constants/identity_provider.py,sha256=gROEezJqsOA_WCZeUq3c-i4rIPesGGLceq954w_OnRI,358
 antimatter/constants/read_context_rule.py,sha256=r2RJrI03-_0vkOhU7WAkk-pdIN26auX9VzFW0XoZ8as,1083
 antimatter/constants/settings_patch.py,sha256=P8VRAyo2yHBNdOXbdNmShZx-9y3Lfq96nyzOfhznwOI,251
 antimatter/constants/write_context.py,sha256=JyvCRvhRMDLloi18MITjFtwY5IpO1E6-SrdPBe82Rr8,174
 antimatter/datatype/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/datatype/datatypes.py,sha256=SsHUO_DLmePuAOc5lSaUDCeNIQceINq4Ii69THppbUY,556
 antimatter/datatype/infer.py,sha256=2SK8AHO9v09nBcy7X0MUJmCIolujK5z1BT6fhRPFXCY,1791
@@ -185,33 +205,33 @@
 antimatter/dependencies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/dependencies/package_hint.py,sha256=Wk184eU3RaoyQ9xalmPtXxwDUQoIpp8E-JR_ddEe78M,3340
 antimatter/dependencies/versions.py,sha256=DPX0GX9-fcKW995iZpa9bXJF1ZB5R1qqcrhQv-3kDAU,2489
 antimatter/dependencies/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/dependencies/tests/test_package_hint.py,sha256=LXOtl0ggpfolOhd9DhU0n3NlOZ_ufvanntQHNFFumls,252
 antimatter/dependencies/tests/test_versions.py,sha256=EbDpwkIJT_TkMcyMlCNqs2cqd2VJiGoIOEHVvf8g9I8,339
 antimatter/errors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-antimatter/errors/errors.py,sha256=lBCz8-ISwn_BIkmWiOtmgO8FXQ5pVcAW9QPQ66eOKBA,2049
+antimatter/errors/errors.py,sha256=9V7wKYtCaHmX3_q2t4KqkN2moXrxTeFY_Kug3HItNuA,2156
 antimatter/fieldtype/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-antimatter/fieldtype/converters.py,sha256=DgTeUAb5jUo2Rr54iYI5O9JrumEnD02VLk4_bwqUq-8,3761
+antimatter/fieldtype/converters.py,sha256=hz4Zh1CdHNOKsedWjU_ufCVDsV0_s9KlGbf2xi8OEpk,3677
 antimatter/fieldtype/fieldtypes.py,sha256=FXn9fqyTnRqFMSv_HNMDi3obXCKmV9tnwmXCvy_DcT0,567
 antimatter/fieldtype/infer.py,sha256=dGzrRP-wadiQvRSD1FeUAVowbe_fHNPa9N5hzlpR_iI,1324
 antimatter/fieldtype/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/fieldtype/tests/test_fieldtypes.py,sha256=pyKHY-PdgcKDzR0uNe2pQE2-OSNdosvyXRp1L15uRSM,1268
 antimatter/filetype/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-antimatter/filetype/extract.py,sha256=roXe7eVgtVISaaD3ImjkzV_T-p-IiuoRSXTDur_WuBE,3186
+antimatter/filetype/extract.py,sha256=2GSNKXRyK8g-UllmmhXLeRIPQ01k1UWp0rFTeRQsXO4,3142
 antimatter/filetype/infer.py,sha256=RylSaRnG75rb7vErw3MLQK_RhSOU3CGHoVETvYNsKkU,2607
 antimatter/filetype/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/filetype/tests/test_filetypes.py,sha256=XlAw3o8Qv8l-8jlGfwva1iO97AzfNEIiECjkeqvfZAw,1491
 antimatter/filetype/tests/test_infer.py,sha256=mLGNHfnAf54BLZ6dT-gz8FNKLQR76EuCGBNubSvmeyA,1446
 antimatter/filetype/tests/fixtures/data-ndjson.json,sha256=bgdGVOT4ZJ3FXFXhh6mKxydyAkdjvCtobVSrCQhEB08,176
 antimatter/filetype/tests/fixtures/data.csv,sha256=qfJLKrWOqGe4IDpvPvYsj3_OPvqs7xNTgTf2uqlaCfE,103
 antimatter/filetype/tests/fixtures/data.json,sha256=V-uMPpE1oVIpzVqq2Qr_i64UhMjoDZY70DgbQE1OIhs,194
 antimatter/filetype/tests/fixtures/data.parquet,sha256=7Bh01acUNLbzJcfl-TZKf7j_qxjUnzY5gefopH8-Tbk,2913
 antimatter/filetype/tests/fixtures/data.txt,sha256=ENNLB7AsAZvcHdSPqowF0_fAv4qJmRLggP7SDCkCOAQ,179
-antimatter/handlers/__init__.py,sha256=XFoRvC3nX-b72_FH5yUp8he-0WPPjVyLVTrg0cLN-V0,1377
+antimatter/handlers/__init__.py,sha256=z2TsdGHR6GEoBVXKalblWHGU9SJaqtig42MOVGhvNGY,1473
 antimatter/handlers/base.py,sha256=a0Oia8Bt5I-D1E4x9C9tNeV--ecNg5xYYrUXqsY_gTc,3602
 antimatter/handlers/dict_list.py,sha256=26HwvymPJpuaoji7ndCuMeSyucI6qf24EudjytbeAtY,2662
 antimatter/handlers/dictionary.py,sha256=W0sS18TUSp8ocMvoliU33FMdi6NearN9Wupm-hSht5Q,2100
 antimatter/handlers/langchain.py,sha256=acfy-eSdFMP-wAZQ9QcW8SenoBJOgImZ-NIYnN2RKSM,8735
 antimatter/handlers/pandas_dataframe.py,sha256=gthzLa1var8-lhMbzTNJo7QU-cXOhr0fUW6je4F7iVc,5001
 antimatter/handlers/pytorch_dataloader.py,sha256=rThurHgKdZ5VlUopdEhoH1wk020N7BqIGVnqlLcX8ek,5617
 antimatter/handlers/scalar.py,sha256=HV3xUX2kuopswHXhm9N3Y7UCmz5eVnKWgCy6jasoGwU,1639
@@ -224,40 +244,41 @@
 antimatter/handlers/tests/test_scalar.py,sha256=pPUcftk_ROG-yFS5Xt6XZSBmj9GcFse2e9aZ3EXaq1Q,1522
 antimatter/location/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/location/infer.py,sha256=Oxar2FlX1LAMAnChdax7aXT9uxHBf5ais4-O9JKrUd8,791
 antimatter/location/locations.py,sha256=MXIOkecP2chZI9zlRBvTBUMR0OtxmlQN8uhWJiugB-w,290
 antimatter/location/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/location/tests/test_infer.py,sha256=FXh3Rfk0_RE6_EjazChCSo0spCEfpOatl5hVIpdkTYY,681
 antimatter/requirements/all.txt,sha256=U6CSQUBH3xk8sJtbcWxhkSu66-Zzgkd7KkelJzBsm-w,118
-antimatter/requirements/core.txt,sha256=FpsmozYtI1M6gZDsEMsWc2IBpFlfAbC1kfTF4drfdtk,220
+antimatter/requirements/core.txt,sha256=G_Zs0-z9HGhgEVSSQjwktRRRH8YKaz8h6vZI5wkPP4A,227
 antimatter/requirements/dev.txt,sha256=W0knDd-UWuCG2-CCkDEgAW1x3w3FD1iQfEPn5RSar9w,12
 antimatter/requirements/langchain-huggingface.txt,sha256=BT3Z5BvYGLWlr5MOrIhL0BHS2mgTkz-H1qd3bjkBqWY,66
 antimatter/requirements/langchain.txt,sha256=ZhuwHgdaB9rCjxxb32UWXrceXu2r5YEFjuaVlXu2Rqg,36
 antimatter/requirements/numpy.txt,sha256=3Xa94dLznztKz48JcDpj63gUAV9pLI0kA2Swu_I99rQ,14
 antimatter/requirements/pandas.txt,sha256=SW_tr3r3MF4IxAhy1EHMyP2Gj7Ne2w0r-7mVaBtNi18,24
 antimatter/requirements/pyarrow.txt,sha256=BRX1kPhEes8B6ZgzrpN_qA6UtwPG99_E6Yv4h62l65s,38
 antimatter/requirements/pytorch.txt,sha256=s28vJIauZ4w_DFcWZRcSBGjZEbXyVOJwEkZ2PfM2k58,11
 antimatter/session_mixins/__init__.py,sha256=CvR_tlLlN4Bp5os-C7YtjKkG-yaiZ-0JyvuZSlX1caQ,949
-antimatter/session_mixins/capability_mixin.py,sha256=YZ5P2rwOe_G2MLBpgAW2eE-HxTQw3m5RShQuAW7KLog,3126
-antimatter/session_mixins/capsule_mixin.py,sha256=VVRFGP8K8R6Ra9_fTgJYLmS0FcjwcUnbhi4zTsFMVy4,4676
-antimatter/session_mixins/domain_mixin.py,sha256=WEIR4Ui0uoZrc_fu_yxqGX2ydTiDXr6asJGKdOKRktY,14365
-antimatter/session_mixins/encryption_mixin.py,sha256=Qs7vFEGUt4kCkh4f6j8KHobzK_u-Mz6x6YD8X3tu1yM,1044
-antimatter/session_mixins/fact_mixin.py,sha256=GgZwiUtK0SQW2-EUMl1TbfK_42DdzpVNZOoOxKVhS78,5639
-antimatter/session_mixins/general_mixin.py,sha256=JObsCPvbMLCHvUX8UxgJCSY8nHohiF0QE7WB3l1DWhc,11226
-antimatter/session_mixins/identity_provider_mixin.py,sha256=___qGwVALI7ywbcIOTKp4D5dzicyl13QjrTnXtsTUD0,10686
-antimatter/session_mixins/policy_rule_mixin.py,sha256=JK_2Gxk82XV5Cb2m2xKepdx3_qDGBylbKU1gvFKKfxA,5727
-antimatter/session_mixins/read_context_mixin.py,sha256=X2t97BatEbOk-lVlcDPc--xinIpOvutmR6JDy5eaImo,5201
-antimatter/session_mixins/root_encryption_key_mixin.py,sha256=HkTR0cpkxRh6U_8Dzk0Inx_lG3piNIowt9DJvxyBBJo,4982
-antimatter/session_mixins/token.py,sha256=w78ixObub65huuP8e53-_AR6KeQgXa-NxcOWxXr4n-Y,2298
-antimatter/session_mixins/verification_mixin.py,sha256=3Rq2lKQf0N-y_sqZIdHedP_5wEzlWIhwUWvAXruSWUM,1614
-antimatter/session_mixins/write_context_mixin.py,sha256=jbtLh1sw69z8IY0au64IOTHGtz4dxUCZ72ubjtFjeGs,5286
+antimatter/session_mixins/capability_mixin.py,sha256=tAA0hxYc6QJndwfiDbko8NFYeumafMYKwVNA3XH1aLo,3391
+antimatter/session_mixins/capsule_mixin.py,sha256=1F80tyT_eQ2ncFC7qA38074b2xdg5YMjDu7SSgsGtUY,5037
+antimatter/session_mixins/domain_mixin.py,sha256=BjNIR4clvl9BdZ6iJXgxJhbC-yP_cxMXMn0XMgQ7wdY,14894
+antimatter/session_mixins/encryption_mixin.py,sha256=uJs0CcovjjJDl3Im33psTdiyaWRcTeBxiyZQ5Oj8CKU,1141
+antimatter/session_mixins/fact_mixin.py,sha256=Cbjx7ZT6sJkHRrgbPTIRCo4-WgrAQYqQqTgcKAC8fJg,6208
+antimatter/session_mixins/general_mixin.py,sha256=gSVqUobHDwMm23PY57nbnXocqjePluQ0mPoByOlUfIk,11843
+antimatter/session_mixins/identity_provider_mixin.py,sha256=yncSlCyGVx5GnL2cSZ5jCy23InTQaF1mzEFjoMZXHGU,12478
+antimatter/session_mixins/policy_rule_mixin.py,sha256=3B5svr4yu71czOdim64aHR7xpiZqYEuQb5PhQLtweS8,6063
+antimatter/session_mixins/read_context_mixin.py,sha256=R1HwCFJmCFNPvp_EtdHNoNKkflb-_wmTZ4n-Cc34yTE,6281
+antimatter/session_mixins/root_encryption_key_mixin.py,sha256=f03sdSNKiHG8rLxodgt7YCWqgJZxADiYBFzH_Y4tx8s,5713
+antimatter/session_mixins/token.py,sha256=bnJhP8sLVMjoUZgcyzd0GOYaDOmS2SQIZC170zm9b3c,2265
+antimatter/session_mixins/verification_mixin.py,sha256=dY0SRW9vRbcOeN38y68AMtnACvnPM7umzykLs4mdLUk,1727
+antimatter/session_mixins/write_context_mixin.py,sha256=bww5NSkaWGtUHkf_UACYGoFmN3IECgxxG11-sk80Kcc,5977
 antimatter/session_mixins/serializers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/session_mixins/serializers/identity_details.py,sha256=PoFvEUR5B6MdvINC_tXpF_PLRMUz0CjaXxQXL6JrWKg,1202
 antimatter/tags/__init__.py,sha256=8rV3j87stTslAEtTFLOPjhoQc57kN-gj-DjLtBfFslc,56
 antimatter/tags/tag.py,sha256=xROB-VxhTdveSuGysio61jui3-qsc9kiiV_KrLQNbyQ,1458
 antimatter/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-antimatter/tests/test_capsule.py,sha256=bJUvmSVd0Ifp1E7qFlJygt3n81D6ygo59pX-7DGQUf4,8076
+antimatter/tests/test_capabilities.py,sha256=0FL4taU5i266vIOM07onGXslB2aMkjD9qcWuPt5U3zM,3444
+antimatter/tests/test_capsule.py,sha256=y2EWln7j1KGIbZmevIxdZ070czMnzhuAA_WTQk5U_Yc,8051
 antimatter/tests/test_cell_path.py,sha256=r-PqBe3xlzvsAy6jZ6YFNh2ABHDEYH3gtcZeKWu3KUc,281
-antimatter-0.2.2.dist-info/METADATA,sha256=cjJCBrF-OzPxCKMk10i9YZwk_V5B7oirr9IGMMNnjHA,1794
-antimatter-0.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-antimatter-0.2.2.dist-info/top_level.txt,sha256=YjU0PM1vIfQRPJOlRFZHrQLnLbJPOvjJ4McyOFnMGso,11
-antimatter-0.2.2.dist-info/RECORD,,
+antimatter-1.0.0.dist-info/METADATA,sha256=LVTI52mF6_6aGK_tYvlLEWuNIdM6gz3S6z4aJiMz7d0,1815
+antimatter-1.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+antimatter-1.0.0.dist-info/top_level.txt,sha256=YjU0PM1vIfQRPJOlRFZHrQLnLbJPOvjJ4McyOFnMGso,11
+antimatter-1.0.0.dist-info/RECORD,,
```

