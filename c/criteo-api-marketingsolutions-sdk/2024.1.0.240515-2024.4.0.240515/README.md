# Comparing `tmp/criteo_api_marketingsolutions_sdk-2024.1.0.240515.tar.gz` & `tmp/criteo_api_marketingsolutions_sdk-2024.4.0.240515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo_api_marketingsolutions_sdk-2024.1.0.240515.tar", last modified: Wed May 15 14:51:30 2024, max compression
+gzip compressed data, was "criteo_api_marketingsolutions_sdk-2024.4.0.240515.tar", last modified: Wed May 15 14:51:35 2024, max compression
```

## Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515.tar` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515.tar`

### file list

```diff
@@ -1,295 +1,295 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:30.354696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 14:51:30.354696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:30.354696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 14:51:30.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20931 2024-05-15 14:51:30.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:51:30.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:51:30.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 14:51:30.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:30.298696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:30.302696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/advertiser_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   103164 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    83985 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    96298 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/creative_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39256 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:30.302696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16743 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/flow_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:30.354696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_input_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_filter_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_request_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/adaptive_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/adaptive_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/adaptive_write_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/algebra_node_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_create_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_delete_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_update_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_compute_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_compute_sizes_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_delete_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_audience_search_metadata_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_name_description.py
--rw-r--r--   0 runner    (1001) docker     (127)    12554 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11782 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_search_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_search_metadata_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_create_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_delete_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_update_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_sizes_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_delete_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_estimate_size_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12618 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12117 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_metadata_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/basic_audience_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/behavioral_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_search_filters_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_search_request_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_spend_limit_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contact_list_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15607 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_geo_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_targeting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_campaign_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_campaign_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_coupon_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_coupon_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_image_slide.py
--rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative.py
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/criteo_api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    14106 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/criteo_api_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/delete_audience_contact_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15174 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/dynamic_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/dynamic_write_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/entity_of_portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/error_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/get_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/html_tag_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/html_tag_write_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_set_base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_slide.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_write_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_size_estimation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/location_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/location_size_estimation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/location_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/location_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/lookalike_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/lookalike_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/lookalike_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/modify_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_gender_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_int32.py
--rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_string.py
--rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/point_of_interest_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    14720 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/problems_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/prospecting_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12516 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/prospecting_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/prospecting_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    15849 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/requests_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/requests_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/responses_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/responses_read_ad_set_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/retargeting_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/retargeting_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/retargeting_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/size.py
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/statistics_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_query_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_report_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_report_data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_report_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_report_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/update_coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/update_coupon_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/update_coupon_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/video_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/write_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/write_model_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    82579 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:30.354696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/models/
--rw-r--r--   0 runner    (1001) docker     (127)    28396 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 14:51:30.354696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:30.354696 criteo_api_marketingsolutions_sdk-2024.1.0.240515/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.1.0.240515/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:35.126695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 14:51:35.126695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:35.126695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 14:51:35.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20931 2024-05-15 14:51:35.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:51:35.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:51:35.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 14:51:35.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:35.074695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:35.074695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/advertiser_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103164 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83985 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96298 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/creative_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39256 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:35.074695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16743 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/flow_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:35.126695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_input_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_delivery_limitations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_delivery_limitations_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_frequency_capping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_frequency_capping_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_geo_location_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_search_filter_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_search_request_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_rule_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/adaptive_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/adaptive_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/adaptive_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/algebra_node_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_bulk_create_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_bulk_delete_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_bulk_update_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_compute_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_compute_sizes_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_create_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_create_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_delete_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_audience_search_metadata_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_id_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_id_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_name_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12554 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_search_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_search_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11782 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_search_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_search_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_create_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_delete_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_update_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_compute_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_compute_sizes_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_create_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_create_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_delete_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_estimate_size_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12618 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_id_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_id_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12117 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_update_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_update_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_update_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_update_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/basic_audience_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/behavioral_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_search_filters_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_search_request_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_spend_limit_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contact_list_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_operation_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15607 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_campaign_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_campaign_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_coupon_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_image_slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/criteo_api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14106 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/criteo_api_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/delete_audience_contact_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15174 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/dynamic_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/dynamic_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/entity_of_portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/error_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/get_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/html_tag_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/html_tag_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_set_base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/location_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/location_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/location_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/location_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/lookalike_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/lookalike_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/lookalike_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/modify_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_v23_q1_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_gender_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_int32.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_campaign_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_campaign_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_result_campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_result_campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/placements_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/placements_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/placements_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/point_of_interest_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14720 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/problems_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/prospecting_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12516 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/prospecting_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/prospecting_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_bidding_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_budget_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_schedule_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15849 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_model_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_model_read_ad_set_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/requests_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/requests_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/response_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/response_read_ad_set_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/responses_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/responses_read_ad_set_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/retargeting_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/retargeting_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/retargeting_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/statistics_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_report_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_report_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_report_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_report_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/update_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/update_coupon_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/update_coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/video_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/write_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/write_model_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82579 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:35.126695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    28396 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 14:51:35.126695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:35.126695 criteo_api_marketingsolutions_sdk-2024.4.0.240515/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-15 14:51:12.000000 criteo_api_marketingsolutions_sdk-2024.4.0.240515/test/test_gateway_api.py
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/PKG-INFO` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
-Version: 2024.1.0.240515
+Version: 2024.4.0.240515
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -22,21 +22,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2024.01.0.240515
+pip install criteo-api-marketingsolutions-sdk==2024.04.0.240515
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240515`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.04.0.240515`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2024_01
+import criteo_api_marketingsolutions_v2024_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/README.md` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 API Client Libraries can facilitate your use of the Criteo API allowing you to build unique and customized solutions to serve your businesses and clients.
 These libraries can reduce the amount of code you need to write in order to start accessing Criteo programmatically. They also can help expedite troubleshooting, should you encounter any issues.
 
 More information: [https://developers.criteo.com/](https://developers.criteo.com/)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- Package version: 2024.01.0.240515
+- Package version: 2024.04.0.240515
 
 ## Requirements
 
 Python 2.7 and 3.5+
 
 ## Installation & Usage
 ### pip install
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2024.01.0.240515
+pip install criteo-api-marketingsolutions-sdk==2024.04.0.240515
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240515`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.04.0.240515`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2024_01
+import criteo_api_marketingsolutions_v2024_04
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
 
 Download the code or clone the repository locally, then execute the following command:
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2024_01
+import criteo_api_marketingsolutions_v2024_04
 ```
 
 ## Example
 There are multiple examples for the different OAuth flows that the SDK supports.
 - See [test/example_application_with_client_credentials.py](test/example_application_with_client_credentials.py) for an example with Client Credentials.
 - See [test/example_application_with_auth_code.py](test/example_application_with_auth_code.py) for an example with Authorization Code.
 Once you follow the authorization code flow, you will have a refresh token that has to be used to regenerate access token for future usage.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
-Version: 2024.1.0.240515
+Version: 2024.4.0.240515
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -22,21 +22,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2024.01.0.240515
+pip install criteo-api-marketingsolutions-sdk==2024.04.0.240515
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240515`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.04.0.240515`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2024_01
+import criteo_api_marketingsolutions_v2024_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,285 +2,285 @@
 setup.cfg
 setup.py
 criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
 criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
 criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
 criteo_api_marketingsolutions_sdk.egg-info/requires.txt
 criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
-criteo_api_marketingsolutions_v2024_01/__init__.py
-criteo_api_marketingsolutions_v2024_01/api_client.py
-criteo_api_marketingsolutions_v2024_01/api_client_builder.py
-criteo_api_marketingsolutions_v2024_01/configuration.py
-criteo_api_marketingsolutions_v2024_01/criteo_api_client.py
-criteo_api_marketingsolutions_v2024_01/criteo_auth.py
-criteo_api_marketingsolutions_v2024_01/criteo_rest.py
-criteo_api_marketingsolutions_v2024_01/exceptions.py
-criteo_api_marketingsolutions_v2024_01/flow_constants.py
-criteo_api_marketingsolutions_v2024_01/model_utils.py
-criteo_api_marketingsolutions_v2024_01/rest.py
-criteo_api_marketingsolutions_v2024_01/api/__init__.py
-criteo_api_marketingsolutions_v2024_01/api/advertiser_api.py
-criteo_api_marketingsolutions_v2024_01/api/analytics_api.py
-criteo_api_marketingsolutions_v2024_01/api/audience_api.py
-criteo_api_marketingsolutions_v2024_01/api/campaign_api.py
-criteo_api_marketingsolutions_v2024_01/api/creative_api.py
-criteo_api_marketingsolutions_v2024_01/api/gateway_api.py
-criteo_api_marketingsolutions_v2024_01/apis/__init__.py
-criteo_api_marketingsolutions_v2024_01/model/__init__.py
-criteo_api_marketingsolutions_v2024_01/model/ad.py
-criteo_api_marketingsolutions_v2024_01/model/ad_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/ad_resource.py
-criteo_api_marketingsolutions_v2024_01/model/ad_response.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_response.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_input_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_resource.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_resource.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_search_filter_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_search_request_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/ad_write.py
-criteo_api_marketingsolutions_v2024_01/model/ad_write_request.py
-criteo_api_marketingsolutions_v2024_01/model/ad_write_resource.py
-criteo_api_marketingsolutions_v2024_01/model/adaptive_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/adaptive_colors.py
-criteo_api_marketingsolutions_v2024_01/model/adaptive_write_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/algebra_node_v1.py
-criteo_api_marketingsolutions_v2024_01/model/application_summary_model.py
-criteo_api_marketingsolutions_v2024_01/model/application_summary_model_resource.py
-criteo_api_marketingsolutions_v2024_01/model/application_summary_model_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_bulk_create_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_bulk_delete_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_bulk_update_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_compute_size_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_compute_sizes_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_delete_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_audience_search_metadata_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_error.py
-criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_name_description.py
-criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_search_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_search_metadata_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_create_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_delete_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_update_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_size_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_sizes_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_delete_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_estimate_size_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_input_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_metadata_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_response.py
-criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/audience_warning.py
-criteo_api_marketingsolutions_v2024_01/model/basic_audience_definition.py
-criteo_api_marketingsolutions_v2024_01/model/behavioral_v1.py
-criteo_api_marketingsolutions_v2024_01/model/campaign_search_filters_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/campaign_search_request_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/campaign_spend_limit_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_response.py
-criteo_api_marketingsolutions_v2024_01/model/common_problem.py
-criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_response.py
-criteo_api_marketingsolutions_v2024_01/model/contact_list_v1.py
-criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment.py
-criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_request.py
-criteo_api_marketingsolutions_v2024_01/model/contactlist_operation.py
-criteo_api_marketingsolutions_v2024_01/model/contactlist_operation_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/coupon.py
-criteo_api_marketingsolutions_v2024_01/model/coupon_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/coupon_resource.py
-criteo_api_marketingsolutions_v2024_01/model/coupon_response.py
-criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes.py
-criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_resource.py
-criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_response.py
-criteo_api_marketingsolutions_v2024_01/model/create_ad_set.py
-criteo_api_marketingsolutions_v2024_01/model/create_ad_set_bidding.py
-criteo_api_marketingsolutions_v2024_01/model/create_ad_set_budget.py
-criteo_api_marketingsolutions_v2024_01/model/create_ad_set_geo_location.py
-criteo_api_marketingsolutions_v2024_01/model/create_ad_set_request.py
-criteo_api_marketingsolutions_v2024_01/model/create_ad_set_resource.py
-criteo_api_marketingsolutions_v2024_01/model/create_ad_set_schedule.py
-criteo_api_marketingsolutions_v2024_01/model/create_ad_set_targeting.py
-criteo_api_marketingsolutions_v2024_01/model/create_campaign.py
-criteo_api_marketingsolutions_v2024_01/model/create_campaign_request.py
-criteo_api_marketingsolutions_v2024_01/model/create_campaign_resource.py
-criteo_api_marketingsolutions_v2024_01/model/create_campaign_spend_limit.py
-criteo_api_marketingsolutions_v2024_01/model/create_coupon.py
-criteo_api_marketingsolutions_v2024_01/model/create_coupon_request.py
-criteo_api_marketingsolutions_v2024_01/model/create_coupon_resource.py
-criteo_api_marketingsolutions_v2024_01/model/create_image_slide.py
-criteo_api_marketingsolutions_v2024_01/model/creative.py
-criteo_api_marketingsolutions_v2024_01/model/creative_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/creative_resource.py
-criteo_api_marketingsolutions_v2024_01/model/creative_response.py
-criteo_api_marketingsolutions_v2024_01/model/creative_write.py
-criteo_api_marketingsolutions_v2024_01/model/creative_write_request.py
-criteo_api_marketingsolutions_v2024_01/model/creative_write_resource.py
-criteo_api_marketingsolutions_v2024_01/model/criteo_api_error.py
-criteo_api_marketingsolutions_v2024_01/model/criteo_api_warning.py
-criteo_api_marketingsolutions_v2024_01/model/delete_audience_contact_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/dynamic_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/dynamic_write_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/entity_of_portfolio_message.py
-criteo_api_marketingsolutions_v2024_01/model/error_code_response.py
-criteo_api_marketingsolutions_v2024_01/model/get_portfolio_response.py
-criteo_api_marketingsolutions_v2024_01/model/html_tag_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/html_tag_write_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/image_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/image_set.py
-criteo_api_marketingsolutions_v2024_01/model/image_set_base64.py
-criteo_api_marketingsolutions_v2024_01/model/image_shape.py
-criteo_api_marketingsolutions_v2024_01/model/image_slide.py
-criteo_api_marketingsolutions_v2024_01/model/image_write_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_resource.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_create_v1.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_size_estimation_v1.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_update_v1.py
-criteo_api_marketingsolutions_v2024_01/model/in_market_v1.py
-criteo_api_marketingsolutions_v2024_01/model/location_create_v1.py
-criteo_api_marketingsolutions_v2024_01/model/location_size_estimation_v1.py
-criteo_api_marketingsolutions_v2024_01/model/location_update_v1.py
-criteo_api_marketingsolutions_v2024_01/model/location_v1.py
-criteo_api_marketingsolutions_v2024_01/model/lookalike_create_v1.py
-criteo_api_marketingsolutions_v2024_01/model/lookalike_update_v1.py
-criteo_api_marketingsolutions_v2024_01/model/lookalike_v1.py
-criteo_api_marketingsolutions_v2024_01/model/modify_audience_response.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1_value.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_value.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_date_time.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_decimal.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_gender_v1.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_int32.py
-criteo_api_marketingsolutions_v2024_01/model/nillable_string.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_bidding.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_budget.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_list_request.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_resource.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_resource.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_list_request.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_resource.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_resource.py
-criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_scheduling.py
-criteo_api_marketingsolutions_v2024_01/model/patch_campaign.py
-criteo_api_marketingsolutions_v2024_01/model/patch_campaign_list_request.py
-criteo_api_marketingsolutions_v2024_01/model/patch_campaign_spend_limit.py
-criteo_api_marketingsolutions_v2024_01/model/patch_campaign_write_resource.py
-criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_list_response.py
-criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_read_resource.py
-criteo_api_marketingsolutions_v2024_01/model/placements_report_query_data_message.py
-criteo_api_marketingsolutions_v2024_01/model/placements_report_query_entity_message.py
-criteo_api_marketingsolutions_v2024_01/model/placements_report_query_message.py
-criteo_api_marketingsolutions_v2024_01/model/point_of_interest_v1.py
-criteo_api_marketingsolutions_v2024_01/model/portfolio_message.py
-criteo_api_marketingsolutions_v2024_01/model/problem_details.py
-criteo_api_marketingsolutions_v2024_01/model/problems_details.py
-criteo_api_marketingsolutions_v2024_01/model/prospecting_create_v1.py
-criteo_api_marketingsolutions_v2024_01/model/prospecting_update_v1.py
-criteo_api_marketingsolutions_v2024_01/model/prospecting_v1.py
-criteo_api_marketingsolutions_v2024_01/model/read_ad_set.py
-criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding.py
-criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget.py
-criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule.py
-criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/read_ad_set_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/read_model_ad_set_id.py
-criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set.py
-criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/requests_ad_set_id.py
-criteo_api_marketingsolutions_v2024_01/model/requests_patch_ad_set.py
-criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set.py
-criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/responses_ad_set_id.py
-criteo_api_marketingsolutions_v2024_01/model/responses_read_ad_set_v23_q1.py
-criteo_api_marketingsolutions_v2024_01/model/retargeting_create_v1.py
-criteo_api_marketingsolutions_v2024_01/model/retargeting_update_v1.py
-criteo_api_marketingsolutions_v2024_01/model/retargeting_v1.py
-criteo_api_marketingsolutions_v2024_01/model/size.py
-criteo_api_marketingsolutions_v2024_01/model/statistics_report_query_message.py
-criteo_api_marketingsolutions_v2024_01/model/tag.py
-criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_data_message.py
-criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_entity_message.py
-criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_message.py
-criteo_api_marketingsolutions_v2024_01/model/transparency_query_message.py
-criteo_api_marketingsolutions_v2024_01/model/transparency_report_attributes.py
-criteo_api_marketingsolutions_v2024_01/model/transparency_report_data_message.py
-criteo_api_marketingsolutions_v2024_01/model/transparency_report_entity_message.py
-criteo_api_marketingsolutions_v2024_01/model/transparency_report_file.py
-criteo_api_marketingsolutions_v2024_01/model/update_coupon.py
-criteo_api_marketingsolutions_v2024_01/model/update_coupon_request.py
-criteo_api_marketingsolutions_v2024_01/model/update_coupon_resource.py
-criteo_api_marketingsolutions_v2024_01/model/video_detail.py
-criteo_api_marketingsolutions_v2024_01/model/write_model_ad_set_id.py
-criteo_api_marketingsolutions_v2024_01/model/write_model_patch_ad_set.py
-criteo_api_marketingsolutions_v2024_01/models/__init__.py
+criteo_api_marketingsolutions_v2024_04/__init__.py
+criteo_api_marketingsolutions_v2024_04/api_client.py
+criteo_api_marketingsolutions_v2024_04/api_client_builder.py
+criteo_api_marketingsolutions_v2024_04/configuration.py
+criteo_api_marketingsolutions_v2024_04/criteo_api_client.py
+criteo_api_marketingsolutions_v2024_04/criteo_auth.py
+criteo_api_marketingsolutions_v2024_04/criteo_rest.py
+criteo_api_marketingsolutions_v2024_04/exceptions.py
+criteo_api_marketingsolutions_v2024_04/flow_constants.py
+criteo_api_marketingsolutions_v2024_04/model_utils.py
+criteo_api_marketingsolutions_v2024_04/rest.py
+criteo_api_marketingsolutions_v2024_04/api/__init__.py
+criteo_api_marketingsolutions_v2024_04/api/advertiser_api.py
+criteo_api_marketingsolutions_v2024_04/api/analytics_api.py
+criteo_api_marketingsolutions_v2024_04/api/audience_api.py
+criteo_api_marketingsolutions_v2024_04/api/campaign_api.py
+criteo_api_marketingsolutions_v2024_04/api/creative_api.py
+criteo_api_marketingsolutions_v2024_04/api/gateway_api.py
+criteo_api_marketingsolutions_v2024_04/apis/__init__.py
+criteo_api_marketingsolutions_v2024_04/model/__init__.py
+criteo_api_marketingsolutions_v2024_04/model/ad.py
+criteo_api_marketingsolutions_v2024_04/model/ad_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/ad_resource.py
+criteo_api_marketingsolutions_v2024_04/model/ad_response.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1_response.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_input_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid_resource.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_delivery_limitations.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_delivery_limitations_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier_resource.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_frequency_capping.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_frequency_capping_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_geo_location.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_geo_location_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_search_filter_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_search_request_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_rule.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_rule_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/ad_write.py
+criteo_api_marketingsolutions_v2024_04/model/ad_write_request.py
+criteo_api_marketingsolutions_v2024_04/model/ad_write_resource.py
+criteo_api_marketingsolutions_v2024_04/model/adaptive_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/adaptive_colors.py
+criteo_api_marketingsolutions_v2024_04/model/adaptive_write_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/algebra_node_v1.py
+criteo_api_marketingsolutions_v2024_04/model/application_summary_model.py
+criteo_api_marketingsolutions_v2024_04/model/application_summary_model_resource.py
+criteo_api_marketingsolutions_v2024_04/model/application_summary_model_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_bulk_create_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_bulk_delete_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_bulk_update_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_compute_size_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_compute_sizes_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_create_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_create_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_delete_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_audience_search_metadata_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_error.py
+criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_id_entity_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_id_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_name_description.py
+criteo_api_marketingsolutions_v2024_04/model/audience_search_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_search_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_search_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_search_metadata_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_create_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_delete_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_update_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_compute_size_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_compute_sizes_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_create_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_create_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_delete_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_estimate_size_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_id_entity_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_id_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_input_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_metadata_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_update_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_segment_update_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1_response.py
+criteo_api_marketingsolutions_v2024_04/model/audience_update_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/audience_update_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/audience_warning.py
+criteo_api_marketingsolutions_v2024_04/model/basic_audience_definition.py
+criteo_api_marketingsolutions_v2024_04/model/behavioral_v1.py
+criteo_api_marketingsolutions_v2024_04/model/campaign_search_filters_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/campaign_search_request_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/campaign_spend_limit_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_response.py
+criteo_api_marketingsolutions_v2024_04/model/common_problem.py
+criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1_response.py
+criteo_api_marketingsolutions_v2024_04/model/contact_list_v1.py
+criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment.py
+criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment_request.py
+criteo_api_marketingsolutions_v2024_04/model/contactlist_operation.py
+criteo_api_marketingsolutions_v2024_04/model/contactlist_operation_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/coupon.py
+criteo_api_marketingsolutions_v2024_04/model/coupon_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/coupon_resource.py
+criteo_api_marketingsolutions_v2024_04/model/coupon_response.py
+criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes.py
+criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes_resource.py
+criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes_response.py
+criteo_api_marketingsolutions_v2024_04/model/create_ad_set.py
+criteo_api_marketingsolutions_v2024_04/model/create_ad_set_bidding.py
+criteo_api_marketingsolutions_v2024_04/model/create_ad_set_budget.py
+criteo_api_marketingsolutions_v2024_04/model/create_ad_set_geo_location.py
+criteo_api_marketingsolutions_v2024_04/model/create_ad_set_request.py
+criteo_api_marketingsolutions_v2024_04/model/create_ad_set_resource.py
+criteo_api_marketingsolutions_v2024_04/model/create_ad_set_schedule.py
+criteo_api_marketingsolutions_v2024_04/model/create_ad_set_targeting.py
+criteo_api_marketingsolutions_v2024_04/model/create_campaign.py
+criteo_api_marketingsolutions_v2024_04/model/create_campaign_request.py
+criteo_api_marketingsolutions_v2024_04/model/create_campaign_resource.py
+criteo_api_marketingsolutions_v2024_04/model/create_campaign_spend_limit.py
+criteo_api_marketingsolutions_v2024_04/model/create_coupon.py
+criteo_api_marketingsolutions_v2024_04/model/create_coupon_request.py
+criteo_api_marketingsolutions_v2024_04/model/create_coupon_resource.py
+criteo_api_marketingsolutions_v2024_04/model/create_image_slide.py
+criteo_api_marketingsolutions_v2024_04/model/creative.py
+criteo_api_marketingsolutions_v2024_04/model/creative_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/creative_resource.py
+criteo_api_marketingsolutions_v2024_04/model/creative_response.py
+criteo_api_marketingsolutions_v2024_04/model/creative_write.py
+criteo_api_marketingsolutions_v2024_04/model/creative_write_request.py
+criteo_api_marketingsolutions_v2024_04/model/creative_write_resource.py
+criteo_api_marketingsolutions_v2024_04/model/criteo_api_error.py
+criteo_api_marketingsolutions_v2024_04/model/criteo_api_warning.py
+criteo_api_marketingsolutions_v2024_04/model/delete_audience_contact_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/dynamic_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/dynamic_write_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/entity_of_portfolio_message.py
+criteo_api_marketingsolutions_v2024_04/model/error_code_response.py
+criteo_api_marketingsolutions_v2024_04/model/get_portfolio_response.py
+criteo_api_marketingsolutions_v2024_04/model/html_tag_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/html_tag_write_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/image_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/image_set.py
+criteo_api_marketingsolutions_v2024_04/model/image_set_base64.py
+criteo_api_marketingsolutions_v2024_04/model/image_shape.py
+criteo_api_marketingsolutions_v2024_04/model/image_slide.py
+criteo_api_marketingsolutions_v2024_04/model/image_write_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1_resource.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_create_v1.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_size_estimation_v1.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_update_v1.py
+criteo_api_marketingsolutions_v2024_04/model/in_market_v1.py
+criteo_api_marketingsolutions_v2024_04/model/location_create_v1.py
+criteo_api_marketingsolutions_v2024_04/model/location_size_estimation_v1.py
+criteo_api_marketingsolutions_v2024_04/model/location_update_v1.py
+criteo_api_marketingsolutions_v2024_04/model/location_v1.py
+criteo_api_marketingsolutions_v2024_04/model/lookalike_create_v1.py
+criteo_api_marketingsolutions_v2024_04/model/lookalike_update_v1.py
+criteo_api_marketingsolutions_v2024_04/model/lookalike_v1.py
+criteo_api_marketingsolutions_v2024_04/model/modify_audience_response.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_v23_q1_value.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_value.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_date_time.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_decimal.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_gender_v1.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_int32.py
+criteo_api_marketingsolutions_v2024_04/model/nillable_string.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_bidding.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_budget.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_list_request.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_resource.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_result_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_result_resource.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_list_request.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_resource.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_result_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_result_resource.py
+criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_scheduling.py
+criteo_api_marketingsolutions_v2024_04/model/patch_campaign.py
+criteo_api_marketingsolutions_v2024_04/model/patch_campaign_list_request.py
+criteo_api_marketingsolutions_v2024_04/model/patch_campaign_spend_limit.py
+criteo_api_marketingsolutions_v2024_04/model/patch_campaign_write_resource.py
+criteo_api_marketingsolutions_v2024_04/model/patch_result_campaign_list_response.py
+criteo_api_marketingsolutions_v2024_04/model/patch_result_campaign_read_resource.py
+criteo_api_marketingsolutions_v2024_04/model/placements_report_query_data_message.py
+criteo_api_marketingsolutions_v2024_04/model/placements_report_query_entity_message.py
+criteo_api_marketingsolutions_v2024_04/model/placements_report_query_message.py
+criteo_api_marketingsolutions_v2024_04/model/point_of_interest_v1.py
+criteo_api_marketingsolutions_v2024_04/model/portfolio_message.py
+criteo_api_marketingsolutions_v2024_04/model/problem_details.py
+criteo_api_marketingsolutions_v2024_04/model/problems_details.py
+criteo_api_marketingsolutions_v2024_04/model/prospecting_create_v1.py
+criteo_api_marketingsolutions_v2024_04/model/prospecting_update_v1.py
+criteo_api_marketingsolutions_v2024_04/model/prospecting_v1.py
+criteo_api_marketingsolutions_v2024_04/model/read_ad_set.py
+criteo_api_marketingsolutions_v2024_04/model/read_ad_set_bidding.py
+criteo_api_marketingsolutions_v2024_04/model/read_ad_set_bidding_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/read_ad_set_budget.py
+criteo_api_marketingsolutions_v2024_04/model/read_ad_set_budget_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/read_ad_set_schedule.py
+criteo_api_marketingsolutions_v2024_04/model/read_ad_set_schedule_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/read_ad_set_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/read_model_ad_set_id.py
+criteo_api_marketingsolutions_v2024_04/model/read_model_read_ad_set.py
+criteo_api_marketingsolutions_v2024_04/model/read_model_read_ad_set_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/requests_ad_set_id.py
+criteo_api_marketingsolutions_v2024_04/model/requests_patch_ad_set.py
+criteo_api_marketingsolutions_v2024_04/model/response_read_ad_set.py
+criteo_api_marketingsolutions_v2024_04/model/response_read_ad_set_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/responses_ad_set_id.py
+criteo_api_marketingsolutions_v2024_04/model/responses_read_ad_set_v23_q1.py
+criteo_api_marketingsolutions_v2024_04/model/retargeting_create_v1.py
+criteo_api_marketingsolutions_v2024_04/model/retargeting_update_v1.py
+criteo_api_marketingsolutions_v2024_04/model/retargeting_v1.py
+criteo_api_marketingsolutions_v2024_04/model/size.py
+criteo_api_marketingsolutions_v2024_04/model/statistics_report_query_message.py
+criteo_api_marketingsolutions_v2024_04/model/tag.py
+criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_data_message.py
+criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_entity_message.py
+criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_message.py
+criteo_api_marketingsolutions_v2024_04/model/transparency_query_message.py
+criteo_api_marketingsolutions_v2024_04/model/transparency_report_attributes.py
+criteo_api_marketingsolutions_v2024_04/model/transparency_report_data_message.py
+criteo_api_marketingsolutions_v2024_04/model/transparency_report_entity_message.py
+criteo_api_marketingsolutions_v2024_04/model/transparency_report_file.py
+criteo_api_marketingsolutions_v2024_04/model/update_coupon.py
+criteo_api_marketingsolutions_v2024_04/model/update_coupon_request.py
+criteo_api_marketingsolutions_v2024_04/model/update_coupon_resource.py
+criteo_api_marketingsolutions_v2024_04/model/video_detail.py
+criteo_api_marketingsolutions_v2024_04/model/write_model_ad_set_id.py
+criteo_api_marketingsolutions_v2024_04/model/write_model_patch_ad_set.py
+criteo_api_marketingsolutions_v2024_04/models/__init__.py
 test/test_gateway_api.py
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/__init__.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2024.01.0.240515"
+__version__ = "2024.04.0.240515"
 
 # import ApiClient
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient
-from criteo_api_marketingsolutions_v2024_01.criteo_api_client import CriteoApiClient
-from criteo_api_marketingsolutions_v2024_01.api_client_builder import ApiClientBuilder
-from criteo_api_marketingsolutions_v2024_01 import flow_constants
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient
+from criteo_api_marketingsolutions_v2024_04.criteo_api_client import CriteoApiClient
+from criteo_api_marketingsolutions_v2024_04.api_client_builder import ApiClientBuilder
+from criteo_api_marketingsolutions_v2024_04 import flow_constants
 
 # import Configuration
-from criteo_api_marketingsolutions_v2024_01.configuration import Configuration
+from criteo_api_marketingsolutions_v2024_04.configuration import Configuration
 
 # import exceptions
-from criteo_api_marketingsolutions_v2024_01.exceptions import OpenApiException
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiTypeError
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiValueError
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiKeyError
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiException
+from criteo_api_marketingsolutions_v2024_04.exceptions import OpenApiException
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiTypeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiValueError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiKeyError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiException
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/advertiser_api.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/advertiser_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2024_01.model.get_portfolio_response import GetPortfolioResponse
+from criteo_api_marketingsolutions_v2024_04.model.get_portfolio_response import GetPortfolioResponse
 
 
 class AdvertiserApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -38,15 +38,15 @@
         self.api_portfolio_get_endpoint = _Endpoint(
             settings={
                 'response_type': (GetPortfolioResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/advertisers/me',
+                'endpoint_path': '/2024-04/advertisers/me',
                 'operation_id': 'api_portfolio_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/analytics_api.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/analytics_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2024_01.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2024_01.model.problems_details import ProblemsDetails
-from criteo_api_marketingsolutions_v2024_01.model.statistics_report_query_message import StatisticsReportQueryMessage
-from criteo_api_marketingsolutions_v2024_01.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2024_01.model.transparency_query_message import TransparencyQueryMessage
-from criteo_api_marketingsolutions_v2024_01.model.transparency_report_data_message import TransparencyReportDataMessage
+from criteo_api_marketingsolutions_v2024_04.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2024_04.model.problems_details import ProblemsDetails
+from criteo_api_marketingsolutions_v2024_04.model.statistics_report_query_message import StatisticsReportQueryMessage
+from criteo_api_marketingsolutions_v2024_04.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2024_04.model.transparency_query_message import TransparencyQueryMessage
+from criteo_api_marketingsolutions_v2024_04.model.transparency_report_data_message import TransparencyReportDataMessage
 
 
 class AnalyticsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -43,15 +43,15 @@
         self.get_adset_report_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/statistics/report',
+                'endpoint_path': '/2024-04/statistics/report',
                 'operation_id': 'get_adset_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'statistics_report_query_message',
@@ -102,15 +102,15 @@
         self.get_placements_report_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/placements/report',
+                'endpoint_path': '/2024-04/placements/report',
                 'operation_id': 'get_placements_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'placements_report_query_data_message',
@@ -161,15 +161,15 @@
         self.get_transactions_report_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/transactions/report',
+                'endpoint_path': '/2024-04/transactions/report',
                 'operation_id': 'get_transactions_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'transactions_report_query_data_message',
@@ -220,15 +220,15 @@
         self.get_transparency_report_endpoint = _Endpoint(
             settings={
                 'response_type': (TransparencyReportDataMessage,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/log-level/advertisers/{advertiser-id}/report',
+                'endpoint_path': '/2024-04/log-level/advertisers/{advertiser-id}/report',
                 'operation_id': 'get_transparency_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/audience_api.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/audience_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2024_01.model.audience_bulk_create_input_v1 import AudienceBulkCreateInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_bulk_delete_input_v1 import AudienceBulkDeleteInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_bulk_update_input_v1 import AudienceBulkUpdateInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_compute_sizes_input_v1 import AudienceComputeSizesInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1_audience_search_metadata_v1_list_response import AudienceEntityV1AudienceSearchMetadataV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1_list_response import AudienceEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_estimate_size_input_v1 import AudienceEstimateSizeInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_id_entity_v1_list_response import AudienceIdEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_search_input_v1 import AudienceSearchInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_bulk_create_input_v1 import AudienceSegmentBulkCreateInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_bulk_delete_input_v1 import AudienceSegmentBulkDeleteInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_bulk_update_input_v1 import AudienceSegmentBulkUpdateInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_compute_sizes_input_v1 import AudienceSegmentComputeSizesInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response import AudienceSegmentEntityV1AudienceSegmentSearchMetadataV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1_list_response import AudienceSegmentEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_estimate_size_input_v1 import AudienceSegmentEstimateSizeInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_id_entity_v1_list_response import AudienceSegmentIdEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_search_input_v1 import AudienceSegmentSearchInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_entity_v1_list_response import AudienceSegmentSizeEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_v1_response import AudienceSegmentSizeEstimationV1Response
-from criteo_api_marketingsolutions_v2024_01.model.audience_size_entity_v1_list_response import AudienceSizeEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_size_estimation_v1_response import AudienceSizeEstimationV1Response
-from criteo_api_marketingsolutions_v2024_01.model.contact_list_statistics_entity_v1_response import ContactListStatisticsEntityV1Response
-from criteo_api_marketingsolutions_v2024_01.model.contactlist_amendment_request import ContactlistAmendmentRequest
-from criteo_api_marketingsolutions_v2024_01.model.delete_audience_contact_list_response import DeleteAudienceContactListResponse
-from criteo_api_marketingsolutions_v2024_01.model.error_code_response import ErrorCodeResponse
-from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_brand_entity_v1_list_response import InMarketAudienceSegmentBrandEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_interest_entity_v1_list_response import InMarketAudienceSegmentInterestEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.modify_audience_response import ModifyAudienceResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_bulk_create_input_v1 import AudienceBulkCreateInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_bulk_delete_input_v1 import AudienceBulkDeleteInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_bulk_update_input_v1 import AudienceBulkUpdateInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_compute_sizes_input_v1 import AudienceComputeSizesInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1_audience_search_metadata_v1_list_response import AudienceEntityV1AudienceSearchMetadataV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1_list_response import AudienceEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_estimate_size_input_v1 import AudienceEstimateSizeInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_id_entity_v1_list_response import AudienceIdEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_search_input_v1 import AudienceSearchInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_bulk_create_input_v1 import AudienceSegmentBulkCreateInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_bulk_delete_input_v1 import AudienceSegmentBulkDeleteInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_bulk_update_input_v1 import AudienceSegmentBulkUpdateInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_compute_sizes_input_v1 import AudienceSegmentComputeSizesInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response import AudienceSegmentEntityV1AudienceSegmentSearchMetadataV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1_list_response import AudienceSegmentEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_estimate_size_input_v1 import AudienceSegmentEstimateSizeInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_id_entity_v1_list_response import AudienceSegmentIdEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_search_input_v1 import AudienceSegmentSearchInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_entity_v1_list_response import AudienceSegmentSizeEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_v1_response import AudienceSegmentSizeEstimationV1Response
+from criteo_api_marketingsolutions_v2024_04.model.audience_size_entity_v1_list_response import AudienceSizeEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_size_estimation_v1_response import AudienceSizeEstimationV1Response
+from criteo_api_marketingsolutions_v2024_04.model.contact_list_statistics_entity_v1_response import ContactListStatisticsEntityV1Response
+from criteo_api_marketingsolutions_v2024_04.model.contactlist_amendment_request import ContactlistAmendmentRequest
+from criteo_api_marketingsolutions_v2024_04.model.delete_audience_contact_list_response import DeleteAudienceContactListResponse
+from criteo_api_marketingsolutions_v2024_04.model.error_code_response import ErrorCodeResponse
+from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_brand_entity_v1_list_response import InMarketAudienceSegmentBrandEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_interest_entity_v1_list_response import InMarketAudienceSegmentInterestEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.modify_audience_response import ModifyAudienceResponse
 
 
 class AudienceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -66,15 +66,15 @@
         self.bulk_create_audience_segments_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceSegmentEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/create',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/create',
                 'operation_id': 'bulk_create_audience_segments',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_bulk_create_input_v1',
@@ -124,15 +124,15 @@
         self.bulk_create_audiences_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audiences/create',
+                'endpoint_path': '/2024-04/marketing-solutions/audiences/create',
                 'operation_id': 'bulk_create_audiences',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_bulk_create_input_v1',
@@ -182,15 +182,15 @@
         self.bulk_delete_audience_segments_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceSegmentIdEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/delete',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/delete',
                 'operation_id': 'bulk_delete_audience_segments',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_bulk_delete_input_v1',
@@ -240,15 +240,15 @@
         self.bulk_delete_audiences_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceIdEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audiences/delete',
+                'endpoint_path': '/2024-04/marketing-solutions/audiences/delete',
                 'operation_id': 'bulk_delete_audiences',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_bulk_delete_input_v1',
@@ -298,15 +298,15 @@
         self.bulk_update_audience_segments_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceSegmentEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments',
                 'operation_id': 'bulk_update_audience_segments',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_bulk_update_input_v1',
@@ -356,15 +356,15 @@
         self.bulk_update_audiences_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audiences',
+                'endpoint_path': '/2024-04/marketing-solutions/audiences',
                 'operation_id': 'bulk_update_audiences',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_bulk_update_input_v1',
@@ -414,15 +414,15 @@
         self.compute_audience_segments_sizes_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceSegmentSizeEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/compute-sizes',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/compute-sizes',
                 'operation_id': 'compute_audience_segments_sizes',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_compute_sizes_input_v1',
@@ -472,15 +472,15 @@
         self.compute_audiences_sizes_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceSizeEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audiences/compute-sizes',
+                'endpoint_path': '/2024-04/marketing-solutions/audiences/compute-sizes',
                 'operation_id': 'compute_audiences_sizes',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_compute_sizes_input_v1',
@@ -530,15 +530,15 @@
         self.delete_contact_list_identifiers_endpoint = _Endpoint(
             settings={
                 'response_type': (DeleteAudienceContactListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/{audience-segment-id}/contact-list',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/{audience-segment-id}/contact-list',
                 'operation_id': 'delete_contact_list_identifiers',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_id',
@@ -582,15 +582,15 @@
         self.estimate_audience_segment_size_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceSegmentSizeEstimationV1Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/estimate-size',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/estimate-size',
                 'operation_id': 'estimate_audience_segment_size',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_estimate_size_input_v1',
@@ -640,15 +640,15 @@
         self.estimate_audience_size_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceSizeEstimationV1Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audiences/estimate-size',
+                'endpoint_path': '/2024-04/marketing-solutions/audiences/estimate-size',
                 'operation_id': 'estimate_audience_size',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_estimate_size_input_v1',
@@ -698,15 +698,15 @@
         self.get_audience_segment_contact_list_statistics_endpoint = _Endpoint(
             settings={
                 'response_type': (ContactListStatisticsEntityV1Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/{audience-segment-id}/contact-list/statistics',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/{audience-segment-id}/contact-list/statistics',
                 'operation_id': 'get_audience_segment_contact_list_statistics',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_id',
@@ -752,15 +752,15 @@
         self.get_audience_segments_in_market_brands_endpoint = _Endpoint(
             settings={
                 'response_type': (InMarketAudienceSegmentBrandEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/in-market-brands',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/in-market-brands',
                 'operation_id': 'get_audience_segments_in_market_brands',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -812,15 +812,15 @@
         self.get_audience_segments_in_market_interests_endpoint = _Endpoint(
             settings={
                 'response_type': (InMarketAudienceSegmentInterestEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/in-market-interests',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/in-market-interests',
                 'operation_id': 'get_audience_segments_in_market_interests',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -872,15 +872,15 @@
         self.search_audience_segments_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceSegmentEntityV1AudienceSegmentSearchMetadataV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/search',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/search',
                 'operation_id': 'search_audience_segments',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_search_input_v1',
@@ -946,15 +946,15 @@
         self.search_audiences_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceEntityV1AudienceSearchMetadataV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audiences/search',
+                'endpoint_path': '/2024-04/marketing-solutions/audiences/search',
                 'operation_id': 'search_audiences',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_search_input_v1',
@@ -1020,15 +1020,15 @@
         self.update_contact_list_identifiers_endpoint = _Endpoint(
             settings={
                 'response_type': (ModifyAudienceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/audience-segments/{audience-segment-id}/contact-list',
+                'endpoint_path': '/2024-04/marketing-solutions/audience-segments/{audience-segment-id}/contact-list',
                 'operation_id': 'update_contact_list_identifiers',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'audience_segment_id',
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/campaign_api.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/campaign_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_entity_v1_response import AdSetAudienceLinkEntityV1Response
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_input_entity_v1 import AdSetAudienceLinkInputEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_search_request_v23_q1 import AdSetSearchRequestV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.campaign_search_request_v23_q1 import CampaignSearchRequestV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1_list_response import CampaignV23Q1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1_response import CampaignV23Q1Response
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_request import CreateAdSetRequest
-from criteo_api_marketingsolutions_v2024_01.model.create_campaign_request import CreateCampaignRequest
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
-from criteo_api_marketingsolutions_v2024_01.model.patch_campaign_list_request import PatchCampaignListRequest
-from criteo_api_marketingsolutions_v2024_01.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
-from criteo_api_marketingsolutions_v2024_01.model.requests_ad_set_id import RequestsAdSetId
-from criteo_api_marketingsolutions_v2024_01.model.requests_patch_ad_set import RequestsPatchAdSet
-from criteo_api_marketingsolutions_v2024_01.model.response_read_ad_set import ResponseReadAdSet
-from criteo_api_marketingsolutions_v2024_01.model.response_read_ad_set_v23_q1 import ResponseReadAdSetV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.responses_ad_set_id import ResponsesAdSetId
-from criteo_api_marketingsolutions_v2024_01.model.responses_read_ad_set_v23_q1 import ResponsesReadAdSetV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_entity_v1_response import AdSetAudienceLinkEntityV1Response
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_input_entity_v1 import AdSetAudienceLinkInputEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_search_request_v23_q1 import AdSetSearchRequestV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.campaign_search_request_v23_q1 import CampaignSearchRequestV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1_list_response import CampaignV23Q1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1_response import CampaignV23Q1Response
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_request import CreateAdSetRequest
+from criteo_api_marketingsolutions_v2024_04.model.create_campaign_request import CreateCampaignRequest
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
+from criteo_api_marketingsolutions_v2024_04.model.patch_campaign_list_request import PatchCampaignListRequest
+from criteo_api_marketingsolutions_v2024_04.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
+from criteo_api_marketingsolutions_v2024_04.model.requests_ad_set_id import RequestsAdSetId
+from criteo_api_marketingsolutions_v2024_04.model.requests_patch_ad_set import RequestsPatchAdSet
+from criteo_api_marketingsolutions_v2024_04.model.response_read_ad_set import ResponseReadAdSet
+from criteo_api_marketingsolutions_v2024_04.model.response_read_ad_set_v23_q1 import ResponseReadAdSetV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.responses_ad_set_id import ResponsesAdSetId
+from criteo_api_marketingsolutions_v2024_04.model.responses_read_ad_set_v23_q1 import ResponsesReadAdSetV23Q1
 
 
 class CampaignApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -59,15 +59,15 @@
         self.create_ad_set_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponseReadAdSet,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets',
                 'operation_id': 'create_ad_set',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'create_ad_set_request',
@@ -117,15 +117,15 @@
         self.create_campaign_endpoint = _Endpoint(
             settings={
                 'response_type': (CampaignV23Q1Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/campaigns',
+                'endpoint_path': '/2024-04/marketing-solutions/campaigns',
                 'operation_id': 'create_campaign',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'create_campaign_request',
@@ -175,15 +175,15 @@
         self.get_ad_set_v23_q1_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponseReadAdSetV23Q1,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/{ad-set-id}',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/{ad-set-id}',
                 'operation_id': 'get_ad_set_v23_q1',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -229,15 +229,15 @@
         self.get_campaign_v23_q1_endpoint = _Endpoint(
             settings={
                 'response_type': (CampaignV23Q1Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/campaigns/{campaign-id}',
+                'endpoint_path': '/2024-04/marketing-solutions/campaigns/{campaign-id}',
                 'operation_id': 'get_campaign_v23_q1',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -283,15 +283,15 @@
         self.get_category_bid_list_endpoint = _Endpoint(
             settings={
                 'response_type': (AdSetCategoryBidListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
                 'operation_id': 'get_category_bid_list',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -337,15 +337,15 @@
         self.get_display_multipliers_endpoint = _Endpoint(
             settings={
                 'response_type': (AdSetDisplayMultiplierListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
                 'operation_id': 'get_display_multipliers',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -391,15 +391,15 @@
         self.patch_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets',
                 'operation_id': 'patch_ad_sets',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_patch_ad_set',
@@ -447,15 +447,15 @@
         self.patch_campaigns_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchResultCampaignListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/campaigns',
+                'endpoint_path': '/2024-04/marketing-solutions/campaigns',
                 'operation_id': 'patch_campaigns',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'patch_campaign_list_request',
@@ -503,15 +503,15 @@
         self.patch_category_bid_list_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchAdSetCategoryBidResultListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
                 'operation_id': 'patch_category_bid_list',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -566,15 +566,15 @@
         self.patch_display_multipliers_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchAdSetDisplayMultiplierResultListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
                 'operation_id': 'patch_display_multipliers',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -629,15 +629,15 @@
         self.search_ad_sets_v23_q1_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesReadAdSetV23Q1,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/search',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/search',
                 'operation_id': 'search_ad_sets_v23_q1',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_search_request_v23_q1',
@@ -685,15 +685,15 @@
         self.search_campaigns_v23_q1_endpoint = _Endpoint(
             settings={
                 'response_type': (CampaignV23Q1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/campaigns/search',
+                'endpoint_path': '/2024-04/marketing-solutions/campaigns/search',
                 'operation_id': 'search_campaigns_v23_q1',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_search_request_v23_q1',
@@ -741,15 +741,15 @@
         self.start_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/start',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/start',
                 'operation_id': 'start_ad_sets',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_ad_set_id',
@@ -797,15 +797,15 @@
         self.stop_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/stop',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/stop',
                 'operation_id': 'stop_ad_sets',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_ad_set_id',
@@ -853,15 +853,15 @@
         self.update_ad_set_audience_endpoint = _Endpoint(
             settings={
                 'response_type': (AdSetAudienceLinkEntityV1Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ad-sets/{ad-set-id}/audience',
+                'endpoint_path': '/2024-04/marketing-solutions/ad-sets/{ad-set-id}/audience',
                 'operation_id': 'update_ad_set_audience',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/creative_api.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/creative_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2024_01.model.ad_list_response import AdListResponse
-from criteo_api_marketingsolutions_v2024_01.model.ad_response import AdResponse
-from criteo_api_marketingsolutions_v2024_01.model.ad_write_request import AdWriteRequest
-from criteo_api_marketingsolutions_v2024_01.model.coupon_list_response import CouponListResponse
-from criteo_api_marketingsolutions_v2024_01.model.coupon_response import CouponResponse
-from criteo_api_marketingsolutions_v2024_01.model.coupon_supported_sizes_response import CouponSupportedSizesResponse
-from criteo_api_marketingsolutions_v2024_01.model.create_coupon_request import CreateCouponRequest
-from criteo_api_marketingsolutions_v2024_01.model.creative_list_response import CreativeListResponse
-from criteo_api_marketingsolutions_v2024_01.model.creative_response import CreativeResponse
-from criteo_api_marketingsolutions_v2024_01.model.creative_write_request import CreativeWriteRequest
-from criteo_api_marketingsolutions_v2024_01.model.update_coupon_request import UpdateCouponRequest
+from criteo_api_marketingsolutions_v2024_04.model.ad_list_response import AdListResponse
+from criteo_api_marketingsolutions_v2024_04.model.ad_response import AdResponse
+from criteo_api_marketingsolutions_v2024_04.model.ad_write_request import AdWriteRequest
+from criteo_api_marketingsolutions_v2024_04.model.coupon_list_response import CouponListResponse
+from criteo_api_marketingsolutions_v2024_04.model.coupon_response import CouponResponse
+from criteo_api_marketingsolutions_v2024_04.model.coupon_supported_sizes_response import CouponSupportedSizesResponse
+from criteo_api_marketingsolutions_v2024_04.model.create_coupon_request import CreateCouponRequest
+from criteo_api_marketingsolutions_v2024_04.model.creative_list_response import CreativeListResponse
+from criteo_api_marketingsolutions_v2024_04.model.creative_response import CreativeResponse
+from criteo_api_marketingsolutions_v2024_04.model.creative_write_request import CreativeWriteRequest
+from criteo_api_marketingsolutions_v2024_04.model.update_coupon_request import UpdateCouponRequest
 
 
 class CreativeApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -48,15 +48,15 @@
         self.create_advertiser_ad_endpoint = _Endpoint(
             settings={
                 'response_type': (AdResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/ads',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/ads',
                 'operation_id': 'create_advertiser_ad',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -112,15 +112,15 @@
         self.create_advertiser_coupon_endpoint = _Endpoint(
             settings={
                 'response_type': (CouponResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/coupons',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/coupons',
                 'operation_id': 'create_advertiser_coupon',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -176,15 +176,15 @@
         self.create_advertiser_creative_endpoint = _Endpoint(
             settings={
                 'response_type': (CreativeResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/creatives',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/creatives',
                 'operation_id': 'create_advertiser_creative',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -240,15 +240,15 @@
         self.delete_ad_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ads/{id}',
+                'endpoint_path': '/2024-04/marketing-solutions/ads/{id}',
                 'operation_id': 'delete_ad',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -290,15 +290,15 @@
         self.delete_advertiser_coupon_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/coupons/{id}',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/coupons/{id}',
                 'operation_id': 'delete_advertiser_coupon',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -346,15 +346,15 @@
         self.delete_creative_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/creatives/{id}',
+                'endpoint_path': '/2024-04/marketing-solutions/creatives/{id}',
                 'operation_id': 'delete_creative',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -396,15 +396,15 @@
         self.edit_advertiser_coupon_endpoint = _Endpoint(
             settings={
                 'response_type': (CouponResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/coupons/{id}',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/coupons/{id}',
                 'operation_id': 'edit_advertiser_coupon',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -466,15 +466,15 @@
         self.edit_creative_endpoint = _Endpoint(
             settings={
                 'response_type': (CreativeResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/creatives/{id}',
+                'endpoint_path': '/2024-04/marketing-solutions/creatives/{id}',
                 'operation_id': 'edit_creative',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -530,15 +530,15 @@
         self.generate_creative_preview_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/creatives/{id}/preview',
+                'endpoint_path': '/2024-04/marketing-solutions/creatives/{id}/preview',
                 'operation_id': 'generate_creative_preview',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -594,15 +594,15 @@
         self.get_ad_endpoint = _Endpoint(
             settings={
                 'response_type': (AdResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/ads/{id}',
+                'endpoint_path': '/2024-04/marketing-solutions/ads/{id}',
                 'operation_id': 'get_ad',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -648,15 +648,15 @@
         self.get_advertiser_ads_endpoint = _Endpoint(
             settings={
                 'response_type': (AdListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/ads',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/ads',
                 'operation_id': 'get_advertiser_ads',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -712,15 +712,15 @@
         self.get_advertiser_coupon_endpoint = _Endpoint(
             settings={
                 'response_type': (CouponResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/coupons/{id}',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/coupons/{id}',
                 'operation_id': 'get_advertiser_coupon',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -772,15 +772,15 @@
         self.get_advertiser_coupon_preview_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/coupons/{id}/preview',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/coupons/{id}/preview',
                 'operation_id': 'get_advertiser_coupon_preview',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -842,15 +842,15 @@
         self.get_advertiser_coupon_supported_sizes_endpoint = _Endpoint(
             settings={
                 'response_type': (CouponSupportedSizesResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/coupons-supported-sizes',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/coupons-supported-sizes',
                 'operation_id': 'get_advertiser_coupon_supported_sizes',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -901,15 +901,15 @@
         self.get_advertiser_coupons_endpoint = _Endpoint(
             settings={
                 'response_type': (CouponListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/coupons',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/coupons',
                 'operation_id': 'get_advertiser_coupons',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -965,15 +965,15 @@
         self.get_advertiser_creatives_endpoint = _Endpoint(
             settings={
                 'response_type': (CreativeListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/advertisers/{advertiser-id}/creatives',
+                'endpoint_path': '/2024-04/marketing-solutions/advertisers/{advertiser-id}/creatives',
                 'operation_id': 'get_advertiser_creatives',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
@@ -1029,15 +1029,15 @@
         self.get_creative_endpoint = _Endpoint(
             settings={
                 'response_type': (CreativeResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/creatives/{id}',
+                'endpoint_path': '/2024-04/marketing-solutions/creatives/{id}',
                 'operation_id': 'get_creative',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api/gateway_api.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api/gateway_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2024_01.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_marketingsolutions_v2024_04.model.application_summary_model_response import ApplicationSummaryModelResponse
 
 
 class GatewayApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -38,15 +38,15 @@
         self.get_current_application_endpoint = _Endpoint(
             settings={
                 'response_type': (ApplicationSummaryModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/marketing-solutions/me',
+                'endpoint_path': '/2024-04/marketing-solutions/me',
                 'operation_id': 'get_current_application',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api_client.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -16,18 +16,18 @@
 import os
 import re
 import typing
 from urllib.parse import quote
 from urllib3.fields import RequestField
 
 
-from criteo_api_marketingsolutions_v2024_01 import rest
-from criteo_api_marketingsolutions_v2024_01.configuration import Configuration
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiTypeError, ApiValueError, ApiException
-from criteo_api_marketingsolutions_v2024_01.model_utils import (
+from criteo_api_marketingsolutions_v2024_04 import rest
+from criteo_api_marketingsolutions_v2024_04.configuration import Configuration
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiTypeError, ApiValueError, ApiException
+from criteo_api_marketingsolutions_v2024_04.model_utils import (
     ModelNormal,
     ModelSimple,
     ModelComposed,
     check_allowed_values,
     check_validations,
     date,
     datetime,
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.01.0.240515/python'
+        self.user_agent = 'OpenAPI-Generator/2024.04.0.240515/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/api_client_builder.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/api_client_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from criteo_api_marketingsolutions_v2024_01.configuration import Configuration
-from criteo_api_marketingsolutions_v2024_01.criteo_api_client import CriteoApiClient
-from criteo_api_marketingsolutions_v2024_01 import flow_constants
+from criteo_api_marketingsolutions_v2024_04.configuration import Configuration
+from criteo_api_marketingsolutions_v2024_04.criteo_api_client import CriteoApiClient
+from criteo_api_marketingsolutions_v2024_04 import flow_constants
 
 class ApiClientBuilder :
 
     @staticmethod
     def WithClientCredentials(clientId, clientSecret, host=None):
         configuration = Configuration(username=clientId, password=clientSecret, host=host)
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/apis/__init__.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/apis/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from criteo_api_marketingsolutions_v2024_01.api.advertiser_api import AdvertiserApi
+#   from criteo_api_marketingsolutions_v2024_04.api.advertiser_api import AdvertiserApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
-from criteo_api_marketingsolutions_v2024_01.api.advertiser_api import AdvertiserApi
-from criteo_api_marketingsolutions_v2024_01.api.analytics_api import AnalyticsApi
-from criteo_api_marketingsolutions_v2024_01.api.audience_api import AudienceApi
-from criteo_api_marketingsolutions_v2024_01.api.campaign_api import CampaignApi
-from criteo_api_marketingsolutions_v2024_01.api.creative_api import CreativeApi
-from criteo_api_marketingsolutions_v2024_01.api.gateway_api import GatewayApi
+from criteo_api_marketingsolutions_v2024_04.api.advertiser_api import AdvertiserApi
+from criteo_api_marketingsolutions_v2024_04.api.analytics_api import AnalyticsApi
+from criteo_api_marketingsolutions_v2024_04.api.audience_api import AudienceApi
+from criteo_api_marketingsolutions_v2024_04.api.campaign_api import CampaignApi
+from criteo_api_marketingsolutions_v2024_04.api.creative_api import CreativeApi
+from criteo_api_marketingsolutions_v2024_04.api.gateway_api import GatewayApi
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/configuration.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 from http import client as http_client
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiValueError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiValueError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
@@ -129,15 +129,15 @@
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("criteo_api_marketingsolutions_v2024_01")
+        self.logger["package_logger"] = logging.getLogger("criteo_api_marketingsolutions_v2024_04")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
@@ -390,16 +390,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2024-01\n"\
-               "SDK Package Version: 2024.01.0.240515".\
+               "Version of the API: 2024-04\n"\
+               "SDK Package Version: 2024.04.0.240515".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/criteo_api_client.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/criteo_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient
-from criteo_api_marketingsolutions_v2024_01.criteo_rest import CriteoRESTClientObject
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient
+from criteo_api_marketingsolutions_v2024_04.criteo_rest import CriteoRESTClientObject
 
 class CriteoApiClient(ApiClient):
     def __init__(self, configuration=None, header_name=None, header_value=None,
              cookie=None, pool_threads=1, additional_parameters= {}):
         super().__init__(configuration=configuration,header_name=header_name, header_value=header_value, cookie=cookie, pool_threads=pool_threads)
         self.rest_client = CriteoRESTClientObject(self.configuration, additional_parameters)
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/criteo_auth.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/criteo_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from datetime import datetime, timedelta
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiException
-from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient
-from criteo_api_marketingsolutions_v2024_01 import flow_constants
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiException
+from criteo_api_marketingsolutions_v2024_04.api_client import ApiClient
+from criteo_api_marketingsolutions_v2024_04 import flow_constants
 
 class Token(object):
 
     def __init__(self, token_string , expiration_date = None):
         self.expiration_date = expiration_date 
         self.token_string = token_string
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/criteo_rest.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/criteo_rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from criteo_api_marketingsolutions_v2024_01.rest import RESTClientObject
-from criteo_api_marketingsolutions_v2024_01.criteo_auth import *
-from criteo_api_marketingsolutions_v2024_01 import flow_constants
+from criteo_api_marketingsolutions_v2024_04.rest import RESTClientObject
+from criteo_api_marketingsolutions_v2024_04.criteo_auth import *
+from criteo_api_marketingsolutions_v2024_04 import flow_constants
 
 
 class CriteoRESTClientObject(RESTClientObject):
 
     def __init__(self, configuration, additional_parameters = {}, pools_size=4, maxsize=None):
         super().__init__(configuration, pools_size, maxsize)
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/exceptions.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class Ad(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_resource import AdResource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.ad_resource import AdResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AdResource'] = AdResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AdListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad import Ad
+    from criteo_api_marketingsolutions_v2024_04.model.ad import Ad
     globals()['Ad'] = Ad
 
 
 class AdResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_resource import AdResource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.ad_resource import AdResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AdResource'] = AdResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AdResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetAudienceLinkEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_entity_v1 import AdSetAudienceLinkEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_entity_v1 import AdSetAudienceLinkEntityV1
     globals()['AdSetAudienceLinkEntityV1'] = AdSetAudienceLinkEntityV1
 
 
 class AdSetAudienceLinkEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_entity_v1_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_entity_v1_resource import AdSetAudienceLinkEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_entity_v1_resource import AdSetAudienceLinkEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AdSetAudienceLinkEntityV1Resource'] = AdSetAudienceLinkEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AdSetAudienceLinkEntityV1Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_input_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_audience_link_input_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_entity_v1_resource import AdSetAudienceLinkEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_entity_v1_resource import AdSetAudienceLinkEntityV1Resource
     globals()['AdSetAudienceLinkEntityV1Resource'] = AdSetAudienceLinkEntityV1Resource
 
 
 class AdSetAudienceLinkInputEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetCategoryBid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_category_bid_resource import AdSetCategoryBidResource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_category_bid_resource import AdSetCategoryBidResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AdSetCategoryBidResource'] = AdSetCategoryBidResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AdSetCategoryBidListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_category_bid_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_category_bid import AdSetCategoryBid
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_category_bid import AdSetCategoryBid
     globals()['AdSetCategoryBid'] = AdSetCategoryBid
 
 
 class AdSetCategoryBidResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_delivery_limitations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetDeliveryLimitations(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_delivery_limitations_v23_q1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetDeliveryLimitationsV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetDisplayMultiplier(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AdSetDisplayMultiplierResource'] = AdSetDisplayMultiplierResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AdSetDisplayMultiplierListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_display_multiplier_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_display_multiplier import AdSetDisplayMultiplier
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_display_multiplier import AdSetDisplayMultiplier
     globals()['AdSetDisplayMultiplier'] = AdSetDisplayMultiplier
 
 
 class AdSetDisplayMultiplierResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_frequency_capping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetFrequencyCapping(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_frequency_capping_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetFrequencyCappingV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_geo_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
     globals()['NillableAdSetTargetingRule'] = NillableAdSetTargetingRule
 
 
 class AdSetGeoLocation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_geo_location_v23_q1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_ad_set_targeting_rule_v23_q1 import NillableAdSetTargetingRuleV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_ad_set_targeting_rule_v23_q1 import NillableAdSetTargetingRuleV23Q1
     globals()['NillableAdSetTargetingRuleV23Q1'] = NillableAdSetTargetingRuleV23Q1
 
 
 class AdSetGeoLocationV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_filter_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_search_filter_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetSearchFilterV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_request_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_search_request_v23_q1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_search_filter_v23_q1 import AdSetSearchFilterV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_search_filter_v23_q1 import AdSetSearchFilterV23Q1
     globals()['AdSetSearchFilterV23Q1'] = AdSetSearchFilterV23Q1
 
 
 class AdSetSearchRequestV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_frequency_capping import AdSetFrequencyCapping
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_geo_location import AdSetGeoLocation
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_frequency_capping import AdSetFrequencyCapping
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_geo_location import AdSetGeoLocation
     globals()['AdSetDeliveryLimitations'] = AdSetDeliveryLimitations
     globals()['AdSetFrequencyCapping'] = AdSetFrequencyCapping
     globals()['AdSetGeoLocation'] = AdSetGeoLocation
 
 
 class AdSetTargeting(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetTargetingRule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_rule_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdSetTargetingRuleV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_set_targeting_v23_q1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_delivery_limitations_v23_q1 import AdSetDeliveryLimitationsV23Q1
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_frequency_capping_v23_q1 import AdSetFrequencyCappingV23Q1
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_geo_location_v23_q1 import AdSetGeoLocationV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_delivery_limitations_v23_q1 import AdSetDeliveryLimitationsV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_frequency_capping_v23_q1 import AdSetFrequencyCappingV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_geo_location_v23_q1 import AdSetGeoLocationV23Q1
     globals()['AdSetDeliveryLimitationsV23Q1'] = AdSetDeliveryLimitationsV23Q1
     globals()['AdSetFrequencyCappingV23Q1'] = AdSetFrequencyCappingV23Q1
     globals()['AdSetGeoLocationV23Q1'] = AdSetGeoLocationV23Q1
 
 
 class AdSetTargetingV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_write.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdWrite(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_write_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_write_resource import AdWriteResource
+    from criteo_api_marketingsolutions_v2024_04.model.ad_write_resource import AdWriteResource
     globals()['AdWriteResource'] = AdWriteResource
 
 
 class AdWriteRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/ad_write_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/ad_write_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_write import AdWrite
+    from criteo_api_marketingsolutions_v2024_04.model.ad_write import AdWrite
     globals()['AdWrite'] = AdWrite
 
 
 class AdWriteResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/adaptive_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/adaptive_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.adaptive_colors import AdaptiveColors
-    from criteo_api_marketingsolutions_v2024_01.model.image_set import ImageSet
-    from criteo_api_marketingsolutions_v2024_01.model.image_shape import ImageShape
-    from criteo_api_marketingsolutions_v2024_01.model.video_detail import VideoDetail
+    from criteo_api_marketingsolutions_v2024_04.model.adaptive_colors import AdaptiveColors
+    from criteo_api_marketingsolutions_v2024_04.model.image_set import ImageSet
+    from criteo_api_marketingsolutions_v2024_04.model.image_shape import ImageShape
+    from criteo_api_marketingsolutions_v2024_04.model.video_detail import VideoDetail
     globals()['AdaptiveColors'] = AdaptiveColors
     globals()['ImageSet'] = ImageSet
     globals()['ImageShape'] = ImageShape
     globals()['VideoDetail'] = VideoDetail
 
 
 class AdaptiveAttributes(ModelNormal):
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/adaptive_colors.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/adaptive_colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AdaptiveColors(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/adaptive_write_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/adaptive_write_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.adaptive_colors import AdaptiveColors
-    from criteo_api_marketingsolutions_v2024_01.model.image_set_base64 import ImageSetBase64
+    from criteo_api_marketingsolutions_v2024_04.model.adaptive_colors import AdaptiveColors
+    from criteo_api_marketingsolutions_v2024_04.model.image_set_base64 import ImageSetBase64
     globals()['AdaptiveColors'] = AdaptiveColors
     globals()['ImageSetBase64'] = ImageSetBase64
 
 
 class AdaptiveWriteAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/algebra_node_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/algebra_node_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AlgebraNodeV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/application_summary_model.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/application_summary_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ApplicationSummaryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/application_summary_model_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.application_summary_model import ApplicationSummaryModel
+    from criteo_api_marketingsolutions_v2024_04.model.application_summary_model import ApplicationSummaryModel
     globals()['ApplicationSummaryModel'] = ApplicationSummaryModel
 
 
 class ApplicationSummaryModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/application_summary_model_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.application_summary_model_resource import ApplicationSummaryModelResource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.application_summary_model_resource import ApplicationSummaryModelResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['ApplicationSummaryModelResource'] = ApplicationSummaryModelResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class ApplicationSummaryModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_create_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_bulk_create_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_create_entity_v1_resource import AudienceCreateEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_create_entity_v1_resource import AudienceCreateEntityV1Resource
     globals()['AudienceCreateEntityV1Resource'] = AudienceCreateEntityV1Resource
 
 
 class AudienceBulkCreateInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_delete_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_bulk_delete_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_delete_entity_v1_resource import AudienceDeleteEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_delete_entity_v1_resource import AudienceDeleteEntityV1Resource
     globals()['AudienceDeleteEntityV1Resource'] = AudienceDeleteEntityV1Resource
 
 
 class AudienceBulkDeleteInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_update_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_bulk_update_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_update_entity_v1_resource import AudienceUpdateEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_update_entity_v1_resource import AudienceUpdateEntityV1Resource
     globals()['AudienceUpdateEntityV1Resource'] = AudienceUpdateEntityV1Resource
 
 
 class AudienceBulkUpdateInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_compute_size_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_compute_size_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceComputeSizeEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_compute_sizes_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_compute_sizes_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_compute_size_entity_v1_resource import AudienceComputeSizeEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_compute_size_entity_v1_resource import AudienceComputeSizeEntityV1Resource
     globals()['AudienceComputeSizeEntityV1Resource'] = AudienceComputeSizeEntityV1Resource
 
 
 class AudienceComputeSizesInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_create_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.algebra_node_v1 import AlgebraNodeV1
+    from criteo_api_marketingsolutions_v2024_04.model.algebra_node_v1 import AlgebraNodeV1
     globals()['AlgebraNodeV1'] = AlgebraNodeV1
 
 
 class AudienceCreateEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_create_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_create_entity_v1 import AudienceCreateEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_create_entity_v1 import AudienceCreateEntityV1
     globals()['AudienceCreateEntityV1'] = AudienceCreateEntityV1
 
 
 class AudienceCreateEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_delete_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_delete_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceDeleteEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.algebra_node_v1 import AlgebraNodeV1
+    from criteo_api_marketingsolutions_v2024_04.model.algebra_node_v1 import AlgebraNodeV1
     globals()['AlgebraNodeV1'] = AlgebraNodeV1
 
 
 class AudienceEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_audience_search_metadata_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_audience_search_metadata_v1_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1_resource import AudienceEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.audience_search_metadata_v1 import AudienceSearchMetadataV1
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1_resource import AudienceEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_search_metadata_v1 import AudienceSearchMetadataV1
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceEntityV1Resource'] = AudienceEntityV1Resource
     globals()['AudienceSearchMetadataV1'] = AudienceSearchMetadataV1
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceEntityV1AudienceSearchMetadataV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1_resource import AudienceEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1_resource import AudienceEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceEntityV1Resource'] = AudienceEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1 import AudienceEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1 import AudienceEntityV1
     globals()['AudienceEntityV1'] = AudienceEntityV1
 
 
 class AudienceEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_error.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_entity_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.algebra_node_v1 import AlgebraNodeV1
+    from criteo_api_marketingsolutions_v2024_04.model.algebra_node_v1 import AlgebraNodeV1
     globals()['AlgebraNodeV1'] = AlgebraNodeV1
 
 
 class AudienceEstimateSizeEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_estimate_size_entity_v1 import AudienceEstimateSizeEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_estimate_size_entity_v1 import AudienceEstimateSizeEntityV1
     globals()['AudienceEstimateSizeEntityV1'] = AudienceEstimateSizeEntityV1
 
 
 class AudienceEstimateSizeEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_estimate_size_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_estimate_size_entity_v1_resource import AudienceEstimateSizeEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_estimate_size_entity_v1_resource import AudienceEstimateSizeEntityV1Resource
     globals()['AudienceEstimateSizeEntityV1Resource'] = AudienceEstimateSizeEntityV1Resource
 
 
 class AudienceEstimateSizeInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_id_entity_v1_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_id_entity_v1_resource import AudienceIdEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_id_entity_v1_resource import AudienceIdEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceIdEntityV1Resource'] = AudienceIdEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceIdEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_id_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceIdEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_name_description.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_name_description.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceNameDescription(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_search_entity_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSearchEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_search_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_search_entity_v1 import AudienceSearchEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_search_entity_v1 import AudienceSearchEntityV1
     globals()['AudienceSearchEntityV1'] = AudienceSearchEntityV1
 
 
 class AudienceSearchEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_search_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_search_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_search_entity_v1_resource import AudienceSearchEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_search_entity_v1_resource import AudienceSearchEntityV1Resource
     globals()['AudienceSearchEntityV1Resource'] = AudienceSearchEntityV1Resource
 
 
 class AudienceSearchInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_search_metadata_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_search_metadata_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSearchMetadataV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_create_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_create_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_create_entity_v1_resource import AudienceSegmentCreateEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_create_entity_v1_resource import AudienceSegmentCreateEntityV1Resource
     globals()['AudienceSegmentCreateEntityV1Resource'] = AudienceSegmentCreateEntityV1Resource
 
 
 class AudienceSegmentBulkCreateInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_delete_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_delete_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_delete_entity_v1_resource import AudienceSegmentDeleteEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_delete_entity_v1_resource import AudienceSegmentDeleteEntityV1Resource
     globals()['AudienceSegmentDeleteEntityV1Resource'] = AudienceSegmentDeleteEntityV1Resource
 
 
 class AudienceSegmentBulkDeleteInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_update_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_bulk_update_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_update_entity_v1_resource import AudienceSegmentUpdateEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_update_entity_v1_resource import AudienceSegmentUpdateEntityV1Resource
     globals()['AudienceSegmentUpdateEntityV1Resource'] = AudienceSegmentUpdateEntityV1Resource
 
 
 class AudienceSegmentBulkUpdateInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_size_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_compute_size_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSegmentComputeSizeEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_sizes_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_compute_sizes_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_compute_size_entity_v1_resource import AudienceSegmentComputeSizeEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_compute_size_entity_v1_resource import AudienceSegmentComputeSizeEntityV1Resource
     globals()['AudienceSegmentComputeSizeEntityV1Resource'] = AudienceSegmentComputeSizeEntityV1Resource
 
 
 class AudienceSegmentComputeSizesInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_create_entity_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.in_market_create_v1 import InMarketCreateV1
-    from criteo_api_marketingsolutions_v2024_01.model.location_create_v1 import LocationCreateV1
-    from criteo_api_marketingsolutions_v2024_01.model.lookalike_create_v1 import LookalikeCreateV1
-    from criteo_api_marketingsolutions_v2024_01.model.prospecting_create_v1 import ProspectingCreateV1
-    from criteo_api_marketingsolutions_v2024_01.model.retargeting_create_v1 import RetargetingCreateV1
+    from criteo_api_marketingsolutions_v2024_04.model.in_market_create_v1 import InMarketCreateV1
+    from criteo_api_marketingsolutions_v2024_04.model.location_create_v1 import LocationCreateV1
+    from criteo_api_marketingsolutions_v2024_04.model.lookalike_create_v1 import LookalikeCreateV1
+    from criteo_api_marketingsolutions_v2024_04.model.prospecting_create_v1 import ProspectingCreateV1
+    from criteo_api_marketingsolutions_v2024_04.model.retargeting_create_v1 import RetargetingCreateV1
     globals()['InMarketCreateV1'] = InMarketCreateV1
     globals()['LocationCreateV1'] = LocationCreateV1
     globals()['LookalikeCreateV1'] = LookalikeCreateV1
     globals()['ProspectingCreateV1'] = ProspectingCreateV1
     globals()['RetargetingCreateV1'] = RetargetingCreateV1
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_create_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_create_entity_v1 import AudienceSegmentCreateEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_create_entity_v1 import AudienceSegmentCreateEntityV1
     globals()['AudienceSegmentCreateEntityV1'] = AudienceSegmentCreateEntityV1
 
 
 class AudienceSegmentCreateEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_delete_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_delete_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSegmentDeleteEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.behavioral_v1 import BehavioralV1
-    from criteo_api_marketingsolutions_v2024_01.model.contact_list_v1 import ContactListV1
-    from criteo_api_marketingsolutions_v2024_01.model.in_market_v1 import InMarketV1
-    from criteo_api_marketingsolutions_v2024_01.model.location_v1 import LocationV1
-    from criteo_api_marketingsolutions_v2024_01.model.lookalike_v1 import LookalikeV1
-    from criteo_api_marketingsolutions_v2024_01.model.prospecting_v1 import ProspectingV1
-    from criteo_api_marketingsolutions_v2024_01.model.retargeting_v1 import RetargetingV1
+    from criteo_api_marketingsolutions_v2024_04.model.behavioral_v1 import BehavioralV1
+    from criteo_api_marketingsolutions_v2024_04.model.contact_list_v1 import ContactListV1
+    from criteo_api_marketingsolutions_v2024_04.model.in_market_v1 import InMarketV1
+    from criteo_api_marketingsolutions_v2024_04.model.location_v1 import LocationV1
+    from criteo_api_marketingsolutions_v2024_04.model.lookalike_v1 import LookalikeV1
+    from criteo_api_marketingsolutions_v2024_04.model.prospecting_v1 import ProspectingV1
+    from criteo_api_marketingsolutions_v2024_04.model.retargeting_v1 import RetargetingV1
     globals()['BehavioralV1'] = BehavioralV1
     globals()['ContactListV1'] = ContactListV1
     globals()['InMarketV1'] = InMarketV1
     globals()['LocationV1'] = LocationV1
     globals()['LookalikeV1'] = LookalikeV1
     globals()['ProspectingV1'] = ProspectingV1
     globals()['RetargetingV1'] = RetargetingV1
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1_resource import AudienceSegmentEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_search_metadata_v1 import AudienceSegmentSearchMetadataV1
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1_resource import AudienceSegmentEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_search_metadata_v1 import AudienceSegmentSearchMetadataV1
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceSegmentEntityV1Resource'] = AudienceSegmentEntityV1Resource
     globals()['AudienceSegmentSearchMetadataV1'] = AudienceSegmentSearchMetadataV1
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceSegmentEntityV1AudienceSegmentSearchMetadataV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1_resource import AudienceSegmentEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1_resource import AudienceSegmentEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceSegmentEntityV1Resource'] = AudienceSegmentEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceSegmentEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1 import AudienceSegmentEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1 import AudienceSegmentEntityV1
     globals()['AudienceSegmentEntityV1'] = AudienceSegmentEntityV1
 
 
 class AudienceSegmentEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_estimate_size_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_estimate_size_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_entity_v1_resource import AudienceSegmentSizeEstimationEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_entity_v1_resource import AudienceSegmentSizeEstimationEntityV1Resource
     globals()['AudienceSegmentSizeEstimationEntityV1Resource'] = AudienceSegmentSizeEstimationEntityV1Resource
 
 
 class AudienceSegmentEstimateSizeInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_id_entity_v1_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_id_entity_v1_resource import AudienceSegmentIdEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_id_entity_v1_resource import AudienceSegmentIdEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceSegmentIdEntityV1Resource'] = AudienceSegmentIdEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceSegmentIdEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_id_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSegmentIdEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSegmentSearchEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_search_entity_v1 import AudienceSegmentSearchEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_search_entity_v1 import AudienceSegmentSearchEntityV1
     globals()['AudienceSegmentSearchEntityV1'] = AudienceSegmentSearchEntityV1
 
 
 class AudienceSegmentSearchEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_input_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_search_entity_v1_resource import AudienceSegmentSearchEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_search_entity_v1_resource import AudienceSegmentSearchEntityV1Resource
     globals()['AudienceSegmentSearchEntityV1Resource'] = AudienceSegmentSearchEntityV1Resource
 
 
 class AudienceSegmentSearchInputV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_metadata_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_search_metadata_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSegmentSearchMetadataV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSegmentSizeEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_entity_v1_resource import AudienceSegmentSizeEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_entity_v1_resource import AudienceSegmentSizeEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceSegmentSizeEntityV1Resource'] = AudienceSegmentSizeEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceSegmentSizeEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_entity_v1 import AudienceSegmentSizeEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_entity_v1 import AudienceSegmentSizeEntityV1
     globals()['AudienceSegmentSizeEntityV1'] = AudienceSegmentSizeEntityV1
 
 
 class AudienceSegmentSizeEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_entity_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.in_market_size_estimation_v1 import InMarketSizeEstimationV1
-    from criteo_api_marketingsolutions_v2024_01.model.location_size_estimation_v1 import LocationSizeEstimationV1
+    from criteo_api_marketingsolutions_v2024_04.model.in_market_size_estimation_v1 import InMarketSizeEstimationV1
+    from criteo_api_marketingsolutions_v2024_04.model.location_size_estimation_v1 import LocationSizeEstimationV1
     globals()['InMarketSizeEstimationV1'] = InMarketSizeEstimationV1
     globals()['LocationSizeEstimationV1'] = LocationSizeEstimationV1
 
 
 class AudienceSegmentSizeEstimationEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_entity_v1 import AudienceSegmentSizeEstimationEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_entity_v1 import AudienceSegmentSizeEstimationEntityV1
     globals()['AudienceSegmentSizeEstimationEntityV1'] = AudienceSegmentSizeEstimationEntityV1
 
 
 class AudienceSegmentSizeEstimationEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSegmentSizeEstimationV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_v1 import AudienceSegmentSizeEstimationV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_v1 import AudienceSegmentSizeEstimationV1
     globals()['AudienceSegmentSizeEstimationV1'] = AudienceSegmentSizeEstimationV1
 
 
 class AudienceSegmentSizeEstimationV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_size_estimation_v1_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_v1_resource import AudienceSegmentSizeEstimationV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_v1_resource import AudienceSegmentSizeEstimationV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceSegmentSizeEstimationV1Resource'] = AudienceSegmentSizeEstimationV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceSegmentSizeEstimationV1Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_update_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.in_market_update_v1 import InMarketUpdateV1
-    from criteo_api_marketingsolutions_v2024_01.model.location_update_v1 import LocationUpdateV1
-    from criteo_api_marketingsolutions_v2024_01.model.lookalike_update_v1 import LookalikeUpdateV1
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_string import NillableString
-    from criteo_api_marketingsolutions_v2024_01.model.prospecting_update_v1 import ProspectingUpdateV1
-    from criteo_api_marketingsolutions_v2024_01.model.retargeting_update_v1 import RetargetingUpdateV1
+    from criteo_api_marketingsolutions_v2024_04.model.in_market_update_v1 import InMarketUpdateV1
+    from criteo_api_marketingsolutions_v2024_04.model.location_update_v1 import LocationUpdateV1
+    from criteo_api_marketingsolutions_v2024_04.model.lookalike_update_v1 import LookalikeUpdateV1
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_string import NillableString
+    from criteo_api_marketingsolutions_v2024_04.model.prospecting_update_v1 import ProspectingUpdateV1
+    from criteo_api_marketingsolutions_v2024_04.model.retargeting_update_v1 import RetargetingUpdateV1
     globals()['InMarketUpdateV1'] = InMarketUpdateV1
     globals()['LocationUpdateV1'] = LocationUpdateV1
     globals()['LookalikeUpdateV1'] = LookalikeUpdateV1
     globals()['NillableString'] = NillableString
     globals()['ProspectingUpdateV1'] = ProspectingUpdateV1
     globals()['RetargetingUpdateV1'] = RetargetingUpdateV1
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_segment_update_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_segment_update_entity_v1 import AudienceSegmentUpdateEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_segment_update_entity_v1 import AudienceSegmentUpdateEntityV1
     globals()['AudienceSegmentUpdateEntityV1'] = AudienceSegmentUpdateEntityV1
 
 
 class AudienceSegmentUpdateEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSizeEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_size_entity_v1_resource import AudienceSizeEntityV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_size_entity_v1_resource import AudienceSizeEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceSizeEntityV1Resource'] = AudienceSizeEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceSizeEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_size_entity_v1 import AudienceSizeEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_size_entity_v1 import AudienceSizeEntityV1
     globals()['AudienceSizeEntityV1'] = AudienceSizeEntityV1
 
 
 class AudienceSizeEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceSizeEstimationV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_size_estimation_v1 import AudienceSizeEstimationV1
+    from criteo_api_marketingsolutions_v2024_04.model.audience_size_estimation_v1 import AudienceSizeEstimationV1
     globals()['AudienceSizeEstimationV1'] = AudienceSizeEstimationV1
 
 
 class AudienceSizeEstimationV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_size_estimation_v1_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_size_estimation_v1_resource import AudienceSizeEstimationV1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.audience_size_estimation_v1_resource import AudienceSizeEstimationV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['AudienceSizeEstimationV1Resource'] = AudienceSizeEstimationV1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AudienceSizeEstimationV1Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_update_entity_v1_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.algebra_node_v1 import AlgebraNodeV1
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_string import NillableString
-    globals()['AlgebraNodeV1'] = AlgebraNodeV1
-    globals()['NillableString'] = NillableString
+    from criteo_api_marketingsolutions_v2024_04.model.audience_update_entity_v1 import AudienceUpdateEntityV1
+    globals()['AudienceUpdateEntityV1'] = AudienceUpdateEntityV1
 
 
-class AudienceUpdateEntityV1(ModelNormal):
+class AudienceUpdateEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,39 +83,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'name': (str, none_type,),  # noqa: E501
-            'description': (NillableString,),  # noqa: E501
-            'algebra': (AlgebraNodeV1,),  # noqa: E501
+            'attributes': (AudienceUpdateEntityV1,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
+            'type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'algebra': 'algebra',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AudienceUpdateEntityV1 - a model defined in OpenAPI
+        """AudienceUpdateEntityV1Resource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,17 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): Name of the audience. [optional]  # noqa: E501
-            description (NillableString): [optional]  # noqa: E501
-            algebra (AlgebraNodeV1): [optional]  # noqa: E501
+            attributes (AudienceUpdateEntityV1): [optional]  # noqa: E501
+            id (str, none_type): Id of the entity. [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -197,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AudienceUpdateEntityV1 - a model defined in OpenAPI
+        """AudienceUpdateEntityV1Resource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,17 +228,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): Name of the audience. [optional]  # noqa: E501
-            description (NillableString): [optional]  # noqa: E501
-            algebra (AlgebraNodeV1): [optional]  # noqa: E501
+            attributes (AudienceUpdateEntityV1): [optional]  # noqa: E501
+            id (str, none_type): Id of the entity. [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_campaign_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_update_entity_v1 import AudienceUpdateEntityV1
-    globals()['AudienceUpdateEntityV1'] = AudienceUpdateEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.create_campaign import CreateCampaign
+    globals()['CreateCampaign'] = CreateCampaign
 
 
-class AudienceUpdateEntityV1Resource(ModelNormal):
+class CreateCampaignResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,39 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (AudienceUpdateEntityV1,),  # noqa: E501
-            'id': (str, none_type,),  # noqa: E501
+            'attributes': (CreateCampaign,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'attributes': 'attributes',  # noqa: E501
-        'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AudienceUpdateEntityV1Resource - a model defined in OpenAPI
+        """CreateCampaignResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (AudienceUpdateEntityV1): [optional]  # noqa: E501
-            id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): [optional]  # noqa: E501
+            attributes (CreateCampaign): [optional]  # noqa: E501
+            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AudienceUpdateEntityV1Resource - a model defined in OpenAPI
+        """CreateCampaignResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (AudienceUpdateEntityV1): [optional]  # noqa: E501
-            id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): [optional]  # noqa: E501
+            attributes (CreateCampaign): [optional]  # noqa: E501
+            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/audience_warning.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AudienceWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/basic_audience_definition.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/basic_audience_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_name_description import AudienceNameDescription
+    from criteo_api_marketingsolutions_v2024_04.model.audience_name_description import AudienceNameDescription
     globals()['AudienceNameDescription'] = AudienceNameDescription
 
 
 class BasicAudienceDefinition(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/behavioral_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/behavioral_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class BehavioralV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_search_filters_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_search_filters_v23_q1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CampaignSearchFiltersV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_search_request_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_search_request_v23_q1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.campaign_search_filters_v23_q1 import CampaignSearchFiltersV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.campaign_search_filters_v23_q1 import CampaignSearchFiltersV23Q1
     globals()['CampaignSearchFiltersV23Q1'] = CampaignSearchFiltersV23Q1
 
 
 class CampaignSearchRequestV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_spend_limit_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_spend_limit_v23_q1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class CampaignSpendLimitV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.campaign_spend_limit_v23_q1 import CampaignSpendLimitV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.campaign_spend_limit_v23_q1 import CampaignSpendLimitV23Q1
     globals()['CampaignSpendLimitV23Q1'] = CampaignSpendLimitV23Q1
 
 
 class CampaignV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1_resource import CampaignV23Q1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1_resource import CampaignV23Q1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['CampaignV23Q1Resource'] = CampaignV23Q1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class CampaignV23Q1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1 import CampaignV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1 import CampaignV23Q1
     globals()['CampaignV23Q1'] = CampaignV23Q1
 
 
 class CampaignV23Q1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/campaign_v23_q1_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1_resource import CampaignV23Q1Resource
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1_resource import CampaignV23Q1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
     globals()['CampaignV23Q1Resource'] = CampaignV23Q1Resource
     globals()['CommonProblem'] = CommonProblem
 
 
 class CampaignV23Q1Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/common_problem.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/common_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CommonProblem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ContactListStatisticsEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.contact_list_statistics_entity_v1 import ContactListStatisticsEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.contact_list_statistics_entity_v1 import ContactListStatisticsEntityV1
     globals()['ContactListStatisticsEntityV1'] = ContactListStatisticsEntityV1
 
 
 class ContactListStatisticsEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contact_list_statistics_entity_v1_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.contact_list_statistics_entity_v1_resource import ContactListStatisticsEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.contact_list_statistics_entity_v1_resource import ContactListStatisticsEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
     globals()['ContactListStatisticsEntityV1Resource'] = ContactListStatisticsEntityV1Resource
 
 
 class ContactListStatisticsEntityV1Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contact_list_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contact_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ContactListV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
     globals()['ContactlistAmendmentAttributes'] = ContactlistAmendmentAttributes
 
 
 class ContactlistAmendment(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ContactlistAmendmentAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_amendment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.contactlist_amendment import ContactlistAmendment
+    from criteo_api_marketingsolutions_v2024_04.model.contactlist_amendment import ContactlistAmendment
     globals()['ContactlistAmendment'] = ContactlistAmendment
 
 
 class ContactlistAmendmentRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.contactlist_operation_attributes import ContactlistOperationAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.contactlist_operation_attributes import ContactlistOperationAttributes
     globals()['ContactlistOperationAttributes'] = ContactlistOperationAttributes
 
 
 class ContactlistOperation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/contactlist_operation_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ContactlistOperationAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.image_slide import ImageSlide
+    from criteo_api_marketingsolutions_v2024_04.model.image_slide import ImageSlide
     globals()['ImageSlide'] = ImageSlide
 
 
 class Coupon(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.coupon_resource import CouponResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.coupon_resource import CouponResource
     globals()['CommonProblem'] = CommonProblem
     globals()['CouponResource'] = CouponResource
 
 
 class CouponListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.coupon import Coupon
+    from criteo_api_marketingsolutions_v2024_04.model.coupon import Coupon
     globals()['Coupon'] = Coupon
 
 
 class CouponResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.coupon_resource import CouponResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.coupon_resource import CouponResource
     globals()['CommonProblem'] = CommonProblem
     globals()['CouponResource'] = CouponResource
 
 
 class CouponResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CouponSupportedSizes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.coupon_supported_sizes import CouponSupportedSizes
+    from criteo_api_marketingsolutions_v2024_04.model.coupon_supported_sizes import CouponSupportedSizes
     globals()['CouponSupportedSizes'] = CouponSupportedSizes
 
 
 class CouponSupportedSizesResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/coupon_supported_sizes_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.coupon_supported_sizes_resource import CouponSupportedSizesResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.coupon_supported_sizes_resource import CouponSupportedSizesResource
     globals()['CommonProblem'] = CommonProblem
     globals()['CouponSupportedSizesResource'] = CouponSupportedSizesResource
 
 
 class CouponSupportedSizesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_bidding import CreateAdSetBidding
-    from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_budget import CreateAdSetBudget
-    from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_schedule import CreateAdSetSchedule
-    from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_targeting import CreateAdSetTargeting
+    from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_bidding import CreateAdSetBidding
+    from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_budget import CreateAdSetBudget
+    from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_schedule import CreateAdSetSchedule
+    from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_targeting import CreateAdSetTargeting
     globals()['CreateAdSetBidding'] = CreateAdSetBidding
     globals()['CreateAdSetBudget'] = CreateAdSetBudget
     globals()['CreateAdSetSchedule'] = CreateAdSetSchedule
     globals()['CreateAdSetTargeting'] = CreateAdSetTargeting
 
 
 class CreateAdSet(ModelNormal):
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_bidding.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_bidding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CreateAdSetBidding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_budget.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CreateAdSetBudget(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_geo_location.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_geo_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting_rule import AdSetTargetingRule
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting_rule import AdSetTargetingRule
     globals()['AdSetTargetingRule'] = AdSetTargetingRule
 
 
 class CreateAdSetGeoLocation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_resource import CreateAdSetResource
+    from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_resource import CreateAdSetResource
     globals()['CreateAdSetResource'] = CreateAdSetResource
 
 
 class CreateAdSetRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_ad_set import CreateAdSet
+    from criteo_api_marketingsolutions_v2024_04.model.create_ad_set import CreateAdSet
     globals()['CreateAdSet'] = CreateAdSet
 
 
 class CreateAdSetResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_schedule.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CreateAdSetSchedule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_targeting.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_ad_set_targeting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_frequency_capping import AdSetFrequencyCapping
-    from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_geo_location import CreateAdSetGeoLocation
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_frequency_capping import AdSetFrequencyCapping
+    from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_geo_location import CreateAdSetGeoLocation
     globals()['AdSetDeliveryLimitations'] = AdSetDeliveryLimitations
     globals()['AdSetFrequencyCapping'] = AdSetFrequencyCapping
     globals()['CreateAdSetGeoLocation'] = CreateAdSetGeoLocation
 
 
 class CreateAdSetTargeting(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_campaign.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_campaign_spend_limit import CreateCampaignSpendLimit
+    from criteo_api_marketingsolutions_v2024_04.model.create_campaign_spend_limit import CreateCampaignSpendLimit
     globals()['CreateCampaignSpendLimit'] = CreateCampaignSpendLimit
 
 
 class CreateCampaign(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_campaign_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_campaign_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_campaign_resource import CreateCampaignResource
+    from criteo_api_marketingsolutions_v2024_04.model.create_campaign_resource import CreateCampaignResource
     globals()['CreateCampaignResource'] = CreateCampaignResource
 
 
 class CreateCampaignRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_campaign_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_result_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_campaign import CreateCampaign
-    globals()['CreateCampaign'] = CreateCampaign
 
-
-class CreateCampaignResource(ModelNormal):
+class PatchAdSetDisplayMultiplierResultResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,54 +62,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'attributes': (CreateCampaign,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attributes': 'attributes',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateCampaignResource - a model defined in OpenAPI
+        """PatchAdSetDisplayMultiplierResultResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +132,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (CreateCampaign): [optional]  # noqa: E501
+            id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -192,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CreateCampaignResource - a model defined in OpenAPI
+        """PatchAdSetDisplayMultiplierResultResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,15 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (CreateCampaign): [optional]  # noqa: E501
+            id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_campaign_spend_limit.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_campaign_spend_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CreateCampaignSpendLimit(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_coupon.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_coupon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_image_slide import CreateImageSlide
+    from criteo_api_marketingsolutions_v2024_04.model.create_image_slide import CreateImageSlide
     globals()['CreateImageSlide'] = CreateImageSlide
 
 
 class CreateCoupon(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_coupon_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_coupon_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_coupon_resource import CreateCouponResource
+    from criteo_api_marketingsolutions_v2024_04.model.create_coupon_resource import CreateCouponResource
     globals()['CreateCouponResource'] = CreateCouponResource
 
 
 class CreateCouponRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_coupon_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_coupon_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.create_coupon import CreateCoupon
+    from criteo_api_marketingsolutions_v2024_04.model.create_coupon import CreateCoupon
     globals()['CreateCoupon'] = CreateCoupon
 
 
 class CreateCouponResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/create_image_slide.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/create_image_slide.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CreateImageSlide(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.adaptive_attributes import AdaptiveAttributes
-    from criteo_api_marketingsolutions_v2024_01.model.dynamic_attributes import DynamicAttributes
-    from criteo_api_marketingsolutions_v2024_01.model.html_tag_attributes import HtmlTagAttributes
-    from criteo_api_marketingsolutions_v2024_01.model.image_attributes import ImageAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.adaptive_attributes import AdaptiveAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.dynamic_attributes import DynamicAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.html_tag_attributes import HtmlTagAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.image_attributes import ImageAttributes
     globals()['AdaptiveAttributes'] = AdaptiveAttributes
     globals()['DynamicAttributes'] = DynamicAttributes
     globals()['HtmlTagAttributes'] = HtmlTagAttributes
     globals()['ImageAttributes'] = ImageAttributes
 
 
 class Creative(ModelNormal):
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.creative_resource import CreativeResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.creative_resource import CreativeResource
     globals()['CommonProblem'] = CommonProblem
     globals()['CreativeResource'] = CreativeResource
 
 
 class CreativeListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.creative import Creative
+    from criteo_api_marketingsolutions_v2024_04.model.creative import Creative
     globals()['Creative'] = Creative
 
 
 class CreativeResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.creative_resource import CreativeResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.creative_resource import CreativeResource
     globals()['CommonProblem'] = CommonProblem
     globals()['CreativeResource'] = CreativeResource
 
 
 class CreativeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_write.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.adaptive_write_attributes import AdaptiveWriteAttributes
-    from criteo_api_marketingsolutions_v2024_01.model.dynamic_write_attributes import DynamicWriteAttributes
-    from criteo_api_marketingsolutions_v2024_01.model.html_tag_write_attributes import HtmlTagWriteAttributes
-    from criteo_api_marketingsolutions_v2024_01.model.image_write_attributes import ImageWriteAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.adaptive_write_attributes import AdaptiveWriteAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.dynamic_write_attributes import DynamicWriteAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.html_tag_write_attributes import HtmlTagWriteAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.image_write_attributes import ImageWriteAttributes
     globals()['AdaptiveWriteAttributes'] = AdaptiveWriteAttributes
     globals()['DynamicWriteAttributes'] = DynamicWriteAttributes
     globals()['HtmlTagWriteAttributes'] = HtmlTagWriteAttributes
     globals()['ImageWriteAttributes'] = ImageWriteAttributes
 
 
 class CreativeWrite(ModelNormal):
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_write_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_gender_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.creative_write_resource import CreativeWriteResource
-    globals()['CreativeWriteResource'] = CreativeWriteResource
 
-
-class CreativeWriteRequest(ModelNormal):
+class NillableGenderV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,63 +51,66 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('value',): {
+            'None': None,
+            'MALE': "Male",
+            'FEMALE': "Female",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (CreativeWriteResource,),  # noqa: E501
+            'value': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreativeWriteRequest - a model defined in OpenAPI
+        """NillableGenderV1 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (CreativeWriteResource): [optional]  # noqa: E501
+            value (str, none_type): The value. If missing or null the value is set to \"null\". [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CreativeWriteRequest - a model defined in OpenAPI
+        """NillableGenderV1 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +221,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (CreativeWriteResource): [optional]  # noqa: E501
+            value (str, none_type): The value. If missing or null the value is set to \"null\". [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/creative_write_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_write_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.creative_write import CreativeWrite
+    from criteo_api_marketingsolutions_v2024_04.model.creative_write import CreativeWrite
     globals()['CreativeWrite'] = CreativeWrite
 
 
 class CreativeWriteResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/criteo_api_error.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/criteo_api_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CriteoApiError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/criteo_api_warning.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/criteo_api_warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CriteoApiWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/delete_audience_contact_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/delete_audience_contact_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2024_01.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2024_01.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2024_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2024_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2024_04.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class DeleteAudienceContactListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/dynamic_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/dynamic_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.image_shape import ImageShape
+    from criteo_api_marketingsolutions_v2024_04.model.image_shape import ImageShape
     globals()['ImageShape'] = ImageShape
 
 
 class DynamicAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/dynamic_write_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/dynamic_write_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class DynamicWriteAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/entity_of_portfolio_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/entity_of_portfolio_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.portfolio_message import PortfolioMessage
+    from criteo_api_marketingsolutions_v2024_04.model.portfolio_message import PortfolioMessage
     globals()['PortfolioMessage'] = PortfolioMessage
 
 
 class EntityOfPortfolioMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/error_code_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/error_code_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2024_01.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2024_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2024_04.model.audience_warning import AudienceWarning
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
 
 
 class ErrorCodeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/get_portfolio_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/get_portfolio_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.criteo_api_error import CriteoApiError
-    from criteo_api_marketingsolutions_v2024_01.model.criteo_api_warning import CriteoApiWarning
-    from criteo_api_marketingsolutions_v2024_01.model.entity_of_portfolio_message import EntityOfPortfolioMessage
+    from criteo_api_marketingsolutions_v2024_04.model.criteo_api_error import CriteoApiError
+    from criteo_api_marketingsolutions_v2024_04.model.criteo_api_warning import CriteoApiWarning
+    from criteo_api_marketingsolutions_v2024_04.model.entity_of_portfolio_message import EntityOfPortfolioMessage
     globals()['CriteoApiError'] = CriteoApiError
     globals()['CriteoApiWarning'] = CriteoApiWarning
     globals()['EntityOfPortfolioMessage'] = EntityOfPortfolioMessage
 
 
 class GetPortfolioResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/html_tag_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/html_tag_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.tag import Tag
+    from criteo_api_marketingsolutions_v2024_04.model.tag import Tag
     globals()['Tag'] = Tag
 
 
 class HtmlTagAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/html_tag_write_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/html_tag_write_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.tag import Tag
+    from criteo_api_marketingsolutions_v2024_04.model.tag import Tag
     globals()['Tag'] = Tag
 
 
 class HtmlTagWriteAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ImageAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_set.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.image_shape import ImageShape
+    from criteo_api_marketingsolutions_v2024_04.model.image_shape import ImageShape
     globals()['ImageShape'] = ImageShape
 
 
 class ImageSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_set_base64.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_set_base64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ImageSetBase64(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_shape.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ImageShape(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_slide.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_slide.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ImageSlide(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/image_write_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/image_write_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ImageWriteAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class InMarketAudienceSegmentBrandEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_brand_entity_v1_resource import InMarketAudienceSegmentBrandEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_brand_entity_v1_resource import InMarketAudienceSegmentBrandEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
     globals()['InMarketAudienceSegmentBrandEntityV1Resource'] = InMarketAudienceSegmentBrandEntityV1Resource
 
 
 class InMarketAudienceSegmentBrandEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_brand_entity_v1_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_brand_entity_v1 import InMarketAudienceSegmentBrandEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_brand_entity_v1 import InMarketAudienceSegmentBrandEntityV1
     globals()['InMarketAudienceSegmentBrandEntityV1'] = InMarketAudienceSegmentBrandEntityV1
 
 
 class InMarketAudienceSegmentBrandEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class InMarketAudienceSegmentInterestEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_interest_entity_v1_resource import InMarketAudienceSegmentInterestEntityV1Resource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_interest_entity_v1_resource import InMarketAudienceSegmentInterestEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
     globals()['InMarketAudienceSegmentInterestEntityV1Resource'] = InMarketAudienceSegmentInterestEntityV1Resource
 
 
 class InMarketAudienceSegmentInterestEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_audience_segment_interest_entity_v1_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_interest_entity_v1 import InMarketAudienceSegmentInterestEntityV1
+    from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_interest_entity_v1 import InMarketAudienceSegmentInterestEntityV1
     globals()['InMarketAudienceSegmentInterestEntityV1'] = InMarketAudienceSegmentInterestEntityV1
 
 
 class InMarketAudienceSegmentInterestEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_create_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_create_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class InMarketCreateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_size_estimation_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_size_estimation_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class InMarketSizeEstimationV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_update_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_update_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_gender_v1 import NillableGenderV1
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_gender_v1 import NillableGenderV1
     globals()['NillableGenderV1'] = NillableGenderV1
 
 
 class InMarketUpdateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/in_market_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/in_market_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class InMarketV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/location_create_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/location_create_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.point_of_interest_v1 import PointOfInterestV1
+    from criteo_api_marketingsolutions_v2024_04.model.point_of_interest_v1 import PointOfInterestV1
     globals()['PointOfInterestV1'] = PointOfInterestV1
 
 
 class LocationCreateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/location_size_estimation_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/location_size_estimation_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.point_of_interest_v1 import PointOfInterestV1
+    from criteo_api_marketingsolutions_v2024_04.model.point_of_interest_v1 import PointOfInterestV1
     globals()['PointOfInterestV1'] = PointOfInterestV1
 
 
 class LocationSizeEstimationV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/location_update_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/location_update_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.point_of_interest_v1 import PointOfInterestV1
+    from criteo_api_marketingsolutions_v2024_04.model.point_of_interest_v1 import PointOfInterestV1
     globals()['PointOfInterestV1'] = PointOfInterestV1
 
 
 class LocationUpdateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/location_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/location_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.point_of_interest_v1 import PointOfInterestV1
+    from criteo_api_marketingsolutions_v2024_04.model.point_of_interest_v1 import PointOfInterestV1
     globals()['PointOfInterestV1'] = PointOfInterestV1
 
 
 class LocationV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/lookalike_create_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/lookalike_create_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class LookalikeCreateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/lookalike_update_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/lookalike_update_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class LookalikeUpdateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/lookalike_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/lookalike_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class LookalikeV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/modify_audience_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/modify_audience_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2024_01.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2024_01.model.contactlist_operation import ContactlistOperation
+    from criteo_api_marketingsolutions_v2024_04.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2024_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2024_04.model.contactlist_operation import ContactlistOperation
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['ContactlistOperation'] = ContactlistOperation
 
 
 class ModifyAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
     globals()['NillableAdSetTargetingRuleValue'] = NillableAdSetTargetingRuleValue
 
 
 class NillableAdSetTargetingRule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_v23_q1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_ad_set_targeting_rule_v23_q1_value import NillableAdSetTargetingRuleV23Q1Value
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_ad_set_targeting_rule_v23_q1_value import NillableAdSetTargetingRuleV23Q1Value
     globals()['NillableAdSetTargetingRuleV23Q1Value'] = NillableAdSetTargetingRuleV23Q1Value
 
 
 class NillableAdSetTargetingRuleV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1_value.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_v23_q1_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting_rule_v23_q1 import AdSetTargetingRuleV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting_rule_v23_q1 import AdSetTargetingRuleV23Q1
     globals()['AdSetTargetingRuleV23Q1'] = AdSetTargetingRuleV23Q1
 
 
 class NillableAdSetTargetingRuleV23Q1Value(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_value.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_ad_set_targeting_rule_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting_rule import AdSetTargetingRule
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting_rule import AdSetTargetingRule
     globals()['AdSetTargetingRule'] = AdSetTargetingRule
 
 
 class NillableAdSetTargetingRuleValue(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_date_time.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_date_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class NillableDateTime(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_decimal.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_decimal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class NillableDecimal(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_gender_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_int32.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
-class NillableGenderV1(ModelNormal):
+class NillableInt32(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,19 +51,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'None': None,
-            'MALE': "Male",
-            'FEMALE': "Female",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -82,15 +77,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str, none_type,),  # noqa: E501
+            'value': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -102,15 +97,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """NillableGenderV1 - a model defined in OpenAPI
+        """NillableInt32 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str, none_type): The value. If missing or null the value is set to \"null\". [optional]  # noqa: E501
+            value (int, none_type): The value. If missing or null the value is set to \"null\". [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """NillableGenderV1 - a model defined in OpenAPI
+        """NillableInt32 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str, none_type): The value. If missing or null the value is set to \"null\". [optional]  # noqa: E501
+            value (int, none_type): The value. If missing or null the value is set to \"null\". [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_int32.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/nillable_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
-class NillableInt32(ModelNormal):
+class NillableString(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,15 +77,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (int, none_type,),  # noqa: E501
+            'value': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -97,15 +97,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """NillableInt32 - a model defined in OpenAPI
+        """NillableString - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (int, none_type): The value. If missing or null the value is set to \"null\". [optional]  # noqa: E501
+            value (str, none_type): The string's value. If missing or null the string's value is set to \"null\". [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """NillableInt32 - a model defined in OpenAPI
+        """NillableString - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (int, none_type): The value. If missing or null the value is set to \"null\". [optional]  # noqa: E501
+            value (str, none_type): The string's value. If missing or null the string's value is set to \"null\". [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/nillable_string.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/creative_write_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_marketingsolutions_v2024_04.model.creative_write_resource import CreativeWriteResource
+    globals()['CreativeWriteResource'] = CreativeWriteResource
 
-class NillableString(ModelNormal):
+
+class CreativeWriteRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,50 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'value': (str, none_type,),  # noqa: E501
+            'data': (CreativeWriteResource,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'value': 'value',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """NillableString - a model defined in OpenAPI
+        """CreativeWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str, none_type): The string's value. If missing or null the string's value is set to \"null\". [optional]  # noqa: E501
+            data (CreativeWriteResource): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """NillableString - a model defined in OpenAPI
+        """CreativeWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str, none_type): The string's value. If missing or null the string's value is set to \"null\". [optional]  # noqa: E501
+            data (CreativeWriteResource): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting import AdSetTargeting
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_bidding import PatchAdSetBidding
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_budget import PatchAdSetBudget
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_scheduling import PatchAdSetScheduling
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting import AdSetTargeting
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_bidding import PatchAdSetBidding
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_budget import PatchAdSetBudget
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_scheduling import PatchAdSetScheduling
     globals()['AdSetTargeting'] = AdSetTargeting
     globals()['PatchAdSetBidding'] = PatchAdSetBidding
     globals()['PatchAdSetBudget'] = PatchAdSetBudget
     globals()['PatchAdSetScheduling'] = PatchAdSetScheduling
 
 
 class PatchAdSet(ModelNormal):
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_bidding.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchAdSetBidding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_budget.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_budget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchAdSetBudget(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetCategoryBid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_list_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_list_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
     globals()['PatchAdSetCategoryBidResource'] = PatchAdSetCategoryBidResource
 
 
 class PatchAdSetCategoryBidListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
     globals()['PatchAdSetCategoryBid'] = PatchAdSetCategoryBid
 
 
 class PatchAdSetCategoryBidResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_result_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
     globals()['CommonProblem'] = CommonProblem
     globals()['PatchAdSetCategoryBidResultResource'] = PatchAdSetCategoryBidResultResource
 
 
 class PatchAdSetCategoryBidResultListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_category_bid_result_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetCategoryBidResultResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetDisplayMultiplier(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_list_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_list_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
     globals()['PatchAdSetDisplayMultiplierResource'] = PatchAdSetDisplayMultiplierResource
 
 
 class PatchAdSetDisplayMultiplierListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
     globals()['PatchAdSetDisplayMultiplier'] = PatchAdSetDisplayMultiplier
 
 
 class PatchAdSetDisplayMultiplierResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_display_multiplier_result_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
     globals()['CommonProblem'] = CommonProblem
     globals()['PatchAdSetDisplayMultiplierResultResource'] = PatchAdSetDisplayMultiplierResultResource
 
 
 class PatchAdSetDisplayMultiplierResultListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_result_campaign_read_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
-class PatchAdSetDisplayMultiplierResultResource(ModelNormal):
+class PatchResultCampaignReadResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -92,22 +92,24 @@
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
+        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchAdSetDisplayMultiplierResultResource - a model defined in OpenAPI
+        """PatchResultCampaignReadResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,15 +135,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchAdSetDisplayMultiplierResultResource - a model defined in OpenAPI
+        """PatchResultCampaignReadResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,15 +222,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_scheduling.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_ad_set_scheduling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_date_time import NillableDateTime
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_date_time import NillableDateTime
     globals()['NillableDateTime'] = NillableDateTime
 
 
 class PatchAdSetScheduling(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_campaign.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
+    from criteo_api_marketingsolutions_v2024_04.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
     globals()['PatchCampaignSpendLimit'] = PatchCampaignSpendLimit
 
 
 class PatchCampaign(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_list_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_campaign_list_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.patch_campaign_write_resource import PatchCampaignWriteResource
+    from criteo_api_marketingsolutions_v2024_04.model.patch_campaign_write_resource import PatchCampaignWriteResource
     globals()['PatchCampaignWriteResource'] = PatchCampaignWriteResource
 
 
 class PatchCampaignListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_spend_limit.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_campaign_spend_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchCampaignSpendLimit(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_write_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_campaign_write_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.patch_campaign import PatchCampaign
+    from criteo_api_marketingsolutions_v2024_04.model.patch_campaign import PatchCampaign
     globals()['PatchCampaign'] = PatchCampaign
 
 
 class PatchCampaignWriteResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_list_response.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/patch_result_campaign_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
     globals()['CommonProblem'] = CommonProblem
     globals()['PatchResultCampaignReadResource'] = PatchResultCampaignReadResource
 
 
 class PatchResultCampaignListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_read_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/write_model_patch_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set import PatchAdSet
+    globals()['PatchAdSet'] = PatchAdSet
 
-class PatchResultCampaignReadResource(ModelNormal):
+
+class WriteModelPatchAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,54 +66,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
+            'attributes': (PatchAdSet,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
-        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchResultCampaignReadResource - a model defined in OpenAPI
+        """WriteModelPatchAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +141,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): [optional]  # noqa: E501
+            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (PatchAdSet): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchResultCampaignReadResource - a model defined in OpenAPI
+        """WriteModelPatchAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +229,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): [optional]  # noqa: E501
+            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (PatchAdSet): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_data_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/placements_report_query_data_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
+    from criteo_api_marketingsolutions_v2024_04.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
     globals()['PlacementsReportQueryEntityMessage'] = PlacementsReportQueryEntityMessage
 
 
 class PlacementsReportQueryDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_entity_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/placements_report_query_entity_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.placements_report_query_message import PlacementsReportQueryMessage
+    from criteo_api_marketingsolutions_v2024_04.model.placements_report_query_message import PlacementsReportQueryMessage
     globals()['PlacementsReportQueryMessage'] = PlacementsReportQueryMessage
 
 
 class PlacementsReportQueryEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/placements_report_query_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class PlacementsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/point_of_interest_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/point_of_interest_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class PointOfInterestV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/portfolio_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/portfolio_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class PortfolioMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/problem_details.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ProblemDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/problems_details.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/problems_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2024_04.model.problem_details import ProblemDetails
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class ProblemsDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/prospecting_create_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/prospecting_create_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ProspectingCreateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/prospecting_update_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/prospecting_update_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_int32 import NillableInt32
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_int32 import NillableInt32
     globals()['NillableInt32'] = NillableInt32
 
 
 class ProspectingUpdateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/prospecting_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/prospecting_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ProspectingV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting import AdSetTargeting
-    from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_bidding import ReadAdSetBidding
-    from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_budget import ReadAdSetBudget
-    from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_schedule import ReadAdSetSchedule
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting import AdSetTargeting
+    from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_bidding import ReadAdSetBidding
+    from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_budget import ReadAdSetBudget
+    from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_schedule import ReadAdSetSchedule
     globals()['AdSetTargeting'] = AdSetTargeting
     globals()['ReadAdSetBidding'] = ReadAdSetBidding
     globals()['ReadAdSetBudget'] = ReadAdSetBudget
     globals()['ReadAdSetSchedule'] = ReadAdSetSchedule
 
 
 class ReadAdSet(ModelNormal):
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_bidding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class ReadAdSetBidding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_bidding_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class ReadAdSetBiddingV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_budget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class ReadAdSetBudget(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_budget_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class ReadAdSetBudgetV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_date_time import NillableDateTime
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_date_time import NillableDateTime
     globals()['NillableDateTime'] = NillableDateTime
 
 
 class ReadAdSetSchedule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_schedule_v23_q1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.nillable_date_time import NillableDateTime
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_date_time import NillableDateTime
     globals()['NillableDateTime'] = NillableDateTime
 
 
 class ReadAdSetScheduleV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_ad_set_v23_q1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting_v23_q1 import AdSetTargetingV23Q1
-    from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_bidding_v23_q1 import ReadAdSetBiddingV23Q1
-    from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_budget_v23_q1 import ReadAdSetBudgetV23Q1
-    from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_schedule_v23_q1 import ReadAdSetScheduleV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting_v23_q1 import AdSetTargetingV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_bidding_v23_q1 import ReadAdSetBiddingV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_budget_v23_q1 import ReadAdSetBudgetV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_schedule_v23_q1 import ReadAdSetScheduleV23Q1
     globals()['AdSetTargetingV23Q1'] = AdSetTargetingV23Q1
     globals()['ReadAdSetBiddingV23Q1'] = ReadAdSetBiddingV23Q1
     globals()['ReadAdSetBudgetV23Q1'] = ReadAdSetBudgetV23Q1
     globals()['ReadAdSetScheduleV23Q1'] = ReadAdSetScheduleV23Q1
 
 
 class ReadAdSetV23Q1(ModelNormal):
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_model_ad_set_id.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_model_ad_set_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ReadModelAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_model_read_ad_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.read_ad_set import ReadAdSet
+    from criteo_api_marketingsolutions_v2024_04.model.read_ad_set import ReadAdSet
     globals()['ReadAdSet'] = ReadAdSet
 
 
 class ReadModelReadAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/read_model_read_ad_set_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_v23_q1 import ReadAdSetV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_v23_q1 import ReadAdSetV23Q1
     globals()['ReadAdSetV23Q1'] = ReadAdSetV23Q1
 
 
 class ReadModelReadAdSetV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/requests_ad_set_id.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/requests_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.write_model_ad_set_id import WriteModelAdSetId
+    from criteo_api_marketingsolutions_v2024_04.model.write_model_ad_set_id import WriteModelAdSetId
     globals()['WriteModelAdSetId'] = WriteModelAdSetId
 
 
 class RequestsAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/requests_patch_ad_set.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/requests_patch_ad_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.write_model_patch_ad_set import WriteModelPatchAdSet
+    from criteo_api_marketingsolutions_v2024_04.model.write_model_patch_ad_set import WriteModelPatchAdSet
     globals()['WriteModelPatchAdSet'] = WriteModelPatchAdSet
 
 
 class RequestsPatchAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/response_read_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.read_model_read_ad_set import ReadModelReadAdSet
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.read_model_read_ad_set import ReadModelReadAdSet
     globals()['CommonProblem'] = CommonProblem
     globals()['ReadModelReadAdSet'] = ReadModelReadAdSet
 
 
 class ResponseReadAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/response_read_ad_set_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.read_model_read_ad_set_v23_q1 import ReadModelReadAdSetV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.read_model_read_ad_set_v23_q1 import ReadModelReadAdSetV23Q1
     globals()['CommonProblem'] = CommonProblem
     globals()['ReadModelReadAdSetV23Q1'] = ReadModelReadAdSetV23Q1
 
 
 class ResponseReadAdSetV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/responses_ad_set_id.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/responses_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.read_model_ad_set_id import ReadModelAdSetId
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.read_model_ad_set_id import ReadModelAdSetId
     globals()['CommonProblem'] = CommonProblem
     globals()['ReadModelAdSetId'] = ReadModelAdSetId
 
 
 class ResponsesAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/responses_read_ad_set_v23_q1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/responses_read_ad_set_v23_q1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_marketingsolutions_v2024_01.model.read_model_read_ad_set_v23_q1 import ReadModelReadAdSetV23Q1
+    from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2024_04.model.read_model_read_ad_set_v23_q1 import ReadModelReadAdSetV23Q1
     globals()['CommonProblem'] = CommonProblem
     globals()['ReadModelReadAdSetV23Q1'] = ReadModelReadAdSetV23Q1
 
 
 class ResponsesReadAdSetV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/retargeting_create_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/retargeting_create_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RetargetingCreateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/retargeting_update_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/retargeting_update_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RetargetingUpdateV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/retargeting_v1.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/retargeting_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RetargetingV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/size.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/size.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class Size(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/statistics_report_query_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/statistics_report_query_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class StatisticsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/tag.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.size import Size
+    from criteo_api_marketingsolutions_v2024_04.model.size import Size
     globals()['Size'] = Size
 
 
 class Tag(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_data_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_data_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
+    from criteo_api_marketingsolutions_v2024_04.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
     globals()['TransactionsReportQueryEntityMessage'] = TransactionsReportQueryEntityMessage
 
 
 class TransactionsReportQueryDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_entity_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_entity_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.transactions_report_query_message import TransactionsReportQueryMessage
+    from criteo_api_marketingsolutions_v2024_04.model.transactions_report_query_message import TransactionsReportQueryMessage
     globals()['TransactionsReportQueryMessage'] = TransactionsReportQueryMessage
 
 
 class TransactionsReportQueryEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transactions_report_query_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class TransactionsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_query_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_query_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class TransparencyQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_report_attributes.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_report_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.transparency_report_file import TransparencyReportFile
+    from criteo_api_marketingsolutions_v2024_04.model.transparency_report_file import TransparencyReportFile
     globals()['TransparencyReportFile'] = TransparencyReportFile
 
 
 class TransparencyReportAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_report_data_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_report_data_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.transparency_report_entity_message import TransparencyReportEntityMessage
+    from criteo_api_marketingsolutions_v2024_04.model.transparency_report_entity_message import TransparencyReportEntityMessage
     globals()['TransparencyReportEntityMessage'] = TransparencyReportEntityMessage
 
 
 class TransparencyReportDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_report_entity_message.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_report_entity_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.transparency_report_attributes import TransparencyReportAttributes
+    from criteo_api_marketingsolutions_v2024_04.model.transparency_report_attributes import TransparencyReportAttributes
     globals()['TransparencyReportAttributes'] = TransparencyReportAttributes
 
 
 class TransparencyReportEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/transparency_report_file.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/transparency_report_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class TransparencyReportFile(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/update_coupon.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/update_coupon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class UpdateCoupon(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/update_coupon_request.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/update_coupon_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.update_coupon_resource import UpdateCouponResource
+    from criteo_api_marketingsolutions_v2024_04.model.update_coupon_resource import UpdateCouponResource
     globals()['UpdateCouponResource'] = UpdateCouponResource
 
 
 class UpdateCouponRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/update_coupon_resource.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/update_coupon_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.update_coupon import UpdateCoupon
+    from criteo_api_marketingsolutions_v2024_04.model.update_coupon import UpdateCoupon
     globals()['UpdateCoupon'] = UpdateCoupon
 
 
 class UpdateCouponResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/video_detail.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/video_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class VideoDetail(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/write_model_ad_set_id.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/write_model_ad_set_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 
 class WriteModelAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model/write_model_patch_ad_set.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model/audience_update_entity_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2024_04.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set import PatchAdSet
-    globals()['PatchAdSet'] = PatchAdSet
+    from criteo_api_marketingsolutions_v2024_04.model.algebra_node_v1 import AlgebraNodeV1
+    from criteo_api_marketingsolutions_v2024_04.model.nillable_string import NillableString
+    globals()['AlgebraNodeV1'] = AlgebraNodeV1
+    globals()['NillableString'] = NillableString
 
 
-class WriteModelPatchAdSet(ModelNormal):
+class AudienceUpdateEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,39 +85,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, none_type,),  # noqa: E501
-            'type': (str, none_type,),  # noqa: E501
-            'attributes': (PatchAdSet,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'description': (NillableString,),  # noqa: E501
+            'algebra': (AlgebraNodeV1,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'algebra': 'algebra',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WriteModelPatchAdSet - a model defined in OpenAPI
+        """AudienceUpdateEntityV1 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +142,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (PatchAdSet): [optional]  # noqa: E501
+            name (str, none_type): Name of the audience. [optional]  # noqa: E501
+            description (NillableString): [optional]  # noqa: E501
+            algebra (AlgebraNodeV1): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +197,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WriteModelPatchAdSet - a model defined in OpenAPI
+        """AudienceUpdateEntityV1 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +230,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (PatchAdSet): [optional]  # noqa: E501
+            name (str, none_type): Name of the audience. [optional]  # noqa: E501
+            description (NillableString): [optional]  # noqa: E501
+            algebra (AlgebraNodeV1): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/model_utils.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
@@ -16,15 +16,15 @@
 import pprint
 import re
 import tempfile
 import uuid
 
 from dateutil.parser import parse
 
-from criteo_api_marketingsolutions_v2024_01.exceptions import (
+from criteo_api_marketingsolutions_v2024_04.exceptions import (
     ApiKeyError,
     ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/models/__init__.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,267 +1,267 @@
 # flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
-# from criteo_api_marketingsolutions_v2024_01.model.pet import Pet
+# from criteo_api_marketingsolutions_v2024_04.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from criteo_api_marketingsolutions_v2024_01.model.ad import Ad
-from criteo_api_marketingsolutions_v2024_01.model.ad_list_response import AdListResponse
-from criteo_api_marketingsolutions_v2024_01.model.ad_resource import AdResource
-from criteo_api_marketingsolutions_v2024_01.model.ad_response import AdResponse
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_entity_v1 import AdSetAudienceLinkEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_entity_v1_resource import AdSetAudienceLinkEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_entity_v1_response import AdSetAudienceLinkEntityV1Response
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_audience_link_input_entity_v1 import AdSetAudienceLinkInputEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_category_bid import AdSetCategoryBid
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_category_bid_resource import AdSetCategoryBidResource
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_delivery_limitations_v23_q1 import AdSetDeliveryLimitationsV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_display_multiplier import AdSetDisplayMultiplier
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_frequency_capping import AdSetFrequencyCapping
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_frequency_capping_v23_q1 import AdSetFrequencyCappingV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_geo_location import AdSetGeoLocation
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_geo_location_v23_q1 import AdSetGeoLocationV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_search_filter_v23_q1 import AdSetSearchFilterV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_search_request_v23_q1 import AdSetSearchRequestV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting import AdSetTargeting
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting_rule import AdSetTargetingRule
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting_rule_v23_q1 import AdSetTargetingRuleV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.ad_set_targeting_v23_q1 import AdSetTargetingV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.ad_write import AdWrite
-from criteo_api_marketingsolutions_v2024_01.model.ad_write_request import AdWriteRequest
-from criteo_api_marketingsolutions_v2024_01.model.ad_write_resource import AdWriteResource
-from criteo_api_marketingsolutions_v2024_01.model.adaptive_attributes import AdaptiveAttributes
-from criteo_api_marketingsolutions_v2024_01.model.adaptive_colors import AdaptiveColors
-from criteo_api_marketingsolutions_v2024_01.model.adaptive_write_attributes import AdaptiveWriteAttributes
-from criteo_api_marketingsolutions_v2024_01.model.algebra_node_v1 import AlgebraNodeV1
-from criteo_api_marketingsolutions_v2024_01.model.application_summary_model import ApplicationSummaryModel
-from criteo_api_marketingsolutions_v2024_01.model.application_summary_model_resource import ApplicationSummaryModelResource
-from criteo_api_marketingsolutions_v2024_01.model.application_summary_model_response import ApplicationSummaryModelResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_bulk_create_input_v1 import AudienceBulkCreateInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_bulk_delete_input_v1 import AudienceBulkDeleteInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_bulk_update_input_v1 import AudienceBulkUpdateInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_compute_size_entity_v1_resource import AudienceComputeSizeEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_compute_sizes_input_v1 import AudienceComputeSizesInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_create_entity_v1 import AudienceCreateEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_create_entity_v1_resource import AudienceCreateEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_delete_entity_v1_resource import AudienceDeleteEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1 import AudienceEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1_audience_search_metadata_v1_list_response import AudienceEntityV1AudienceSearchMetadataV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1_list_response import AudienceEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_entity_v1_resource import AudienceEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_error import AudienceError
-from criteo_api_marketingsolutions_v2024_01.model.audience_estimate_size_entity_v1 import AudienceEstimateSizeEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_estimate_size_entity_v1_resource import AudienceEstimateSizeEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_estimate_size_input_v1 import AudienceEstimateSizeInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_id_entity_v1_list_response import AudienceIdEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_id_entity_v1_resource import AudienceIdEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_name_description import AudienceNameDescription
-from criteo_api_marketingsolutions_v2024_01.model.audience_search_entity_v1 import AudienceSearchEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_search_entity_v1_resource import AudienceSearchEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_search_input_v1 import AudienceSearchInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_search_metadata_v1 import AudienceSearchMetadataV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_bulk_create_input_v1 import AudienceSegmentBulkCreateInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_bulk_delete_input_v1 import AudienceSegmentBulkDeleteInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_bulk_update_input_v1 import AudienceSegmentBulkUpdateInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_compute_size_entity_v1_resource import AudienceSegmentComputeSizeEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_compute_sizes_input_v1 import AudienceSegmentComputeSizesInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_create_entity_v1 import AudienceSegmentCreateEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_create_entity_v1_resource import AudienceSegmentCreateEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_delete_entity_v1_resource import AudienceSegmentDeleteEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1 import AudienceSegmentEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response import AudienceSegmentEntityV1AudienceSegmentSearchMetadataV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1_list_response import AudienceSegmentEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_entity_v1_resource import AudienceSegmentEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_estimate_size_input_v1 import AudienceSegmentEstimateSizeInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_id_entity_v1_list_response import AudienceSegmentIdEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_id_entity_v1_resource import AudienceSegmentIdEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_search_entity_v1 import AudienceSegmentSearchEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_search_entity_v1_resource import AudienceSegmentSearchEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_search_input_v1 import AudienceSegmentSearchInputV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_search_metadata_v1 import AudienceSegmentSearchMetadataV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_entity_v1 import AudienceSegmentSizeEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_entity_v1_list_response import AudienceSegmentSizeEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_entity_v1_resource import AudienceSegmentSizeEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_entity_v1 import AudienceSegmentSizeEstimationEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_entity_v1_resource import AudienceSegmentSizeEstimationEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_v1 import AudienceSegmentSizeEstimationV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_v1_resource import AudienceSegmentSizeEstimationV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_size_estimation_v1_response import AudienceSegmentSizeEstimationV1Response
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_update_entity_v1 import AudienceSegmentUpdateEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_segment_update_entity_v1_resource import AudienceSegmentUpdateEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_size_entity_v1 import AudienceSizeEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_size_entity_v1_list_response import AudienceSizeEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.audience_size_entity_v1_resource import AudienceSizeEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_size_estimation_v1 import AudienceSizeEstimationV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_size_estimation_v1_resource import AudienceSizeEstimationV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_size_estimation_v1_response import AudienceSizeEstimationV1Response
-from criteo_api_marketingsolutions_v2024_01.model.audience_update_entity_v1 import AudienceUpdateEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.audience_update_entity_v1_resource import AudienceUpdateEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.audience_warning import AudienceWarning
-from criteo_api_marketingsolutions_v2024_01.model.basic_audience_definition import BasicAudienceDefinition
-from criteo_api_marketingsolutions_v2024_01.model.behavioral_v1 import BehavioralV1
-from criteo_api_marketingsolutions_v2024_01.model.campaign_search_filters_v23_q1 import CampaignSearchFiltersV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.campaign_search_request_v23_q1 import CampaignSearchRequestV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.campaign_spend_limit_v23_q1 import CampaignSpendLimitV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1 import CampaignV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1_list_response import CampaignV23Q1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1_resource import CampaignV23Q1Resource
-from criteo_api_marketingsolutions_v2024_01.model.campaign_v23_q1_response import CampaignV23Q1Response
-from criteo_api_marketingsolutions_v2024_01.model.common_problem import CommonProblem
-from criteo_api_marketingsolutions_v2024_01.model.contact_list_statistics_entity_v1 import ContactListStatisticsEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.contact_list_statistics_entity_v1_resource import ContactListStatisticsEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.contact_list_statistics_entity_v1_response import ContactListStatisticsEntityV1Response
-from criteo_api_marketingsolutions_v2024_01.model.contact_list_v1 import ContactListV1
-from criteo_api_marketingsolutions_v2024_01.model.contactlist_amendment import ContactlistAmendment
-from criteo_api_marketingsolutions_v2024_01.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
-from criteo_api_marketingsolutions_v2024_01.model.contactlist_amendment_request import ContactlistAmendmentRequest
-from criteo_api_marketingsolutions_v2024_01.model.contactlist_operation import ContactlistOperation
-from criteo_api_marketingsolutions_v2024_01.model.contactlist_operation_attributes import ContactlistOperationAttributes
-from criteo_api_marketingsolutions_v2024_01.model.coupon import Coupon
-from criteo_api_marketingsolutions_v2024_01.model.coupon_list_response import CouponListResponse
-from criteo_api_marketingsolutions_v2024_01.model.coupon_resource import CouponResource
-from criteo_api_marketingsolutions_v2024_01.model.coupon_response import CouponResponse
-from criteo_api_marketingsolutions_v2024_01.model.coupon_supported_sizes import CouponSupportedSizes
-from criteo_api_marketingsolutions_v2024_01.model.coupon_supported_sizes_resource import CouponSupportedSizesResource
-from criteo_api_marketingsolutions_v2024_01.model.coupon_supported_sizes_response import CouponSupportedSizesResponse
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set import CreateAdSet
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_bidding import CreateAdSetBidding
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_budget import CreateAdSetBudget
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_geo_location import CreateAdSetGeoLocation
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_request import CreateAdSetRequest
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_resource import CreateAdSetResource
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_schedule import CreateAdSetSchedule
-from criteo_api_marketingsolutions_v2024_01.model.create_ad_set_targeting import CreateAdSetTargeting
-from criteo_api_marketingsolutions_v2024_01.model.create_campaign import CreateCampaign
-from criteo_api_marketingsolutions_v2024_01.model.create_campaign_request import CreateCampaignRequest
-from criteo_api_marketingsolutions_v2024_01.model.create_campaign_resource import CreateCampaignResource
-from criteo_api_marketingsolutions_v2024_01.model.create_campaign_spend_limit import CreateCampaignSpendLimit
-from criteo_api_marketingsolutions_v2024_01.model.create_coupon import CreateCoupon
-from criteo_api_marketingsolutions_v2024_01.model.create_coupon_request import CreateCouponRequest
-from criteo_api_marketingsolutions_v2024_01.model.create_coupon_resource import CreateCouponResource
-from criteo_api_marketingsolutions_v2024_01.model.create_image_slide import CreateImageSlide
-from criteo_api_marketingsolutions_v2024_01.model.creative import Creative
-from criteo_api_marketingsolutions_v2024_01.model.creative_list_response import CreativeListResponse
-from criteo_api_marketingsolutions_v2024_01.model.creative_resource import CreativeResource
-from criteo_api_marketingsolutions_v2024_01.model.creative_response import CreativeResponse
-from criteo_api_marketingsolutions_v2024_01.model.creative_write import CreativeWrite
-from criteo_api_marketingsolutions_v2024_01.model.creative_write_request import CreativeWriteRequest
-from criteo_api_marketingsolutions_v2024_01.model.creative_write_resource import CreativeWriteResource
-from criteo_api_marketingsolutions_v2024_01.model.criteo_api_error import CriteoApiError
-from criteo_api_marketingsolutions_v2024_01.model.criteo_api_warning import CriteoApiWarning
-from criteo_api_marketingsolutions_v2024_01.model.delete_audience_contact_list_response import DeleteAudienceContactListResponse
-from criteo_api_marketingsolutions_v2024_01.model.dynamic_attributes import DynamicAttributes
-from criteo_api_marketingsolutions_v2024_01.model.dynamic_write_attributes import DynamicWriteAttributes
-from criteo_api_marketingsolutions_v2024_01.model.entity_of_portfolio_message import EntityOfPortfolioMessage
-from criteo_api_marketingsolutions_v2024_01.model.error_code_response import ErrorCodeResponse
-from criteo_api_marketingsolutions_v2024_01.model.get_portfolio_response import GetPortfolioResponse
-from criteo_api_marketingsolutions_v2024_01.model.html_tag_attributes import HtmlTagAttributes
-from criteo_api_marketingsolutions_v2024_01.model.html_tag_write_attributes import HtmlTagWriteAttributes
-from criteo_api_marketingsolutions_v2024_01.model.image_attributes import ImageAttributes
-from criteo_api_marketingsolutions_v2024_01.model.image_set import ImageSet
-from criteo_api_marketingsolutions_v2024_01.model.image_set_base64 import ImageSetBase64
-from criteo_api_marketingsolutions_v2024_01.model.image_shape import ImageShape
-from criteo_api_marketingsolutions_v2024_01.model.image_slide import ImageSlide
-from criteo_api_marketingsolutions_v2024_01.model.image_write_attributes import ImageWriteAttributes
-from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_brand_entity_v1 import InMarketAudienceSegmentBrandEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_brand_entity_v1_list_response import InMarketAudienceSegmentBrandEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_brand_entity_v1_resource import InMarketAudienceSegmentBrandEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_interest_entity_v1 import InMarketAudienceSegmentInterestEntityV1
-from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_interest_entity_v1_list_response import InMarketAudienceSegmentInterestEntityV1ListResponse
-from criteo_api_marketingsolutions_v2024_01.model.in_market_audience_segment_interest_entity_v1_resource import InMarketAudienceSegmentInterestEntityV1Resource
-from criteo_api_marketingsolutions_v2024_01.model.in_market_create_v1 import InMarketCreateV1
-from criteo_api_marketingsolutions_v2024_01.model.in_market_size_estimation_v1 import InMarketSizeEstimationV1
-from criteo_api_marketingsolutions_v2024_01.model.in_market_update_v1 import InMarketUpdateV1
-from criteo_api_marketingsolutions_v2024_01.model.in_market_v1 import InMarketV1
-from criteo_api_marketingsolutions_v2024_01.model.location_create_v1 import LocationCreateV1
-from criteo_api_marketingsolutions_v2024_01.model.location_size_estimation_v1 import LocationSizeEstimationV1
-from criteo_api_marketingsolutions_v2024_01.model.location_update_v1 import LocationUpdateV1
-from criteo_api_marketingsolutions_v2024_01.model.location_v1 import LocationV1
-from criteo_api_marketingsolutions_v2024_01.model.lookalike_create_v1 import LookalikeCreateV1
-from criteo_api_marketingsolutions_v2024_01.model.lookalike_update_v1 import LookalikeUpdateV1
-from criteo_api_marketingsolutions_v2024_01.model.lookalike_v1 import LookalikeV1
-from criteo_api_marketingsolutions_v2024_01.model.modify_audience_response import ModifyAudienceResponse
-from criteo_api_marketingsolutions_v2024_01.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
-from criteo_api_marketingsolutions_v2024_01.model.nillable_ad_set_targeting_rule_v23_q1 import NillableAdSetTargetingRuleV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.nillable_ad_set_targeting_rule_v23_q1_value import NillableAdSetTargetingRuleV23Q1Value
-from criteo_api_marketingsolutions_v2024_01.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
-from criteo_api_marketingsolutions_v2024_01.model.nillable_date_time import NillableDateTime
-from criteo_api_marketingsolutions_v2024_01.model.nillable_decimal import NillableDecimal
-from criteo_api_marketingsolutions_v2024_01.model.nillable_gender_v1 import NillableGenderV1
-from criteo_api_marketingsolutions_v2024_01.model.nillable_int32 import NillableInt32
-from criteo_api_marketingsolutions_v2024_01.model.nillable_string import NillableString
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set import PatchAdSet
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_bidding import PatchAdSetBidding
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_budget import PatchAdSetBudget
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
-from criteo_api_marketingsolutions_v2024_01.model.patch_ad_set_scheduling import PatchAdSetScheduling
-from criteo_api_marketingsolutions_v2024_01.model.patch_campaign import PatchCampaign
-from criteo_api_marketingsolutions_v2024_01.model.patch_campaign_list_request import PatchCampaignListRequest
-from criteo_api_marketingsolutions_v2024_01.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
-from criteo_api_marketingsolutions_v2024_01.model.patch_campaign_write_resource import PatchCampaignWriteResource
-from criteo_api_marketingsolutions_v2024_01.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
-from criteo_api_marketingsolutions_v2024_01.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
-from criteo_api_marketingsolutions_v2024_01.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2024_01.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
-from criteo_api_marketingsolutions_v2024_01.model.placements_report_query_message import PlacementsReportQueryMessage
-from criteo_api_marketingsolutions_v2024_01.model.point_of_interest_v1 import PointOfInterestV1
-from criteo_api_marketingsolutions_v2024_01.model.portfolio_message import PortfolioMessage
-from criteo_api_marketingsolutions_v2024_01.model.problem_details import ProblemDetails
-from criteo_api_marketingsolutions_v2024_01.model.problems_details import ProblemsDetails
-from criteo_api_marketingsolutions_v2024_01.model.prospecting_create_v1 import ProspectingCreateV1
-from criteo_api_marketingsolutions_v2024_01.model.prospecting_update_v1 import ProspectingUpdateV1
-from criteo_api_marketingsolutions_v2024_01.model.prospecting_v1 import ProspectingV1
-from criteo_api_marketingsolutions_v2024_01.model.read_ad_set import ReadAdSet
-from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_bidding import ReadAdSetBidding
-from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_bidding_v23_q1 import ReadAdSetBiddingV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_budget import ReadAdSetBudget
-from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_budget_v23_q1 import ReadAdSetBudgetV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_schedule import ReadAdSetSchedule
-from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_schedule_v23_q1 import ReadAdSetScheduleV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.read_ad_set_v23_q1 import ReadAdSetV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.read_model_ad_set_id import ReadModelAdSetId
-from criteo_api_marketingsolutions_v2024_01.model.read_model_read_ad_set import ReadModelReadAdSet
-from criteo_api_marketingsolutions_v2024_01.model.read_model_read_ad_set_v23_q1 import ReadModelReadAdSetV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.requests_ad_set_id import RequestsAdSetId
-from criteo_api_marketingsolutions_v2024_01.model.requests_patch_ad_set import RequestsPatchAdSet
-from criteo_api_marketingsolutions_v2024_01.model.response_read_ad_set import ResponseReadAdSet
-from criteo_api_marketingsolutions_v2024_01.model.response_read_ad_set_v23_q1 import ResponseReadAdSetV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.responses_ad_set_id import ResponsesAdSetId
-from criteo_api_marketingsolutions_v2024_01.model.responses_read_ad_set_v23_q1 import ResponsesReadAdSetV23Q1
-from criteo_api_marketingsolutions_v2024_01.model.retargeting_create_v1 import RetargetingCreateV1
-from criteo_api_marketingsolutions_v2024_01.model.retargeting_update_v1 import RetargetingUpdateV1
-from criteo_api_marketingsolutions_v2024_01.model.retargeting_v1 import RetargetingV1
-from criteo_api_marketingsolutions_v2024_01.model.size import Size
-from criteo_api_marketingsolutions_v2024_01.model.statistics_report_query_message import StatisticsReportQueryMessage
-from criteo_api_marketingsolutions_v2024_01.model.tag import Tag
-from criteo_api_marketingsolutions_v2024_01.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2024_01.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
-from criteo_api_marketingsolutions_v2024_01.model.transactions_report_query_message import TransactionsReportQueryMessage
-from criteo_api_marketingsolutions_v2024_01.model.transparency_query_message import TransparencyQueryMessage
-from criteo_api_marketingsolutions_v2024_01.model.transparency_report_attributes import TransparencyReportAttributes
-from criteo_api_marketingsolutions_v2024_01.model.transparency_report_data_message import TransparencyReportDataMessage
-from criteo_api_marketingsolutions_v2024_01.model.transparency_report_entity_message import TransparencyReportEntityMessage
-from criteo_api_marketingsolutions_v2024_01.model.transparency_report_file import TransparencyReportFile
-from criteo_api_marketingsolutions_v2024_01.model.update_coupon import UpdateCoupon
-from criteo_api_marketingsolutions_v2024_01.model.update_coupon_request import UpdateCouponRequest
-from criteo_api_marketingsolutions_v2024_01.model.update_coupon_resource import UpdateCouponResource
-from criteo_api_marketingsolutions_v2024_01.model.video_detail import VideoDetail
-from criteo_api_marketingsolutions_v2024_01.model.write_model_ad_set_id import WriteModelAdSetId
-from criteo_api_marketingsolutions_v2024_01.model.write_model_patch_ad_set import WriteModelPatchAdSet
+from criteo_api_marketingsolutions_v2024_04.model.ad import Ad
+from criteo_api_marketingsolutions_v2024_04.model.ad_list_response import AdListResponse
+from criteo_api_marketingsolutions_v2024_04.model.ad_resource import AdResource
+from criteo_api_marketingsolutions_v2024_04.model.ad_response import AdResponse
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_entity_v1 import AdSetAudienceLinkEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_entity_v1_resource import AdSetAudienceLinkEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_entity_v1_response import AdSetAudienceLinkEntityV1Response
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_audience_link_input_entity_v1 import AdSetAudienceLinkInputEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_category_bid import AdSetCategoryBid
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_category_bid_resource import AdSetCategoryBidResource
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_delivery_limitations_v23_q1 import AdSetDeliveryLimitationsV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_display_multiplier import AdSetDisplayMultiplier
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_frequency_capping import AdSetFrequencyCapping
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_frequency_capping_v23_q1 import AdSetFrequencyCappingV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_geo_location import AdSetGeoLocation
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_geo_location_v23_q1 import AdSetGeoLocationV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_search_filter_v23_q1 import AdSetSearchFilterV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_search_request_v23_q1 import AdSetSearchRequestV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting import AdSetTargeting
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting_rule import AdSetTargetingRule
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting_rule_v23_q1 import AdSetTargetingRuleV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.ad_set_targeting_v23_q1 import AdSetTargetingV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.ad_write import AdWrite
+from criteo_api_marketingsolutions_v2024_04.model.ad_write_request import AdWriteRequest
+from criteo_api_marketingsolutions_v2024_04.model.ad_write_resource import AdWriteResource
+from criteo_api_marketingsolutions_v2024_04.model.adaptive_attributes import AdaptiveAttributes
+from criteo_api_marketingsolutions_v2024_04.model.adaptive_colors import AdaptiveColors
+from criteo_api_marketingsolutions_v2024_04.model.adaptive_write_attributes import AdaptiveWriteAttributes
+from criteo_api_marketingsolutions_v2024_04.model.algebra_node_v1 import AlgebraNodeV1
+from criteo_api_marketingsolutions_v2024_04.model.application_summary_model import ApplicationSummaryModel
+from criteo_api_marketingsolutions_v2024_04.model.application_summary_model_resource import ApplicationSummaryModelResource
+from criteo_api_marketingsolutions_v2024_04.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_bulk_create_input_v1 import AudienceBulkCreateInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_bulk_delete_input_v1 import AudienceBulkDeleteInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_bulk_update_input_v1 import AudienceBulkUpdateInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_compute_size_entity_v1_resource import AudienceComputeSizeEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_compute_sizes_input_v1 import AudienceComputeSizesInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_create_entity_v1 import AudienceCreateEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_create_entity_v1_resource import AudienceCreateEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_delete_entity_v1_resource import AudienceDeleteEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1 import AudienceEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1_audience_search_metadata_v1_list_response import AudienceEntityV1AudienceSearchMetadataV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1_list_response import AudienceEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_entity_v1_resource import AudienceEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_error import AudienceError
+from criteo_api_marketingsolutions_v2024_04.model.audience_estimate_size_entity_v1 import AudienceEstimateSizeEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_estimate_size_entity_v1_resource import AudienceEstimateSizeEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_estimate_size_input_v1 import AudienceEstimateSizeInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_id_entity_v1_list_response import AudienceIdEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_id_entity_v1_resource import AudienceIdEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_name_description import AudienceNameDescription
+from criteo_api_marketingsolutions_v2024_04.model.audience_search_entity_v1 import AudienceSearchEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_search_entity_v1_resource import AudienceSearchEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_search_input_v1 import AudienceSearchInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_search_metadata_v1 import AudienceSearchMetadataV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_bulk_create_input_v1 import AudienceSegmentBulkCreateInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_bulk_delete_input_v1 import AudienceSegmentBulkDeleteInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_bulk_update_input_v1 import AudienceSegmentBulkUpdateInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_compute_size_entity_v1_resource import AudienceSegmentComputeSizeEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_compute_sizes_input_v1 import AudienceSegmentComputeSizesInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_create_entity_v1 import AudienceSegmentCreateEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_create_entity_v1_resource import AudienceSegmentCreateEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_delete_entity_v1_resource import AudienceSegmentDeleteEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1 import AudienceSegmentEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response import AudienceSegmentEntityV1AudienceSegmentSearchMetadataV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1_list_response import AudienceSegmentEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_entity_v1_resource import AudienceSegmentEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_estimate_size_input_v1 import AudienceSegmentEstimateSizeInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_id_entity_v1_list_response import AudienceSegmentIdEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_id_entity_v1_resource import AudienceSegmentIdEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_search_entity_v1 import AudienceSegmentSearchEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_search_entity_v1_resource import AudienceSegmentSearchEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_search_input_v1 import AudienceSegmentSearchInputV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_search_metadata_v1 import AudienceSegmentSearchMetadataV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_entity_v1 import AudienceSegmentSizeEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_entity_v1_list_response import AudienceSegmentSizeEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_entity_v1_resource import AudienceSegmentSizeEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_entity_v1 import AudienceSegmentSizeEstimationEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_entity_v1_resource import AudienceSegmentSizeEstimationEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_v1 import AudienceSegmentSizeEstimationV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_v1_resource import AudienceSegmentSizeEstimationV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_size_estimation_v1_response import AudienceSegmentSizeEstimationV1Response
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_update_entity_v1 import AudienceSegmentUpdateEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_segment_update_entity_v1_resource import AudienceSegmentUpdateEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_size_entity_v1 import AudienceSizeEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_size_entity_v1_list_response import AudienceSizeEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.audience_size_entity_v1_resource import AudienceSizeEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_size_estimation_v1 import AudienceSizeEstimationV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_size_estimation_v1_resource import AudienceSizeEstimationV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_size_estimation_v1_response import AudienceSizeEstimationV1Response
+from criteo_api_marketingsolutions_v2024_04.model.audience_update_entity_v1 import AudienceUpdateEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.audience_update_entity_v1_resource import AudienceUpdateEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.audience_warning import AudienceWarning
+from criteo_api_marketingsolutions_v2024_04.model.basic_audience_definition import BasicAudienceDefinition
+from criteo_api_marketingsolutions_v2024_04.model.behavioral_v1 import BehavioralV1
+from criteo_api_marketingsolutions_v2024_04.model.campaign_search_filters_v23_q1 import CampaignSearchFiltersV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.campaign_search_request_v23_q1 import CampaignSearchRequestV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.campaign_spend_limit_v23_q1 import CampaignSpendLimitV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1 import CampaignV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1_list_response import CampaignV23Q1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1_resource import CampaignV23Q1Resource
+from criteo_api_marketingsolutions_v2024_04.model.campaign_v23_q1_response import CampaignV23Q1Response
+from criteo_api_marketingsolutions_v2024_04.model.common_problem import CommonProblem
+from criteo_api_marketingsolutions_v2024_04.model.contact_list_statistics_entity_v1 import ContactListStatisticsEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.contact_list_statistics_entity_v1_resource import ContactListStatisticsEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.contact_list_statistics_entity_v1_response import ContactListStatisticsEntityV1Response
+from criteo_api_marketingsolutions_v2024_04.model.contact_list_v1 import ContactListV1
+from criteo_api_marketingsolutions_v2024_04.model.contactlist_amendment import ContactlistAmendment
+from criteo_api_marketingsolutions_v2024_04.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
+from criteo_api_marketingsolutions_v2024_04.model.contactlist_amendment_request import ContactlistAmendmentRequest
+from criteo_api_marketingsolutions_v2024_04.model.contactlist_operation import ContactlistOperation
+from criteo_api_marketingsolutions_v2024_04.model.contactlist_operation_attributes import ContactlistOperationAttributes
+from criteo_api_marketingsolutions_v2024_04.model.coupon import Coupon
+from criteo_api_marketingsolutions_v2024_04.model.coupon_list_response import CouponListResponse
+from criteo_api_marketingsolutions_v2024_04.model.coupon_resource import CouponResource
+from criteo_api_marketingsolutions_v2024_04.model.coupon_response import CouponResponse
+from criteo_api_marketingsolutions_v2024_04.model.coupon_supported_sizes import CouponSupportedSizes
+from criteo_api_marketingsolutions_v2024_04.model.coupon_supported_sizes_resource import CouponSupportedSizesResource
+from criteo_api_marketingsolutions_v2024_04.model.coupon_supported_sizes_response import CouponSupportedSizesResponse
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set import CreateAdSet
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_bidding import CreateAdSetBidding
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_budget import CreateAdSetBudget
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_geo_location import CreateAdSetGeoLocation
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_request import CreateAdSetRequest
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_resource import CreateAdSetResource
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_schedule import CreateAdSetSchedule
+from criteo_api_marketingsolutions_v2024_04.model.create_ad_set_targeting import CreateAdSetTargeting
+from criteo_api_marketingsolutions_v2024_04.model.create_campaign import CreateCampaign
+from criteo_api_marketingsolutions_v2024_04.model.create_campaign_request import CreateCampaignRequest
+from criteo_api_marketingsolutions_v2024_04.model.create_campaign_resource import CreateCampaignResource
+from criteo_api_marketingsolutions_v2024_04.model.create_campaign_spend_limit import CreateCampaignSpendLimit
+from criteo_api_marketingsolutions_v2024_04.model.create_coupon import CreateCoupon
+from criteo_api_marketingsolutions_v2024_04.model.create_coupon_request import CreateCouponRequest
+from criteo_api_marketingsolutions_v2024_04.model.create_coupon_resource import CreateCouponResource
+from criteo_api_marketingsolutions_v2024_04.model.create_image_slide import CreateImageSlide
+from criteo_api_marketingsolutions_v2024_04.model.creative import Creative
+from criteo_api_marketingsolutions_v2024_04.model.creative_list_response import CreativeListResponse
+from criteo_api_marketingsolutions_v2024_04.model.creative_resource import CreativeResource
+from criteo_api_marketingsolutions_v2024_04.model.creative_response import CreativeResponse
+from criteo_api_marketingsolutions_v2024_04.model.creative_write import CreativeWrite
+from criteo_api_marketingsolutions_v2024_04.model.creative_write_request import CreativeWriteRequest
+from criteo_api_marketingsolutions_v2024_04.model.creative_write_resource import CreativeWriteResource
+from criteo_api_marketingsolutions_v2024_04.model.criteo_api_error import CriteoApiError
+from criteo_api_marketingsolutions_v2024_04.model.criteo_api_warning import CriteoApiWarning
+from criteo_api_marketingsolutions_v2024_04.model.delete_audience_contact_list_response import DeleteAudienceContactListResponse
+from criteo_api_marketingsolutions_v2024_04.model.dynamic_attributes import DynamicAttributes
+from criteo_api_marketingsolutions_v2024_04.model.dynamic_write_attributes import DynamicWriteAttributes
+from criteo_api_marketingsolutions_v2024_04.model.entity_of_portfolio_message import EntityOfPortfolioMessage
+from criteo_api_marketingsolutions_v2024_04.model.error_code_response import ErrorCodeResponse
+from criteo_api_marketingsolutions_v2024_04.model.get_portfolio_response import GetPortfolioResponse
+from criteo_api_marketingsolutions_v2024_04.model.html_tag_attributes import HtmlTagAttributes
+from criteo_api_marketingsolutions_v2024_04.model.html_tag_write_attributes import HtmlTagWriteAttributes
+from criteo_api_marketingsolutions_v2024_04.model.image_attributes import ImageAttributes
+from criteo_api_marketingsolutions_v2024_04.model.image_set import ImageSet
+from criteo_api_marketingsolutions_v2024_04.model.image_set_base64 import ImageSetBase64
+from criteo_api_marketingsolutions_v2024_04.model.image_shape import ImageShape
+from criteo_api_marketingsolutions_v2024_04.model.image_slide import ImageSlide
+from criteo_api_marketingsolutions_v2024_04.model.image_write_attributes import ImageWriteAttributes
+from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_brand_entity_v1 import InMarketAudienceSegmentBrandEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_brand_entity_v1_list_response import InMarketAudienceSegmentBrandEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_brand_entity_v1_resource import InMarketAudienceSegmentBrandEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_interest_entity_v1 import InMarketAudienceSegmentInterestEntityV1
+from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_interest_entity_v1_list_response import InMarketAudienceSegmentInterestEntityV1ListResponse
+from criteo_api_marketingsolutions_v2024_04.model.in_market_audience_segment_interest_entity_v1_resource import InMarketAudienceSegmentInterestEntityV1Resource
+from criteo_api_marketingsolutions_v2024_04.model.in_market_create_v1 import InMarketCreateV1
+from criteo_api_marketingsolutions_v2024_04.model.in_market_size_estimation_v1 import InMarketSizeEstimationV1
+from criteo_api_marketingsolutions_v2024_04.model.in_market_update_v1 import InMarketUpdateV1
+from criteo_api_marketingsolutions_v2024_04.model.in_market_v1 import InMarketV1
+from criteo_api_marketingsolutions_v2024_04.model.location_create_v1 import LocationCreateV1
+from criteo_api_marketingsolutions_v2024_04.model.location_size_estimation_v1 import LocationSizeEstimationV1
+from criteo_api_marketingsolutions_v2024_04.model.location_update_v1 import LocationUpdateV1
+from criteo_api_marketingsolutions_v2024_04.model.location_v1 import LocationV1
+from criteo_api_marketingsolutions_v2024_04.model.lookalike_create_v1 import LookalikeCreateV1
+from criteo_api_marketingsolutions_v2024_04.model.lookalike_update_v1 import LookalikeUpdateV1
+from criteo_api_marketingsolutions_v2024_04.model.lookalike_v1 import LookalikeV1
+from criteo_api_marketingsolutions_v2024_04.model.modify_audience_response import ModifyAudienceResponse
+from criteo_api_marketingsolutions_v2024_04.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
+from criteo_api_marketingsolutions_v2024_04.model.nillable_ad_set_targeting_rule_v23_q1 import NillableAdSetTargetingRuleV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.nillable_ad_set_targeting_rule_v23_q1_value import NillableAdSetTargetingRuleV23Q1Value
+from criteo_api_marketingsolutions_v2024_04.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
+from criteo_api_marketingsolutions_v2024_04.model.nillable_date_time import NillableDateTime
+from criteo_api_marketingsolutions_v2024_04.model.nillable_decimal import NillableDecimal
+from criteo_api_marketingsolutions_v2024_04.model.nillable_gender_v1 import NillableGenderV1
+from criteo_api_marketingsolutions_v2024_04.model.nillable_int32 import NillableInt32
+from criteo_api_marketingsolutions_v2024_04.model.nillable_string import NillableString
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set import PatchAdSet
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_bidding import PatchAdSetBidding
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_budget import PatchAdSetBudget
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
+from criteo_api_marketingsolutions_v2024_04.model.patch_ad_set_scheduling import PatchAdSetScheduling
+from criteo_api_marketingsolutions_v2024_04.model.patch_campaign import PatchCampaign
+from criteo_api_marketingsolutions_v2024_04.model.patch_campaign_list_request import PatchCampaignListRequest
+from criteo_api_marketingsolutions_v2024_04.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
+from criteo_api_marketingsolutions_v2024_04.model.patch_campaign_write_resource import PatchCampaignWriteResource
+from criteo_api_marketingsolutions_v2024_04.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
+from criteo_api_marketingsolutions_v2024_04.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
+from criteo_api_marketingsolutions_v2024_04.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2024_04.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
+from criteo_api_marketingsolutions_v2024_04.model.placements_report_query_message import PlacementsReportQueryMessage
+from criteo_api_marketingsolutions_v2024_04.model.point_of_interest_v1 import PointOfInterestV1
+from criteo_api_marketingsolutions_v2024_04.model.portfolio_message import PortfolioMessage
+from criteo_api_marketingsolutions_v2024_04.model.problem_details import ProblemDetails
+from criteo_api_marketingsolutions_v2024_04.model.problems_details import ProblemsDetails
+from criteo_api_marketingsolutions_v2024_04.model.prospecting_create_v1 import ProspectingCreateV1
+from criteo_api_marketingsolutions_v2024_04.model.prospecting_update_v1 import ProspectingUpdateV1
+from criteo_api_marketingsolutions_v2024_04.model.prospecting_v1 import ProspectingV1
+from criteo_api_marketingsolutions_v2024_04.model.read_ad_set import ReadAdSet
+from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_bidding import ReadAdSetBidding
+from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_bidding_v23_q1 import ReadAdSetBiddingV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_budget import ReadAdSetBudget
+from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_budget_v23_q1 import ReadAdSetBudgetV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_schedule import ReadAdSetSchedule
+from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_schedule_v23_q1 import ReadAdSetScheduleV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.read_ad_set_v23_q1 import ReadAdSetV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.read_model_ad_set_id import ReadModelAdSetId
+from criteo_api_marketingsolutions_v2024_04.model.read_model_read_ad_set import ReadModelReadAdSet
+from criteo_api_marketingsolutions_v2024_04.model.read_model_read_ad_set_v23_q1 import ReadModelReadAdSetV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.requests_ad_set_id import RequestsAdSetId
+from criteo_api_marketingsolutions_v2024_04.model.requests_patch_ad_set import RequestsPatchAdSet
+from criteo_api_marketingsolutions_v2024_04.model.response_read_ad_set import ResponseReadAdSet
+from criteo_api_marketingsolutions_v2024_04.model.response_read_ad_set_v23_q1 import ResponseReadAdSetV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.responses_ad_set_id import ResponsesAdSetId
+from criteo_api_marketingsolutions_v2024_04.model.responses_read_ad_set_v23_q1 import ResponsesReadAdSetV23Q1
+from criteo_api_marketingsolutions_v2024_04.model.retargeting_create_v1 import RetargetingCreateV1
+from criteo_api_marketingsolutions_v2024_04.model.retargeting_update_v1 import RetargetingUpdateV1
+from criteo_api_marketingsolutions_v2024_04.model.retargeting_v1 import RetargetingV1
+from criteo_api_marketingsolutions_v2024_04.model.size import Size
+from criteo_api_marketingsolutions_v2024_04.model.statistics_report_query_message import StatisticsReportQueryMessage
+from criteo_api_marketingsolutions_v2024_04.model.tag import Tag
+from criteo_api_marketingsolutions_v2024_04.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2024_04.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
+from criteo_api_marketingsolutions_v2024_04.model.transactions_report_query_message import TransactionsReportQueryMessage
+from criteo_api_marketingsolutions_v2024_04.model.transparency_query_message import TransparencyQueryMessage
+from criteo_api_marketingsolutions_v2024_04.model.transparency_report_attributes import TransparencyReportAttributes
+from criteo_api_marketingsolutions_v2024_04.model.transparency_report_data_message import TransparencyReportDataMessage
+from criteo_api_marketingsolutions_v2024_04.model.transparency_report_entity_message import TransparencyReportEntityMessage
+from criteo_api_marketingsolutions_v2024_04.model.transparency_report_file import TransparencyReportFile
+from criteo_api_marketingsolutions_v2024_04.model.update_coupon import UpdateCoupon
+from criteo_api_marketingsolutions_v2024_04.model.update_coupon_request import UpdateCouponRequest
+from criteo_api_marketingsolutions_v2024_04.model.update_coupon_resource import UpdateCouponResource
+from criteo_api_marketingsolutions_v2024_04.model.video_detail import VideoDetail
+from criteo_api_marketingsolutions_v2024_04.model.write_model_ad_set_id import WriteModelAdSetId
+from criteo_api_marketingsolutions_v2024_04.model.write_model_patch_ad_set import WriteModelPatchAdSet
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/criteo_api_marketingsolutions_v2024_01/rest.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/criteo_api_marketingsolutions_v2024_04/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
@@ -15,15 +15,15 @@
 import ssl
 from urllib.parse import urlencode
 from urllib.parse import urlparse
 from urllib.request import proxy_bypass_environment
 import urllib3
 import ipaddress
 
-from criteo_api_marketingsolutions_v2024_01.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from criteo_api_marketingsolutions_v2024_04.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/setup.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-marketingsolutions-sdk"
-VERSION = "2024.01.0.240515"
+VERSION = "2024.04.0.240515"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -20,21 +20,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2024.01.0.240515
+pip install criteo-api-marketingsolutions-sdk==2024.04.0.240515
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240515`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.04.0.240515`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2024_01
+import criteo_api_marketingsolutions_v2024_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo_api_marketingsolutions_sdk-2024.1.0.240515/test/test_gateway_api.py` & `criteo_api_marketingsolutions_sdk-2024.4.0.240515/test/test_gateway_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import os
 
-from criteo_api_marketingsolutions_v2024_01.api.gateway_api import GatewayApi
-from criteo_api_marketingsolutions_v2024_01.api_client_builder import ApiClientBuilder
-from criteo_api_marketingsolutions_v2024_01.rest import ApiException
+from criteo_api_marketingsolutions_v2024_04.api.gateway_api import GatewayApi
+from criteo_api_marketingsolutions_v2024_04.api_client_builder import ApiClientBuilder
+from criteo_api_marketingsolutions_v2024_04.rest import ApiException
 from example_application_with_client_credentials import ExampleApplication
 
 class TestGatewayApi:
   @pytest.fixture(autouse=True)
   def before_each(self):
     self.client_id = os.environ.get("TEST_CLIENT_ID")
     self.client_secret = os.environ.get("TEST_CLIENT_SECRET")
```

